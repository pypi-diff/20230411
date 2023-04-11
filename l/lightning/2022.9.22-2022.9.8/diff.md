# Comparing `tmp/lightning-2022.9.22.tar.gz` & `tmp/lightning-2022.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-2022.9.22.tar", last modified: Thu Sep 22 15:57:03 2022, max compression
+gzip compressed data, was "lightning-2022.9.8.tar", last modified: Thu Sep  8 12:46:12 2022, max compression
```

## Comparing `lightning-2022.9.22.tar` & `lightning-2022.9.8.tar`

### file list

```diff
@@ -1,464 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.498002 lightning-2022.9.22/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.438001 lightning-2022.9.22/.actions/
--rw-r--r--   0 runner    (1001) docker     (121)    22865 2022-09-22 15:56:45.000000 lightning-2022.9.22/.actions/setup_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-22 15:56:45.000000 lightning-2022.9.22/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)    11349 2022-09-22 15:56:45.000000 lightning-2022.9.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-22 15:57:02.000000 lightning-2022.9.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22889 2022-09-22 15:57:03.498002 lightning-2022.9.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23546 2022-09-22 15:56:45.000000 lightning-2022.9.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.438001 lightning-2022.9.22/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-22 15:57:02.000000 lightning-2022.9.22/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-22 15:57:03.502002 lightning-2022.9.22/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     5513 2022-09-22 15:57:02.000000 lightning-2022.9.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.434002 lightning-2022.9.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning/
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-22 15:56:45.000000 lightning-2022.9.22/src/lightning/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-22 15:56:45.000000 lightning-2022.9.22/src/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-22 15:56:45.000000 lightning-2022.9.22/src/lightning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-09-22 15:56:45.000000 lightning-2022.9.22/src/lightning/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning/app/
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning/app/api/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning/app/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/cmd_react_ui_init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning/app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/commands/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/components/python/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/gradio.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/core/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.446002 lightning-2022.9.22/src/lightning/app/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/runners/
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/runtime_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/runners/singleprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/source_code/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/storage/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.450002 lightning-2022.9.22/src/lightning/app/structures/
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.454002 lightning-2022.9.22/src/lightning/app/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.458002 lightning-2022.9.22/src/lightning/app/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/cluster_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.458002 lightning-2022.9.22/src/lightning/app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.458002 lightning-2022.9.22/src/lightning/app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/app/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.458002 lightning-2022.9.22/src/lightning/lite/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/lite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.462002 lightning-2022.9.22/src/lightning/lite/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/lite/utilities/xla_device.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.462002 lightning-2022.9.22/src/lightning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.462002 lightning-2022.9.22/src/lightning/pytorch/accelerators/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/hpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/ipu.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/accelerators/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.466002 lightning-2022.9.22/src/lightning/pytorch/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/device_stats_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/fault_tolerance.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/prediction_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.466002 lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/pruning.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/quantization.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/rich_model_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/callbacks/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/core/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/mixins/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/mixins/hparams_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/core/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/demos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/demos/boring_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/demos/mnist_datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/lite/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/lite/lite.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/lite/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/loggers/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/neptune.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/loops/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.470002 lightning-2022.9.22/src/lightning/pytorch/loops/batch/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/batch/training_batch_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.474002 lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/dataloader_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/evaluation_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/prediction_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.474002 lightning-2022.9.22/src/lightning/pytorch/loops/epoch/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/epoch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/epoch/evaluation_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/epoch/prediction_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/epoch/training_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/fit_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.474002 lightning-2022.9.22/src/lightning/pytorch/loops/optimization/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/optimization/closure.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/optimization/manual_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/optimization/optimizer_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/loops/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.474002 lightning-2022.9.22/src/lightning/pytorch/overrides/
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/fairscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/overrides/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.474002 lightning-2022.9.22/src/lightning/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.478002 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/bagua_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/kubeflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/lightning_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/lsf_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/slurm_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/torchelastic_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/environments/xla_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.478002 lightning-2022.9.22/src/lightning/pytorch/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/async_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/hpu_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/torch_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/io/xla_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/layer_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.482002 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/apex_amp.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/fsdp_native_native_amp.py
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/fully_sharded_native_amp.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/hpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/ipu.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/mixed.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/native_amp.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/precision_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/sharded_native_amp.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/precision/tpu_bf16.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.482002 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/ddp.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/ddp2.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/ddp_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/dp.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/fully_sharded.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/horovod.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/ipu.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/sharded.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/sharded_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/single_device.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/tpu_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/training_type_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.486002 lightning-2022.9.22/src/lightning/pytorch/profiler/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profiler/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.486002 lightning-2022.9.22/src/lightning/pytorch/profilers/
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/profilers/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.486002 lightning-2022.9.22/src/lightning/pytorch/serve/
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/serve/servable_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/serve/servable_module_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.490002 lightning-2022.9.22/src/lightning/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/bagua.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/ddp2.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/ddp_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/fully_sharded.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/fully_sharded_native.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/horovod.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/hpu_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/ipu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.490002 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/sharded.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/sharded_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/single_hpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/strategy_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/tpu_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/strategies/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.490002 lightning-2022.9.22/src/lightning/pytorch/trainer/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/callback_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/configuration_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.494002 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/callback_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/data_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.494002 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/signal_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/states.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/supporters.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.494002 lightning-2022.9.22/src/lightning/pytorch/tuner/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/tuner/auto_gpu_select.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/tuner/batch_size_scaling.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/tuner/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/tuner/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.498002 lightning-2022.9.22/src/lightning/pytorch/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/argparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/fetching.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/finite_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/grads.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/migration.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/model_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.498002 lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/parameter_tying.py
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/signature_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/upgrade_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-22 15:57:02.000000 lightning-2022.9.22/src/lightning/pytorch/utilities/xla_device.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 15:57:03.442001 lightning-2022.9.22/src/lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22889 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18072 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-22 15:57:03.000000 lightning-2022.9.22/src/lightning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.593405 lightning-2022.9.8/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/.actions/
+-rw-r--r--   0 runner    (1001) docker     (121)    22720 2022-09-08 12:45:59.000000 lightning-2022.9.8/.actions/setup_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-08 12:45:59.000000 lightning-2022.9.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)    11349 2022-09-08 12:45:59.000000 lightning-2022.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-08 12:46:12.000000 lightning-2022.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    22875 2022-09-08 12:46:12.593405 lightning-2022.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    23546 2022-09-08 12:45:59.000000 lightning-2022.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-08 12:46:12.000000 lightning-2022.9.8/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-08 12:46:12.593405 lightning-2022.9.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5513 2022-09-08 12:46:12.000000 lightning-2022.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.557405 lightning-2022.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-08 12:45:59.000000 lightning-2022.9.8/src/lightning/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-08 12:45:59.000000 lightning-2022.9.8/src/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-08 12:45:59.000000 lightning-2022.9.8/src/lightning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-09-08 12:45:59.000000 lightning-2022.9.8/src/lightning/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/cmd_react_ui_init.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/commands/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/components/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning/app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/runtime_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/runners/singleprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/structures/
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.565405 lightning-2022.9.8/src/lightning/app/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.569405 lightning-2022.9.8/src/lightning/app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/cluster_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.569405 lightning-2022.9.8/src/lightning/app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.569405 lightning-2022.9.8/src/lightning/app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/app/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.569405 lightning-2022.9.8/src/lightning/lite/
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/lite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.573405 lightning-2022.9.8/src/lightning/lite/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/lite/utilities/xla_device.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.573405 lightning-2022.9.8/src/lightning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.573405 lightning-2022.9.8/src/lightning/pytorch/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/hpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/ipu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/accelerators/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.573405 lightning-2022.9.8/src/lightning/pytorch/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/device_stats_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/fault_tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/prediction_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/rich_model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/callbacks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/mixins/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/mixins/hparams_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/core/saving.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/demos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/demos/boring_classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/demos/mnist_datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/lite/
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/lite/lite.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/lite/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loggers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loops/
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loops/batch/
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/batch/training_batch_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/dataloader_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/evaluation_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/prediction_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loops/epoch/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/epoch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/epoch/evaluation_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/epoch/prediction_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/epoch/training_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/fit_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.577405 lightning-2022.9.8/src/lightning/pytorch/loops/optimization/
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/optimization/closure.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/optimization/manual_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/optimization/optimizer_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/loops/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.581405 lightning-2022.9.8/src/lightning/pytorch/overrides/
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/fairscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/overrides/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.581405 lightning-2022.9.8/src/lightning/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.581405 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/bagua_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/kubeflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/lightning_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/lsf_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/slurm_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/torchelastic_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/environments/xla_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.581405 lightning-2022.9.8/src/lightning/pytorch/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/async_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/hpu_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/torch_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/io/xla_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/layer_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.581405 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/apex_amp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/fsdp_native_native_amp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/fully_sharded_native_amp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/hpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/ipu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/native_amp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/precision_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/sharded_native_amp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/precision/tpu_bf16.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.585405 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/ddp2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/ddp_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/dp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/fully_sharded.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/ipu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/sharded.py
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/sharded_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/tpu_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/training_type_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.585405 lightning-2022.9.8/src/lightning/pytorch/profiler/
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profiler/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.585405 lightning-2022.9.8/src/lightning/pytorch/profilers/
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/profilers/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.585405 lightning-2022.9.8/src/lightning/pytorch/serve/
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/serve/servable_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/serve/servable_module_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.585405 lightning-2022.9.8/src/lightning/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/bagua.py
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/ddp2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/ddp_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/fully_sharded.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/fully_sharded_native.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/hpu_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/ipu.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.589405 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/sharded.py
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/sharded_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/single_hpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/strategy_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/tpu_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/strategies/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.589405 lightning-2022.9.8/src/lightning/pytorch/trainer/
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/callback_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/configuration_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.589405 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/callback_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/data_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.589405 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/signal_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/states.py
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/supporters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.589405 lightning-2022.9.8/src/lightning/pytorch/tuner/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/tuner/auto_gpu_select.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/tuner/batch_size_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/tuner/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/tuner/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.593405 lightning-2022.9.8/src/lightning/pytorch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/finite_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/grads.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/migration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/model_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.593405 lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/parameter_tying.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/signature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/upgrade_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning/pytorch/utilities/xla_device.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 12:46:12.561405 lightning-2022.9.8/src/lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22875 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18025 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-08 12:46:12.000000 lightning-2022.9.8/src/lightning.egg-info/top_level.txt
```

### Comparing `lightning-2022.9.22/.actions/setup_tools.py` & `lightning-2022.9.8/.actions/setup_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import tempfile
 import urllib.request
 from datetime import datetime
 from distutils.version import LooseVersion
 from importlib.util import module_from_spec, spec_from_file_location
 from itertools import chain, groupby
 from types import ModuleType
