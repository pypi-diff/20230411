# Comparing `tmp/gordo-5.0.0rc1.tar.gz` & `tmp/gordo-5.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gordo-5.0.0rc1.tar", last modified: Thu Apr  6 11:36:55 2023, max compression
+gzip compressed data, was "gordo-5.0.0rc2.tar", last modified: Tue Apr 11 11:15:25 2023, max compression
```

## Comparing `gordo-5.0.0rc1.tar` & `gordo-5.0.0rc2.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.963843 gordo-5.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.github/dependabot.yml 
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.github/workflows/master-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/.trivyignore
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-06 11:36:55.963843 gordo-5.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/benchmarks/load_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/benchmarks/load_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/benchmarks/load_test/load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/benchmarks/load_test/task_set.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/benchmarks/test_ml_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3334 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docker_push.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.931843 gordo-5.0.0rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/_static/Gordo_C4.README
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/_static/Gordo_C4.svg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/_static/_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/_static/endpoint-metadata.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/docs/components/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/docs/components/machine/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/docs/components/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/model/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/model/model-factories.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/model/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/model/transformer-funcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/model/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/machine/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/serializer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/docs/components/server/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/server/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/server/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/server/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/components/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/docs/general/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/general/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/general/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/general/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/examples/Gordo-Workflow-High-Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/examples/Pipelines-with-Gordo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/builder/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/builder/local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/cli/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/cli/exceptions_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/cli/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/anomaly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/anomaly/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/model/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/factories/feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/factories/lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/factories/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/model/transformer_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/transformer_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/transformer_funcs/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/machine/model/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/transformers/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/machine/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/reporters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/reporters/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/reporters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/serializer/from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/serializer/into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/serializer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/blueprints/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/blueprints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.939843 gordo-5.0.0rc1/gordo/server/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/prometheus/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/prometheus/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/util/disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/gordo/workflow/config_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/config_elements/normalized_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/config_elements/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/gordo/workflow/workflow_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/workflow_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/workflow_generator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/gordo/workflow/workflow_generator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/workflow_generator/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/gordo/workflow/workflow_generator/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.935843 gordo-5.0.0rc1/gordo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:36:55.000000 gordo-5.0.0rc1/gordo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/docs_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/full_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/mlflow_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/postgres_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/test_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/requirements/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.927843 gordo-5.0.0rc1/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.927843 gordo-5.0.0rc1/resources/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/resources/grafana/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/resources/grafana/dashboards/how_to_modify_dashboard.md
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/resources/grafana/dashboards/machines.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/run_workflow_and_argo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/scripts/download_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/scripts/github_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/scripts/trivy_scan.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-06 11:36:55.963843 gordo-5.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/config-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/tests/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/tests/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/builder/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/builder/test_local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/builder/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/tests/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/cli/test_exception_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.943843 gordo-5.0.0rc1/tests/gordo/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/metadata/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_factories_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_raw_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/model/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/reporters/test_mlflow_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/reporters/test_postgres_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/serializer/definition_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_load_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_anomaly_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_base_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_gordo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/server/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/util/test_disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/util/test_sensor_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/util/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.951843 gordo-5.0.0rc1/tests/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_config_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_normalized_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.959843 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:36:55.963843 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/mocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-06 11:34:51.000000 gordo-5.0.0rc1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.729534 gordo-5.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.github/dependabot.yml 
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.github/workflows/master-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/.trivyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-11 11:15:25.729534 gordo-5.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/benchmarks/load_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/benchmarks/load_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/benchmarks/load_test/load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/benchmarks/load_test/task_set.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/benchmarks/test_ml_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/_static/Gordo_C4.README
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/_static/Gordo_C4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/_static/_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/_static/endpoint-metadata.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/components/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/components/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/model/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/model/model-factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/model/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/model/transformer-funcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/model/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/machine/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/serializer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/components/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/server/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/server/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/server/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/components/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/docs/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/general/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/general/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/general/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.709534 gordo-5.0.0rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/examples/Gordo-Workflow-High-Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/examples/Pipelines-with-Gordo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/examples/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/builder/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/builder/local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/cli/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/cli/exceptions_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/cli/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/anomaly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/anomaly/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo/machine/model/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/factories/feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/factories/lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/factories/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/machine/model/transformer_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/transformer_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/transformer_funcs/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/machine/model/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/transformers/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/machine/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/reporters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/reporters/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/reporters/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/serializer/from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/serializer/into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/serializer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/blueprints/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/blueprints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/server/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/prometheus/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/prometheus/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/util/disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/workflow/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/config_elements/normalized_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/config_elements/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/workflow/workflow_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/workflow_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/workflow_generator/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.717534 gordo-5.0.0rc2/gordo/workflow/workflow_generator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/workflow_generator/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/gordo/workflow/workflow_generator/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.713534 gordo-5.0.0rc2/gordo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:15:25.000000 gordo-5.0.0rc2/gordo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/docs_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/full_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/mlflow_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/postgres_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/test_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/requirements/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.705534 gordo-5.0.0rc2/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.705534 gordo-5.0.0rc2/resources/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/resources/grafana/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/resources/grafana/dashboards/how_to_modify_dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/resources/grafana/dashboards/machines.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/run_workflow_and_argo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/scripts/download_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/scripts/github_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/scripts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/scripts/trivy_scan.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:15:25.729534 gordo-5.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/config-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/builder/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/builder/test_local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/builder/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/cli/test_exception_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.721534 gordo-5.0.0rc2/tests/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/metadata/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_factories_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_raw_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/model/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/reporters/test_mlflow_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/reporters/test_postgres_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/serializer/definition_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_load_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_anomaly_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_base_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_gordo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/server/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/util/test_disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/util/test_sensor_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_normalized_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.725534 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:15:25.729534 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/mocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-11 11:13:15.000000 gordo-5.0.0rc2/tests/utils.py
```

### Comparing `gordo-5.0.0rc1/.github/workflows/main.yml` & `gordo-5.0.0rc2/.github/workflows/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 name: CI
 
 on:
+  pull_request:
+    paths-ignore:
+      - '**.md'
   push:
+    branches:
+      - 'master'
+    paths-ignore:
+      - '**.md'
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         os: [ubuntu-latest]
-        component: [builder, cli, client, machine, reporters, serializer, server, util, workflow, formatting, allelse]
-        python-version: [3.9]
+        component: [builder, cli, client, machine, reporters, serializer, server, util, workflow, formatting, allelse, docker]
+        python-version: ["3.10"]
     steps:
       - uses: actions/checkout@v1
 
       - uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
-          architecture: 'x64'
+          architecture: "x64"
 
       - uses: actions/cache@v1
         if: startsWith(runner.os, 'Linux')
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-${{ matrix.python-version }}-pip-new-${{ hashFiles('requirements/*requirements.txt') }}
           restore-keys: |
             ${{ runner.os }}-${{ matrix.python-version }}-pip-new-
 
       - name: Install
         run: |
-          pip install --upgrade "pip>=22.2.2,<23.0.0"
           pip install -r requirements/full_requirements.txt
           pip install -r requirements/test_requirements.txt
 
       - name: Test ${{ matrix.component }}
-        run: python setup.py test${{ matrix.component }}
+        run: bash scripts/tests.sh -n -p ${{ matrix.component }}
```

### Comparing `gordo-5.0.0rc1/.github/workflows/master-ci.yml` & `gordo-5.0.0rc2/.github/workflows/master-ci.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/.github/workflows/release.yml` & `gordo-5.0.0rc2/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 
 jobs:
   publish-to-pypi:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: [3.9]
+        python-version: ["3.10"]
     steps:
       - uses: actions/checkout@v1
 
       - uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
-          architecture: 'x64'
+          architecture: "x64"
 
       - name: Install deps
         run: |
-          pip install --upgrade "pip>=22.2.2,<23.0.0"
           pip install -r requirements/full_requirements.txt
 
       - name: Build
         run: |
           python setup.py sdist
           python setup.py bdist_wheel
```

### Comparing `gordo-5.0.0rc1/.gitignore` & `gordo-5.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/Dockerfile` & `gordo-5.0.0rc2/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Gordo base image
-FROM python:3.9-bullseye as builder
+FROM python:3.10-bullseye as builder
 
 # Copy source code
 COPY . /code
 # Copy .git to deduce version number
 COPY .git /code/
 
 WORKDIR /code
@@ -13,15 +13,15 @@
 
 # Extract a few big dependencies which docker will cache even when other dependencies change
 RUN cat /code/requirements/full_requirements.txt | grep tensorflow== > /code/prereq.txt \
     && cat /code/requirements/full_requirements.txt | grep pyarrow== >> /code/prereq.txt \
     && cat /code/requirements/full_requirements.txt | grep scipy== >> /code/prereq.txt \
     && cat /code/requirements/full_requirements.txt | grep catboost== >> /code/prereq.txt
 
-FROM python:3.9-slim-bullseye
+FROM python:3.10-slim-bullseye
 
 # Nonroot user for running CMD
 RUN groupadd -g 999 gordo && \
     useradd -r -u 999 -g gordo gordo
 
 ENV HOME "/home/gordo"
 ENV PATH "${HOME}/.local/bin:${PATH}"
```

### Comparing `gordo-5.0.0rc1/LICENSE` & `gordo-5.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/Makefile` & `gordo-5.0.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/PKG-INFO` & `gordo-5.0.0rc2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
@@ -37,95 +36,96 @@
 <div align="center">
   <a href="https://github.com/equinor/gordo/actions?query=branch=master">
     <img src="https://github.com/equinor/gordo/workflows/CI/badge.svg?branch=master" alt="Build Status"/>
   </a>
 </div>
 
 ---
