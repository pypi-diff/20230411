# Comparing `tmp/phiterm-1.5.7.tar.gz` & `tmp/phiterm-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.5.7.tar", last modified: Sun Apr  9 21:34:10 2023, max compression
+gzip compressed data, was "phiterm-1.5.8.tar", last modified: Tue Apr 11 01:26:29 2023, max compression
```

## Comparing `phiterm-1.5.7.tar` & `phiterm-1.5.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.182790 phiterm-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-09 21:33:46.000000 phiterm-1.5.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 21:34:10.178790 phiterm-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 21:33:46.000000 phiterm-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.158790 phiterm-1.5.7/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.158790 phiterm-1.5.7/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.158790 phiterm-1.5.7/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.158790 phiterm-1.5.7/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.162790 phiterm-1.5.7/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.166790 phiterm-1.5.7/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.166790 phiterm-1.5.7/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26450 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.166790 phiterm-1.5.7/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.166790 phiterm-1.5.7/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.170790 phiterm-1.5.7/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.154790 phiterm-1.5.7/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.170790 phiterm-1.5.7/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.174790 phiterm-1.5.7/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.174790 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.174790 phiterm-1.5.7/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.174790 phiterm-1.5.7/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.178790 phiterm-1.5.7/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.178790 phiterm-1.5.7/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.178790 phiterm-1.5.7/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12664 2023-04-09 21:33:46.000000 phiterm-1.5.7/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.158790 phiterm-1.5.7/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 21:34:10.000000 phiterm-1.5.7/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-09 21:33:46.000000 phiterm-1.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:34:10.182790 phiterm-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 21:33:46.000000 phiterm-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:10.178790 phiterm-1.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 21:33:46.000000 phiterm-1.5.7/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.570136 phiterm-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-11 01:26:04.000000 phiterm-1.5.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 01:26:29.570136 phiterm-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 01:26:04.000000 phiterm-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.542136 phiterm-1.5.8/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.542136 phiterm-1.5.8/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.546136 phiterm-1.5.8/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26450 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.550136 phiterm-1.5.8/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.554136 phiterm-1.5.8/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.554136 phiterm-1.5.8/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.538136 phiterm-1.5.8/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.554136 phiterm-1.5.8/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.558136 phiterm-1.5.8/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.558136 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.558136 phiterm-1.5.8/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.558136 phiterm-1.5.8/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.562136 phiterm-1.5.8/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.566136 phiterm-1.5.8/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.566136 phiterm-1.5.8/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41711 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12664 2023-04-11 01:26:04.000000 phiterm-1.5.8/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.542136 phiterm-1.5.8/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 01:26:29.000000 phiterm-1.5.8/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 01:26:04.000000 phiterm-1.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:26:29.570136 phiterm-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 01:26:04.000000 phiterm-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:26:29.566136 phiterm-1.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 01:26:04.000000 phiterm-1.5.8/tests/test_backend_api.py
```

### Comparing `phiterm-1.5.7/LICENSE.md` & `phiterm-1.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/api/client.py` & `phiterm-1.5.8/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/api/routes.py` & `phiterm-1.5.8/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/api/user.py` & `phiterm-1.5.8/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/api/workspace.py` & `phiterm-1.5.8/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/aws/aws_operator.py` & `phiterm-1.5.8/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/cli_app.py` & `phiterm-1.5.8/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/cli_operator.py` & `phiterm-1.5.8/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/dx/dx_app.py` & `phiterm-1.5.8/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.5.8/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.5.8/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.5.8/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/wf/wf_app.py` & `phiterm-1.5.8/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/cli/ws/ws_app.py` & `phiterm-1.5.8/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/conf/auth.py` & `phiterm-1.5.8/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/conf/constants.py` & `phiterm-1.5.8/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/conf/phi_conf.py` & `phiterm-1.5.8/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/databox/databox_operator.py` & `phiterm-1.5.8/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/docker/docker_operator.py` & `phiterm-1.5.8/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/enums/user.py` & `phiterm-1.5.8/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/k8s/k8s_operator.py` & `phiterm-1.5.8/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.5.8/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.5.8/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.5.8/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.5.8/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/local/local_operator.py` & `phiterm-1.5.8/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/release/release_schemas.py` & `phiterm-1.5.8/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/release/ws_releases.py` & `phiterm-1.5.8/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/schemas/user.py` & `phiterm-1.5.8/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/schemas/user_schemas.py` & `phiterm-1.5.8/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/schemas/workspace.py` & `phiterm-1.5.8/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.5.8/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.5.8/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.5.8/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.5.8/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.5.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.5.8/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.5.8/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.5.8/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/cli_auth_server.py` & `phiterm-1.5.8/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/cli_console.py` & `phiterm-1.5.8/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/common.py` & `phiterm-1.5.8/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/dttm.py` & `phiterm-1.5.8/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/enums.py` & `phiterm-1.5.8/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/filesystem.py` & `phiterm-1.5.8/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/git.py` & `phiterm-1.5.8/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/load_env.py` & `phiterm-1.5.8/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/log.py` & `phiterm-1.5.8/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/pyproject.py` & `phiterm-1.5.8/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/utils/ws_filter.py` & `phiterm-1.5.8/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workflow/wf_operator.py` & `phiterm-1.5.8/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workflow/wf_utils.py` & `phiterm-1.5.8/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workspace/phi_ws_data.py` & `phiterm-1.5.8/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workspace/ws_enums.py` & `phiterm-1.5.8/phiterm/workspace/ws_enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 class WorkspaceVisibilityEnum(ExtendedEnum):
     PRIVATE = "PRIVATE"
     PUBLIC = "PUBLIC"
 
 
 class WorkspaceStarterTemplate(ExtendedEnum):
