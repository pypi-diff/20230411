# Comparing `tmp/lightning-app-2.0.1.tar.gz` & `tmp/lightning-app-2.0.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.1.tar", last modified: Thu Mar 30 14:46:34 2023, max compression
+gzip compressed data, was "lightning-app-2.0.1.post0.tar", last modified: Tue Apr 11 18:44:10 2023, max compression
```

## Comparing `lightning-app-2.0.1.tar` & `lightning-app-2.0.1.post0.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.478862 lightning-app-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.406861 lightning-app-2.0.1/.actions/
--rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-03-30 14:46:22.000000 lightning-app-2.0.1/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-03-30 14:46:22.000000 lightning-app-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-03-30 14:46:34.478862 lightning-app-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22118 2023-03-30 14:46:22.000000 lightning-app-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-03-30 14:46:22.000000 lightning-app-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.394861 lightning-app-2.0.1/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.410861 lightning-app-2.0.1/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-03-30 14:46:22.000000 lightning-app-2.0.1/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 14:46:34.478862 lightning-app-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-03-30 14:46:22.000000 lightning-app-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.410861 lightning-app-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.410861 lightning-app-2.0.1/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (122)    32540 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4826 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.414861 lightning-app-2.0.1/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8700 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.398861 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.418861 lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (122)    16500 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    21746 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     6723 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     4382 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.422861 lightning-app-2.0.1/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5043 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12620 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4327 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9547 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (122)     3738 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.422861 lightning-app-2.0.1/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.398861 lightning-app-2.0.1/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.422861 lightning-app-2.0.1/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.422861 lightning-app-2.0.1/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.426861 lightning-app-2.0.1/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.426861 lightning-app-2.0.1/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10662 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    20545 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     8947 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.426861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.426861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13108 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.426861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.430861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.430861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.430861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.430861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.430861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.434861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.434861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4364 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.434861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     5647 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.434861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.434861 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.438861 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.438861 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.438861 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.438861 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.438861 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (122)    55270 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.442861 lightning-app-2.0.1/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.442861 lightning-app-2.0.1/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     8480 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     9225 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.442861 lightning-app-2.0.1/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4657 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.442861 lightning-app-2.0.1/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.446862 lightning-app-2.0.1/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30252 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)    20105 2023-03-30 14:46:32.000000 lightning-app-2.0.1/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (122)     2853 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2927 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    11367 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (122)     5609 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.446862 lightning-app-2.0.1/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.446862 lightning-app-2.0.1/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18413 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    30187 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (122)    18071 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (122)    30759 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.450862 lightning-app-2.0.1/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.450862 lightning-app-2.0.1/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.450862 lightning-app-2.0.1/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3288 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     6300 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.450862 lightning-app-2.0.1/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.450862 lightning-app-2.0.1/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6605 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.454862 lightning-app-2.0.1/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.454862 lightning-app-2.0.1/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5290 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    45888 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.454862 lightning-app-2.0.1/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6861 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5530 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6044 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.458862 lightning-app-2.0.1/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6124 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)     9419 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (122)    18598 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.458862 lightning-app-2.0.1/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     6680 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.458862 lightning-app-2.0.1/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18595 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.458862 lightning-app-2.0.1/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.462862 lightning-app-2.0.1/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.462862 lightning-app-2.0.1/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.1/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.462862 lightning-app-2.0.1/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (122)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (122)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.1/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.1/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.466862 lightning-app-2.0.1/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (122)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (122)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (122)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (122)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (122)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.1/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.1/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.474862 lightning-app-2.0.1/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4615 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    20581 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    13389 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.478862 lightning-app-2.0.1/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11147 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3391 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3310 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (122)     8994 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (122)    10765 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7924 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     6202 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    60241 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10409 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.478862 lightning-app-2.0.1/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (122)     4667 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     5960 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (122)    30463 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     6667 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-03-30 14:46:33.000000 lightning-app-2.0.1/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:46:34.414861 lightning-app-2.0.1/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14208 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-30 14:46:34.000000 lightning-app-2.0.1/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-30 14:46:22.000000 lightning-app-2.0.1/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/.actions/
+-rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    22128 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.539529 lightning-app-2.0.1.post0/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (122)    32714 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4826 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8700 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.543529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6148 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16500 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21746 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6723 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4382 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5043 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12620 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4327 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9547 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3738 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.543529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10662 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20545 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8947 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13108 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4364 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     5647 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    55270 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8480 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9225 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4657 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30252 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20105 2023-04-11 18:44:07.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2853 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2927 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11367 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5609 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18413 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30187 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18071 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30759 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3288 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6300 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6605 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5290 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45888 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6861 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5530 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6044 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6124 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9419 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18598 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6680 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18595 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (122)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.571529 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (122)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4615 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20581 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13389 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11147 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3391 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8994 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10765 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7924 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6202 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60241 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10409 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4667 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5960 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30463 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6667 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14208 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/version.info
```

### Comparing `lightning-app-2.0.1/.actions/assistant.py` & `lightning-app-2.0.1.post0/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/LICENSE` & `lightning-app-2.0.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/PKG-INFO` & `lightning-app-2.0.1.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.1
+Version: 2.0.1.post0
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -22,17 +22,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cloud
-Provides-Extra: ui
 Provides-Extra: components
 Provides-Extra: test