-
-## Table of content
-* [About](#About)
-* [Examples](#Examples)
-* [Install](#Install)
-* [Uninstall](#Uninstall)
-* [Developer manual](#Developer-manual)
-    * [How to prepare working environment](#How-to-prepare-working-environment)
-        * [How to update packages](#How-to-update-packages)
-    * [How to run tests locally](#How-to-run-tests-locally)
-        * [Tests system requirements](#Tests-system-requirements)
-        * [Run tests](#Run-tests)
-
 ## About
 
 Gordo fulfills the role of inhaling config files and supplying components to the pipeline of:
 
 1. Fetching data
 2. Training model
 3. Serving model
 
----
-
-## Examples
+## Components
 
-See our [example](./examples) notebooks for how to develop with `gordo` locally.
+* [gordo-controller](https://github.com/equinor/gordo-controller/) - Kubernetes controller for the Gordo CRD.
+* [gordo-core](https://github.com/equinor/gordo-core/) - Gordo core library.
+* [gordo-client](https://github.com/equinor/gordo-client/) - Gordo server's client. It is able to make predictions from deployed models.
 
 ---
+## Install
+
+[gordo-helm](https://github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to deploy gordo infrastructure to your Kubernetes cluster. 
+
+### Python package 
 
-## Install 
 `pip install --upgrade gordo`  
 
 With additional extras:
 `pip install gordo[postgres,mlflow]`  
 
 Bleeding edge:  
 `pip install git+https://github.com/equinor/gordo.git`
 
-## Uninstall
-`pip uninstall gordo`
 
 ## Developer manual
+
 This section will explain how to start development of Gordo.
 
-### How to prepare working environment
-- Install pip-tools
+### Setup
+
+Create and activate a virtual environment first. As a default option, it can be [venv](https://docs.python.org/3/library/venv.html) module.
+
+Install pip-tools
 ```
 pip install --upgrade pip
 pip install --upgrade pip-tools
 ```
 
-- Install requirements
+Install requirements
 ```
 pip install -r requirements/full_requirements.txt
 pip install -r requirements/test_requirements.txt
 ```
 
+Install package:
+```
+python3 setup.py install
+```
+
 #### How to update packages
+
 Note: you have to install `pip-tools` version higher then `6` for requirements to have same multi-line output format.
 
 To update some package in `full_requirements.txt`:
 - Change its version in `requirements.in` file;
 - Compile and upgrade requirements:
 ```shell
 pip-compile --upgrade --output-file=full_requirements.txt mlflow_requirements.in postgres_requirements.in requirements.in  
 ```
 
-### How to run tests locally
+### Examples
 
-#### Tests system requirements
-To run tests it's required for your system to has (note: commands might differ from your OS):
-- Running docker process;
-- Available 5432 port for postgres container 
-(`postgresql` container is used, so better to stop your local instance for tests running). 
+See our [example](./examples) notebooks for how to develop with `gordo` locally.
+
+### How to run tests locally
 
-#### Run tests
 List of commands to run tests can be found [here](/setup.cfg).
 Running of tests takes some time, so it's faster to run tests in parallel:
 ```
-python3 setup.py test
+pytest -n auto -m 'not dockertest' --ignore benchmarks
 ```
+Run docker-related tests:
+```
+pytest -m 'dockertest'
+```
+
+> **_NOTE:_**  To run tests it's required for your system to has (note: commands might differ from your OS):
+> - Running docker daemon.
+> - Available 5432 port for `postgres` container.
 
 > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the code of the tests.  
 > On the configuration setup for test running add to `Additional arguments:` in `pytest` 
 > section following string: `--ignore benchmarks --cov-report= --no-cov ` 
-> or TEMPORARY remove `--cov-report=xml` and `--cov=gordo` from `pytest.ini` file.
-
-
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.0rc1 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.0rc2 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
-Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3 Platform:
-UNKNOWN Classifier: Intended Audience :: Developers Classifier: License :: OSI
-Approved :: GNU Affero General Public License v3 Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Provides-Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-
-Extra: tests Provides-Extra: full License-File: LICENSE
+Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU Affero General Public License v3 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
+Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
+tests Provides-Extra: full License-File: LICENSE
                               ****** Gordo ******
 
      Building thousands of models with timeseries data to monitor systems.
 
                                 [Build_Status]
---- ## Table of content * [About](#About) * [Examples](#Examples) * [Install]
-(#Install) * [Uninstall](#Uninstall) * [Developer manual](#Developer-manual) *
-[How to prepare working environment](#How-to-prepare-working-environment) *
-[How to update packages](#How-to-update-packages) * [How to run tests locally]
-(#How-to-run-tests-locally) * [Tests system requirements](#Tests-system-
-requirements) * [Run tests](#Run-tests) ## About Gordo fulfills the role of
-inhaling config files and supplying components to the pipeline of: 1. Fetching
-data 2. Training model 3. Serving model --- ## Examples See our [example](./
-examples) notebooks for how to develop with `gordo` locally. --- ## Install
-`pip install --upgrade gordo` With additional extras: `pip install gordo
+--- ## About Gordo fulfills the role of inhaling config files and supplying
+components to the pipeline of: 1. Fetching data 2. Training model 3. Serving
+model ## Components * [gordo-controller](https://github.com/equinor/gordo-
+controller/) - Kubernetes controller for the Gordo CRD. * [gordo-core](https://
+github.com/equinor/gordo-core/) - Gordo core library. * [gordo-client](https://
+github.com/equinor/gordo-client/) - Gordo server's client. It is able to make
+predictions from deployed models. --- ## Install [gordo-helm](https://
+github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/
+equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to
+deploy gordo infrastructure to your Kubernetes cluster. ### Python package `pip
+install --upgrade gordo` With additional extras: `pip install gordo
 [postgres,mlflow]` Bleeding edge: `pip install git+https://github.com/equinor/
-gordo.git` ## Uninstall `pip uninstall gordo` ## Developer manual This section
-will explain how to start development of Gordo. ### How to prepare working
-environment - Install pip-tools ``` pip install --upgrade pip pip install --
-upgrade pip-tools ``` - Install requirements ``` pip install -r requirements/
+gordo.git` ## Developer manual This section will explain how to start
+development of Gordo. ### Setup Create and activate a virtual environment
+first. As a default option, it can be [venv](https://docs.python.org/3/library/
+venv.html) module. Install pip-tools ``` pip install --upgrade pip pip install
+--upgrade pip-tools ``` Install requirements ``` pip install -r requirements/
 full_requirements.txt pip install -r requirements/test_requirements.txt ```
-#### How to update packages Note: you have to install `pip-tools` version
-higher then `6` for requirements to have same multi-line output format. To
-update some package in `full_requirements.txt`: - Change its version in
-`requirements.in` file; - Compile and upgrade requirements: ```shell pip-
-compile --upgrade --output-file=full_requirements.txt mlflow_requirements.in
-postgres_requirements.in requirements.in ``` ### How to run tests locally ####
-Tests system requirements To run tests it's required for your system to has
-(note: commands might differ from your OS): - Running docker process; -
-Available 5432 port for postgres container (`postgresql` container is used, so
-better to stop your local instance for tests running). #### Run tests List of
+Install package: ``` python3 setup.py install ``` #### How to update packages
+Note: you have to install `pip-tools` version higher then `6` for requirements
+to have same multi-line output format. To update some package in
+`full_requirements.txt`: - Change its version in `requirements.in` file; -
+Compile and upgrade requirements: ```shell pip-compile --upgrade --output-
+file=full_requirements.txt mlflow_requirements.in postgres_requirements.in
+requirements.in ``` ### Examples See our [example](./examples) notebooks for
+how to develop with `gordo` locally. ### How to run tests locally List of
 commands to run tests can be found [here](/setup.cfg). Running of tests takes
-some time, so it's faster to run tests in parallel: ``` python3 setup.py test
-``` > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the
-code of the tests. > On the configuration setup for test running add to
-`Additional arguments:` in `pytest` > section following string: `--ignore
-benchmarks --cov-report= --no-cov ` > or TEMPORARY remove `--cov-report=xml`
-and `--cov=gordo` from `pytest.ini` file.
+some time, so it's faster to run tests in parallel: ``` pytest -n auto -m 'not
+dockertest' --ignore benchmarks ``` Run docker-related tests: ``` pytest -
+m 'dockertest' ``` > **_NOTE:_** To run tests it's required for your system to
+has (note: commands might differ from your OS): > - Running docker daemon. > -
+Available 5432 port for `postgres` container. > **_NOTE:_** this example is for
+Pycharm IDE to use `breakpoints` in the code of the tests. > On the
+configuration setup for test running add to `Additional arguments:` in `pytest`
+> section following string: `--ignore benchmarks --cov-report= --no-cov `
```

### Comparing `gordo-5.0.0rc1/benchmarks/load_test/README.md` & `gordo-5.0.0rc2/benchmarks/load_test/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/benchmarks/load_test/load_test.py` & `gordo-5.0.0rc2/benchmarks/load_test/load_test.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/benchmarks/test_ml_server.py` & `gordo-5.0.0rc2/benchmarks/test_ml_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/Makefile` & `gordo-5.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/_static/Gordo_C4.svg` & `gordo-5.0.0rc2/docs/_static/Gordo_C4.svg`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/_static/endpoint-metadata.png` & `gordo-5.0.0rc2/docs/_static/endpoint-metadata.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/machine/machine.rst` & `gordo-5.0.0rc2/docs/components/machine/machine.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/machine/metadata.rst` & `gordo-5.0.0rc2/docs/components/machine/metadata.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/machine/model/anomaly.rst` & `gordo-5.0.0rc2/docs/components/machine/model/anomaly.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/machine/model/model-factories.rst` & `gordo-5.0.0rc2/docs/components/machine/model/model-factories.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/machine/model/model.rst` & `gordo-5.0.0rc2/docs/components/machine/model/model.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/serializer.rst` & `gordo-5.0.0rc2/docs/components/serializer.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/server/server.rst` & `gordo-5.0.0rc2/docs/components/server/server.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/components/workflow.rst` & `gordo-5.0.0rc2/docs/components/workflow.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/conf.py` & `gordo-5.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/general/endpoints.rst` & `gordo-5.0.0rc2/docs/general/endpoints.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/general/quickstart.rst` & `gordo-5.0.0rc2/docs/general/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/docs/index.rst` & `gordo-5.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/examples/Gordo-Workflow-High-Level.ipynb` & `gordo-5.0.0rc2/examples/Gordo-Workflow-High-Level.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/examples/Pipelines-with-Gordo.ipynb` & `gordo-5.0.0rc2/examples/Pipelines-with-Gordo.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/examples/config.yaml` & `gordo-5.0.0rc2/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/functions.sh` & `gordo-5.0.0rc2/functions.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/__init__.py` & `gordo-5.0.0rc2/gordo/__init__.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/builder/build_model.py` & `gordo-5.0.0rc2/gordo/builder/build_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/builder/local_build.py` & `gordo-5.0.0rc2/gordo/builder/local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/builder/utils.py` & `gordo-5.0.0rc2/gordo/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/cli/cli.py` & `gordo-5.0.0rc2/gordo/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/cli/custom_types.py` & `gordo-5.0.0rc2/gordo/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/cli/exceptions_reporter.py` & `gordo-5.0.0rc2/gordo/cli/exceptions_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/cli/workflow_generator.py` & `gordo-5.0.0rc2/gordo/cli/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/encoders.py` & `gordo-5.0.0rc2/gordo/machine/encoders.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/loader.py` & `gordo-5.0.0rc2/gordo/machine/loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/machine.py` & `gordo-5.0.0rc2/gordo/machine/machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/metadata/metadata.py` & `gordo-5.0.0rc2/gordo/machine/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/anomaly/base.py` & `gordo-5.0.0rc2/gordo/machine/model/anomaly/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/anomaly/diff.py` & `gordo-5.0.0rc2/gordo/machine/model/anomaly/diff.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/base.py` & `gordo-5.0.0rc2/gordo/machine/model/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/factories/feedforward_autoencoder.py` & `gordo-5.0.0rc2/gordo/machine/model/factories/feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/factories/lstm_autoencoder.py` & `gordo-5.0.0rc2/gordo/machine/model/factories/lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/factories/utils.py` & `gordo-5.0.0rc2/gordo/machine/model/factories/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/models.py` & `gordo-5.0.0rc2/gordo/machine/model/models.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/register.py` & `gordo-5.0.0rc2/gordo/machine/model/register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/transformer_funcs/general.py` & `gordo-5.0.0rc2/gordo/machine/model/transformer_funcs/general.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/transformers/imputer.py` & `gordo-5.0.0rc2/gordo/machine/model/transformers/imputer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/model/utils.py` & `gordo-5.0.0rc2/gordo/machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/machine/validators.py` & `gordo-5.0.0rc2/gordo/machine/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
-import collections
 import copy
 import re
 import datetime
 
 import pandas as pd
 import dateutil.parser
 import logging
 
+from collections.abc import Mapping
+
 from gordo.serializer import from_definition
 from gordo_core.sensor_tag import SensorTag
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -158,15 +159,15 @@
     """A valid runtime description must satisfy that any resource
     description must have that limit >= requests. This function will bump any limits
     that is too low."""
     runtime_dict = copy.deepcopy(runtime_dict)
     # We must also limit/request errors
 
     for key, val in runtime_dict.items():
-        if isinstance(val, collections.Mapping):
+        if isinstance(val, Mapping):
             resource = val.get("resources")
             if resource:
                 runtime_dict[key]["resources"] = fix_resource_limits(resource)
     return runtime_dict
 
 
 def fix_resource_limits(resources: dict) -> dict:
```

### Comparing `gordo-5.0.0rc1/gordo/reporters/base.py` & `gordo-5.0.0rc2/gordo/reporters/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/reporters/mlflow.py` & `gordo-5.0.0rc2/gordo/reporters/mlflow.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/reporters/postgres.py` & `gordo-5.0.0rc2/gordo/reporters/postgres.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/serializer/from_definition.py` & `gordo-5.0.0rc2/gordo/serializer/from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/serializer/into_definition.py` & `gordo-5.0.0rc2/gordo/serializer/into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/serializer/serializer.py` & `gordo-5.0.0rc2/gordo/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/serializer/utils.py` & `gordo-5.0.0rc2/gordo/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/blueprints/anomaly.py` & `gordo-5.0.0rc2/gordo/server/blueprints/anomaly.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/blueprints/base.py` & `gordo-5.0.0rc2/gordo/server/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/model_io.py` & `gordo-5.0.0rc2/gordo/server/model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/prometheus/metrics.py` & `gordo-5.0.0rc2/gordo/server/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/prometheus/server.py` & `gordo-5.0.0rc2/gordo/server/prometheus/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/properties.py` & `gordo-5.0.0rc2/gordo/server/properties.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/server.py` & `gordo-5.0.0rc2/gordo/server/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/server/utils.py` & `gordo-5.0.0rc2/gordo/server/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/util/disk_registry.py` & `gordo-5.0.0rc2/gordo/util/disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/util/utils.py` & `gordo-5.0.0rc2/gordo/util/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/util/version.py` & `gordo-5.0.0rc2/gordo/util/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class GordoSpecial(Version):
     special: Special
 
     def get_version(self):
         return self.special.value
 
 
-release_re = re.compile(r"^(\d{1,5})(\.(\d+)(\.(\d+)(.*?)?)?)?$")
+release_re = re.compile(r"^(\d{1,5})(\.(\d+)((\.(\d+))?(.*?)?)?)?$")
 
 
 @dataclass(frozen=True)
 class GordoRelease(Version):
     major: int
     minor: Optional[int] = None
     patch: Optional[int] = None
@@ -115,15 +115,15 @@
         try:
             number = int(gordo_version[len(pr_prefix) :])
         except ValueError:
             raise ValueError("Malformed gordo PR version '%s'" % gordo_version)
         return GordoPR(number)
     m = release_re.match(gordo_version)
     if m:
-        (major, _, minor, _, patch, suffix) = m.groups()
+        (major, _, minor, _, _, patch, suffix) = m.groups()
         return GordoRelease(
             int(major),
             int(minor) if minor else None,
             int(patch) if patch else None,
             suffix if suffix else None,
         )
     m = sha_re.match(gordo_version)
```

### Comparing `gordo-5.0.0rc1/gordo/utils.py` & `gordo-5.0.0rc2/gordo/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/workflow/config_elements/normalized_config.py` & `gordo-5.0.0rc2/gordo/workflow/config_elements/normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/workflow/config_elements/schemas.py` & `gordo-5.0.0rc2/gordo/workflow/config_elements/schemas.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/workflow/workflow_generator/helpers.py` & `gordo-5.0.0rc2/gordo/workflow/workflow_generator/helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template` & `gordo-5.0.0rc2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo/workflow/workflow_generator/workflow_generator.py` & `gordo-5.0.0rc2/gordo/workflow/workflow_generator/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/gordo.egg-info/PKG-INFO` & `gordo-5.0.0rc2/gordo.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
@@ -37,95 +36,96 @@
 <div align="center">
   <a href="https://github.com/equinor/gordo/actions?query=branch=master">
     <img src="https://github.com/equinor/gordo/workflows/CI/badge.svg?branch=master" alt="Build Status"/>
   </a>
 </div>
 
 ---
-
-## Table of content
-* [About](#About)
-* [Examples](#Examples)
-* [Install](#Install)
-* [Uninstall](#Uninstall)
-* [Developer manual](#Developer-manual)
-    * [How to prepare working environment](#How-to-prepare-working-environment)
-        * [How to update packages](#How-to-update-packages)
-    * [How to run tests locally](#How-to-run-tests-locally)
-        * [Tests system requirements](#Tests-system-requirements)
-        * [Run tests](#Run-tests)
-
 ## About
 
 Gordo fulfills the role of inhaling config files and supplying components to the pipeline of:
 
 1. Fetching data
 2. Training model
 3. Serving model
 
----
-
-## Examples
+## Components
 
-See our [example](./examples) notebooks for how to develop with `gordo` locally.
+* [gordo-controller](https://github.com/equinor/gordo-controller/) - Kubernetes controller for the Gordo CRD.
+* [gordo-core](https://github.com/equinor/gordo-core/) - Gordo core library.
+* [gordo-client](https://github.com/equinor/gordo-client/) - Gordo server's client. It is able to make predictions from deployed models.
 
 ---
+## Install
+
+[gordo-helm](https://github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to deploy gordo infrastructure to your Kubernetes cluster. 
+
+### Python package 
 
-## Install 
 `pip install --upgrade gordo`  
 
 With additional extras:
 `pip install gordo[postgres,mlflow]`  
 
 Bleeding edge:  
 `pip install git+https://github.com/equinor/gordo.git`
 
-## Uninstall
-`pip uninstall gordo`
 
 ## Developer manual
+
 This section will explain how to start development of Gordo.
 
-### How to prepare working environment
-- Install pip-tools
+### Setup
+
+Create and activate a virtual environment first. As a default option, it can be [venv](https://docs.python.org/3/library/venv.html) module.
+
+Install pip-tools
 ```
 pip install --upgrade pip
 pip install --upgrade pip-tools
 ```
 
-- Install requirements
+Install requirements
 ```
 pip install -r requirements/full_requirements.txt
 pip install -r requirements/test_requirements.txt
 ```
 
+Install package:
+```
+python3 setup.py install
+```
+
 #### How to update packages
+
 Note: you have to install `pip-tools` version higher then `6` for requirements to have same multi-line output format.
 
 To update some package in `full_requirements.txt`:
 - Change its version in `requirements.in` file;
 - Compile and upgrade requirements:
 ```shell
 pip-compile --upgrade --output-file=full_requirements.txt mlflow_requirements.in postgres_requirements.in requirements.in  
 ```
 
-### How to run tests locally
+### Examples
 
-#### Tests system requirements
-To run tests it's required for your system to has (note: commands might differ from your OS):
-- Running docker process;
-- Available 5432 port for postgres container 
-(`postgresql` container is used, so better to stop your local instance for tests running). 
+See our [example](./examples) notebooks for how to develop with `gordo` locally.
+
+### How to run tests locally
 
-#### Run tests
 List of commands to run tests can be found [here](/setup.cfg).
 Running of tests takes some time, so it's faster to run tests in parallel:
 ```
-python3 setup.py test
+pytest -n auto -m 'not dockertest' --ignore benchmarks
 ```
+Run docker-related tests:
+```
+pytest -m 'dockertest'
+```
+
+> **_NOTE:_**  To run tests it's required for your system to has (note: commands might differ from your OS):
+> - Running docker daemon.
+> - Available 5432 port for `postgres` container.
 
 > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the code of the tests.  
 > On the configuration setup for test running add to `Additional arguments:` in `pytest` 
 > section following string: `--ignore benchmarks --cov-report= --no-cov ` 
-> or TEMPORARY remove `--cov-report=xml` and `--cov=gordo` from `pytest.ini` file.
-
-
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.0rc1 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.0rc2 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
-Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3 Platform:
-UNKNOWN Classifier: Intended Audience :: Developers Classifier: License :: OSI
-Approved :: GNU Affero General Public License v3 Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Provides-Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-
-Extra: tests Provides-Extra: full License-File: LICENSE
+Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU Affero General Public License v3 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
+Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
+tests Provides-Extra: full License-File: LICENSE
                               ****** Gordo ******
 
      Building thousands of models with timeseries data to monitor systems.
 
                                 [Build_Status]
---- ## Table of content * [About](#About) * [Examples](#Examples) * [Install]
-(#Install) * [Uninstall](#Uninstall) * [Developer manual](#Developer-manual) *
-[How to prepare working environment](#How-to-prepare-working-environment) *
-[How to update packages](#How-to-update-packages) * [How to run tests locally]
-(#How-to-run-tests-locally) * [Tests system requirements](#Tests-system-
-requirements) * [Run tests](#Run-tests) ## About Gordo fulfills the role of
-inhaling config files and supplying components to the pipeline of: 1. Fetching
-data 2. Training model 3. Serving model --- ## Examples See our [example](./
-examples) notebooks for how to develop with `gordo` locally. --- ## Install
-`pip install --upgrade gordo` With additional extras: `pip install gordo
+--- ## About Gordo fulfills the role of inhaling config files and supplying
+components to the pipeline of: 1. Fetching data 2. Training model 3. Serving
+model ## Components * [gordo-controller](https://github.com/equinor/gordo-
+controller/) - Kubernetes controller for the Gordo CRD. * [gordo-core](https://
+github.com/equinor/gordo-core/) - Gordo core library. * [gordo-client](https://
+github.com/equinor/gordo-client/) - Gordo server's client. It is able to make
+predictions from deployed models. --- ## Install [gordo-helm](https://
+github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/
+equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to
+deploy gordo infrastructure to your Kubernetes cluster. ### Python package `pip
+install --upgrade gordo` With additional extras: `pip install gordo
 [postgres,mlflow]` Bleeding edge: `pip install git+https://github.com/equinor/
-gordo.git` ## Uninstall `pip uninstall gordo` ## Developer manual This section
-will explain how to start development of Gordo. ### How to prepare working
-environment - Install pip-tools ``` pip install --upgrade pip pip install --
-upgrade pip-tools ``` - Install requirements ``` pip install -r requirements/
+gordo.git` ## Developer manual This section will explain how to start
+development of Gordo. ### Setup Create and activate a virtual environment
+first. As a default option, it can be [venv](https://docs.python.org/3/library/
+venv.html) module. Install pip-tools ``` pip install --upgrade pip pip install
+--upgrade pip-tools ``` Install requirements ``` pip install -r requirements/
 full_requirements.txt pip install -r requirements/test_requirements.txt ```
-#### How to update packages Note: you have to install `pip-tools` version
-higher then `6` for requirements to have same multi-line output format. To
-update some package in `full_requirements.txt`: - Change its version in
-`requirements.in` file; - Compile and upgrade requirements: ```shell pip-
-compile --upgrade --output-file=full_requirements.txt mlflow_requirements.in
-postgres_requirements.in requirements.in ``` ### How to run tests locally ####
-Tests system requirements To run tests it's required for your system to has
-(note: commands might differ from your OS): - Running docker process; -
-Available 5432 port for postgres container (`postgresql` container is used, so
-better to stop your local instance for tests running). #### Run tests List of
+Install package: ``` python3 setup.py install ``` #### How to update packages
+Note: you have to install `pip-tools` version higher then `6` for requirements
+to have same multi-line output format. To update some package in
+`full_requirements.txt`: - Change its version in `requirements.in` file; -
+Compile and upgrade requirements: ```shell pip-compile --upgrade --output-
+file=full_requirements.txt mlflow_requirements.in postgres_requirements.in
+requirements.in ``` ### Examples See our [example](./examples) notebooks for
+how to develop with `gordo` locally. ### How to run tests locally List of
 commands to run tests can be found [here](/setup.cfg). Running of tests takes
-some time, so it's faster to run tests in parallel: ``` python3 setup.py test
-``` > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the
-code of the tests. > On the configuration setup for test running add to
-`Additional arguments:` in `pytest` > section following string: `--ignore
-benchmarks --cov-report= --no-cov ` > or TEMPORARY remove `--cov-report=xml`
-and `--cov=gordo` from `pytest.ini` file.
+some time, so it's faster to run tests in parallel: ``` pytest -n auto -m 'not
+dockertest' --ignore benchmarks ``` Run docker-related tests: ``` pytest -
+m 'dockertest' ``` > **_NOTE:_** To run tests it's required for your system to
+has (note: commands might differ from your OS): > - Running docker daemon. > -
+Available 5432 port for `postgres` container. > **_NOTE:_** this example is for
+Pycharm IDE to use `breakpoints` in the code of the tests. > On the
+configuration setup for test running add to `Additional arguments:` in `pytest`
+> section following string: `--ignore benchmarks --cov-report= --no-cov `
```

### Comparing `gordo-5.0.0rc1/gordo.egg-info/SOURCES.txt` & `gordo-5.0.0rc2/gordo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 .readthedocs.yml
 .trivyignore
 Dockerfile
 LICENSE
 Makefile
 README.md
 build.sh
-docker_push.sh
 functions.sh
 mypy.ini
 pytest.ini
 run_workflow_and_argo.sh
-setup.cfg
 setup.py
 .github/dependabot.yml 
 .github/workflows/main.yml
 .github/workflows/master-ci.yml
 .github/workflows/release.yml
 benchmarks/README.md
 benchmarks/test_ml_server.py
@@ -140,14 +138,15 @@
 requirements/test_requirements.in
 requirements/test_requirements.txt
 resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
 resources/grafana/dashboards/how_to_modify_dashboard.md
 resources/grafana/dashboards/machines.json
 scripts/download_argo.py
 scripts/github_docker.py
+scripts/tests.sh
 scripts/trivy_scan.sh
 tests/__init__.py
 tests/config-test.yaml
 tests/conftest.py
 tests/mocs.py
 tests/test_examples.py
 tests/test_formatting.py
```

### Comparing `gordo-5.0.0rc1/gordo.egg-info/requires.txt` & `gordo-5.0.0rc2/gordo.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,23 @@
 attrs==22.1.0
 backcall==0.2.0
 beautifulsoup4==4.11.1
 black==22.12.0
 bleach==5.0.1
 certifi==2022.12.7
 cffi==1.15.1
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 click==8.1.3
-coverage==6.5.0
+coverage[toml]==6.5.0
 debugpy==1.6.3
 decorator==5.1.1
 defusedxml==0.7.1
 docker==6.0.1
 entrypoints==0.4
+exceptiongroup==1.1.1
 execnet==1.9.0
 executing==1.2.0
 fastjsonschema==2.16.2
 filelock==3.8.0
 idna==3.4
 iniconfig==1.1.1
 ipykernel==6.17.0
@@ -72,55 +73,53 @@
 jupyter-server==1.21.0
 jupyterlab-pygments==0.2.2
 markupsafe==2.1.2
 matplotlib-inline==0.1.6
 mistune==0.8.4
 mock==4.0.3
 mypy==0.982
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
 nbclassic==0.4.8
 nbclient==0.5.13
 nbconvert==6.4.5
 nbformat==5.7.0
 nest-asyncio==1.5.6
 notebook==6.5.2
 notebook-shim==0.2.2
 packaging==21.3
 pandocfilters==1.5.0
 parso==0.8.3
-pathspec==0.10.2
+pathspec==0.11.1
 pexpect==4.8.0
 pickleshare==0.7.5
 platformdirs==2.5.2
 pluggy==1.0.0
-prometheus-client==0.15.0
+prometheus-client==0.16.0
 prompt-toolkit==3.0.31
 psutil==5.9.3
 ptyprocess==0.7.0
 pure-eval==0.2.2
-py==1.11.0
 py-cpuinfo==9.0.0
 pycparser==2.21
 pyflakes==2.5.0
-pygments==2.13.0
+pygments==2.14.0
 pyparsing==3.0.9
 pyrsistent==0.19.2
 pysocks==1.7.1
-pytest==6.2.5
-pytest-benchmark==3.4.1
-pytest-cov==2.12.1
+pytest==7.2.2
+pytest-benchmark==4.0.0
+pytest-cov==4.0.0
 pytest-flakes==4.0.5
-pytest-forked==1.4.0
 pytest-mock==3.10.0
 pytest-mypy==0.10.0
-pytest-timeout==1.4.2
-pytest-xdist==2.5.0
+pytest-timeout==2.1.0
+pytest-xdist==3.2.1
 python-dateutil==2.8.2
 pyzmq==24.0.1
-requests[socks]==2.28.1
+requests[socks]==2.28.2
 responses==0.22.0
 send2trash==1.8.0
 six==1.16.0
 sniffio==1.3.0
 soupsieve==2.3.2.post1
 stack-data==0.6.0
 terminado==0.17.0
@@ -134,12 +133,12 @@
 types-pytz==2022.6.0.1
 types-pyyaml==6.0.12.1
 types-requests==2.28.11.2
 types-setuptools==65.5.0.2
 types-simplejson==3.17.7.1
 types-toml==0.10.8
 types-urllib3==1.26.25.1
-typing-extensions==4.4.0
-urllib3==1.26.13
+typing-extensions==4.5.0
+urllib3==1.26.15
 wcwidth==0.2.5
 webencodings==0.5.1
-websocket-client==1.4.2
+websocket-client==1.5.1
```

### Comparing `gordo-5.0.0rc1/pytest.ini` & `gordo-5.0.0rc2/pytest.ini`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/requirements/full_requirements.txt` & `gordo-5.0.0rc2/requirements/full_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/requirements/test_requirements.txt` & `gordo-5.0.0rc2/requirements/test_requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     # via
     #   -c full_requirements.txt
     #   requests
 cffi==1.15.1
     # via
     #   -c full_requirements.txt
     #   argon2-cffi-bindings
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   -c full_requirements.txt
     #   requests
 click==8.1.3
     # via
     #   -c full_requirements.txt
     #   black
-coverage==6.5.0
+coverage[toml]==6.5.0
     # via pytest-cov
 debugpy==1.6.3
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
@@ -57,14 +57,16 @@
     #   -c full_requirements.txt
     #   -r test_requirements.in
 entrypoints==0.4
     # via
     #   -c full_requirements.txt
     #   jupyter-client
     #   nbconvert
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
 executing==1.2.0
     # via stack-data
 fastjsonschema==2.16.2
     # via nbformat
 filelock==3.8.0
@@ -129,15 +131,15 @@
     #   ipython
 mistune==0.8.4
     # via nbconvert
 mock==4.0.3
     # via -r test_requirements.in
 mypy==0.982
     # via pytest-mypy
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   -c full_requirements.txt
     #   black
     #   mypy
 nbclassic==0.4.8
     # via notebook
 nbclient==0.5.13
@@ -173,27 +175,27 @@
     #   ipykernel
     #   jupyter-server
     #   pytest
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.10.2
+pathspec==0.11.1
     # via
     #   -c full_requirements.txt
     #   black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 platformdirs==2.5.2
     # via black
 pluggy==1.0.0
     # via pytest
-prometheus-client==0.15.0
+prometheus-client==0.16.0
     # via
     #   -c full_requirements.txt
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.31
     # via ipython
@@ -201,80 +203,73 @@
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 py-cpuinfo==9.0.0
     # via pytest-benchmark
 pycparser==2.21
     # via
     #   -c full_requirements.txt
     #   cffi
 pyflakes==2.5.0
     # via pytest-flakes
-pygments==2.13.0
+pygments==2.14.0
     # via
     #   -c full_requirements.txt
     #   ipython
     #   nbconvert
 pyparsing==3.0.9
     # via
     #   -c full_requirements.txt
     #   packaging
 pyrsistent==0.19.2
     # via jsonschema
 pysocks==1.7.1
     # via
     #   -c full_requirements.txt
     #   requests
-pytest==6.2.5
+pytest==7.2.2
     # via
     #   -r test_requirements.in
     #   pytest-benchmark
     #   pytest-cov
     #   pytest-flakes
-    #   pytest-forked
     #   pytest-mock
     #   pytest-mypy
     #   pytest-timeout
     #   pytest-xdist
-pytest-benchmark==3.4.1
+pytest-benchmark==4.0.0
     # via -r test_requirements.in
-pytest-cov==2.12.1
+pytest-cov==4.0.0
     # via -r test_requirements.in
 pytest-flakes==4.0.5
     # via -r test_requirements.in
-pytest-forked==1.4.0
-    # via pytest-xdist
 pytest-mock==3.10.0
     # via -r test_requirements.in
 pytest-mypy==0.10.0
     # via -r test_requirements.in
-pytest-timeout==1.4.2
+pytest-timeout==2.1.0
     # via -r test_requirements.in
-pytest-xdist==2.5.0
+pytest-xdist==3.2.1
     # via -r test_requirements.in
 python-dateutil==2.8.2
     # via
     #   -c full_requirements.txt
     #   jupyter-client
 pyzmq==24.0.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
-requests[socks]==2.28.1
+requests[socks]==2.28.2
     # via
     #   -c full_requirements.txt
     #   docker
     #   responses
 responses==0.22.0
     # via -r test_requirements.in
 send2trash==1.8.0
@@ -297,22 +292,21 @@
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 testpath==0.6.0
     # via nbconvert
 toml==0.10.2
-    # via
-    #   pytest
-    #   pytest-cov
-    #   responses
+    # via responses
 tomli==1.2.3
     # via
     #   black
+    #   coverage
     #   mypy
+    #   pytest
 tornado==6.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
@@ -344,27 +338,27 @@
     # via -r test_requirements.in
 types-simplejson==3.17.7.1
     # via -r test_requirements.in
 types-toml==0.10.8
     # via responses
 types-urllib3==1.26.25.1
     # via types-requests
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   -c full_requirements.txt
     #   black
     #   mypy
-urllib3==1.26.13
+urllib3==1.26.15
     # via
     #   -c full_requirements.txt
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.5
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
-websocket-client==1.4.2
+websocket-client==1.5.1
     # via
     #   -c full_requirements.txt
     #   docker
     #   jupyter-server
```

### Comparing `gordo-5.0.0rc1/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json` & `gordo-5.0.0rc2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/resources/grafana/dashboards/machines.json` & `gordo-5.0.0rc2/resources/grafana/dashboards/machines.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/run_workflow_and_argo.sh` & `gordo-5.0.0rc2/run_workflow_and_argo.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/scripts/download_argo.py` & `gordo-5.0.0rc2/scripts/download_argo.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/scripts/github_docker.py` & `gordo-5.0.0rc2/scripts/github_docker.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/scripts/trivy_scan.sh` & `gordo-5.0.0rc2/scripts/trivy_scan.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/setup.py` & `gordo-5.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/config-test.yaml` & `gordo-5.0.0rc2/tests/config-test.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/conftest.py` & `gordo-5.0.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/builder/test_builder.py` & `gordo-5.0.0rc2/tests/gordo/builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/builder/test_local_build.py` & `gordo-5.0.0rc2/tests/gordo/builder/test_local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/builder/test_utils.py` & `gordo-5.0.0rc2/tests/gordo/builder/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/cli/test_cli.py` & `gordo-5.0.0rc2/tests/gordo/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/cli/test_exception_reporter.py` & `gordo-5.0.0rc2/tests/gordo/cli/test_exception_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/client/test_client.py` & `gordo-5.0.0rc2/tests/gordo/client/test_client.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/metadata/test_metadata.py` & `gordo-5.0.0rc2/tests/gordo/machine/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_factories_utils.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_factories_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_feedforward_autoencoder.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_lstm_autoencoder.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_model.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_raw_keras.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_raw_keras.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_register.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_transformers.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_transformers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/model/test_utils.py` & `gordo-5.0.0rc2/tests/gordo/machine/model/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/test_descriptors.py` & `gordo-5.0.0rc2/tests/gordo/machine/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/test_loader.py` & `gordo-5.0.0rc2/tests/gordo/machine/test_loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/machine/test_machine.py` & `gordo-5.0.0rc2/tests/gordo/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/reporters/test_mlflow_reporter.py` & `gordo-5.0.0rc2/tests/gordo/reporters/test_mlflow_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/reporters/test_postgres_reporter.py` & `gordo-5.0.0rc2/tests/gordo/reporters/test_postgres_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_from_definition.py` & `gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_into_definition.py` & `gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/serializer/test_serializer_load_dump.py` & `gordo-5.0.0rc2/tests/gordo/serializer/test_serializer_load_dump.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_anomaly_blueprint.py` & `gordo-5.0.0rc2/tests/gordo/server/test_anomaly_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_base_blueprint.py` & `gordo-5.0.0rc2/tests/gordo/server/test_base_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_gordo_server.py` & `gordo-5.0.0rc2/tests/gordo/server/test_gordo_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_model_io.py` & `gordo-5.0.0rc2/tests/gordo/server/test_model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_prometheus.py` & `gordo-5.0.0rc2/tests/gordo/server/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/server/test_utils.py` & `gordo-5.0.0rc2/tests/gordo/server/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/test_version.py` & `gordo-5.0.0rc2/tests/gordo/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/util/test_disk_registry.py` & `gordo-5.0.0rc2/tests/gordo/util/test_disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/util/test_version.py` & `gordo-5.0.0rc2/tests/gordo/util/test_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 @pytest.mark.parametrize(
     "gordo_version,expected",
     [
         ("1.2.3", GordoRelease(1, 2, 3)),
         ("3.4.5dev2", GordoRelease(3, 4, 5, "dev2")),
+        ("0.1.dev0", GordoRelease(0, 1, None, ".dev0")),
         ("5.7", GordoRelease(5, 7)),
         ("latest", GordoSpecial(Special.LATEST)),
         ("pr-43", GordoPR(43)),
         ("dke0832k", GordoSHA("dke0832k")),
     ],
 )
 def test_versions(gordo_version, expected):
```

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_config_elements.py` & `gordo-5.0.0rc2/tests/gordo/workflow/test_config_elements.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_helpers.py` & `gordo-5.0.0rc2/tests/gordo/workflow/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_normalized_config.py` & `gordo-5.0.0rc2/tests/gordo/workflow/test_normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py` & `gordo-5.0.0rc2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/test_examples.py` & `gordo-5.0.0rc2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.0rc1/tests/utils.py` & `gordo-5.0.0rc2/tests/utils.py`

 * *Files identical despite different names*