-from typing import List, Sequence
+from typing import List
 
 from pkg_resources import parse_requirements
 
 _PROJECT_ROOT = os.path.dirname(os.path.dirname(__file__))
 _PACKAGE_MAPPING = {"pytorch": "pytorch_lightning", "app": "lightning_app"}
 
 # TODO: remove this once lightning-ui package is ready as a dependency
@@ -496,30 +496,26 @@
         print("The Lightning UI has successfully been downloaded!")
 
     # If installing from source without internet connection, we don't want to break the installation
     except Exception:
         print("The Lightning UI downloading has failed!")
 
 
-def _relax_require_versions(
-    source_dir: str = "src", req_dir: str = "requirements", strict_pkgs: Sequence[str] = ("lightning_app",)
-) -> None:
+def _relax_require_versions(source_dir: str = "src", req_dir: str = "requirements") -> None:
     """Parse the base requirements and append  as version adjustments if needed `pkg>=X1.Y1.Z1,==X2.Y2.*`.
 
     >>> _relax_require_versions("../src", "../requirements")
     """
-    strict_pkgs = strict_pkgs or tuple()
     reqs = load_requirements(req_dir, file_name="base.txt")
     for i, req in enumerate(parse_requirements(reqs)):
-        ver = parse_version_from_file(os.path.join(source_dir, req.name))
-        if not ver:
+        ver_ = parse_version_from_file(os.path.join(source_dir, req.name))
+        if not ver_:
             continue
-        if req.name not in strict_pkgs:
-            ver = ".".join(ver.split(".")[:2] + ["*"])
-        reqs[i] = f"{req}, =={ver}"
+        ver2 = ".".join(ver_.split(".")[:2] + ["*"])
+        reqs[i] = f"{req}, =={ver2}"
 
     with open(os.path.join(req_dir, "base.txt"), "w") as fp:
         fp.writelines([ln + os.linesep for ln in reqs])
 
 
 def _load_aggregate_requirements(req_dir: str = "requirements", freeze_requirements: bool = False) -> None:
     """Load all base requirements from all particular packages and prune duplicates."""