+    ai_app = "ai-app"
+    ml_app = "ml-app"
     duck_gpt = "duck-gpt"
-    aws_ai_app = "aws-ai-app"
-    aws_ml_api = "aws-ml-api"
     aws_dp = "aws-data-platform"
     aws_spark_dp = "aws-spark-data-platform"
     aws_snowflake_dp = "aws-snowflake-data-platform"
 
 
 class WorkspaceEnv(ExtendedEnum):
     dev = "dev"
```

### Comparing `phiterm-1.5.7/phiterm/workspace/ws_loader.py` & `phiterm-1.5.8/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workspace/ws_operator.py` & `phiterm-1.5.8/phiterm/workspace/ws_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     WorkspaceStarterTemplate,
 )
 from phiterm.workspace.exceptions import WorkspaceConfigException
 
 # List of reserved workspace names
 RESERVED_WS_NAMES = ["root", "bedi", "ashpreet", "ashpreetbedi"]
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
+    WorkspaceStarterTemplate.ai_app: "ai-app",
+    WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.duck_gpt: "duck-gpt",
-    WorkspaceStarterTemplate.aws_ai_app: "ai-app",
-    WorkspaceStarterTemplate.aws_ml_api: "ml-api",
     WorkspaceStarterTemplate.aws_dp: "data-platform",
     WorkspaceStarterTemplate.aws_spark_dp: "spark-data-platform",
     WorkspaceStarterTemplate.aws_snowflake_dp: "snowflake-data-platform",
 }
 TEMPLATE_TO_REPO_MAP: Dict[WorkspaceStarterTemplate, str] = {
+    WorkspaceStarterTemplate.ai_app: "https://github.com/phidatahq/ai-app.git",
+    WorkspaceStarterTemplate.ml_app: "https://github.com/phidatahq/ml-app.git",
     WorkspaceStarterTemplate.duck_gpt: "https://github.com/phidatahq/duck-gpt.git",
-    WorkspaceStarterTemplate.aws_ai_app: "https://github.com/phidatahq/aws-ai-app-template.git",
-    WorkspaceStarterTemplate.aws_ml_api: "https://github.com/phidatahq/aws-ml-api-template.git",
     WorkspaceStarterTemplate.aws_dp: "https://github.com/phidatahq/aws-dp-template.git",
     WorkspaceStarterTemplate.aws_spark_dp: "https://github.com/phidatahq/aws-spark-dp-template.git",
     WorkspaceStarterTemplate.aws_snowflake_dp: "https://github.com/phidatahq/aws-snowflake-dp-template.git",
 }
 
 
 def create_new_workspace(ws_name: str, template: WorkspaceStarterTemplate) -> bool:
@@ -157,24 +157,24 @@
 
 def create_workspace_using_input():
     """Takes input from the user and calls create_new_workspace()"""
 
     from phiterm.utils.common import is_empty, str_to_int
 
     # Display available starter templates and ask user to select one
-    print_info("Select Template (default: duck-gpt)")
+    print_info("Input Template Number (default: ai-app)")
     templates = WorkspaceStarterTemplate.values_list()
     for idx, prvdr in enumerate(templates, start=1):
         print_info("  [{}] {}".format(idx, prvdr))
 
     # Get starter template from the user
     template_inp_raw = input(": ")
     # Convert input to int value.
     template_inp = str_to_int(template_inp_raw)
-    template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.duck_gpt
+    template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.ai_app
 
     if template_inp is not None:
         try:
             template = cast(
                 WorkspaceStarterTemplate,
                 WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
             )
```

### Comparing `phiterm-1.5.7/phiterm/workspace/ws_schemas.py` & `phiterm-1.5.8/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm/workspace/ws_utils.py` & `phiterm-1.5.8/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/phiterm.egg-info/SOURCES.txt` & `phiterm-1.5.8/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.7/pyproject.toml` & `phiterm-1.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.5.7"
+version = "1.5.8"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