+Provides-Extra: ui
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1 Summary: Use Lightning
-Apps to build everything from production-ready, multi-cloud ML systems to
-simple research demos. Home-page: https://github.com/Lightning-AI/lightning
-Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
-Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
-Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
-Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
-https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
-Platform: UNKNOWN Classifier: Environment :: Console Classifier: Natural
-Language :: English Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
-Information Analysis Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: cloud Provides-Extra: ui Provides-
-Extra: components Provides-Extra: test Provides-Extra: extra Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1.post0 Summary: Use
+Lightning Apps to build everything from production-ready, multi-cloud ML
+systems to simple research demos. Home-page: https://github.com/Lightning-AI/
+lightning Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai
+License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
+Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
+Project-URL: Documentation, https://lightning.ai/lightning-docs Project-URL:
+Source Code, https://github.com/Lightning-AI/lightning Keywords: deep
+learning,pytorch,AI Platform: UNKNOWN Classifier: Environment :: Console
+Classifier: Natural Language :: English Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Information Analysis Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: cloud
+Provides-Extra: components Provides-Extra: test Provides-Extra: ui Provides-
+Extra: extra Provides-Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.1/README.md` & `lightning-app-2.0.1.post0/README.md`

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

### Comparing `lightning-app-2.0.1/pyproject.toml` & `lightning-app-2.0.1.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/requirements/app/base.txt` & `lightning-app-2.0.1.post0/requirements/app/base.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/setup.py` & `lightning-app-2.0.1.post0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.1.post0/src/lightning_app/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
+## [2.0.1post] - 2023-04-12
+
+### Fixed
+
+- Fix frontend hosts when running with multi-process in the cloud ([#17324](https://github.com/Lightning-AI/lightning/pull/17324))
+
+
+
 ## [2.0.1] - 2023-03-30
 
 No changes.
 
 
 ## [2.0.0] - 2023-03-15
```

### Comparing `lightning-app-2.0.1/src/lightning_app/README.md` & `lightning-app-2.0.1.post0/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/__about__.py` & `lightning-app-2.0.1.post0/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/__init__.py` & `lightning-app-2.0.1.post0/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/__setup__.py` & `lightning-app-2.0.1.post0/src/lightning_app/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.1.post0/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/api/request_types.py` & `lightning-app-2.0.1.post0/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/maverick.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/core.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_create.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/__init__.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/database/client.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/database/server.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/components/training.py` & `lightning-app-2.0.1.post0/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/api.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/app.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/constants.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/flow.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/queues.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/core/work.py` & `lightning-app-2.0.1.post0/src/lightning_app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/frontend/web.py` & `lightning-app-2.0.1.post0/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.1.post0/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.1.post0/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.1.post0/src/lightning_app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/multiprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,18 +62,25 @@
             os.environ.update(self.env_vars)
 
             # refresh the layout with the populated urls.
             self.app._update_layout()
 
             _set_frontend_context()
             for frontend in self.app.frontends.values():
-                host = "localhost"
                 port = find_free_network_port()
-                frontend.start_server(host="localhost", port=port)
-                frontend.flow._layout["target"] = f"http://{host}:{port}/{frontend.flow.name}"
+
+                server_host = "0.0.0.0" if in_cloudspace else "localhost"
+                server_target = (
+                    f"https://{port}-{constants.LIGHTNING_CLOUDSPACE_HOST}"
+                    if in_cloudspace
+                    else f"http://localhost:{port}"
+                )
+
+                frontend.start_server(host=server_host, port=port)
+                frontend.flow._layout["target"] = f"{server_target}/{frontend.flow.name}"
 
             _set_flow_context()
 
             storage_orchestrator = StorageOrchestrator(
                 self.app,
                 self.app.request_queues,
                 self.app.response_queues,
```

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.1.post0/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.1.post0/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.1.post0/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/source_code/local.py` & `lightning-app-2.0.1.post0/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.1.post0/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.1.post0/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/copier.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/drive.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/mount.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/path.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/payload.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/storage/requests.py` & `lightning-app-2.0.1.post0/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/structures/dict.py` & `lightning-app-2.0.1.post0/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/structures/list.py` & `lightning-app-2.0.1.post0/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/testing/config.py` & `lightning-app-2.0.1.post0/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.1.post0/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/testing/testing.py` & `lightning-app-2.0.1.post0/src/lightning_app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.1.post0/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/index.html` & `lightning-app-2.0.1.post0/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/component.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/git.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/log.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/login.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/network.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/port.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/state.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/types.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.1.post0/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.1.post0/src/lightning_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.1
+Version: 2.0.1.post0
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -22,17 +22,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cloud
-Provides-Extra: ui
 Provides-Extra: components
 Provides-Extra: test
+Provides-Extra: ui
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1 Summary: Use Lightning
-Apps to build everything from production-ready, multi-cloud ML systems to
-simple research demos. Home-page: https://github.com/Lightning-AI/lightning
-Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
-Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
-Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
-Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
-https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
-Platform: UNKNOWN Classifier: Environment :: Console Classifier: Natural
-Language :: English Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
-Information Analysis Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: cloud Provides-Extra: ui Provides-
-Extra: components Provides-Extra: test Provides-Extra: extra Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1.post0 Summary: Use
+Lightning Apps to build everything from production-ready, multi-cloud ML
+systems to simple research demos. Home-page: https://github.com/Lightning-AI/
+lightning Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai
+License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
+Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
+Project-URL: Documentation, https://lightning.ai/lightning-docs Project-URL:
+Source Code, https://github.com/Lightning-AI/lightning Keywords: deep
+learning,pytorch,AI Platform: UNKNOWN Classifier: Environment :: Console
+Classifier: Natural Language :: English Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Information Analysis Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: cloud
+Provides-Extra: components Provides-Extra: test Provides-Extra: ui Provides-
+Extra: extra Provides-Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.1/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.1.post0/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.1.post0/src/lightning_app.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
 playwright==1.30.0
 httpx
 trio<1.0
 pympler
 psutil
-setuptools<66.0
+setuptools<68.0
 sqlmodel
 requests-mock
 
 [extra]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
 s3fs<2023.0,>=2022.5.0
@@ -93,14 +93,14 @@
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
 playwright==1.30.0
 httpx
 trio<1.0
 pympler
 psutil
-setuptools<66.0
+setuptools<68.0
 sqlmodel
 requests-mock
 
 [ui]
 streamlit<2.0,>=1.13.0
 panel<1.0,>=0.12.7
```