```

### Comparing `lightning-2022.9.22/CITATION.cff` & `lightning-2022.9.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/LICENSE` & `lightning-2022.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/PKG-INFO` & `lightning-2022.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2022.9.22
+Version: 2022.9.8
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Download-URL: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -36,30 +36,30 @@
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://www.lightning.ai/">Lightning Gallery</a> •
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2022.9.22">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2022.9.8">Docs</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
 [![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning/release/2022.9.22/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
+[![codecov](https://codecov.io/gh/Lightning-AI/lightning/release/2022.9.8/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.22)](https://pytorch-lightning.readthedocs.io/en/2022.9.22)
+[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.8)](https://pytorch-lightning.readthedocs.io/en/2022.9.8)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
@@ -118,21 +118,21 @@
 
 <center>
 
 |   System / PyTorch ver.    |                                                                                                               1.9                                                                                                               |                                                                                                              1.10                                                                                                               |                                                                                                       1.12 (latest)                                                                                                        |
 | :------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 |  Linux py3.7 \[GPUs\*\*\]  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
 | Linux py3.7 \[TPUs\*\*\*\] |                                       [![CircleCI](https://circleci.com/gh/Lightning-AI/lightning/tree/master.svg?style=svg)](https://circleci.com/gh/Lightning-AI/lightning/tree/master)                                       |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
-|    Linux py3.8 \[IPUs\]    | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(IPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=25&branchName=master) |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
-|    Linux py3.8 \[HPUs\]    |                                                                                                                -                                                                                                                | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(HPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=26&branchName=master) |                                                                                                             -                                                                                                              |
-|  Linux py3.8 (with Conda)  |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |                                                                                                             -                                                                                                              |
-|  Linux py3.9 (with Conda)  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) |
-|      Linux py3.{7,9}       |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
-|       OSX py3.{7,9}        |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
-|     Windows py3.{7,9}      |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|    Linux py3.8 \[IPUs\]    | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(IPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=25&branchName=master) |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
+|    Linux py3.8 \[HPUs\]    |                                                                                                                -                                                                                                                | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(HPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=26&branchName=master) |                                                                                                             -                                                                                                              |
+|  Linux py3.8 (with Conda)  |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |                                                                                                             -                                                                                                              |
+|  Linux py3.9 (with Conda)  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) |
+|      Linux py3.{7,9}       |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|       OSX py3.{7,9}        |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|     Windows py3.{7,9}      |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
 
 - _\*\* tests run on two NVIDIA P100_
 - _\*\*\* tests run on Google GKE TPUv2/3. TPU py3.7 means we support Colab and Kaggle env._
 
 </center>
 </details>
 
@@ -346,15 +346,15 @@
 
 <div align="center">
   <img src="docs/source-pytorch/_static/images/lightning_lite/lite.gif" height="200px" width="600px">
 </div>
 
 In the Lightning v1.5 release, LightningLite now enables you to leverage all the capabilities of PyTorch Lightning Accelerators without any refactoring to your training loop. Check out the
 [blogpost](https://devblog.pytorchlightning.ai/scale-your-pytorch-code-with-lightninglite-d5692a303f00) and
-[docs](https://pytorch-lightning.readthedocs.io/en/2022.9.22starter/lightning_lite.html) for more info.
+[docs](https://pytorch-lightning.readthedocs.io/en/2022.9.8starter/lightning_lite.html) for more info.
 
 ______________________________________________________________________
 
 ## Examples
 
 ###### Hello world
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning Version: 2022.9.22 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning Version: 2022.9.8 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Download-URL: https://github.com/Lightning-AI/lightning Author: Lightning AI et
 al. Author-email: pytorch@lightning.ai License: Apache-2.0 Project-URL: Bug
 Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -31,22 +31,21 @@
  //badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-
 lightning) [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://
 pepy.tech/project/pytorch-lightning) [![Conda](https://img.shields.io/conda/v/
 conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/
   conda-forge/pytorch-lightning) [![DockerHub](https://img.shields.io/docker/
    pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/
     pytorchlightning/pytorch_lightning) [![codecov](https://codecov.io/gh/
-  Lightning-AI/lightning/release/2022.9.22/graph/badge.svg?token=SmzX8mnKlA)]
+  Lightning-AI/lightning/release/2022.9.8/graph/badge.svg?token=SmzX8mnKlA)]
     (https://codecov.io/gh/Lightning-AI/lightning) [![ReadTheDocs](https://
-readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.22)](https://
-       pytorch-lightning.readthedocs.io/en/2022.9.22) [![Slack](https://
-        img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://
- www.pytorchlightning.ai/community) [![license](https://img.shields.io/badge/
-License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/
-                               master/LICENSE)
+ readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.8)](https://
+pytorch-lightning.readthedocs.io/en/2022.9.8) [![Slack](https://img.shields.io/
+   badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/
+   community) [![license](https://img.shields.io/badge/License-Apache%202.0-
+  blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 ###### \*Codecov is > 90%+ but build delays may show less
 ______________________________________________________________________ ##
 PyTorch Lightning is just organized PyTorch Lightning disentangles PyTorch code
 to decouple the science from the engineering. ![PT to PL](docs/source-pytorch/
 _static/images/general/pl_quick_start_full_compressed.gif) ## Build AI products
 with Lightning Apps Once you're done building models, publish a paper demo or
 build a full production end-to-end ML system with Lightning Apps. Lightning
@@ -84,38 +83,38 @@
 -------------------------------------------------------------------------------
 --------------------------------------------: | | Linux py3.7 \[GPUs\*\*\] | -
 | - | - | | Linux py3.7 \[TPUs\*\*\*\] | [![CircleCI](https://circleci.com/gh/
   Lightning-AI/lightning/tree/master.svg?style=svg)](https://circleci.com/gh/
 Lightning-AI/lightning/tree/master) | - | - | | Linux py3.8 \[IPUs\] | [![Build
                                    Status](
  dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20
- (IPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-
-AI/lightning/_build/latest?definitionId=25&branchName=master) | - | - | | Linux
+(IPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/
+ lightning/_build/latest?definitionId=25&branchName=master) | - | - | | Linux
                     py3.8 \[HPUs\] | - | [![Build Status](
  dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20
- (HPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-
-  AI/lightning/_build/latest?definitionId=26&branchName=master) | - | | Linux
-   py3.8 (with Conda) | [![Test](https://github.com/Lightning-AI/lightning/
-actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://
+(HPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/
+lightning/_build/latest?definitionId=26&branchName=master) | - | | Linux py3.8
+  (with Conda) | [![Test](https://github.com/Lightning-AI/lightning/actions/
+     workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://
 github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)
   | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-
-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-
+ pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-
 AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) | - | | Linux py3.9
   (with Conda) | - | - | [![Test](https://github.com/Lightning-AI/lightning/
-actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://
+ actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://
 github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)
     | | Linux py3.{7,9} | - | - | [![Test](https://github.com/Lightning-AI/
-lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)]
+ lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)]
  (https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-
 full.yml) | | OSX py3.{7,9} | - | - | [![Test](https://github.com/Lightning-AI/
-lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)]
+ lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)]
  (https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-
     full.yml) | | Windows py3.{7,9} | - | - | [![Test](https://github.com/
       Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/
- badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/
+  badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/
  workflows/ci-pytorch-test-full.yml) | - _\*\* tests run on two NVIDIA P100_ -
  _\*\*\* tests run on Google GKE TPUv2/3. TPU py3.7 means we support Colab and
                                  Kaggle env._
  ______________________________________________________________________ ## How
 To Use ### Step 0: Install Simple installation from PyPI ```bash pip install
 pytorch-lightning ```  ### Step 1: Add these imports ```python import os import
 torch from torch import nn import torch.nn.functional as F from
@@ -189,15 +188,15 @@
 Lightning Lite
          [docs/source-pytorch/_static/images/lightning_lite/lite.gif]
 In the Lightning v1.5 release, LightningLite now enables you to leverage all
 the capabilities of PyTorch Lightning Accelerators without any refactoring to
 your training loop. Check out the [blogpost](https://
 devblog.pytorchlightning.ai/scale-your-pytorch-code-with-lightninglite-
 d5692a303f00) and [docs](https://pytorch-lightning.readthedocs.io/en/
-2022.9.22starter/lightning_lite.html) for more info.
+2022.9.8starter/lightning_lite.html) for more info.
 ______________________________________________________________________ ##
 Examples ###### Hello world - [MNIST hello world](https://pytorch-
 lightning.readthedocs.io/en/latest/notebooks/lightning_examples/mnist-hello-
 world.html) ###### Contrastive Learning - [BYOL](https://lightning-
 bolts.readthedocs.io/en/stable/deprecated/models/self_supervised.html#byol) -
 [CPC v2](https://lightning-bolts.readthedocs.io/en/stable/deprecated/models/
 self_supervised.html#cpc-v2) - [Moco v2](https://lightning-
```

### Comparing `lightning-2022.9.22/README.md` & `lightning-2022.9.8/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/setup.cfg` & `lightning-2022.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/setup.py` & `lightning-2022.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/__about__.py` & `lightning-2022.9.8/src/lightning/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/__init__.py` & `lightning-2022.9.8/src/lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/__setup__.py` & `lightning-2022.9.8/src/lightning/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/app/__about__.py` & `lightning-2022.9.8/src/lightning/app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/app/__init__.py` & `lightning-2022.9.8/src/lightning/app/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     from lightning_app import _PROJECT_ROOT  # noqa: F401
     from lightning_app import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/api/http_methods.py` & `lightning-2022.9.8/src/lightning/app/api/http_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 try:
-    from lightning_app.api.http_methods import logger  # noqa: F401
     from lightning_app.api.http_methods import _signature_proxy_function  # noqa: F401
     from lightning_app.api.http_methods import HttpMethod  # noqa: F401
     from lightning_app.api.http_methods import Post  # noqa: F401
     from lightning_app.api.http_methods import Get  # noqa: F401
     from lightning_app.api.http_methods import Put  # noqa: F401
     from lightning_app.api.http_methods import Delete  # noqa: F401
     from lightning_app.api.http_methods import _add_tags_to_api  # noqa: F401
     from lightning_app.api.http_methods import _validate_api  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/api/request_types.py` & `lightning-2022.9.8/src/lightning/app/api/request_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.api.request_types import CommandRequest  # noqa: F401
     from lightning_app.api.request_types import APIRequest  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/cmd_clusters.py` & `lightning-2022.9.8/src/lightning/app/cli/cmd_clusters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 try:
     from lightning_app.cli.cmd_clusters import CLUSTER_STATE_CHECKING_TIMEOUT  # noqa: F401
     from lightning_app.cli.cmd_clusters import MAX_CLUSTER_WAIT_TIME  # noqa: F401
-    from lightning_app.cli.cmd_clusters import ClusterList  # noqa: F401
     from lightning_app.cli.cmd_clusters import AWSClusterManager  # noqa: F401
+    from lightning_app.cli.cmd_clusters import ClusterList  # noqa: F401
     from lightning_app.cli.cmd_clusters import _wait_for_cluster_state  # noqa: F401
     from lightning_app.cli.cmd_clusters import _check_cluster_name_is_valid  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/cmd_install.py` & `lightning-2022.9.8/src/lightning/app/cli/cmd_install.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
+
     from lightning_app.cli.cmd_install import logger  # noqa: F401
     from lightning_app.cli.cmd_install import gallery_component  # noqa: F401
     from lightning_app.cli.cmd_install import non_gallery_component  # noqa: F401
     from lightning_app.cli.cmd_install import gallery_app  # noqa: F401
     from lightning_app.cli.cmd_install import non_gallery_app  # noqa: F401
     from lightning_app.cli.cmd_install import _show_install_component_prompt  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/cmd_pl_init.py` & `lightning-2022.9.8/src/lightning/app/cli/cmd_pl_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 try:
     from lightning_app.cli.cmd_pl_init import _REPORT_HELP_TEXTS  # noqa: F401
     from lightning_app.cli.cmd_pl_init import _REPORT_IGNORE_PATTERNS  # noqa: F401
     from lightning_app.cli.cmd_pl_init import pl_app  # noqa: F401
     from lightning_app.cli.cmd_pl_init import download_frontend  # noqa: F401
     from lightning_app.cli.cmd_pl_init import project_file_from_template  # noqa: F401
     from lightning_app.cli.cmd_pl_init import print_pretty_report  # noqa: F401
-    from lightning_app.cli.cmd_pl_init import _can_encode_icon  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/commands/app_commands.py` & `lightning-2022.9.8/src/lightning/app/cli/commands/app_commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,9 +3,9 @@
     from lightning_app.cli.commands.app_commands import _handle_command_without_client  # noqa: F401
     from lightning_app.cli.commands.app_commands import _handle_command_with_client  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/commands/connection.py` & `lightning-2022.9.8/src/lightning/app/cli/commands/connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from lightning_app.cli.commands.connection import _resolve_command_path  # noqa: F401
     from lightning_app.cli.commands.connection import _list_app_commands  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/cli/lightning_cli.py` & `lightning-2022.9.8/src/lightning/app/cli/lightning_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     from lightning_app.cli.lightning_cli import init_react_ui  # noqa: F401
     from lightning_app.cli.lightning_cli import _prepare_file  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/components/python/tracer.py` & `lightning-2022.9.8/src/lightning/app/components/python/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.components.python.tracer import TracerPythonScript  # noqa: F401
     from lightning_app.components.python.tracer import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/components/serve/serve.py` & `lightning-2022.9.8/src/lightning/app/components/serve/serve.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from lightning_app.components.serve.serve import maybe_create_instance  # noqa: F401
     from lightning_app.components.serve.serve import instance  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/components/training.py` & `lightning-2022.9.8/src/lightning/app/frontend/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 try:
-    from lightning_app.components.training import _logger  # noqa: F401
-    from lightning_app.components.training import PyTorchLightningScriptRunner  # noqa: F401
-    from lightning_app.components.training import LightningTrainingComponent  # noqa: F401
+    from lightning_app.frontend.frontend import Frontend
+    from lightning_app.frontend.panel import PanelFrontend
+    from lightning_app.frontend.stream_lit import StreamlitFrontend
+    from lightning_app.frontend.web import StaticWebFrontend
+
+    from lightning_app.frontend import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/core/api.py` & `lightning-2022.9.8/src/lightning/app/core/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,21 @@
     from lightning_app.core.api import openapi_tags  # noqa: F401
     from lightning_app.core.api import app  # noqa: F401
     from lightning_app.core.api import fastapi_service  # noqa: F401
     from lightning_app.core.api import get_state  # noqa: F401
     from lightning_app.core.api import get_spec  # noqa: F401
     from lightning_app.core.api import post_delta  # noqa: F401
     from lightning_app.core.api import post_state  # noqa: F401
-    from lightning_app.core.api import upload_file  # noqa: F401
     from lightning_app.core.api import healthz  # noqa: F401
     from lightning_app.core.api import websocket_endpoint  # noqa: F401
     from lightning_app.core.api import api_catch_all  # noqa: F401
     from lightning_app.core.api import frontend_route  # noqa: F401
     from lightning_app.core.api import register_global_routes  # noqa: F401
     from lightning_app.core.api import LightningUvicornServer  # noqa: F401
     from lightning_app.core.api import start_server  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/core/constants.py` & `lightning-2022.9.8/src/lightning/app/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,17 @@
     from lightning_app.core.constants import FRONTEND_DIR  # noqa: F401
     from lightning_app.core.constants import PACKAGE_LIGHTNING  # noqa: F401
     from lightning_app.core.constants import CLOUD_UPLOAD_WARNING  # noqa: F401
     from lightning_app.core.constants import DISABLE_DEPENDENCY_CACHE  # noqa: F401
     from lightning_app.core.constants import LIGHTNING_CLOUD_PROJECT_ID  # noqa: F401
     from lightning_app.core.constants import LIGHTNING_CREDENTIAL_PATH  # noqa: F401
     from lightning_app.core.constants import DOT_IGNORE_FILENAME  # noqa: F401
-    from lightning_app.core.constants import DEBUG_ENABLED  # noqa: F401
     from lightning_app.core.constants import LIGHTNING_COMPONENT_PUBLIC_REGISTRY  # noqa: F401
     from lightning_app.core.constants import LIGHTNING_APPS_PUBLIC_REGISTRY  # noqa: F401
-    from lightning_app.core.constants import ENABLE_STATE_WEBSOCKET  # noqa: F401
-    from lightning_app.core.constants import DEBUG  # noqa: F401
     from lightning_app.core.constants import get_lightning_cloud_url  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/core/queues.py` & `lightning-2022.9.8/src/lightning/app/core/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     from lightning_app.core.queues import MultiProcessQueue  # noqa: F401
     from lightning_app.core.queues import RedisQueue  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/frontend/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/deepspeed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 try:
-    from lightning_app.frontend.frontend import Frontend
-    from lightning_app.frontend.panel import PanelFrontend
-    from lightning_app.frontend.stream_lit import StreamlitFrontend
-    from lightning_app.frontend.web import StaticWebFrontend
 
-    from lightning_app.frontend import __all__  # noqa: F401
+    from pytorch_lightning.utilities.deepspeed import CPU_DEVICE  # noqa: F401
+    from pytorch_lightning.utilities.deepspeed import ds_checkpoint_dir  # noqa: F401
+    from pytorch_lightning.utilities.deepspeed import convert_zero_checkpoint_to_fp32_state_dict  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
-    from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    from pytorch_lightning import __version__
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/frontend/panel/app_state_comm.py` & `lightning-2022.9.8/src/lightning/app/frontend/panel/app_state_comm.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     from lightning_app.frontend.panel.app_state_comm import _start_websocket  # noqa: F401
     from lightning_app.frontend.panel.app_state_comm import watch_app_state  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/frontend/panel/panel_frontend.py` & `lightning-2022.9.8/src/lightning/app/frontend/panel/panel_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.frontend.panel.panel_frontend import PanelFrontend  # noqa: F401
     from lightning_app.frontend.panel.panel_frontend import _get_allowed_hosts  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/frontend/panel/panel_serve_render_fn.py` & `lightning-2022.9.8/src/lightning/app/frontend/panel/panel_serve_render_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,9 +3,9 @@
     from lightning_app.frontend.panel.panel_serve_render_fn import _get_render_fn  # noqa: F401
     from lightning_app.frontend.panel.panel_serve_render_fn import main  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/frontend/web.py` & `lightning-2022.9.8/src/lightning/app/frontend/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
         from lightning_app.frontend.web import parser  # noqa: F401
         from lightning_app.frontend.web import args  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/runners/__init__.py` & `lightning-2022.9.8/src/lightning/app/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
     from lightning_app.runners import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/runners/backends/__init__.py` & `lightning-2022.9.8/src/lightning/app/runners/backends/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 
     from lightning_app.runners.backends import BackendType  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/source_code/copytree.py` & `lightning-2022.9.8/src/lightning/app/source_code/copytree.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from lightning_app.source_code.copytree import _read_lightningignore  # noqa: F401
     from lightning_app.source_code.copytree import _ignore_filename_spell_check  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/source_code/tar.py` & `lightning-2022.9.8/src/lightning/app/source_code/tar.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from lightning_app.source_code.tar import _tar_path_python  # noqa: F401
     from lightning_app.source_code.tar import _tar_path_subprocess  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/storage/copier.py` & `lightning-2022.9.8/src/lightning/app/storage/copier.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from lightning_app.storage.copier import _find_matching_path  # noqa: F401
     from lightning_app.storage.copier import copy_files  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/storage/orchestrator.py` & `lightning-2022.9.8/src/lightning/app/storage/orchestrator.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.storage.orchestrator import _logger  # noqa: F401
     from lightning_app.storage.orchestrator import StorageOrchestrator  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/storage/path.py` & `lightning-2022.9.8/src/lightning/app/storage/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     from lightning_app.storage.path import path_to_work_artifact  # noqa: F401
     from lightning_app.storage.path import filesystem  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/storage/requests.py` & `lightning-2022.9.8/src/lightning/app/storage/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.storage.requests import ExistsRequest  # noqa: F401
     from lightning_app.storage.requests import ExistsResponse  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/testing/helpers.py` & `lightning-2022.9.8/src/lightning/app/testing/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from lightning_app.testing.helpers import EmptyFlow  # noqa: F401
     from lightning_app.testing.helpers import EmptyWork  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/testing/testing.py` & `lightning-2022.9.8/src/lightning/app/testing/testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 try:
-    from lightning_app.testing.testing import _on_error_callback  # noqa: F401
-    from lightning_app.testing.testing import print_logs  # noqa: F401
+    from lightning_app.testing.testing import _logger  # noqa: F401
     from lightning_app.testing.testing import LightningTestApp  # noqa: F401
     from lightning_app.testing.testing import application_testing  # noqa: F401
     from lightning_app.testing.testing import SingleWorkFlow  # noqa: F401
     from lightning_app.testing.testing import run_work_isolated  # noqa: F401
     from lightning_app.testing.testing import browser_context_args  # noqa: F401
     from lightning_app.testing.testing import run_cli  # noqa: F401
     from lightning_app.testing.testing import run_app_in_cloud  # noqa: F401
     from lightning_app.testing.testing import wait_for  # noqa: F401
     from lightning_app.testing.testing import delete_cloud_lightning_apps  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/app_helpers.py` & `lightning-2022.9.8/src/lightning/app/utilities/app_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     from lightning_app.utilities.app_helpers import _delta_to_app_state_delta  # noqa: F401
     from lightning_app.utilities.app_helpers import _walk_to_component  # noqa: F401
     from lightning_app.utilities.app_helpers import _collect_child_process_pids  # noqa: F401
     from lightning_app.utilities.app_helpers import _print_to_logger_info  # noqa: F401
     from lightning_app.utilities.app_helpers import convert_print_to_logger_info  # noqa: F401
     from lightning_app.utilities.app_helpers import pretty_state  # noqa: F401
     from lightning_app.utilities.app_helpers import LightningJSONEncoder  # noqa: F401
-    from lightning_app.utilities.app_helpers import Logger  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/app_logs.py` & `lightning-2022.9.8/src/lightning/app/utilities/app_logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.utilities.app_logs import _push_log_events_to_read_queue_callback  # noqa: F401
     from lightning_app.utilities.app_logs import _app_logs_reader  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/cli_helpers.py` & `lightning-2022.9.8/src/lightning/app/utilities/cli_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from lightning_app.utilities.cli_helpers import _retrieve_application_url_and_available_commands  # noqa: F401
     from lightning_app.utilities.cli_helpers import _arrow_time_callback  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/cluster_logs.py` & `lightning-2022.9.8/src/lightning/app/utilities/cluster_logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 try:
     from lightning_app.utilities.cluster_logs import _ClusterLogEventLabels  # noqa: F401
     from lightning_app.utilities.cluster_logs import _ClusterLogEvent  # noqa: F401
     from lightning_app.utilities.cluster_logs import _push_log_events_to_read_queue_callback  # noqa: F401
-    from lightning_app.utilities.cluster_logs import _parse_log_event  # noqa: F401
     from lightning_app.utilities.cluster_logs import _cluster_logs_reader  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/commands/base.py` & `lightning-2022.9.8/src/lightning/app/utilities/commands/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     from lightning_app.utilities.commands.base import _collect_open_api_extras  # noqa: F401
     from lightning_app.utilities.commands.base import _commands_to_api  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/component.py` & `lightning-2022.9.8/src/lightning/app/utilities/component.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     from lightning_app.utilities.component import _set_flow_context  # noqa: F401
     from lightning_app.utilities.component import _set_work_context  # noqa: F401
     from lightning_app.utilities.component import _set_frontend_context  # noqa: F401
     from lightning_app.utilities.component import _is_flow_context  # noqa: F401
     from lightning_app.utilities.component import _is_work_context  # noqa: F401
     from lightning_app.utilities.component import _is_frontend_context  # noqa: F401
     from lightning_app.utilities.component import _context  # noqa: F401
-    from lightning_app.utilities.component import _validate_root_flow  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/enum.py` & `lightning-2022.9.8/src/lightning/app/utilities/enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     from lightning_app.utilities.enum import CacheCallsKeys  # noqa: F401
     from lightning_app.utilities.enum import OpenAPITags  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/exceptions.py` & `lightning-2022.9.8/src/lightning/app/utilities/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     from lightning_app.utilities.exceptions import LightningComponentException  # noqa: F401
     from lightning_app.utilities.exceptions import InvalidPathException  # noqa: F401
     from lightning_app.utilities.exceptions import LightningFlowException  # noqa: F401
     from lightning_app.utilities.exceptions import LightningWorkException  # noqa: F401
     from lightning_app.utilities.exceptions import LightningPlatformException  # noqa: F401
     from lightning_app.utilities.exceptions import LightningAppStateException  # noqa: F401
     from lightning_app.utilities.exceptions import LightningSigtermStateException  # noqa: F401
-    from lightning_app.utilities.exceptions import LogLinesLimitExceeded  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/git.py` & `lightning-2022.9.8/src/lightning/app/utilities/packaging/app_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 try:
-    from lightning_app.utilities.git import execute_git_command  # noqa: F401
-    from lightning_app.utilities.git import get_dir_name  # noqa: F401
-    from lightning_app.utilities.git import check_github_repository  # noqa: F401
-    from lightning_app.utilities.git import get_git_relative_path  # noqa: F401
-    from lightning_app.utilities.git import check_if_remote_head_is_different  # noqa: F401
-    from lightning_app.utilities.git import has_uncommitted_files  # noqa: F401
+    from lightning_app.utilities.packaging.app_config import _APP_CONFIG_FILENAME  # noqa: F401
+    from lightning_app.utilities.packaging.app_config import AppConfig  # noqa: F401
+    from lightning_app.utilities.packaging.app_config import find_config_file  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/imports.py` & `lightning-2022.9.8/src/lightning/app/utilities/imports.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     from lightning_app.utilities.imports import _is_s3fs_available  # noqa: F401
     from lightning_app.utilities.imports import _CLOUD_TEST_RUN  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/introspection.py` & `lightning-2022.9.8/src/lightning/app/utilities/introspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     from lightning_app.utilities.introspection import _is_init_context  # noqa: F401
     from lightning_app.utilities.introspection import _is_run_context  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/load_app.py` & `lightning-2022.9.8/src/lightning/app/utilities/load_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from lightning_app.utilities.load_app import component_to_metadata  # noqa: F401
     from lightning_app.utilities.load_app import extract_metadata_from_app  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/login.py` & `lightning-2022.9.8/src/lightning/app/utilities/logs_socket_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 try:
-    from lightning_app.utilities.login import logger  # noqa: F401
-    from lightning_app.utilities.login import Keys  # noqa: F401
-    from lightning_app.utilities.login import Auth  # noqa: F401
-    from lightning_app.utilities.login import AuthServer  # noqa: F401
+    from lightning_app.utilities.logs_socket_api import _LogsSocketAPI  # noqa: F401
+    from lightning_app.utilities.logs_socket_api import _LightningLogsSocketAPI  # noqa: F401
+    from lightning_app.utilities.logs_socket_api import _ClusterLogsSocketAPI  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/logs_socket_api.py` & `lightning-2022.9.8/src/lightning/pytorch/accelerators/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 try:
-    from lightning_app.utilities.logs_socket_api import _LogsSocketAPI  # noqa: F401
-    from lightning_app.utilities.logs_socket_api import _LightningLogsSocketAPI  # noqa: F401
-    from lightning_app.utilities.logs_socket_api import _ClusterLogsSocketAPI  # noqa: F401
+
+    from pytorch_lightning.accelerators.registry import _AcceleratorRegistry  # noqa: F401
+    from pytorch_lightning.accelerators.registry import AcceleratorRegistry  # noqa: F401
+    from pytorch_lightning.accelerators.registry import call_register_accelerators  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
-    from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    from pytorch_lightning import __version__
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/network.py` & `lightning-2022.9.8/src/lightning/app/utilities/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     from lightning_app.utilities.network import _MethodsWrapper  # noqa: F401
     from lightning_app.utilities.network import LightningClient  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/openapi.py` & `lightning-2022.9.8/src/lightning/app/utilities/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.utilities.openapi import is_openapi  # noqa: F401
     from lightning_app.utilities.openapi import create_openapi_object  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/packaging/app_config.py` & `lightning-2022.9.8/src/lightning/app/components/training.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
-    from lightning_app.utilities.packaging.app_config import _APP_CONFIG_FILENAME  # noqa: F401
-    from lightning_app.utilities.packaging.app_config import AppConfig  # noqa: F401
-    from lightning_app.utilities.packaging.app_config import find_config_file  # noqa: F401
+    from lightning_app.components.training import _logger  # noqa: F401
+    from lightning_app.components.training import PyTorchLightningScriptRunner  # noqa: F401
+    from lightning_app.components.training import LightningTrainingComponent  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/packaging/build_config.py` & `lightning-2022.9.8/src/lightning/app/utilities/packaging/build_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,9 +3,9 @@
     from lightning_app.utilities.packaging.build_config import load_requirements  # noqa: F401
     from lightning_app.utilities.packaging.build_config import BuildConfig  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/packaging/lightning_utils.py` & `lightning-2022.9.8/src/lightning/app/utilities/packaging/lightning_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     from lightning_app.utilities.packaging.lightning_utils import _fetch_latest_version  # noqa: F401
     from lightning_app.utilities.packaging.lightning_utils import _verify_lightning_version  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/proxies.py` & `lightning-2022.9.8/src/lightning/app/utilities/proxies.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     from lightning_app.utilities.proxies import WorkRunner  # noqa: F401
     from lightning_app.utilities.proxies import persist_artifacts  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/state.py` & `lightning-2022.9.8/src/lightning/app/utilities/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from lightning_app.utilities.state import headers_for  # noqa: F401
     from lightning_app.utilities.state import AppState  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/app/utilities/tree.py` & `lightning-2022.9.8/src/lightning/app/utilities/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from lightning_app.utilities.tree import _BreadthFirstVisitor  # noqa: F401
     from lightning_app.utilities.tree import _DepthFirstVisitor  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from lightning_app import __version__
-    msg = f'Your `lightning` package was built for `lightning_app==0.6.2`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `lightning_app==0.6.0`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/lite/__about__.py` & `lightning-2022.9.8/src/lightning/lite/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/__init__.py` & `lightning-2022.9.8/src/lightning/lite/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/__init__.py` & `lightning-2022.9.8/src/lightning/lite/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/apply_func.py` & `lightning-2022.9.8/src/lightning/lite/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/data.py` & `lightning-2022.9.8/src/lightning/lite/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/device_parser.py` & `lightning-2022.9.8/src/lightning/lite/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/distributed.py` & `lightning-2022.9.8/src/lightning/lite/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/enums.py` & `lightning-2022.9.8/src/lightning/lite/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/imports.py` & `lightning-2022.9.8/src/lightning/lite/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/rank_zero.py` & `lightning-2022.9.8/src/lightning/lite/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/seed.py` & `lightning-2022.9.8/src/lightning/lite/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/types.py` & `lightning-2022.9.8/src/lightning/lite/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/lite/utilities/xla_device.py` & `lightning-2022.9.8/src/lightning/lite/utilities/xla_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/pytorch/__about__.py` & `lightning-2022.9.8/src/lightning/pytorch/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2022.9.22/src/lightning/pytorch/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
     from pytorch_lightning import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/accelerators/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/accelerators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 
     from pytorch_lightning.accelerators import ACCELERATORS_BASE_MODULE  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/accelerators/cpu.py` & `lightning-2022.9.8/src/lightning/pytorch/accelerators/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from pytorch_lightning.accelerators.cpu import _CPU_SWAP_PERCENT  # noqa: F401
     from pytorch_lightning.accelerators.cpu import get_cpu_stats  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/accelerators/cuda.py` & `lightning-2022.9.8/src/lightning/pytorch/accelerators/cuda.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.accelerators.cuda import get_nvidia_gpu_stats  # noqa: F401
     from pytorch_lightning.accelerators.cuda import _get_gpu_id  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/accelerators/mps.py` & `lightning-2022.9.8/src/lightning/pytorch/accelerators/mps.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.accelerators.mps import _SWAP_PERCENT  # noqa: F401
     from pytorch_lightning.accelerators.mps import get_device_stats  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/accelerators/registry.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/optimization/manual_loop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 try:
 
-    from pytorch_lightning.accelerators.registry import _AcceleratorRegistry  # noqa: F401
-    from pytorch_lightning.accelerators.registry import AcceleratorRegistry  # noqa: F401
-    from pytorch_lightning.accelerators.registry import call_register_accelerators  # noqa: F401
+    from pytorch_lightning.loops.optimization.manual_loop import ManualResult  # noqa: F401
+    from pytorch_lightning.loops.optimization.manual_loop import _OUTPUTS_TYPE  # noqa: F401
+    from pytorch_lightning.loops.optimization.manual_loop import ManualOptimization  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
     from pytorch_lightning.callbacks import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/device_stats_monitor.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/device_stats_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.callbacks.device_stats_monitor import _prefix_metric_keys  # noqa: F401
     from pytorch_lightning.callbacks.device_stats_monitor import prefix_metric_keys  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/finetuning.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/finetuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.callbacks.finetuning import BaseFinetuning  # noqa: F401
     from pytorch_lightning.callbacks.finetuning import BackboneFinetuning  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/model_checkpoint.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/model_checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.callbacks.model_checkpoint import warning_cache  # noqa: F401
     from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.callbacks.progress.rich_progress import RichProgressBar  # noqa: F401
     from pytorch_lightning.callbacks.progress.tqdm_progress import TQDMProgressBar  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/rich_progress.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/rich_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     from pytorch_lightning.callbacks.progress.rich_progress import RichProgressBar  # noqa: F401
     from pytorch_lightning.callbacks.progress.rich_progress import _detect_light_colab_theme  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/progress/tqdm_progress.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/progress/tqdm_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from pytorch_lightning.callbacks.progress.tqdm_progress import convert_inf  # noqa: F401
     from pytorch_lightning.callbacks.progress.tqdm_progress import _update_n  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/pruning.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/pruning.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.callbacks.pruning import _LayerRef  # noqa: F401
     from pytorch_lightning.callbacks.pruning import ModelPruning  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/callbacks/quantization.py` & `lightning-2022.9.8/src/lightning/pytorch/callbacks/quantization.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.callbacks.quantization import _recursive_hasattr  # noqa: F401
     from pytorch_lightning.callbacks.quantization import QuantizationAwareTraining  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/cli.py` & `lightning-2022.9.8/src/lightning/pytorch/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     from pytorch_lightning.cli import instantiate_class  # noqa: F401
     from pytorch_lightning.cli import _get_short_description  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/core/optimizer.py` & `lightning-2022.9.8/src/lightning/pytorch/core/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     from pytorch_lightning.core.optimizer import _validate_optim_conf  # noqa: F401
     from pytorch_lightning.core.optimizer import _MockOptimizer  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/core/saving.py` & `lightning-2022.9.8/src/lightning/pytorch/core/saving.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     from pytorch_lightning.core.saving import save_hparams_to_yaml  # noqa: F401
     from pytorch_lightning.core.saving import convert  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/demos/boring_classes.py` & `lightning-2022.9.8/src/lightning/pytorch/demos/boring_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     from pytorch_lightning.demos.boring_classes import DemoModel  # noqa: F401
     from pytorch_lightning.demos.boring_classes import Net  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/demos/mnist_datamodule.py` & `lightning-2022.9.8/src/lightning/pytorch/demos/mnist_datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.demos.mnist_datamodule import MNIST  # noqa: F401
     from pytorch_lightning.demos.mnist_datamodule import MNISTDataModule  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/lite/wrappers.py` & `lightning-2022.9.8/src/lightning/pytorch/lite/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.lite.wrappers import _LiteModule  # noqa: F401
     from pytorch_lightning.lite.wrappers import _LiteDataLoader  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 
         os.environ["COMET_DISABLE_AUTO_LOGGING"] = "1"
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/base.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.loggers.base import DummyLogger  # noqa: F401
     from pytorch_lightning.loggers.base import merge_dicts  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/logger.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.loggers.logger import DummyLogger  # noqa: F401
     from pytorch_lightning.loggers.logger import merge_dicts  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/mlflow.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/mlflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.loggers.mlflow import _MLFLOW_AVAILABLE  # noqa: F401
     from pytorch_lightning.loggers.mlflow import MLFlowLogger  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/neptune.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/neptune.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.loggers.neptune import _LEGACY_NEPTUNE_LOGGER_KWARGS  # noqa: F401
     from pytorch_lightning.loggers.neptune import NeptuneLogger  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loggers/wandb.py` & `lightning-2022.9.8/src/lightning/pytorch/loggers/wandb.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.loggers.wandb import _WANDB_GREATER_EQUAL_0_12_10  # noqa: F401
     from pytorch_lightning.loggers.wandb import WandbLogger  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.loops.fit_loop import FitLoop  # noqa: F401
     from pytorch_lightning.loops.optimization import ManualOptimization, OptimizerLoop  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/dataloader/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/dataloader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.loops.dataloader.evaluation_loop import EvaluationLoop  # noqa: F401
     from pytorch_lightning.loops.dataloader.prediction_loop import PredictionLoop  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/epoch/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/epoch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.loops.epoch.prediction_epoch_loop import PredictionEpochLoop  # noqa: F401
     from pytorch_lightning.loops.epoch.training_epoch_loop import TrainingEpochLoop  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/epoch/training_epoch_loop.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/epoch/training_epoch_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.loops.epoch.training_epoch_loop import _get_max_shape  # noqa: F401
     from pytorch_lightning.loops.epoch.training_epoch_loop import _iterate_nested_array  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/optimization/closure.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/optimization/closure.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.loops.optimization.closure import OutputResult  # noqa: F401
     from pytorch_lightning.loops.optimization.closure import AbstractClosure  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/optimization/manual_loop.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/ddp_spawn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 try:
 
-    from pytorch_lightning.loops.optimization.manual_loop import ManualResult  # noqa: F401
-    from pytorch_lightning.loops.optimization.manual_loop import _OUTPUTS_TYPE  # noqa: F401
-    from pytorch_lightning.loops.optimization.manual_loop import ManualOptimization  # noqa: F401
+    from pytorch_lightning.strategies.ddp_spawn import log  # noqa: F401
+    from pytorch_lightning.strategies.ddp_spawn import _DDP_FORK_ALIASES  # noqa: F401
+    from pytorch_lightning.strategies.ddp_spawn import DDPSpawnStrategy  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/optimization/optimizer_loop.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/optimization/optimizer_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.loops.optimization.optimizer_loop import _OUTPUTS_TYPE  # noqa: F401
     from pytorch_lightning.loops.optimization.optimizer_loop import OptimizerLoop  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/loops/utilities.py` & `lightning-2022.9.8/src/lightning/pytorch/loops/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     from pytorch_lightning.loops.utilities import _v1_8_output_format  # noqa: F401
     from pytorch_lightning.loops.utilities import _set_sampler_epoch  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/overrides/base.py` & `lightning-2022.9.8/src/lightning/pytorch/overrides/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.overrides.base import _LightningModuleWrapperBase  # noqa: F401
     from pytorch_lightning.overrides.base import unwrap_lightning_module  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/overrides/data_parallel.py` & `lightning-2022.9.8/src/lightning/pytorch/overrides/data_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.overrides.data_parallel import python_scalar_to_tensor  # noqa: F401
     from pytorch_lightning.overrides.data_parallel import unsqueeze_scalar_tensor  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/overrides/distributed.py` & `lightning-2022.9.8/src/lightning/pytorch/overrides/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.overrides.distributed import UnrepeatedDistributedSamplerWrapper  # noqa: F401
     from pytorch_lightning.overrides.distributed import IndexBatchSamplerWrapper  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/overrides/fairscale.py` & `lightning-2022.9.8/src/lightning/pytorch/overrides/fairscale.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
         from pytorch_lightning.overrides.fairscale import LightningShardedDataParallel  # noqa: F401
         from pytorch_lightning.overrides.fairscale import unwrap_lightning_module_sharded  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/overrides/torch_distributed.py` & `lightning-2022.9.8/src/lightning/pytorch/overrides/torch_distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         from pytorch_lightning.overrides.torch_distributed import _broadcast_noop  # noqa: F401
         from pytorch_lightning.overrides.torch_distributed import broadcast_object_list  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,9 @@
     from pytorch_lightning.plugins import PLUGIN_INPUT  # noqa: F401
     from pytorch_lightning.plugins import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/environments/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/environments/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.plugins.environments.torchelastic_environment import TorchElasticEnvironment  # noqa: F401
     from pytorch_lightning.plugins.environments.xla_environment import XLAEnvironment  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/io/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 
     from pytorch_lightning.plugins.io import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/layer_sync.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/layer_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.plugins.layer_sync import NativeSyncBatchNorm  # noqa: F401
     from pytorch_lightning.plugins.layer_sync import _BatchNormXd  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/precision/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/precision/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 
     from pytorch_lightning.plugins.precision import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/precision/deepspeed.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/precision/deepspeed.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.plugins.precision.deepspeed import warning_cache  # noqa: F401
     from pytorch_lightning.plugins.precision.deepspeed import DeepSpeedPrecisionPlugin  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/plugins/training_type/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/plugins/training_type/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     from pytorch_lightning.plugins.training_type.tpu_spawn import TPUSpawnPlugin  # noqa: F401
     from pytorch_lightning.plugins.training_type.training_type_plugin import TrainingTypePlugin  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/profiler/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/profiler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 
     from pytorch_lightning.profiler import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/profiler/pytorch.py` & `lightning-2022.9.8/src/lightning/pytorch/profiler/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.profiler.pytorch import ScheduleWrapper  # noqa: F401
     from pytorch_lightning.profiler.pytorch import PyTorchProfiler  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/profilers/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/profilers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
     from pytorch_lightning.profilers import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/profilers/pytorch.py` & `lightning-2022.9.8/src/lightning/pytorch/profilers/pytorch.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.profilers.pytorch import ScheduleWrapper  # noqa: F401
     from pytorch_lightning.profilers.pytorch import PyTorchProfiler  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/profilers/simple.py` & `lightning-2022.9.8/src/lightning/pytorch/profilers/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     from pytorch_lightning.profilers.simple import _TABLE_DATA  # noqa: F401
     from pytorch_lightning.profilers.simple import SimpleProfiler  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/serve/servable_module_validator.py` & `lightning-2022.9.8/src/lightning/pytorch/serve/servable_module_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,9 +3,9 @@
     from pytorch_lightning.serve.servable_module_validator import _logger  # noqa: F401
     from pytorch_lightning.serve.servable_module_validator import ServableModuleValidator  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 
     from pytorch_lightning.strategies import STRATEGIES_BASE_MODULE  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/bagua.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/bagua.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from pytorch_lightning.strategies.bagua import LightningBaguaModule  # noqa: F401
     from pytorch_lightning.strategies.bagua import BaguaStrategy  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/ddp_spawn.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/strategy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 try:
 
-    from pytorch_lightning.strategies.ddp_spawn import log  # noqa: F401
-    from pytorch_lightning.strategies.ddp_spawn import _DDP_FORK_ALIASES  # noqa: F401
-    from pytorch_lightning.strategies.ddp_spawn import DDPSpawnStrategy  # noqa: F401
+    from pytorch_lightning.strategies.strategy import TBroadcast  # noqa: F401
+    from pytorch_lightning.strategies.strategy import TReduce  # noqa: F401
+    from pytorch_lightning.strategies.strategy import log  # noqa: F401
+    from pytorch_lightning.strategies.strategy import Strategy  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/deepspeed.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/deepspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from pytorch_lightning.strategies.deepspeed import LightningDeepSpeedModule  # noqa: F401
     from pytorch_lightning.strategies.deepspeed import DeepSpeedStrategy  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/fully_sharded_native.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 try:
 
-    from pytorch_lightning.strategies.fully_sharded_native import _distributed_available  # noqa: F401
-    from pytorch_lightning.strategies.fully_sharded_native import _fsdp_available  # noqa: F401
-    from pytorch_lightning.strategies.fully_sharded_native import log  # noqa: F401
-    from pytorch_lightning.strategies.fully_sharded_native import DDPFullyShardedNativeStrategy  # noqa: F401
+    from pytorch_lightning.strategies.launchers.base import _Launcher
+    from pytorch_lightning.strategies.launchers.multiprocessing import _MultiProcessingLauncher
+    from pytorch_lightning.strategies.launchers.subprocess_script import _SubprocessScriptLauncher
+    from pytorch_lightning.strategies.launchers.xla import _XLALauncher
+
+    from pytorch_lightning.strategies.launchers import __all__  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/parameter_tying.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 try:
 
-    from pytorch_lightning.strategies.launchers.base import _Launcher
-    from pytorch_lightning.strategies.launchers.multiprocessing import _MultiProcessingLauncher
-    from pytorch_lightning.strategies.launchers.subprocess_script import _SubprocessScriptLauncher
-    from pytorch_lightning.strategies.launchers.xla import _XLALauncher
-
-    from pytorch_lightning.strategies.launchers import __all__  # noqa: F401
+    from pytorch_lightning.utilities.parameter_tying import find_shared_parameters  # noqa: F401
+    from pytorch_lightning.utilities.parameter_tying import _find_shared_parameters  # noqa: F401
+    from pytorch_lightning.utilities.parameter_tying import set_shared_parameters  # noqa: F401
+    from pytorch_lightning.utilities.parameter_tying import _get_module_by_path  # noqa: F401
+    from pytorch_lightning.utilities.parameter_tying import _set_module_by_path  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/launchers/multiprocessing.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/launchers/multiprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     from pytorch_lightning.strategies.launchers.multiprocessing import _GlobalStateSnapshot  # noqa: F401
     from pytorch_lightning.strategies.launchers.multiprocessing import _is_forking_disabled  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/strategy.py` & `lightning-2022.9.8/src/lightning/pytorch/strategies/strategy_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 try:
 
-    from pytorch_lightning.strategies.strategy import TBroadcast  # noqa: F401
-    from pytorch_lightning.strategies.strategy import TReduce  # noqa: F401
-    from pytorch_lightning.strategies.strategy import log  # noqa: F401
-    from pytorch_lightning.strategies.strategy import Strategy  # noqa: F401
+    from pytorch_lightning.strategies.strategy_registry import _StrategyRegistry  # noqa: F401
+    from pytorch_lightning.strategies.strategy_registry import StrategyRegistry  # noqa: F401
+    from pytorch_lightning.strategies.strategy_registry import call_register_strategies  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/strategies/strategy_registry.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/seed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 try:
 
-    from pytorch_lightning.strategies.strategy_registry import _StrategyRegistry  # noqa: F401
-    from pytorch_lightning.strategies.strategy_registry import StrategyRegistry  # noqa: F401
-    from pytorch_lightning.strategies.strategy_registry import call_register_strategies  # noqa: F401
+    from pytorch_lightning.utilities.seed import log  # noqa: F401
+    from pytorch_lightning.utilities.seed import max_seed_value  # noqa: F401
+    from pytorch_lightning.utilities.seed import min_seed_value  # noqa: F401
+    from pytorch_lightning.utilities.seed import seed_everything  # noqa: F401
+    from pytorch_lightning.utilities.seed import _select_seed_randomly  # noqa: F401
+    from pytorch_lightning.utilities.seed import reset_seed  # noqa: F401
+    from pytorch_lightning.utilities.seed import pl_worker_init_function  # noqa: F401
+    from pytorch_lightning.utilities.seed import _collect_rng_states  # noqa: F401
+    from pytorch_lightning.utilities.seed import _set_rng_states  # noqa: F401
+    from pytorch_lightning.utilities.seed import isolate_rng  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/configuration_validator.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/configuration_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.trainer.configuration_validator import _check_datamodule_checkpoint_hooks  # noqa: F401
     from pytorch_lightning.trainer.configuration_validator import _check_setup_method  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/accelerator_connector.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/accelerator_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.trainer.connectors.accelerator_connector import _LITERAL_WARN  # noqa: F401
     from pytorch_lightning.trainer.connectors.accelerator_connector import AcceleratorConnector  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/callback_connector.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/data_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 try:
 
-    from pytorch_lightning.trainer.connectors.callback_connector import _log  # noqa: F401
-    from pytorch_lightning.trainer.connectors.callback_connector import CallbackConnector  # noqa: F401
-    from pytorch_lightning.trainer.connectors.callback_connector import _configure_external_callbacks  # noqa: F401
+    from pytorch_lightning.trainer.connectors.data_connector import warning_cache  # noqa: F401
+    from pytorch_lightning.trainer.connectors.data_connector import DataConnector  # noqa: F401
+    from pytorch_lightning.trainer.connectors.data_connector import _DataLoaderSource  # noqa: F401
+    from pytorch_lightning.trainer.connectors.data_connector import _DataHookSelector  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/data_connector.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/signal_connector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 try:
-
-    from pytorch_lightning.trainer.connectors.data_connector import warning_cache  # noqa: F401
-    from pytorch_lightning.trainer.connectors.data_connector import DataConnector  # noqa: F401
-    from pytorch_lightning.trainer.connectors.data_connector import _DataLoaderSource  # noqa: F401
-    from pytorch_lightning.trainer.connectors.data_connector import _DataHookSelector  # noqa: F401
-    from pytorch_lightning.trainer.connectors.data_connector import _check_dataloader_none  # noqa: F401
+    from pytorch_lightning.trainer.connectors.signal_connector import _SIGNUM  # noqa: F401
+    from pytorch_lightning.trainer.connectors.signal_connector import _HANDLER  # noqa: F401
+    from pytorch_lightning.trainer.connectors.signal_connector import log  # noqa: F401
+    from pytorch_lightning.trainer.connectors.signal_connector import HandlersCompose  # noqa: F401
+    from pytorch_lightning.trainer.connectors.signal_connector import SignalConnector  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/logger_connector/result.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/connectors/logger_connector/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     from pytorch_lightning.trainer.connectors.logger_connector.result import _METRIC_COLLECTION  # noqa: F401
     from pytorch_lightning.trainer.connectors.logger_connector.result import _ResultCollection  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/connectors/signal_connector.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/xla_device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
-    from pytorch_lightning.trainer.connectors.signal_connector import _SIGNUM  # noqa: F401
-    from pytorch_lightning.trainer.connectors.signal_connector import _HANDLER  # noqa: F401
-    from pytorch_lightning.trainer.connectors.signal_connector import log  # noqa: F401
-    from pytorch_lightning.trainer.connectors.signal_connector import HandlersCompose  # noqa: F401
-    from pytorch_lightning.trainer.connectors.signal_connector import SignalConnector  # noqa: F401
+
+    from pytorch_lightning.utilities.xla_device import TPU_CHECK_TIMEOUT  # noqa: F401
+    from pytorch_lightning.utilities.xla_device import inner_f  # noqa: F401
+    from pytorch_lightning.utilities.xla_device import pl_multi_process  # noqa: F401
+    from pytorch_lightning.utilities.xla_device import XLADeviceUtils  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/progress.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     from pytorch_lightning.trainer.progress import OptimizerProgress  # noqa: F401
     from pytorch_lightning.trainer.progress import OptimizationProgress  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/states.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.trainer.states import RunningStage  # noqa: F401
     from pytorch_lightning.trainer.states import TrainerState  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/supporters.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/supporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     from pytorch_lightning.trainer.supporters import CombinedLoaderIterator  # noqa: F401
     from pytorch_lightning.trainer.supporters import _nested_calc_num_data  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/trainer/trainer.py` & `lightning-2022.9.8/src/lightning/pytorch/trainer/trainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     from pytorch_lightning.trainer.trainer import _evaluation_context  # noqa: F401
     from pytorch_lightning.trainer.trainer import _determine_batch_limits  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/tuner/batch_size_scaling.py` & `lightning-2022.9.8/src/lightning/pytorch/tuner/batch_size_scaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     from pytorch_lightning.tuner.batch_size_scaling import _is_valid_batch_size  # noqa: F401
     from pytorch_lightning.tuner.batch_size_scaling import _reset_progress  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/tuner/lr_finder.py` & `lightning-2022.9.8/src/lightning/pytorch/tuner/lr_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.tuner.lr_finder import _LinearLR  # noqa: F401
     from pytorch_lightning.tuner.lr_finder import _ExponentialLR  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
     from pytorch_lightning.utilities import FLOAT32_EPSILON  # noqa: F401
     from pytorch_lightning.utilities import FLOAT64_EPSILON  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/apply_func.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/apply_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     from pytorch_lightning.utilities.apply_func import move_data_to_device  # noqa: F401
     from pytorch_lightning.utilities.apply_func import convert_to_tensors  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/argparse.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     from pytorch_lightning.utilities.argparse import _precision_allowed_type  # noqa: F401
     from pytorch_lightning.utilities.argparse import _defaults_from_env_vars  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/auto_restart.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/auto_restart.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     from pytorch_lightning.utilities.auto_restart import _validate_fault_tolerant_automatic  # noqa: F401
     from pytorch_lightning.utilities.auto_restart import _collect_states_on_rank_zero_over_collection  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/cli.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     from pytorch_lightning.utilities.cli import LightningCLI  # noqa: F401
     from pytorch_lightning.utilities.cli import instantiate_class  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/data.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     from pytorch_lightning.utilities.data import _apply_fault_tolerant_automatic_capture_dataset_wrapper  # noqa: F401
     from pytorch_lightning.utilities.data import _is_dataloader_shuffled  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/deepspeed.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/warnings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 try:
 
-    from pytorch_lightning.utilities.deepspeed import CPU_DEVICE  # noqa: F401
-    from pytorch_lightning.utilities.deepspeed import ds_checkpoint_dir  # noqa: F401
-    from pytorch_lightning.utilities.deepspeed import convert_zero_checkpoint_to_fp32_state_dict  # noqa: F401
+    from pytorch_lightning.utilities.warnings import PossibleUserWarning  # noqa: F401
+    from pytorch_lightning.utilities.warnings import WarningCache  # noqa: F401
+    from pytorch_lightning.utilities.warnings import rank_zero_warn  # noqa: F401
+    from pytorch_lightning.utilities.warnings import rank_zero_deprecation  # noqa: F401
+    from pytorch_lightning.utilities.warnings import LightningDeprecationWarning  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/device_parser.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/device_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     from pytorch_lightning.utilities.device_parser import num_cuda_devices  # noqa: F401
     from pytorch_lightning.utilities.device_parser import is_cuda_available  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/distributed.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     from pytorch_lightning.utilities.distributed import rank_zero_info  # noqa: F401
     from pytorch_lightning.utilities.distributed import rank_zero_debug  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/enums.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     from pytorch_lightning.utilities.enums import _AcceleratorType  # noqa: F401
     from pytorch_lightning.utilities.enums import _FaultTolerantMode  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/exceptions.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.utilities.exceptions import DeadlockDetectedException  # noqa: F401
     from pytorch_lightning.utilities.exceptions import ExitGracefullyException  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/fetching.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/fetching.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     from pytorch_lightning.utilities.fetching import StepFuncDataLoaderIter  # noqa: F401
     from pytorch_lightning.utilities.fetching import DataLoaderIterDataFetcher  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/finite_checks.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/finite_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.utilities.finite_checks import print_nan_gradients  # noqa: F401
     from pytorch_lightning.utilities.finite_checks import detect_nan_parameters  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/imports.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,9 +43,9 @@
         from pytorch_lightning.utilities.imports import _HPU_AVAILABLE  # noqa: F401
     from pytorch_lightning.utilities.imports import _fault_tolerant_training  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/logger.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     from pytorch_lightning.utilities.logger import _name  # noqa: F401
     from pytorch_lightning.utilities.logger import _version  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/memory.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     from pytorch_lightning.utilities.memory import get_gpu_memory_map  # noqa: F401
     from pytorch_lightning.utilities.memory import get_model_size_mb  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/meta.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     from pytorch_lightning.utilities.meta import init_meta_context  # noqa: F401
     from pytorch_lightning.utilities.meta import is_on_meta_device  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/__init__.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     )
     from pytorch_lightning.utilities.model_summary.model_summary_deepspeed import DeepSpeedSummary  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/model_summary.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/model_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     from pytorch_lightning.utilities.model_summary.model_summary import _is_lazy_weight_tensor  # noqa: F401
     from pytorch_lightning.utilities.model_summary.model_summary import summarize  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     from pytorch_lightning.utilities.model_summary.model_summary_deepspeed import DeepSpeedLayerSummary  # noqa: F401
     from pytorch_lightning.utilities.model_summary.model_summary_deepspeed import DeepSpeedSummary  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/parameter_tying.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/rank_zero.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 try:
 
-    from pytorch_lightning.utilities.parameter_tying import find_shared_parameters  # noqa: F401
-    from pytorch_lightning.utilities.parameter_tying import _find_shared_parameters  # noqa: F401
-    from pytorch_lightning.utilities.parameter_tying import set_shared_parameters  # noqa: F401
-    from pytorch_lightning.utilities.parameter_tying import _get_module_by_path  # noqa: F401
-    from pytorch_lightning.utilities.parameter_tying import _set_module_by_path  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import log  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import rank_zero_only  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import _get_rank  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import _info  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import _debug  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import rank_zero_debug  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import rank_zero_info  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import _warn  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import rank_zero_warn  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import LightningDeprecationWarning  # noqa: F401
+    from pytorch_lightning.utilities.rank_zero import rank_zero_deprecation  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/parsing.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     from pytorch_lightning.utilities.parsing import lightning_getattr  # noqa: F401
     from pytorch_lightning.utilities.parsing import lightning_setattr  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/seed.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/upgrade_checkpoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 try:
 
-    from pytorch_lightning.utilities.seed import log  # noqa: F401
-    from pytorch_lightning.utilities.seed import max_seed_value  # noqa: F401
-    from pytorch_lightning.utilities.seed import min_seed_value  # noqa: F401
-    from pytorch_lightning.utilities.seed import seed_everything  # noqa: F401
-    from pytorch_lightning.utilities.seed import _select_seed_randomly  # noqa: F401
-    from pytorch_lightning.utilities.seed import reset_seed  # noqa: F401
-    from pytorch_lightning.utilities.seed import pl_worker_init_function  # noqa: F401
-    from pytorch_lightning.utilities.seed import _collect_rng_states  # noqa: F401
-    from pytorch_lightning.utilities.seed import _set_rng_states  # noqa: F401
-    from pytorch_lightning.utilities.seed import isolate_rng  # noqa: F401
+    from pytorch_lightning.utilities.upgrade_checkpoint import KEYS_MAPPING  # noqa: F401
+    from pytorch_lightning.utilities.upgrade_checkpoint import log  # noqa: F401
+    from pytorch_lightning.utilities.upgrade_checkpoint import upgrade_checkpoint  # noqa: F401
+    if __name__ == "__main__":
+
+        from pytorch_lightning.utilities.upgrade_checkpoint import parser  # noqa: F401
+        from pytorch_lightning.utilities.upgrade_checkpoint import args  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning/pytorch/utilities/types.py` & `lightning-2022.9.8/src/lightning/pytorch/utilities/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     from pytorch_lightning.utilities.types import LRSchedulerType  # noqa: F401
     from pytorch_lightning.utilities.types import LRSchedulerConfig  # noqa: F401
 
 except ImportError as err:
 
     from os import linesep
     from pytorch_lightning import __version__
-    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.6`, but you are running {__version__}'
+    msg = f'Your `lightning` package was built for `pytorch_lightning==1.7.5`, but you are running {__version__}'
     raise type(err)(str(err) + linesep + msg)
```

### Comparing `lightning-2022.9.22/src/lightning.egg-info/PKG-INFO` & `lightning-2022.9.8/src/lightning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2022.9.22
+Version: 2022.9.8
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Download-URL: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -36,30 +36,30 @@
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://www.lightning.ai/">Lightning Gallery</a> •
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2022.9.22">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2022.9.8">Docs</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
 [![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning/release/2022.9.22/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
+[![codecov](https://codecov.io/gh/Lightning-AI/lightning/release/2022.9.8/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.22)](https://pytorch-lightning.readthedocs.io/en/2022.9.22)
+[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.8)](https://pytorch-lightning.readthedocs.io/en/2022.9.8)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
@@ -118,21 +118,21 @@
 
 <center>
 
 |   System / PyTorch ver.    |                                                                                                               1.9                                                                                                               |                                                                                                              1.10                                                                                                               |                                                                                                       1.12 (latest)                                                                                                        |
 | :------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 |  Linux py3.7 \[GPUs\*\*\]  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
 | Linux py3.7 \[TPUs\*\*\*\] |                                       [![CircleCI](https://circleci.com/gh/Lightning-AI/lightning/tree/master.svg?style=svg)](https://circleci.com/gh/Lightning-AI/lightning/tree/master)                                       |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
-|    Linux py3.8 \[IPUs\]    | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(IPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=25&branchName=master) |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
-|    Linux py3.8 \[HPUs\]    |                                                                                                                -                                                                                                                | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(HPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=26&branchName=master) |                                                                                                             -                                                                                                              |
-|  Linux py3.8 (with Conda)  |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |                                                                                                             -                                                                                                              |
-|  Linux py3.9 (with Conda)  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) |
-|      Linux py3.{7,9}       |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
-|       OSX py3.{7,9}        |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
-|     Windows py3.{7,9}      |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|    Linux py3.8 \[IPUs\]    | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(IPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=25&branchName=master) |                                                                                                                -                                                                                                                |                                                                                                             -                                                                                                              |
+|    Linux py3.8 \[HPUs\]    |                                                                                                                -                                                                                                                | [![Build Status](<https://dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20(HPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=26&branchName=master) |                                                                                                             -                                                                                                              |
+|  Linux py3.8 (with Conda)  |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |   [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)    |                                                                                                             -                                                                                                              |
+|  Linux py3.9 (with Conda)  |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) |
+|      Linux py3.{7,9}       |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|       OSX py3.{7,9}        |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
+|     Windows py3.{7,9}      |                                                                                                                -                                                                                                                |                                                                                                                -                                                                                                                |  [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml)  |
 
 - _\*\* tests run on two NVIDIA P100_
 - _\*\*\* tests run on Google GKE TPUv2/3. TPU py3.7 means we support Colab and Kaggle env._
 
 </center>
 </details>
 
@@ -346,15 +346,15 @@
 
 <div align="center">
   <img src="docs/source-pytorch/_static/images/lightning_lite/lite.gif" height="200px" width="600px">
 </div>
 
 In the Lightning v1.5 release, LightningLite now enables you to leverage all the capabilities of PyTorch Lightning Accelerators without any refactoring to your training loop. Check out the
 [blogpost](https://devblog.pytorchlightning.ai/scale-your-pytorch-code-with-lightninglite-d5692a303f00) and
-[docs](https://pytorch-lightning.readthedocs.io/en/2022.9.22starter/lightning_lite.html) for more info.
+[docs](https://pytorch-lightning.readthedocs.io/en/2022.9.8starter/lightning_lite.html) for more info.
 
 ______________________________________________________________________
 
 ## Examples
 
 ###### Hello world
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning Version: 2022.9.22 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning Version: 2022.9.8 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Download-URL: https://github.com/Lightning-AI/lightning Author: Lightning AI et
 al. Author-email: pytorch@lightning.ai License: Apache-2.0 Project-URL: Bug
 Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -31,22 +31,21 @@
  //badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-
 lightning) [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://
 pepy.tech/project/pytorch-lightning) [![Conda](https://img.shields.io/conda/v/
 conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/
   conda-forge/pytorch-lightning) [![DockerHub](https://img.shields.io/docker/
    pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/
     pytorchlightning/pytorch_lightning) [![codecov](https://codecov.io/gh/
-  Lightning-AI/lightning/release/2022.9.22/graph/badge.svg?token=SmzX8mnKlA)]
+  Lightning-AI/lightning/release/2022.9.8/graph/badge.svg?token=SmzX8mnKlA)]
     (https://codecov.io/gh/Lightning-AI/lightning) [![ReadTheDocs](https://
-readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.22)](https://
-       pytorch-lightning.readthedocs.io/en/2022.9.22) [![Slack](https://
-        img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://
- www.pytorchlightning.ai/community) [![license](https://img.shields.io/badge/
-License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/
-                               master/LICENSE)
+ readthedocs.org/projects/pytorch-lightning/badge/?version=2022.9.8)](https://
+pytorch-lightning.readthedocs.io/en/2022.9.8) [![Slack](https://img.shields.io/
+   badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/
+   community) [![license](https://img.shields.io/badge/License-Apache%202.0-
+  blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 ###### \*Codecov is > 90%+ but build delays may show less
 ______________________________________________________________________ ##
 PyTorch Lightning is just organized PyTorch Lightning disentangles PyTorch code
 to decouple the science from the engineering. ![PT to PL](docs/source-pytorch/
 _static/images/general/pl_quick_start_full_compressed.gif) ## Build AI products
 with Lightning Apps Once you're done building models, publish a paper demo or
 build a full production end-to-end ML system with Lightning Apps. Lightning
@@ -84,38 +83,38 @@
 -------------------------------------------------------------------------------
 --------------------------------------------: | | Linux py3.7 \[GPUs\*\*\] | -
 | - | - | | Linux py3.7 \[TPUs\*\*\*\] | [![CircleCI](https://circleci.com/gh/
   Lightning-AI/lightning/tree/master.svg?style=svg)](https://circleci.com/gh/
 Lightning-AI/lightning/tree/master) | - | - | | Linux py3.8 \[IPUs\] | [![Build
                                    Status](
  dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20
- (IPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-
-AI/lightning/_build/latest?definitionId=25&branchName=master) | - | - | | Linux
+(IPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/
+ lightning/_build/latest?definitionId=25&branchName=master) | - | - | | Linux
                     py3.8 \[HPUs\] | - | [![Build Status](
  dev.azure.com/Lightning-AI/lightning/_apis/build/status/pytorch-lightning%20
- (HPUs)?branchName=refs%2Ftags%2F2022.9.22>)](https://dev.azure.com/Lightning-
-  AI/lightning/_build/latest?definitionId=26&branchName=master) | - | | Linux
-   py3.8 (with Conda) | [![Test](https://github.com/Lightning-AI/lightning/
-actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://
+(HPUs)?branchName=refs%2Ftags%2F2022.9.8>)](https://dev.azure.com/Lightning-AI/
+lightning/_build/latest?definitionId=26&branchName=master) | - | | Linux py3.8
+  (with Conda) | [![Test](https://github.com/Lightning-AI/lightning/actions/
+     workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://
 github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)
   | [![Test](https://github.com/Lightning-AI/lightning/actions/workflows/ci-
-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://github.com/Lightning-
+ pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://github.com/Lightning-
 AI/lightning/actions/workflows/ci-pytorch-test-conda.yml) | - | | Linux py3.9
   (with Conda) | - | - | [![Test](https://github.com/Lightning-AI/lightning/
-actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.22)](https://
+ actions/workflows/ci-pytorch-test-conda.yml/badge.svg?tag=2022.9.8)](https://
 github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-conda.yml)
     | | Linux py3.{7,9} | - | - | [![Test](https://github.com/Lightning-AI/
-lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)]
+ lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)]
  (https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-
 full.yml) | | OSX py3.{7,9} | - | - | [![Test](https://github.com/Lightning-AI/
-lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.22)]
+ lightning/actions/workflows/ci-pytorch-test-full.yml/badge.svg?tag=2022.9.8)]
  (https://github.com/Lightning-AI/lightning/actions/workflows/ci-pytorch-test-
     full.yml) | | Windows py3.{7,9} | - | - | [![Test](https://github.com/
       Lightning-AI/lightning/actions/workflows/ci-pytorch-test-full.yml/
- badge.svg?tag=2022.9.22)](https://github.com/Lightning-AI/lightning/actions/
+  badge.svg?tag=2022.9.8)](https://github.com/Lightning-AI/lightning/actions/
  workflows/ci-pytorch-test-full.yml) | - _\*\* tests run on two NVIDIA P100_ -
  _\*\*\* tests run on Google GKE TPUv2/3. TPU py3.7 means we support Colab and
                                  Kaggle env._
  ______________________________________________________________________ ## How
 To Use ### Step 0: Install Simple installation from PyPI ```bash pip install
 pytorch-lightning ```  ### Step 1: Add these imports ```python import os import
 torch from torch import nn import torch.nn.functional as F from
@@ -189,15 +188,15 @@
 Lightning Lite
          [docs/source-pytorch/_static/images/lightning_lite/lite.gif]
 In the Lightning v1.5 release, LightningLite now enables you to leverage all
 the capabilities of PyTorch Lightning Accelerators without any refactoring to
 your training loop. Check out the [blogpost](https://
 devblog.pytorchlightning.ai/scale-your-pytorch-code-with-lightninglite-
 d5692a303f00) and [docs](https://pytorch-lightning.readthedocs.io/en/
-2022.9.22starter/lightning_lite.html) for more info.
+2022.9.8starter/lightning_lite.html) for more info.
 ______________________________________________________________________ ##
 Examples ###### Hello world - [MNIST hello world](https://pytorch-
 lightning.readthedocs.io/en/latest/notebooks/lightning_examples/mnist-hello-
 world.html) ###### Contrastive Learning - [BYOL](https://lightning-
 bolts.readthedocs.io/en/stable/deprecated/models/self_supervised.html#byol) -
 [CPC v2](https://lightning-bolts.readthedocs.io/en/stable/deprecated/models/
 self_supervised.html#cpc-v2) - [Moco v2](https://lightning-
```

### Comparing `lightning-2022.9.22/src/lightning.egg-info/SOURCES.txt` & `lightning-2022.9.8/src/lightning.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 src/lightning/app/utilities/__init__.py
 src/lightning/app/utilities/app_helpers.py
 src/lightning/app/utilities/app_logs.py
 src/lightning/app/utilities/cli_helpers.py
 src/lightning/app/utilities/cloud.py
 src/lightning/app/utilities/cluster_logs.py
 src/lightning/app/utilities/component.py
-src/lightning/app/utilities/data_structures.py
 src/lightning/app/utilities/dependency_caching.py
 src/lightning/app/utilities/enum.py
 src/lightning/app/utilities/exceptions.py
 src/lightning/app/utilities/git.py
 src/lightning/app/utilities/imports.py
 src/lightning/app/utilities/introspection.py
 src/lightning/app/utilities/layout.py
```

