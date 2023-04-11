# Comparing `tmp/cortex_cli-1.12.3.tar.gz` & `tmp/cortex_cli-1.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.12.3.tar", last modified: Tue Apr 11 16:16:30 2023, max compression
+gzip compressed data, was "cortex_cli-1.12.4.tar", last modified: Tue Apr 11 16:36:27 2023, max compression
```

## Comparing `cortex_cli-1.12.3.tar` & `cortex_cli-1.12.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.3/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-07 17:57:53.000000 cortex_cli-1.12.3/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.3/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22303 2023-04-07 20:22:18.000000 cortex_cli-1.12.3/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4124 2023-04-11 16:15:11.000000 cortex_cli-1.12.3/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    10969 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7010 2023-03-21 15:45:49.000000 cortex_cli-1.12.3/cortex_cli/core/models/cortex_model.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      346 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      164 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1909 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.3/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      206 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.3/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.4/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-11 16:35:05.000000 cortex_cli-1.12.4/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.4/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.4/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22343 2023-04-11 16:30:05.000000 cortex_cli-1.12.4/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.4/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4124 2023-04-11 16:15:11.000000 cortex_cli-1.12.4/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    10969 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7010 2023-03-21 15:45:49.000000 cortex_cli-1.12.4/cortex_cli/core/models/cortex_model.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-11 16:29:39.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-11 16:28:41.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1893 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.4/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.4/setup.py
```

### Comparing `cortex_cli-1.12.3/README.md` & `cortex_cli-1.12.4/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.12.4/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.12.4/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.12.4/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.12.4/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/configure.py` & `cortex_cli-1.12.4/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.12.4/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/generic_get.py` & `cortex_cli-1.12.4/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/inferences.py` & `cortex_cli-1.12.4/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/models.py` & `cortex_cli-1.12.4/cortex_cli/cli/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,18 @@
 
     def _generate_template_repo(self):
         cookiecutter(
             self._template_location,
             no_input=True,
             output_dir=self._path,
             extra_context={
-                'model_name':  self._name,
+                'model_name': self._name,
+                'model_repo': self._repo,
                 'description': self._description,
-                '__version': __version__
+                'version': __version__
             }
         )
 
 
     def _create_repo(self, github):
         if self._token:
             try:
```

### Comparing `cortex_cli-1.12.3/cortex_cli/cli/pipelines.py` & `cortex_cli-1.12.4/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/core/cortex_data.py` & `cortex_cli-1.12.4/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/core/drift_checks.py` & `cortex_cli-1.12.4/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.12.4/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.12.4/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.12.4/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/.gitignore` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/README.md` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.12.4/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.12.4/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.3/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.12.4/cortex_cli.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 cortex_cli/core/models/__init__.py
 cortex_cli/core/models/cortex_model.py
 cortex_cli/ml_model_template/.gitignore
 cortex_cli/ml_model_template/README.md
 cortex_cli/ml_model_template/__init__.py
 cortex_cli/ml_model_template/cookiecutter.json
 cortex_cli/ml_model_template/requirements.txt
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/conda.yml
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/.gitkeep
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/.gitkeep
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/__init__.py
-cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
 cortex_cli/tests/__init__.py
 cortex_cli/tests/test_cortex_data.py
 cortex_cli/tests/test_ethics_checks.py
```

### Comparing `cortex_cli-1.12.3/setup.py` & `cortex_cli-1.12.4/setup.py`

 * *Files identical despite different names*

