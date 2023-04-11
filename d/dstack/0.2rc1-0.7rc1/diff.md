# Comparing `tmp/dstack-0.2rc1.tar.gz` & `tmp/dstack-0.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.2rc1.tar", last modified: Tue Mar  7 07:58:35 2023, max compression
+gzip compressed data, was "dstack-0.7rc1.tar", last modified: Tue Apr 11 14:42:51 2023, max compression
```

## Comparing `dstack-0.2rc1.tar` & `dstack-0.7rc1.tar`

### file list

```diff
@@ -1,184 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.365079 dstack-0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-03-07 07:58:02.000000 dstack-0.2rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-07 07:58:35.365079 dstack-0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-07 07:58:02.000000 dstack-0.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.349079 dstack-0.2rc1/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.349079 dstack-0.2rc1/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/api/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22337 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26901 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.353079 dstack-0.2rc1/cli/dstack/backend/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/hub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/hub/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/pull/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/pull/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/push/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/push/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.357079 dstack-0.2rc1/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/core/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/repository/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/repository/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/repository/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/routers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-07 07:58:02.000000 dstack-0.2rc1/cli/dstack/hub/security/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    16893 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.361079 dstack-0.2rc1/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.365079 dstack-0.2rc1/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.365079 dstack-0.2rc1/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.365079 dstack-0.2rc1/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.349079 dstack-0.2rc1/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-07 07:58:35.000000 dstack-0.2rc1/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:35.365079 dstack-0.2rc1/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:58:03.000000 dstack-0.2rc1/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 07:58:35.365079 dstack-0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-03-07 07:58:03.000000 dstack-0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-04-11 14:42:02.000000 dstack-0.7rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.143200 dstack-0.7rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 14:42:02.000000 dstack-0.7rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/pull/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/pull/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/push/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/push/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 14:42:50.000000 dstack-0.7rc1/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:42:51.143200 dstack-0.7rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-11 14:42:02.000000 dstack-0.7rc1/setup.py
```

### Comparing `dstack-0.2rc1/LICENSE.md` & `dstack-0.7rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/PKG-INFO` & `dstack-0.7rc1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.2rc1
-Summary: Easy-to-run ML workflows on any cloud
+Version: 0.7rc1
+Summary: The hassle-free tool for managing ML workflows on any cloud platform.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,134 +20,147 @@
 <h1 align="center">
   <a target="_blank" href="https://dstack.ai">
     <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
   </a>
 </h1>
 
 <h4 align="center">
-Easy-to-run ML workflows on any cloud
+Automate your ML workflows on any cloud
 </h4>
 
 <p align="center">
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within teams. 
+The hassle-free tool for managing ML workflows on any cloud platform. 
 </p>
 
-[![Slack](https://img.shields.io/badge/slack-join%20community-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
+[![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://docs.dstack.ai" target="_blank"><b>Docs</b></a> • 
 <a href="https://docs.dstack.ai/quick-start"><b>Quick start</b></a> • 
-<a href="https://docs.dstack.ai/basics/hello-world" target="_blank"><b>Basics</b></a> • 
-<a href="https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ" target="_blank"><b>Slack</b></a> 
+<a href="https://docs.dstack.ai/playground" target="_blank"><b>Playground</b></a> •   
+<a href="https://docs.dstack.ai/setup"><b>Setup</b></a> • 
+<a href="https://docs.dstack.ai/usage/hello-world" target="_blank"><b>Usage</b></a>  • 
+<a href="https://docs.dstack.ai/examples/tensorboard" target="_blank"><b>Examples</b></a>
 </p>
 
 [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)](https://github.com/dstackai/dstack/commits/)
 [![PyPI - License](https://img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/dstackai/dstack/blob/master/LICENSE.md)
 
 </div>
 
-`dstack` is the most easy way to define ML workflows as code and run them either locally or remotely on any cloud.
+## What is dstack?
 
-### Highlighted features
+`dstack` is an open-source tool that automates ML workflows, enabling effective management on any cloud platform. 
 
-* Define ML workflows declaratively as code
-* Run workflows locally or remotely on any cloud (AWS, GCP, etc)
-* Use on-demand on spot instances conveniently
-* Save data, checkpoints, environments as artifacts and reuse them across workflows
-* No need to use custom Docker images or Kubernetes
+It empowers your team to prepare data, train, and fine-tune models using their preferred frameworks and dev
+environments without spending time on engineering and infrastructure.
 
-## Installation
+## Install the CLI
 
-Use pip to install the `dstack` CLI:
+Use `pip` to install `dstack`:
 
 ```shell
-pip install dstack --upgrade
+pip install dstack
 ```
 
-## Example
+## Configure a remote
 
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
+By default, workflows run locally. To run workflows remotely (e.g. in a configured cloud account),
+configure a remote using the `dstack config` command.
+
+```shell
+dstack config
+
+? Choose backend. Use arrows to move, type to filter
+> [aws]
+  [gcp]
+  [hub]
+```
+
+Choose [`hub`](https://docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and settings through a user
+interface while working in a team.
+
+For running remote workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/setup/aws.md)
+or [`gcp`](https://docs.dstack.ai/setup/gcp.md).
+
+## Define workflows
+
+Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
 
 ```yaml
 workflows:
-  - name: mnist-data
-    provider: bash
-    commands:
-      - pip install torchvision
-      - python mnist/mnist_data.py
-    artifacts:
-      - path: ./data
-
   - name: train-mnist
     provider: bash
-    deps:
-      - workflow: mnist-data
     commands:
       - pip install torchvision pytorch-lightning tensorboard
-      - python mnist/train_mnist.py
+      - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-YAML-defined workflows eliminate the need to modify code in your scripts, giving you the freedom to choose frameworks,
-experiment trackers, and cloud providers.
-
 ## Run locally
 
-Use the `dstack` CLI to run workflows locally:
+By default, workflows run locally on your machine.
 
 ```shell
-dstack run mnist-data
+dstack run train-mnist
+
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
+
+Provisioning... It may take up to a minute. ✓
+
+To interrupt, press Ctrl+C.
+
+GPU available: True, used: True
+
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
 ## Run remotely
 
-To run workflows remotely (e.g. in the cloud) or share artifacts outside your machine, 
-you must configure your remote settings using the `dstack config` command:
+To run a workflow remotely (e.g. in a configured cloud account), add the `--remote` flag to the `dstack run` command:
+
+The necessary hardware resources can be configured either via YAML or through arguments in the `dstack run` command, such
+as `--gpu` and `--gpu-name`.
 
 ```shell
-dstack config
-```
+dstack run train-mnist --remote --gpu 1
 
-This command will ask you to choose the type of backend (e.g. AWS), and the corresponding
-settings (e.g. the region where to run workflows, an S3 bucket where to store artifacts, etc).
+RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+turtle-1  train-mnist  now        Submitted       aws
 
-```shell
-Backend: aws
-AWS profile: default
-AWS region: eu-west-1
-S3 bucket: dstack-142421590066-eu-west-1
-EC2 subnet: none
-```
+Provisioning... It may take up to a minute. ✓
 
-For more details on how to configure a remote, check the [installation](https://docs.dstack.ai/installation/#configure-a-remote) guide.
+To interrupt, press Ctrl+C.
 
-Once a remote is configured, use the `--remote` flag with the `dstack run` command to run the 
-workflow in the configured cloud:
+GPU available: True, used: True
 
-```shell
-dstack run mnist-data --remote
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-You can configure the required resources to run the workflows either via the `resources` property in YAML
-or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`, etc:
+Upon running a workflow remotely, `dstack` automatically creates resources in the configured cloud account and destroys them
+once the workflow is complete.
 
-```shell
-dstack run train-mnist --remote --gpu 1
-```
+## Providers
+
+`dstack` supports multiple [providers](https://docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch interactive development environments and applications.
+
+## Artifacts
 
-When you run a workflow remotely, `dstack` automatically creates resources in the configured cloud,
-and releases them once the workflow is finished.
+`dstack` allows you to save output artifacts and conveniently reuse them across workflows.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Docs](https://docs.dstack.ai/)
-* [Installation](https://docs.dstack.ai/installation)
 * [Quick start](https://docs.dstack.ai/quick-start)
-* [Basics](https://docs.dstack.ai/basics/hello-world)
+* [Playground](https://github.com/dstackai/dstack-playground)
+* [Setup](https://docs.dstack.ai/setup)
+* [Usage](https://docs.dstack.ai/usage/hello-world)
+* [Examples](https://docs.dstack.ai/examples/tensorboard)
  
 ##  Licence
 
 [Mozilla Public License 2.0](LICENSE.md)
```

#### html2text {}

```diff
@@ -1,56 +1,61 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.2rc1 Summary: Easy-to-run ML
-workflows on any cloud Home-page: https://dstack.ai Author: Andrey Cheptsov
-Author-email: andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://
-github.com/dstackai/dstack Platform: UNKNOWN Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: Mozilla Public License 2.0
-(MPL 2.0) Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dstack Version: 0.7rc1 Summary: The hassle-free
+tool for managing ML workflows on any cloud platform. Home-page: https://
+dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
+UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
+UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE.md
                             ****** [dstack] ******
-                 *** Easy-to-run ML workflows on any cloud ***
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within
-                                    teams.
-        [![Slack](https://img.shields.io/badge/slack-join%20community-
+                *** Automate your ML workflows on any cloud ***
+     The hassle-free tool for managing ML workflows on any cloud platform.
+           [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
-                   Docs â¢ Quick_start â¢ Basics â¢ Slack
+     Docs â¢ Quick_start â¢ Playground â¢ Setup â¢ Usage â¢ Examples
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
-`dstack` is the most easy way to define ML workflows as code and run them
-either locally or remotely on any cloud. ### Highlighted features * Define ML
-workflows declaratively as code * Run workflows locally or remotely on any
-cloud (AWS, GCP, etc) * Use on-demand on spot instances conveniently * Save
-data, checkpoints, environments as artifacts and reuse them across workflows *
-No need to use custom Docker images or Kubernetes ## Installation Use pip to
-install the `dstack` CLI: ```shell pip install dstack --upgrade ``` ## Example
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
-```yaml workflows: - name: mnist-data provider: bash commands: - pip install
-torchvision - python mnist/mnist_data.py artifacts: - path: ./data - name:
-train-mnist provider: bash deps: - workflow: mnist-data commands: - pip install
-torchvision pytorch-lightning tensorboard - python mnist/train_mnist.py
-artifacts: - path: ./lightning_logs ``` YAML-defined workflows eliminate the
-need to modify code in your scripts, giving you the freedom to choose
-frameworks, experiment trackers, and cloud providers. ## Run locally Use the
-`dstack` CLI to run workflows locally: ```shell dstack run mnist-data ``` ##
-Run remotely To run workflows remotely (e.g. in the cloud) or share artifacts
-outside your machine, you must configure your remote settings using the `dstack
-config` command: ```shell dstack config ``` This command will ask you to choose
-the type of backend (e.g. AWS), and the corresponding settings (e.g. the region
-where to run workflows, an S3 bucket where to store artifacts, etc). ```shell
-Backend: aws AWS profile: default AWS region: eu-west-1 S3 bucket: dstack-
-142421590066-eu-west-1 EC2 subnet: none ``` For more details on how to
-configure a remote, check the [installation](https://docs.dstack.ai/
-installation/#configure-a-remote) guide. Once a remote is configured, use the
-`--remote` flag with the `dstack run` command to run the workflow in the
-configured cloud: ```shell dstack run mnist-data --remote ``` You can configure
-the required resources to run the workflows either via the `resources` property
-in YAML or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`,
-etc: ```shell dstack run train-mnist --remote --gpu 1 ``` When you run a
-workflow remotely, `dstack` automatically creates resources in the configured
-cloud, and releases them once the workflow is finished. ## More information For
-additional information and examples, see the following links: * [Docs](https://
-docs.dstack.ai/) * [Installation](https://docs.dstack.ai/installation) * [Quick
-start](https://docs.dstack.ai/quick-start) * [Basics](https://docs.dstack.ai/
-basics/hello-world) ## Licence [Mozilla Public License 2.0](LICENSE.md)
+## What is dstack? `dstack` is an open-source tool that automates ML workflows,
+enabling effective management on any cloud platform. It empowers your team to
+prepare data, train, and fine-tune models using their preferred frameworks and
+dev environments without spending time on engineering and infrastructure. ##
+Install the CLI Use `pip` to install `dstack`: ```shell pip install dstack ```
+## Configure a remote By default, workflows run locally. To run workflows
+remotely (e.g. in a configured cloud account), configure a remote using the
+`dstack config` command. ```shell dstack config ? Choose backend. Use arrows to
+move, type to filter > [aws] [gcp] [hub] ``` Choose [`hub`](https://
+docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and
+settings through a user interface while working in a team. For running remote
+workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/
+setup/aws.md) or [`gcp`](https://docs.dstack.ai/setup/gcp.md). ## Define
+workflows Define ML workflows, their output artifacts, hardware requirements,
+and dependencies via YAML. ```yaml workflows: - name: train-mnist provider:
+bash commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run
+locally By default, workflows run locally on your machine. ```shell dstack run
+train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist
+now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` ## Run remotely To run a workflow remotely
+(e.g. in a configured cloud account), add the `--remote` flag to the `dstack
+run` command: The necessary hardware resources can be configured either via
+YAML or through arguments in the `dstack run` command, such as `--gpu` and `--
+gpu-name`. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW
+SUBMITTED STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws
+Provisioning... It may take up to a minute. â To interrupt, press Ctrl+C. GPU
+available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35,
+v_num=0] ``` Upon running a workflow remotely, `dstack` automatically creates
+resources in the configured cloud account and destroys them once the workflow
+is complete. ## Providers `dstack` supports multiple [providers](https://
+docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch
+interactive development environments and applications. ## Artifacts `dstack`
+allows you to save output artifacts and conveniently reuse them across
+workflows. ## More information For additional information and examples, see the
+following links: * [Docs](https://docs.dstack.ai/) * [Quick start](https://
+docs.dstack.ai/quick-start) * [Playground](https://github.com/dstackai/dstack-
+playground) * [Setup](https://docs.dstack.ai/setup) * [Usage](https://
+docs.dstack.ai/usage/hello-world) * [Examples](https://docs.dstack.ai/examples/
+tensorboard) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.2rc1/README.md` & `dstack-0.7rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,133 +5,146 @@
       <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo-dark.svg"/>
       <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
     </picture>
   </a>
 </h1>
 
 <h4 align="center">
-Easy-to-run ML workflows on any cloud
+Automate your ML workflows on any cloud
 </h4>
 
 <p align="center">
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within teams. 
+The hassle-free tool for managing ML workflows on any cloud platform. 
 </p>
 
-[![Slack](https://img.shields.io/badge/slack-join%20community-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
+[![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://docs.dstack.ai" target="_blank"><b>Docs</b></a> • 
 <a href="https://docs.dstack.ai/quick-start"><b>Quick start</b></a> • 
-<a href="https://docs.dstack.ai/basics/hello-world" target="_blank"><b>Basics</b></a> • 
-<a href="https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ" target="_blank"><b>Slack</b></a> 
+<a href="https://docs.dstack.ai/playground" target="_blank"><b>Playground</b></a> •   
+<a href="https://docs.dstack.ai/setup"><b>Setup</b></a> • 
+<a href="https://docs.dstack.ai/usage/hello-world" target="_blank"><b>Usage</b></a>  • 
+<a href="https://docs.dstack.ai/examples/tensorboard" target="_blank"><b>Examples</b></a>
 </p>
 
 [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)](https://github.com/dstackai/dstack/commits/)
 [![PyPI - License](https://img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/dstackai/dstack/blob/master/LICENSE.md)
 
 </div>
 
-`dstack` is the most easy way to define ML workflows as code and run them either locally or remotely on any cloud.
+## What is dstack?
 
-### Highlighted features
+`dstack` is an open-source tool that automates ML workflows, enabling effective management on any cloud platform. 
 
-* Define ML workflows declaratively as code
-* Run workflows locally or remotely on any cloud (AWS, GCP, etc)
-* Use on-demand on spot instances conveniently
-* Save data, checkpoints, environments as artifacts and reuse them across workflows
-* No need to use custom Docker images or Kubernetes
+It empowers your team to prepare data, train, and fine-tune models using their preferred frameworks and dev
+environments without spending time on engineering and infrastructure.
 
-## Installation
+## Install the CLI
 
-Use pip to install the `dstack` CLI:
+Use `pip` to install `dstack`:
 
 ```shell
-pip install dstack --upgrade
+pip install dstack
 ```
 
-## Example
+## Configure a remote
 
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
+By default, workflows run locally. To run workflows remotely (e.g. in a configured cloud account),
+configure a remote using the `dstack config` command.
+
+```shell
+dstack config
+
+? Choose backend. Use arrows to move, type to filter
+> [aws]
+  [gcp]
+  [hub]
+```
+
+Choose [`hub`](https://docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and settings through a user
+interface while working in a team.
+
+For running remote workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/setup/aws.md)
+or [`gcp`](https://docs.dstack.ai/setup/gcp.md).
+
+## Define workflows
+
+Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
 
 ```yaml
 workflows:
-  - name: mnist-data
-    provider: bash
-    commands:
-      - pip install torchvision
-      - python mnist/mnist_data.py
-    artifacts:
-      - path: ./data
-
   - name: train-mnist
     provider: bash
-    deps:
-      - workflow: mnist-data
     commands:
       - pip install torchvision pytorch-lightning tensorboard
-      - python mnist/train_mnist.py
+      - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-YAML-defined workflows eliminate the need to modify code in your scripts, giving you the freedom to choose frameworks,
-experiment trackers, and cloud providers.
-
 ## Run locally
 
-Use the `dstack` CLI to run workflows locally:
+By default, workflows run locally on your machine.
 
 ```shell
-dstack run mnist-data
+dstack run train-mnist
+
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
+
+Provisioning... It may take up to a minute. ✓
+
+To interrupt, press Ctrl+C.
+
+GPU available: True, used: True
+
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
 ## Run remotely
 
-To run workflows remotely (e.g. in the cloud) or share artifacts outside your machine, 
-you must configure your remote settings using the `dstack config` command:
+To run a workflow remotely (e.g. in a configured cloud account), add the `--remote` flag to the `dstack run` command:
+
+The necessary hardware resources can be configured either via YAML or through arguments in the `dstack run` command, such
+as `--gpu` and `--gpu-name`.
 
 ```shell
-dstack config
-```
+dstack run train-mnist --remote --gpu 1
 
-This command will ask you to choose the type of backend (e.g. AWS), and the corresponding
-settings (e.g. the region where to run workflows, an S3 bucket where to store artifacts, etc).
+RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+turtle-1  train-mnist  now        Submitted       aws
 
-```shell
-Backend: aws
-AWS profile: default
-AWS region: eu-west-1
-S3 bucket: dstack-142421590066-eu-west-1
-EC2 subnet: none
-```
+Provisioning... It may take up to a minute. ✓
 
-For more details on how to configure a remote, check the [installation](https://docs.dstack.ai/installation/#configure-a-remote) guide.
+To interrupt, press Ctrl+C.
 
-Once a remote is configured, use the `--remote` flag with the `dstack run` command to run the 
-workflow in the configured cloud:
+GPU available: True, used: True
 
-```shell
-dstack run mnist-data --remote
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-You can configure the required resources to run the workflows either via the `resources` property in YAML
-or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`, etc:
+Upon running a workflow remotely, `dstack` automatically creates resources in the configured cloud account and destroys them
+once the workflow is complete.
 
-```shell
-dstack run train-mnist --remote --gpu 1
-```
+## Providers
+
+`dstack` supports multiple [providers](https://docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch interactive development environments and applications.
+
+## Artifacts
 
-When you run a workflow remotely, `dstack` automatically creates resources in the configured cloud,
-and releases them once the workflow is finished.
+`dstack` allows you to save output artifacts and conveniently reuse them across workflows.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Docs](https://docs.dstack.ai/)
-* [Installation](https://docs.dstack.ai/installation)
 * [Quick start](https://docs.dstack.ai/quick-start)
-* [Basics](https://docs.dstack.ai/basics/hello-world)
+* [Playground](https://github.com/dstackai/dstack-playground)
+* [Setup](https://docs.dstack.ai/setup)
+* [Usage](https://docs.dstack.ai/usage/hello-world)
+* [Examples](https://docs.dstack.ai/examples/tensorboard)
  
 ##  Licence
 
 [Mozilla Public License 2.0](LICENSE.md)
```

#### html2text {}

```diff
@@ -1,48 +1,52 @@
                            ****** __[dstack]_ ******
-                 *** Easy-to-run ML workflows on any cloud ***
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within
-                                    teams.
-        [![Slack](https://img.shields.io/badge/slack-join%20community-
+                *** Automate your ML workflows on any cloud ***
+     The hassle-free tool for managing ML workflows on any cloud platform.
+           [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
-                   Docs â¢ Quick_start â¢ Basics â¢ Slack
+     Docs â¢ Quick_start â¢ Playground â¢ Setup â¢ Usage â¢ Examples
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
-`dstack` is the most easy way to define ML workflows as code and run them
-either locally or remotely on any cloud. ### Highlighted features * Define ML
-workflows declaratively as code * Run workflows locally or remotely on any
-cloud (AWS, GCP, etc) * Use on-demand on spot instances conveniently * Save
-data, checkpoints, environments as artifacts and reuse them across workflows *
-No need to use custom Docker images or Kubernetes ## Installation Use pip to
-install the `dstack` CLI: ```shell pip install dstack --upgrade ``` ## Example
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
-```yaml workflows: - name: mnist-data provider: bash commands: - pip install
-torchvision - python mnist/mnist_data.py artifacts: - path: ./data - name:
-train-mnist provider: bash deps: - workflow: mnist-data commands: - pip install
-torchvision pytorch-lightning tensorboard - python mnist/train_mnist.py
-artifacts: - path: ./lightning_logs ``` YAML-defined workflows eliminate the
-need to modify code in your scripts, giving you the freedom to choose
-frameworks, experiment trackers, and cloud providers. ## Run locally Use the
-`dstack` CLI to run workflows locally: ```shell dstack run mnist-data ``` ##
-Run remotely To run workflows remotely (e.g. in the cloud) or share artifacts
-outside your machine, you must configure your remote settings using the `dstack
-config` command: ```shell dstack config ``` This command will ask you to choose
-the type of backend (e.g. AWS), and the corresponding settings (e.g. the region
-where to run workflows, an S3 bucket where to store artifacts, etc). ```shell
-Backend: aws AWS profile: default AWS region: eu-west-1 S3 bucket: dstack-
-142421590066-eu-west-1 EC2 subnet: none ``` For more details on how to
-configure a remote, check the [installation](https://docs.dstack.ai/
-installation/#configure-a-remote) guide. Once a remote is configured, use the
-`--remote` flag with the `dstack run` command to run the workflow in the
-configured cloud: ```shell dstack run mnist-data --remote ``` You can configure
-the required resources to run the workflows either via the `resources` property
-in YAML or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`,
-etc: ```shell dstack run train-mnist --remote --gpu 1 ``` When you run a
-workflow remotely, `dstack` automatically creates resources in the configured
-cloud, and releases them once the workflow is finished. ## More information For
-additional information and examples, see the following links: * [Docs](https://
-docs.dstack.ai/) * [Installation](https://docs.dstack.ai/installation) * [Quick
-start](https://docs.dstack.ai/quick-start) * [Basics](https://docs.dstack.ai/
-basics/hello-world) ## Licence [Mozilla Public License 2.0](LICENSE.md)
+## What is dstack? `dstack` is an open-source tool that automates ML workflows,
+enabling effective management on any cloud platform. It empowers your team to
+prepare data, train, and fine-tune models using their preferred frameworks and
+dev environments without spending time on engineering and infrastructure. ##
+Install the CLI Use `pip` to install `dstack`: ```shell pip install dstack ```
+## Configure a remote By default, workflows run locally. To run workflows
+remotely (e.g. in a configured cloud account), configure a remote using the
+`dstack config` command. ```shell dstack config ? Choose backend. Use arrows to
+move, type to filter > [aws] [gcp] [hub] ``` Choose [`hub`](https://
+docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and
+settings through a user interface while working in a team. For running remote
+workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/
+setup/aws.md) or [`gcp`](https://docs.dstack.ai/setup/gcp.md). ## Define
+workflows Define ML workflows, their output artifacts, hardware requirements,
+and dependencies via YAML. ```yaml workflows: - name: train-mnist provider:
+bash commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run
+locally By default, workflows run locally on your machine. ```shell dstack run
+train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist
+now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` ## Run remotely To run a workflow remotely
+(e.g. in a configured cloud account), add the `--remote` flag to the `dstack
+run` command: The necessary hardware resources can be configured either via
+YAML or through arguments in the `dstack run` command, such as `--gpu` and `--
+gpu-name`. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW
+SUBMITTED STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws
+Provisioning... It may take up to a minute. â To interrupt, press Ctrl+C. GPU
+available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35,
+v_num=0] ``` Upon running a workflow remotely, `dstack` automatically creates
+resources in the configured cloud account and destroys them once the workflow
+is complete. ## Providers `dstack` supports multiple [providers](https://
+docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch
+interactive development environments and applications. ## Artifacts `dstack`
+allows you to save output artifacts and conveniently reuse them across
+workflows. ## More information For additional information and examples, see the
+following links: * [Docs](https://docs.dstack.ai/) * [Quick start](https://
+docs.dstack.ai/quick-start) * [Playground](https://github.com/dstackai/dstack-
+playground) * [Setup](https://docs.dstack.ai/setup) * [Usage](https://
+docs.dstack.ai/usage/hello-world) * [Examples](https://docs.dstack.ai/examples/
+tensorboard) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.2rc1/cli/dstack/api/artifacts.py` & `dstack-0.7rc1/cli/dstack/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/backend.py` & `dstack-0.7rc1/cli/dstack/api/backend.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/config.py` & `dstack-0.7rc1/cli/dstack/api/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/logs.py` & `dstack-0.7rc1/cli/dstack/api/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/repo.py` & `dstack-0.7rc1/cli/dstack/api/repo.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/run.py` & `dstack-0.7rc1/cli/dstack/api/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/api/tags.py` & `dstack-0.7rc1/cli/dstack/api/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/aws/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from pathlib import Path
-from typing import Any, Dict, Generator, List, Optional
+from typing import Generator, List, Optional
 
 import boto3
 from botocore.client import BaseClient
 
 from dstack.backend.aws import config, logs
 from dstack.backend.aws.compute import AWSCompute
 from dstack.backend.aws.config import AWSConfig, AWSConfigurator
 from dstack.backend.aws.secrets import AWSSecretsManager
 from dstack.backend.aws.storage import AWSStorage
 from dstack.backend.base import CloudBackend
 from dstack.backend.base import artifacts as base_artifacts
+from dstack.backend.base import cache as base_cache
 from dstack.backend.base import jobs as base_jobs
 from dstack.backend.base import repos as base_repos
 from dstack.backend.base import runs as base_runs
 from dstack.backend.base import secrets as base_secrets
 from dstack.backend.base import tags as base_tags
 from dstack.core.artifact import Artifact
-from dstack.core.config import BackendConfig
 from dstack.core.error import ConfigError
-from dstack.core.job import Job, JobHead
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
+from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 
 
 class AwsBackend(CloudBackend):
-
     _session: Optional[boto3.Session] = None
     backend_config: AWSConfig
 
     @property
     def name(self):
         return "aws"
 
@@ -118,16 +117,16 @@
 
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         return base_jobs.get_job(self._storage, repo_address, job_id)
 
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         return base_jobs.list_jobs(self._storage, repo_address, run_name)
 
-    def run_job(self, job: Job):
-        base_jobs.run_job(self._storage, self._compute, job)
+    def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
+        base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         base_jobs.stop_job(self._storage, self._compute, repo_address, job_id, abort)
 
     def list_job_heads(
         self, repo_address: RepoAddress, run_name: Optional[str] = None
     ) -> List[JobHead]:
@@ -137,18 +136,23 @@
         base_jobs.delete_job_head(self._storage, repo_address, job_id)
 
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         job_heads = self.list_job_heads(repo_address, run_name)
         return base_runs.get_run_heads(
-            self._storage, self._compute, job_heads, include_request_heads
+            self._storage,
+            self._compute,
+            job_heads,
+            include_request_heads,
+            interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
         repo_address: RepoAddress,
         job_heads: List[JobHead],
         start_time: int,
@@ -169,21 +173,23 @@
         return base_artifacts.list_run_artifact_files(self._storage, repo_address, run_name)
 
     def download_run_artifact_files(
         self,
         repo_address: RepoAddress,
         run_name: str,
         output_dir: Optional[str],
+        files_path: Optional[str] = None,
     ):
         artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
             repo_address=repo_address,
             artifacts=artifacts,
             output_dir=output_dir,
+            files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
         repo_address: RepoAddress,
         job_id: str,
         artifact_name: str,
@@ -230,14 +236,17 @@
             local_dirs,
             self.type,
         )
 
     def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
         base_tags.delete_tag(self._storage, repo_address, tag_head)
 
+    def list_repo_heads(self) -> List[RepoHead]:
+        return base_repos.list_repo_heads(self._storage)
+
     def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
         base_repos.update_repo_last_run_at(
             self._storage,
             repo_address,
             last_run_at,
         )
 
@@ -285,7 +294,10 @@
         return self._storage.get_signed_download_url(object_key)
 
     def get_signed_upload_url(self, object_key: str) -> str:
         return self._storage.get_signed_upload_url(object_key)
 
     def get_configurator(self):
         return AWSConfigurator()
+
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_address, username, workflow_name)
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/compute.py` & `dstack-0.7rc1/cli/dstack/backend/aws/compute.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             region_name=self.region_name,
             subnet_id=self.subnet_id,
             runner_id=job.runner_id,
             instance_type=instance_type,
             local_repo_user_name=job.local_repo_user_name,
             local_repo_user_email=job.local_repo_user_email,
             repo_address=job.repo_address,
+            ssh_key_pub=job.ssh_key_pub,
         )
 
     def terminate_instance(self, request_id: str):
         runners.terminate_instance(
             ec2_client=self.ec2_client,
             request_id=request_id,
         )
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/config.py` & `dstack-0.7rc1/cli/dstack/backend/aws/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 import json
 import os
 import re
+from argparse import Namespace
 from pathlib import Path
 from typing import Dict, Optional
 
 import boto3
+import botocore.exceptions
 import yaml
+from boto3.session import Session
 from botocore.client import BaseClient
 from rich import print
 from rich.prompt import Confirm, Prompt
+from rich_argparse import RichHelpFormatter
 
-from dstack.cli.common import _is_termios_available, ask_choice
+from dstack.cli.common import ask_choice, is_termios_available
 from dstack.core.config import BackendConfig, Configurator, get_config_path
-from dstack.core.error import ConfigError
-from dstack.hub.models import AWSHubValues, HubElement, HubElementValue
+from dstack.core.error import ConfigError, HubConfigError
+from dstack.hub.models import (
+    AWSBucketProjectElement,
+    AWSBucketProjectElementValue,
+    AWSProjectValues,
+    ProjectElement,
+    ProjectElementValue,
+)
 
 regions = [
     ("US East, N. Virginia", "us-east-1"),
     ("US East, Ohio", "us-east-2"),
     ("US West, N. California", "us-west-1"),
     ("US West, Oregon", "us-west-2"),
     ("Asia Pacific, Singapore", "ap-southeast-1"),
@@ -25,14 +35,18 @@
     ("Europe, Frankfurt", "eu-central-1"),
     ("Europe, Ireland", "eu-west-1"),
     ("Europe, London", "eu-west-2"),
     ("Europe, Paris", "eu-west-3"),
     ("Europe, Stockholm", "eu-north-1"),
 ]
 
+_DEFAULT_REGION_NAME = "us-east-1"
+
+cache = {}
+
 
 class AWSConfig(BackendConfig):
     bucket_name = None
     region_name = None
     profile_name = None
     subnet_id = None
     credentials = None
@@ -41,25 +55,25 @@
         self,
         bucket_name: Optional[str] = None,
         region_name: Optional[str] = None,
         profile_name: Optional[str] = None,
         subnet_id: Optional[str] = None,
         credentials: Optional[Dict] = None,
     ):
-        self.bucket_name = bucket_name or os.getenv("DSTACK_AWS_S3_BUCKET") or None
+        self.bucket_name = bucket_name or os.getenv("DSTACK_AWS_S3_BUCKET")
         self.region_name = (
             region_name
             or os.getenv("DSTACK_AWS_REGION")
             or os.getenv("AWS_DEFAULT_REGION")
-            or None
+            or _DEFAULT_REGION_NAME
         )
         self.profile_name = (
-            profile_name or os.getenv("DSTACK_AWS_PROFILE") or os.getenv("AWS_PROFILE") or None
+            profile_name or os.getenv("DSTACK_AWS_PROFILE") or os.getenv("AWS_PROFILE")
         )
-        self.subnet_id = subnet_id or os.getenv("DSTACK_AWS_EC2_SUBNET") or None
+        self.subnet_id = subnet_id or os.getenv("DSTACK_AWS_EC2_SUBNET")
         self.credentials = credentials
 
     def load(self, path: Path = get_config_path()):
         if path.exists():
             with path.open() as f:
                 config_data = yaml.load(f, Loader=yaml.FullLoader)
                 if config_data.get("backend") != "aws":
@@ -95,24 +109,29 @@
     def serialize_yaml(self) -> str:
         return yaml.dump(self.serialize())
 
     def serialize_json(self) -> str:
         return json.dumps(self.serialize())
 
     @classmethod
-    def deserialize(cls, data: Dict) -> Optional["AWSConfig"]:
-        bucket_name = data.get("bucket_name") or data.get("s3_bucket_name")
-        region_name = data.get("region_name")
-        profile_name = data.get("profile_name")
-        subnet_id = data.get("subnet_id") or data.get("ec2_subnet_id") or data.get("subnet")
+    def deserialize(cls, config_data: Dict, auth_data: Dict = None) -> Optional["AWSConfig"]:
+        bucket_name = config_data.get("bucket_name") or config_data.get("s3_bucket_name")
+        region_name = config_data.get("region_name") or _DEFAULT_REGION_NAME
+        profile_name = config_data.get("profile_name")
+        subnet_id = (
+            config_data.get("subnet_id")
+            or config_data.get("ec2_subnet_id")
+            or config_data.get("subnet")
+        )
         return cls(
             bucket_name=bucket_name,
             region_name=region_name,
             profile_name=profile_name,
             subnet_id=subnet_id,
+            credentials=auth_data,
         )
 
     @classmethod
     def deserialize_yaml(cls, yaml_content: str) -> Optional["AWSConfig"]:
         content = yaml.load(yaml_content, yaml.FullLoader)
         if content is None:
             return None
@@ -126,73 +145,136 @@
         return cls.deserialize(content)
 
 
 class AWSConfigurator(Configurator):
     NAME = "aws"
     config: AWSConfig
 
-    def get_config(self, data: Dict) -> Optional[BackendConfig]:
-        return AWSConfig.deserialize(data=data)
+    def get_config_from_hub_config_data(self, config_data: Dict, auth_data: Dict) -> BackendConfig:
+        return AWSConfig.deserialize(config_data, auth_data)
 
-    def parse_args(self, args: list = []):
-        pass
+    def register_parser(self, parser):
+        aws_parser = parser.add_parser("aws", help="", formatter_class=RichHelpFormatter)
+        aws_parser.add_argument("--bucket", type=str, help="", required=True)
+        aws_parser.add_argument("--region", type=str, help="", required=True)
+        aws_parser.add_argument(
+            "--profile",
+            type=str,
+            help="",
+        )
+        aws_parser.add_argument(
+            "--subnet-id",
+            type=str,
+            help="",
+        )
+        aws_parser.set_defaults(func=self._command)
+
+    def _command(self, args: Namespace):
+        config = AWSConfig()
+        config.bucket_name = args.bucket
+        config.region_name = args.region
+        if args.profile is not None:
+            config.profile_name = args.profile
+        if args.subnet_id is not None:
+            config.subnet_id = args.subnet_id
+        config.save()
+        print(f"[grey58]OK[/]")
 
-    def configure_hub(self, data: Dict):
-        # Step 1: create client and check access
-        config = AWSConfig.deserialize(data=data)
+    def configure_hub(self, config_data: Dict) -> AWSProjectValues:
+        config = AWSConfig.deserialize(config_data)
 
-        access_key = data.get("access_key") or ""
-        secret_key = data.get("secret_key") or ""
+        if config.region_name is not None and config.region_name not in {r[1] for r in regions}:
+            raise HubConfigError(f"Invalid AWS region {config.region_name}")
 
         try:
-            session = boto3.session.Session(
-                # profile_name=profile_name,
+            session = Session(
                 region_name=config.region_name,
-                aws_access_key_id=access_key,
-                aws_secret_access_key=secret_key,
+                aws_access_key_id=config_data.get("access_key"),
+                aws_secret_access_key=config_data.get("secret_key"),
             )
-        except Exception as ex:
-            return AWSHubValues()
-        if session is None:
-            return AWSHubValues()
-        hub_values = AWSHubValues()
-        hub_values.region_name = HubElement(selected=config.region_name)
+            sts = session.client("sts")
+            sts.get_caller_identity()
+        except botocore.exceptions.ClientError:
+            raise HubConfigError(
+                "Credentials are not valid",
+                code="invalid_credentials",
+                fields=["access_key", "secret_key"],
+            )
+
+        # TODO validate config values
+        project_values = AWSProjectValues()
+        project_values.region_name = self._get_hub_regions(default_region=config.region_name)
+        project_values.s3_bucket_name = self._get_hub_buckets(
+            session=session, region=config.region_name, default_bucket=config.bucket_name
+        )
+        project_values.ec2_subnet_id = self._get_hub_subnet(
+            session=session, default_subnet=config.subnet_id
+        )
+        return project_values
+
+    def _get_hub_regions(self, default_region: Optional[str]) -> ProjectElement:
+        element = ProjectElement(selected=default_region)
         for r in regions:
-            hub_values.region_name.values.append(HubElementValue(value=r[1], label=r[0]))
-        # Step 2: get bucket list
-        try:
-            _s3 = session.client("s3")
-            response = _s3.list_buckets()
-            hub_values.s3_bucket_name = HubElement(selected=config.bucket_name)
-            for bucket in response["Buckets"]:
-                hub_values.s3_bucket_name.values.append(
-                    HubElementValue(
-                        name=bucket["Name"],
-                        created=bucket["CreationDate"].strftime("%d.%m.%Y %H:%M:%S"),
-                        region=config.region_name,
-                    )
+            element.values.append(ProjectElementValue(value=r[1], label=r[0]))
+        return element
+
+    def _get_hub_buckets(
+        self, session: Session, region: str, default_bucket: Optional[str]
+    ) -> AWSBucketProjectElement:
+        if default_bucket is not None:
+            self._validate_hub_bucket(session=session, region=region, bucket_name=default_bucket)
+        element = AWSBucketProjectElement(selected=default_bucket)
+        s3_client = session.client("s3")
+        response = s3_client.list_buckets()
+        for bucket in response["Buckets"]:
+            element.values.append(
+                AWSBucketProjectElementValue(
+                    name=bucket["Name"],
+                    created=bucket["CreationDate"].strftime("%d.%m.%Y %H:%M:%S"),
+                    region=region,
                 )
-        except Exception as ex:
-            return hub_values
-        # Step 3: get subnet_id list
+            )
+        return element
+
+    def _validate_hub_bucket(self, session: Session, region: str, bucket_name: str):
+        s3_client = session.client("s3")
         try:
-            _ec2 = session.client("ec2")
-            response = _ec2.describe_subnets()
-            hub_values.ec2_subnet_id = HubElement(selected=config.subnet_id)
-            for subnet in response["Subnets"]:
-                hub_values.ec2_subnet_id.values.append(
-                    HubElementValue(
-                        value=subnet["SubnetId"],
-                        label=subnet["SubnetId"],
-                    )
+            response = s3_client.head_bucket(Bucket=bucket_name)
+            bucket_region = response["ResponseMetadata"]["HTTPHeaders"]["x-amz-bucket-region"]
+            if bucket_region.lower() != region:
+                raise HubConfigError(
+                    "The bucket belongs to another AWS region",
+                    code="invalid_bucket",
+                    fields=["s3_bucket_name"],
+                )
+        except botocore.exceptions.ClientError as e:
+            if (
+                hasattr(e, "response")
+                and e.response.get("Error")
+                and e.response["Error"].get("Code") in ["404", "403"]
+            ):
+                raise HubConfigError(
+                    f"The bucket {bucket_name} does not exist",
+                    code="invalid_bucket",
+                    fields=["s3_bucket_name"],
                 )
-        except Exception as ex:
-            return hub_values
+            raise e
 
-        return hub_values
+    def _get_hub_subnet(self, session: Session, default_subnet: Optional[str]) -> ProjectElement:
+        element = ProjectElement(selected=default_subnet)
+        _ec2 = session.client("ec2")
+        response = _ec2.describe_subnets()
+        for subnet in response["Subnets"]:
+            element.values.append(
+                ProjectElementValue(
+                    value=subnet["SubnetId"],
+                    label=subnet["SubnetId"],
+                )
+            )
+        return element
 
     def configure_cli(self):
         self.config = AWSConfig()
         try:
             self.config.load()
         except ConfigError:
             pass
@@ -203,15 +285,15 @@
 
         self.config.profile_name = self._ask_profile_name(default_profile_name)
         if not default_region_name or default_profile_name != self.config.profile_name:
             try:
                 my_session = boto3.session.Session(profile_name=self.config.profile_name)
                 default_region_name = my_session.region_name
             except Exception:
-                default_region_name = "us-east-1"
+                default_region_name = _DEFAULT_REGION_NAME
         self.config.region_name = ask_choice(
             "Choose AWS region",
             [(r[0] + " [" + r[1] + "]") for r in regions],
             [r[1] for r in regions],
             default_region_name,
         )
         if self.config.region_name != default_region_name:
@@ -254,15 +336,15 @@
                     and e.response["Error"].get("Code") == "404"
                 ):
                     if Confirm.ask(
                         f"[sea_green3 bold]?[/sea_green3 bold] "
                         f"[red bold]The bucket doesn't exist. Create it?[/red bold]",
                         default="y",
                     ):
-                        if self.config.region_name != "us-east-1":
+                        if self.config.region_name != _DEFAULT_REGION_NAME:
                             s3_client.create_bucket(
                                 Bucket=bucket_name,
                                 CreateBucketConfiguration={
                                     "LocationConstraint": self.config.region_name
                                 },
                             )
                         else:
@@ -312,15 +394,15 @@
                 default_bucket_name = f"dstack-{account_id}-{self.config.region_name}"
                 bucket_options.append(f"Default [{default_bucket_name}]")
             except Exception:
                 pass
         else:
             bucket_options.append(f"Default [{default_bucket_name}]")
         bucket_options.append("Custom...")
-        if _is_termios_available and len(bucket_options) == 2:
+        if is_termios_available and len(bucket_options) == 2:
             from simple_term_menu import TerminalMenu
 
             print(
                 "[sea_green3 bold]?[/sea_green3 bold] [bold]Choose S3 bucket[/bold] "
                 "[gray46]Use arrows to move, type to filter[/gray46]"
             )
             bucket_menu = TerminalMenu(
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/logs.py` & `dstack-0.7rc1/cli/dstack/backend/aws/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,37 +133,40 @@
     start_time: int,
     attached: bool,
 ) -> Generator[LogEvent, None, None]:
     run_name = job_heads[0].run_name
     filter_logs_events_kwargs = _filter_logs_events_kwargs(
         bucket_name, repo_address, run_name, start_time, end_time=None, next_token=None
     )
+    jobs_cache = {}
     try:
         if attached:
             for event in _filter_log_events_loop(
                 storage,
                 compute,
                 logs_client,
                 repo_address,
                 job_heads,
                 filter_logs_events_kwargs,
             ):
                 yield render_log_message(
                     storage,
                     event,
                     repo_address,
+                    jobs_cache,
                 )
         else:
             paginator = logs_client.get_paginator("filter_log_events")
             for page in paginator.paginate(**filter_logs_events_kwargs):
                 for event in page["events"]:
                     yield render_log_message(
                         storage,
                         event,
                         repo_address,
+                        jobs_cache,
                     )
     except Exception as e:
         if (
             hasattr(e, "response")
             and e.response.get("Error")
             and e.response["Error"].get("Code") == "ResourceNotFoundException"
         ):
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/runners.py` & `dstack-0.7rc1/cli/dstack/backend/aws/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import time
 from functools import reduce
 from typing import List, Optional, Tuple
 
+import botocore.exceptions
 from botocore.client import BaseClient
 
 from dstack import version
-from dstack.backend.base.compute import choose_instance_type
+from dstack.backend.base.compute import NoCapacityError, choose_instance_type
 from dstack.core.instance import InstanceType
-from dstack.core.job import Job, JobStatus, Requirements
+from dstack.core.job import Job, Requirements
 from dstack.core.repo import RepoAddress
 from dstack.core.request import RequestHead, RequestStatus
 from dstack.core.runners import Gpu, Resources
 
 CREATE_INSTANCE_RETRY_RATE_SECS = 3
 
 
@@ -101,29 +102,20 @@
                 },
             ],
             **group_specification,
         )
         security_group_id = security_group["GroupId"]
         ip_permissions = [
             {
-                "FromPort": 3000,
-                "ToPort": 4000,
+                "FromPort": 22,
+                "ToPort": 22,
                 "IpProtocol": "tcp",
                 "IpRanges": [{"CidrIp": "0.0.0.0/0"}],
             }
         ]
-        if not version.__is_release__:
-            ip_permissions.append(
-                {
-                    "FromPort": 22,
-                    "ToPort": 22,
-                    "IpProtocol": "tcp",
-                    "IpRanges": [{"CidrIp": "0.0.0.0/0"}],
-                }
-            )
         ec2_client.authorize_security_group_ingress(
             GroupId=security_group_id, IpPermissions=ip_permissions
         )
         ec2_client.authorize_security_group_egress(
             GroupId=security_group_id,
             IpPermissions=[
                 {
@@ -162,14 +154,15 @@
 
 
 def _user_data(
     bucket_name,
     region_name,
     runner_id: str,
     resources: Resources,
+    ssh_key_pub: str,
     port_range_from: int = 3000,
     port_range_to: int = 4000,
 ) -> str:
     sysctl_port_range_from = int((port_range_to - port_range_from) / 2) + port_range_from
     sysctl_port_range_to = port_range_to - 1
     runner_port_range_from = port_range_from
     runner_port_range_to = sysctl_port_range_from - 1
@@ -184,15 +177,16 @@
 sudo sysctl -w net.ipv4.ip_local_port_range="{sysctl_port_range_from} ${sysctl_port_range_to}"
 mkdir -p /root/.dstack/
 echo $'{_serialize_config_yaml(bucket_name, region_name)}' > /root/.dstack/config.yaml
 echo $'{_serialize_runner_yaml(runner_id, resources, runner_port_range_from, runner_port_range_to)}' > /root/.dstack/runner.yaml
 die() {{ status=$1; shift; echo "FATAL: $*"; exit $status; }}
 EC2_PUBLIC_HOSTNAME="`wget -q -O - http://169.254.169.254/latest/meta-data/public-hostname || die \"wget public-hostname has failed: $?\"`"
 echo "hostname: $EC2_PUBLIC_HOSTNAME" >> /root/.dstack/runner.yaml
-HOME=/root nohup dstack-runner start --http-port 4000 &
+mkdir ~/.ssh; chmod 700 ~/.ssh; echo "{ssh_key_pub}" > ~/.ssh/authorized_keys; chmod 600 ~/.ssh/authorized_keys
+HOME=/root nohup dstack-runner --log-level 6 start --http-port 4000 &
 """
     return user_data
 
 
 def role_name(iam_client: BaseClient, bucket_name: str) -> str:
     policy_name = "dstack_policy_" + bucket_name.replace("-", "_").lower()
     _role_name = "dstack_role_" + bucket_name.replace("-", "_").lower()
@@ -347,24 +341,25 @@
     region_name: str,
     subnet_id: Optional[str],
     runner_id: str,
     instance_type: InstanceType,
     local_repo_user_name: Optional[str],
     local_repo_user_email: Optional[str],
     repo_address: RepoAddress,
+    ssh_key_pub: str,
 ) -> str:
     launch_specification = {}
     if not version.__is_release__:
-        launch_specification["KeyName"] = "stgn_dstack"
+        launch_specification["KeyName"] = "dstack_victor"
     if instance_type.resources.interruptible:
         launch_specification["InstanceMarketOptions"] = {
             "MarketType": "spot",
             "SpotOptions": {
-                "SpotInstanceType": "persistent",
-                "InstanceInterruptionBehavior": "stop",
+                "SpotInstanceType": "one-time",
+                "InstanceInterruptionBehavior": "terminate",
             },
         }
     if subnet_id:
         launch_specification["NetworkInterfaces"] = [
             {
                 "AssociatePublicIpAddress": True,
                 "DeviceIndex": 0,
@@ -398,15 +393,17 @@
         ImageId=_get_ami_image(ec2_client, len(instance_type.resources.gpus) > 0)[0],
         InstanceType=instance_type.instance_name,
         MinCount=1,
         MaxCount=1,
         IamInstanceProfile={
             "Arn": _get_instance_profile_arn(iam_client, bucket_name),
         },
-        UserData=_user_data(bucket_name, region_name, runner_id, instance_type.resources),
+        UserData=_user_data(
+            bucket_name, region_name, runner_id, instance_type.resources, ssh_key_pub=ssh_key_pub
+        ),
         TagSpecifications=[
             {
                 "ResourceType": "instance",
                 "Tags": tags,
             },
         ],
         **launch_specification,
@@ -426,54 +423,55 @@
     region_name: str,
     subnet_id: Optional[str],
     runner_id: str,
     instance_type: InstanceType,
     local_repo_user_name: Optional[str],
     local_repo_user_email: Optional[str],
     repo_address: RepoAddress,
+    ssh_key_pub: str,
     attempts: int = 3,
 ) -> str:
     try:
         return _run_instance(
             ec2_client,
             iam_client,
             bucket_name,
             region_name,
             subnet_id,
             runner_id,
             instance_type,
             local_repo_user_name,
             local_repo_user_email,
             repo_address,
+            ssh_key_pub,
         )
-    except Exception as e:
-        if (
-            hasattr(e, "response")
-            and e.response.get("Error")
-            and e.response["Error"].get("Code") == "InvalidParameterValue"
-        ):
+    except botocore.exceptions.ClientError as e:
+        # FIXME: why retry on "InvalidParameterValue"
+        if e.response["Error"]["Code"] == "InvalidParameterValue":
             if attempts > 0:
                 time.sleep(CREATE_INSTANCE_RETRY_RATE_SECS)
                 return run_instance_retry(
                     ec2_client,
                     iam_client,
                     bucket_name,
                     region_name,
                     subnet_id,
                     runner_id,
                     instance_type,
                     local_repo_user_name,
                     local_repo_user_email,
                     repo_address,
+                    ssh_key_pub,
                     attempts - 1,
                 )
             else:
                 raise Exception("Failed to retry", e)
-        else:
-            raise e
+        elif e.response["Error"]["Code"] == "InsufficientInstanceCapacity":
+            raise NoCapacityError()
+        raise e
 
 
 def cancel_spot_request(ec2_client: BaseClient, request_id: str):
     ec2_client.cancel_spot_instance_requests(SpotInstanceRequestIds=[request_id])
     response = ec2_client.describe_instances(
         Filters=[
             {"Name": "spot-instance-request-id", "Values": [request_id]},
@@ -519,41 +517,44 @@
                 SpotInstanceRequestIds=[request_id]
             )
             if response.get("SpotInstanceRequests"):
                 status = response["SpotInstanceRequests"][0]["Status"]
                 if status["Code"] in [
                     "fulfilled",
                     "request-canceled-and-instance-running",
+                    "marked-for-stop-by-experiment",
+                    "marked-for-stop",
+                    "marked-for-termination",
                 ]:
                     request_status = RequestStatus.RUNNING
                 elif status["Code"] in [
                     "not-scheduled-yet",
                     "pending-evaluation",
                     "pending-fulfillment",
                 ]:
                     request_status = RequestStatus.PENDING
                 elif status["Code"] in [
                     "capacity-not-available",
                     "instance-stopped-no-capacity",
                     "instance-terminated-by-price",
                     "instance-stopped-by-price",
                     "instance-terminated-no-capacity",
+                    "instance-stopped-by-experiment",
+                    "instance-terminated-by-experiment",
                     "limit-exceeded",
                     "price-too-low",
                 ]:
                     request_status = RequestStatus.NO_CAPACITY
                 elif status["Code"] in [
                     "instance-terminated-by-user",
                     "instance-stopped-by-user",
                     "canceled-before-fulfillment",
                     "instance-terminated-by-schedule",
                     "instance-terminated-by-service",
                     "spot-instance-terminated-by-user",
-                    "marked-for-stop",
-                    "marked-for-termination",
                 ]:
                     request_status = RequestStatus.TERMINATED
                 else:
                     raise Exception(
                         f"Unsupported EC2 spot instance request status code: {status['Code']}"
                     )
                 return RequestHead(
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/storage.py` & `dstack-0.7rc1/cli/dstack/backend/aws/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/aws/utils.py` & `dstack-0.7rc1/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/base/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Any, Generator, List, Optional
 
+from dstack.backend.base import jobs
 from dstack.core.artifact import Artifact
-from dstack.core.config import BackendConfig
-from dstack.core.job import Job, JobHead
+from dstack.core.config import BackendConfig, Configurator
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
+from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
 from dstack.core.run import RunHead
-from dstack.core.runners import Runner
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 
 
 class BackendType(Enum):
     REMOTE = "remote"
     LOCAL = "local"
@@ -48,28 +48,32 @@
     def create_run(self, repo_address: RepoAddress) -> str:
         pass
 
     @abstractmethod
     def create_job(self, job: Job):
         pass
 
-    def submit_job(self, job: Job):
+    def submit_job(self, job: Job, failed_to_start_job_new_status: JobStatus = JobStatus.FAILED):
         self.create_job(job)
-        self.run_job(job)
+        self.run_job(job, failed_to_start_job_new_status)
+
+    def resubmit_job(self, job: Job, failed_to_start_job_new_status: JobStatus = JobStatus.FAILED):
+        jobs.update_job_submission(job)
+        self.run_job(job, failed_to_start_job_new_status)
 
     @abstractmethod
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         pass
 
     @abstractmethod
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         pass
 
     @abstractmethod
-    def run_job(self, job: Job) -> Runner:
+    def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
         pass
 
     @abstractmethod
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         pass
 
     def stop_jobs(self, repo_address: RepoAddress, run_name: Optional[str], abort: bool):
@@ -101,14 +105,15 @@
 
     @abstractmethod
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         pass
 
     @abstractmethod
     def poll_logs(
         self,
         repo_address: RepoAddress,
@@ -126,14 +131,15 @@
 
     @abstractmethod
     def download_run_artifact_files(
         self,
         repo_address: RepoAddress,
         run_name: str,
         output_dir: Optional[str],
+        files_path: Optional[str] = None,
     ):
         pass
 
     @abstractmethod
     def upload_job_artifact_files(
         self,
         repo_address: RepoAddress,
@@ -201,28 +207,36 @@
         pass
 
     @abstractmethod
     def delete_secret(self, repo_address: RepoAddress, secret_name: str):
         pass
 
     @abstractmethod
-    def get_configurator(self):
+    def get_configurator(self) -> Configurator:
+        pass
+
+    @abstractmethod
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
         pass
 
 
 class RemoteBackend(Backend):
     def __init__(self, backend_config: Optional[BackendConfig] = None, custom_client: Any = None):
         pass
 
     @property
     def type(self) -> BackendType:
         return BackendType.REMOTE
 
 
 class CloudBackend(RemoteBackend):
     @abstractmethod
+    def list_repo_heads(self) -> List[RepoHead]:
+        pass
+
+    @abstractmethod
     def get_signed_download_url(self, object_key: str) -> str:
         pass
 
     @abstractmethod
     def get_signed_upload_url(self, object_key: str) -> str:
         pass
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/artifacts.py` & `dstack-0.7rc1/cli/dstack/backend/base/artifacts.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,31 +35,43 @@
 
 
 def download_run_artifact_files(
     storage: Storage,
     repo_address: RepoAddress,
     artifacts: List[Artifact],
     output_dir: Optional[str],
+    files_path: Optional[str],
 ):
     if output_dir is None:
         output_dir = os.getcwd()
     for artifact in artifacts:
-        total_size = sum(f.filesize_in_bytes for f in artifact.files)
+        files = []
+        for file in artifact.files:
+            file_full_path = os.path.join(artifact.path, file.filepath)
+            if (
+                files_path is None
+                or Path(file_full_path) == Path(files_path)
+                or Path(files_path) in Path(file_full_path).parents
+            ):
+                files.append(file)
+        if len(files) == 0:
+            continue
+        total_size = sum(f.filesize_in_bytes for f in files)
         with tqdm(
             total=total_size,
             unit="B",
             unit_scale=True,
             unit_divisor=1024,
             desc=f"Downloading artifact '{artifact.name}'",
         ) as pbar:
 
             def callback(size):
                 pbar.update(size)
 
-            for file in artifact.files:
+            for file in files:
                 artifacts_dir = _get_job_artifacts_dir(repo_address, artifact.job_id)
                 source_path = os.path.join(artifacts_dir, artifact.path, file.filepath)
                 dest_path = os.path.join(output_dir, artifact.job_id, artifact.path, file.filepath)
                 Path(dest_path).parent.mkdir(parents=True, exist_ok=True)
                 storage.download_file(source_path, dest_path, callback)
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/compute.py` & `dstack-0.7rc1/cli/dstack/backend/base/compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 from dstack.core.instance import InstanceType
 from dstack.core.job import Job, Requirements
 from dstack.core.request import RequestHead
 from dstack.core.runners import Resources
 
 
+class ComputeError(Exception):
+    pass
+
+
+class NoCapacityError(ComputeError):
+    pass
+
+
 class Compute(ABC):
     @abstractmethod
     def get_request_head(self, job: Job, request_id: Optional[str]) -> RequestHead:
         pass
 
     @abstractmethod
     def get_instance_type(self, job: Job) -> Optional[InstanceType]:
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/jobs.py` & `dstack-0.7rc1/cli/dstack/backend/base/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
 from typing import List, Optional
 
 import yaml
 
 from dstack.backend.base import runners
-from dstack.backend.base.compute import Compute
+from dstack.backend.base.compute import Compute, NoCapacityError
 from dstack.backend.base.storage import Storage
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.repo import RepoAddress
 from dstack.core.request import RequestStatus
 from dstack.core.runners import Runner
+from dstack.utils.common import get_milliseconds_since_epoch
 
 
 def create_job(
     storage: Storage,
     job: Job,
     create_head: bool = True,
 ):
@@ -140,14 +141,15 @@
         storage.delete_object(job_head_key)
 
 
 def run_job(
     storage: Storage,
     compute: Compute,
     job: Job,
+    failed_to_start_job_new_status: JobStatus,
 ):
     if job.status != JobStatus.SUBMITTED:
         raise Exception("Can't create a request for a job which status is not SUBMITTED")
 
     runner = None
     try:
         job.runner_id = uuid.uuid4().hex
@@ -160,14 +162,18 @@
 
         runner = Runner(
             runner_id=job.runner_id, request_id=None, resources=instance_type.resources, job=job
         )
         runners.create_runner(storage, runner)
         runner.request_id = compute.run_instance(job, instance_type)
         runners.update_runner(storage, runner)
+    except NoCapacityError:
+        job.status = failed_to_start_job_new_status
+        job.request_id = runner.request_id if runner else None
+        update_job(storage, job)
     except Exception as e:
         job.status = JobStatus.FAILED
         job.request_id = runner.request_id if runner else None
         update_job(storage, job)
         raise e
 
 
@@ -233,14 +239,20 @@
                 and job.status.is_unfinished()
                 and job.status != new_status
             ):
                 job.status = new_status
                 update_job(storage, job)
 
 
+def update_job_submission(job: Job):
+    job.status = JobStatus.SUBMITTED
+    job.submission_num += 1
+    job.submitted_at = get_milliseconds_since_epoch()
+
+
 def _get_jobs_dir(repo_address: RepoAddress) -> str:
     return f"jobs/{repo_address.path()}/"
 
 
 def _get_job_filename(repo_address: RepoAddress, job_id: str) -> str:
     return f"{_get_jobs_dir(repo_address)}{job_id}.yaml"
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/logs.py` & `dstack-0.7rc1/cli/dstack/backend/base/logs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import re
 import urllib.parse
-from typing import Any, Dict, List
+from typing import Any, Dict, Optional
 
 from dstack.backend.base import jobs
 from dstack.backend.base.storage import Storage
-from dstack.core.app import AppSpec
 from dstack.core.job import Job
 from dstack.core.log_event import LogEvent, LogEventSource
 from dstack.core.repo import RepoAddress
 
 WAIT_N_ONCE_FINISHED = 1
 
 CHECK_STATUS_EVERY_N = 3
@@ -17,53 +16,55 @@
 POLL_LOGS_RATE_SECS = 1
 
 
 def render_log_message(
     storage: Storage,
     event: Dict[str, Any],
     repo_address: RepoAddress,
+    jobs_cache: Dict[str, Job],
 ) -> LogEvent:
     if isinstance(event, str):
         event = json.loads(event)
     message = event["message"]
     if isinstance(message, str):
         message = json.loads(message)
     job_id = message["job_id"]
     log = message["log"]
-    job = jobs.get_job(storage, repo_address, job_id)
-    log = fix_urls(log.encode(), job).decode()
+    job = jobs_cache.get(job_id)
+    if job is None:
+        job = jobs.get_job(storage, repo_address, job_id)
+        jobs_cache[job_id] = job
+    log = fix_urls(log.encode(), job, {}).decode()
     return LogEvent(
         event_id=event["eventId"],
         timestamp=event["timestamp"],
         job_id=job_id,
         log_message=log,
         log_source=LogEventSource.STDOUT
         if message["source"] == "stdout"
         else LogEventSource.STDERR,
     )
 
 
-def fix_urls(log: bytes, job: Job) -> bytes:
+def fix_urls(log: bytes, job: Job, ports: Dict[int, int], hostname: Optional[str] = None) -> bytes:
     if not (job.host_name and job.ports and job.app_specs):
         return log
-    for app_spec in job.app_specs:
-        log = _fix_url_for_app(log, job, app_spec)
-    return log
 
+    hostname = hostname or job.host_name
+    app_specs = {job.ports[app_spec.port_index]: app_spec for app_spec in job.app_specs}
+    ports_re = "|".join(str(port) for port in job.ports)
+    url_pattern = rf"http://(?:localhost|0.0.0.0|127.0.0.1|{job.host_name}):({ports_re})\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)".encode()
+
+    def replace_url(match: re.Match) -> bytes:
+        remote_port = int(match.group(1))
+        local_port = ports.get(remote_port, remote_port)
+        app_spec = app_specs[remote_port]
+        url = urllib.parse.urlparse(match.group(0))
+        qs = {k: v[0] for k, v in urllib.parse.parse_qs(url.query).items()}
+        if app_spec.url_query_params is not None:
+            qs.update({k.encode(): v.encode() for k, v in app_spec.url_query_params.items()})
+        url = url._replace(
+            netloc=f"{hostname}:{local_port}".encode(), query=urllib.parse.urlencode(qs).encode()
+        )
+        return url.geturl()
 
-def _fix_url_for_app(log: bytes, job: Job, app_spec: AppSpec) -> bytes:
-    port = job.ports[app_spec.port_index]
-    url_pattern = f"http://(localhost|0.0.0.0|127.0.0.1|{job.host_name}):{port}\S*".encode()
-    match = re.search(url_pattern, log)
-    if match is None:
-        return log
-    url = match.group(0)
-    parsed_url = urllib.parse.urlparse(url)
-    qs = urllib.parse.parse_qs(parsed_url.query)
-    qs = {k: v[0] for k, v in qs.items()}
-    if app_spec.url_query_params is not None:
-        for k, v in app_spec.url_query_params.items():
-            qs[k.encode()] = v.encode()
-    new_url = parsed_url._replace(
-        netloc=f"{job.host_name}:{port}".encode(), query=urllib.parse.urlencode(qs).encode()
-    ).geturl()
-    return log.replace(url, new_url)
+    return re.sub(url_pattern, replace_url, log)
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/repos.py` & `dstack-0.7rc1/cli/dstack/backend/base/repos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from typing import List, Optional
 
 from dstack.backend.base.secrets import SecretsManager
 from dstack.backend.base.storage import Storage
 from dstack.core.repo import RepoAddress, RepoCredentials, RepoHead, RepoProtocol
-from dstack.core.secret import Secret
 
 
 def get_repo_head(storage: Storage, repo_address: RepoAddress) -> Optional[RepoHead]:
     repo_head_prefix = _get_repo_head_filename_prefix(repo_address)
     repo_heads_keys = storage.list_objects(repo_head_prefix)
     if len(repo_heads_keys) == 0:
         return None
@@ -27,35 +26,31 @@
 def list_repo_heads(storage: Storage) -> List[RepoHead]:
     repo_heads_prefix = _get_repo_heads_prefix()
     repo_heads_keys = storage.list_objects(repo_heads_prefix)
     repo_heads = []
     for repo_head_key in repo_heads_keys:
         tokens = repo_head_key[len(repo_heads_prefix) :].split(";")
         # Skipt legacy repo heads
-        if len(tokens) == 5:
-            (
-                repo_host_port,
-                repo_user_name,
-                repo_name,
-                last_run_at,
-                tags_count,
-            ) = tuple(tokens)
-            t = repo_host_port.split(":")
-            repo_host_name = t[0]
-            repo_port = t[1] if len(t) > 1 else None
-            repo_heads.append(
-                RepoHead(
-                    repo_host_name=repo_host_name,
-                    repo_port=repo_port,
-                    repo_user_name=repo_user_name,
-                    repo_name=repo_name,
-                    last_run_at=int(last_run_at) if last_run_at else None,
-                    tags_count=int(tags_count),
-                )
+        if len(tokens) != 3:
+            continue
+        repo_str, last_run_at, tags_count = tokens
+        repo_host_port, repo_user_name, repo_name = repo_str.split(",")
+        t = repo_host_port.split(":")
+        repo_host_name = t[0]
+        repo_port = t[1] if len(t) > 1 else None
+        repo_heads.append(
+            RepoHead(
+                repo_host_name=repo_host_name,
+                repo_port=repo_port,
+                repo_user_name=repo_user_name,
+                repo_name=repo_name,
+                last_run_at=int(last_run_at) if last_run_at else None,
+                tags_count=int(tags_count),
             )
+        )
     return repo_heads
 
 
 def update_repo_last_run_at(storage: Storage, repo_address: RepoAddress, last_run_at: int):
     repo_head = get_repo_head(storage, repo_address)
     if repo_head is None:
         repo_head = RepoHead(
@@ -77,19 +72,15 @@
 def get_repo_credentials(
     secrets_manager: SecretsManager, repo_address: RepoAddress
 ) -> Optional[RepoCredentials]:
     credentials_value = secrets_manager.get_credentials(repo_address)
     if credentials_value is None:
         return None
     credentials_data = json.loads(credentials_value)
-    return RepoCredentials(
-        protocol=RepoProtocol(credentials_data["protocol"]),
-        private_key=credentials_data.get("private_key"),
-        oauth_token=credentials_data.get("oauth_token"),
-    )
+    return RepoCredentials(**credentials_data)
 
 
 def save_repo_credentials(
     secrets_manager: SecretsManager,
     repo_address: RepoAddress,
     repo_credentials: RepoCredentials,
 ):
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/runners.py` & `dstack-0.7rc1/cli/dstack/backend/base/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/runs.py` & `dstack-0.7rc1/cli/dstack/backend/base/runs.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import yaml
 
 from dstack.backend.base import BackendType, jobs, runners
 from dstack.backend.base.compute import Compute
 from dstack.backend.base.storage import Storage
 from dstack.core.app import AppHead
 from dstack.core.artifact import ArtifactHead
-from dstack.core.job import JobHead
+from dstack.core.job import JobHead, JobStatus
 from dstack.core.repo import RepoAddress
 from dstack.core.run import (
-    RequestHead,
+    RequestStatus,
     RunHead,
     generate_local_run_name_prefix,
     generate_remote_run_name_prefix,
 )
 
 
 def create_run(
@@ -44,32 +44,38 @@
 
 
 def get_run_heads(
     storage: Storage,
     compute: Compute,
     job_heads: List[JobHead],
     include_request_heads: bool,
+    interrupted_job_new_status: JobStatus = JobStatus.FAILED,
 ) -> List[RunHead]:
     runs_by_id = {}
     for job_head in job_heads:
         run_id = ",".join([job_head.run_name, job_head.workflow_name or ""])
         if run_id not in runs_by_id:
-            runs_by_id[run_id] = _create_run(storage, compute, job_head, include_request_heads)
+            runs_by_id[run_id] = _create_run(
+                storage, compute, job_head, include_request_heads, interrupted_job_new_status
+            )
         else:
             run = runs_by_id[run_id]
-            _update_run(storage, compute, run, job_head, include_request_heads)
+            _update_run(
+                storage, compute, run, job_head, include_request_heads, interrupted_job_new_status
+            )
     run_heads = list(sorted(runs_by_id.values(), key=lambda r: r.submitted_at, reverse=True))
     return run_heads
 
 
 def _create_run(
     storage: Storage,
     compute: Compute,
     job_head: JobHead,
     include_request_heads: bool,
+    interrupted_job_new_status: JobStatus,
 ) -> RunHead:
     app_heads = (
         list(
             map(
                 lambda app_name: AppHead(job_id=job_head.job_id, app_name=app_name),
                 job_head.app_names,
             )
@@ -97,14 +103,17 @@
         request_id = job.request_id
         if request_id is None and job.runner_id is not None:
             runner = runners.get_runner(storage, job.runner_id)
             if not (runner is None):
                 request_id = runner.request_id
         request_head = compute.get_request_head(job, request_id)
         request_heads.append(request_head)
+        if request_head.status == RequestStatus.NO_CAPACITY:
+            job.status = job_head.status = interrupted_job_new_status
+            jobs.update_job(storage, job)
     run_head = RunHead(
         repo_address=job_head.repo_address,
         run_name=job_head.run_name,
         workflow_name=job_head.workflow_name,
         provider_name=job_head.provider_name,
         local_repo_user_name=job_head.local_repo_user_name,
         artifact_heads=artifact_heads or None,
@@ -119,14 +128,15 @@
 
 def _update_run(
     storage: Storage,
     compute: Compute,
     run: RunHead,
     job_head: JobHead,
     include_request_heads: bool,
+    interrupted_job_new_status: JobStatus,
 ):
     run.submitted_at = min(run.submitted_at, job_head.submitted_at)
     if job_head.artifact_paths:
         if run.artifact_heads is None:
             run.artifact_heads = []
         run.artifact_heads.extend(
             list(
@@ -146,18 +156,21 @@
                 map(
                     lambda app_name: AppHead(job_id=job_head.job_id, app_name=app_name),
                     job_head.app_names,
                 )
             )
         )
     if job_head.status.is_unfinished():
-        run.status = job_head.status
         if include_request_heads:
             if run.request_heads is None:
                 run.request_heads = []
             job = jobs.get_job(storage, job_head.repo_address, job_head.job_id)
             request_id = job.request_id
             if request_id is None and job.runner_id is not None:
                 runner = runners.get_runner(storage, job.runner_id)
                 request_id = runner.request_id
             request_head = compute.get_request_head(job, request_id)
             run.request_heads.append(request_head)
+            if request_head.status == RequestStatus.NO_CAPACITY:
+                job.status = job_head.status = interrupted_job_new_status
+                jobs.update_job(storage, job)
+        run.status = job_head.status
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/base/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/storage.py` & `dstack-0.7rc1/cli/dstack/backend/base/storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     def upload_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         """
         `source_path` - local absolute path.
         `dest_path` - storage path relative to the storage root.
         """
         pass
 
+    def delete_prefix(self, keys_prefix: str):
+        for key in self.list_objects(keys_prefix):
+            self.delete_object(key)
+
 
 class CloudStorage(Storage):
     @abstractmethod
     def get_signed_download_url(self, key: str) -> str:
         pass
 
     @abstractmethod
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/base/tags.py` & `dstack-0.7rc1/cli/dstack/backend/base/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dstack.backend.base import BackendType, artifacts, jobs, runs
 from dstack.backend.base.storage import Storage
 from dstack.core.artifact import ArtifactHead, ArtifactSpec
 from dstack.core.error import BackendError
 from dstack.core.job import Job, JobStatus
 from dstack.core.repo import LocalRepoData, RepoAddress
 from dstack.core.tag import TagHead
+from dstack.utils.common import get_milliseconds_since_epoch
 
 
 def get_tag_head(storage: Storage, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
     tag_head_key_prefix = _get_tag_head_filename_prefix(repo_address, tag_name)
     tag_head_keys = storage.list_objects(keys_prefix=tag_head_key_prefix)
     if len(tag_head_keys) == 0:
         return None
@@ -159,15 +160,15 @@
         repo_data=repo_data,
         run_name=run_name,
         workflow_name=None,
         provider_name="bash",
         local_repo_user_name=repo_data.local_repo_user_name,
         local_repo_user_email=repo_data.local_repo_user_email,
         status=JobStatus.DONE,
-        submitted_at=int(round(time.time() * 1000)),
+        submitted_at=get_milliseconds_since_epoch(),
         image_name="scratch",
         commands=None,
         env=None,
         working_dir=None,
         artifact_specs=[ArtifactSpec(artifact_path=a, mount=False) for a in tag_artifacts],
         port_count=None,
         ports=None,
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 from typing import Generator, List, Optional
 
 from google.auth._default import _CLOUD_SDK_CREDENTIALS_WARNING
 from google.oauth2 import service_account
 
 from dstack.backend.base import CloudBackend
 from dstack.backend.base import artifacts as base_artifacts
+from dstack.backend.base import cache as base_cache
 from dstack.backend.base import jobs as base_jobs
 from dstack.backend.base import repos as base_repos
 from dstack.backend.base import runs as base_runs
 from dstack.backend.base import secrets as base_secrets
 from dstack.backend.base import tags as base_tags
 from dstack.backend.gcp.compute import GCPCompute
 from dstack.backend.gcp.config import GCPConfig, GCPConfigurator
 from dstack.backend.gcp.logs import GCPLogging
 from dstack.backend.gcp.secrets import GCPSecretsManager
 from dstack.backend.gcp.storage import BucketNotFoundError, GCPStorage
 from dstack.cli.common import console
 from dstack.core.artifact import Artifact
 from dstack.core.error import ConfigError
-from dstack.core.job import Job, JobHead
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
+from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 
 warnings.filterwarnings("ignore", message=_CLOUD_SDK_CREDENTIALS_WARNING)
 
 
@@ -94,16 +95,16 @@
 
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         return base_jobs.get_job(self._storage, repo_address, job_id)
 
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         return base_jobs.list_jobs(self._storage, repo_address, run_name)
 
-    def run_job(self, job: Job):
-        base_jobs.run_job(self._storage, self._compute, job)
+    def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
+        base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         base_jobs.stop_job(self._storage, self._compute, repo_address, job_id, abort)
 
     def list_job_heads(
         self, repo_address: RepoAddress, run_name: Optional[str] = None
     ) -> List[JobHead]:
@@ -113,48 +114,56 @@
         base_jobs.delete_job_head(self._storage, repo_address, job_id)
 
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         job_heads = self.list_job_heads(repo_address, run_name)
         return base_runs.get_run_heads(
-            self._storage, self._compute, job_heads, include_request_heads
+            self._storage,
+            self._compute,
+            job_heads,
+            include_request_heads,
+            interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
         repo_address: RepoAddress,
         job_heads: List[JobHead],
         start_time: int,
         attached: bool,
     ) -> Generator[LogEvent, None, None]:
         yield from self._logging.poll_logs(
             storage=self._storage,
             repo_address=repo_address,
             run_name=job_heads[0].run_name,
+            start_time=start_time,
         )
 
     def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
         return base_artifacts.list_run_artifact_files(self._storage, repo_address, run_name)
 
     def download_run_artifact_files(
         self,
         repo_address: RepoAddress,
         run_name: str,
         output_dir: Optional[str],
+        files_path: Optional[str] = None,
     ):
         artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
             repo_address=repo_address,
             artifacts=artifacts,
             output_dir=output_dir,
+            files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
         repo_address: RepoAddress,
         job_id: str,
         artifact_name: str,
@@ -201,14 +210,17 @@
             local_dirs,
             self.type,
         )
 
     def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
         base_tags.delete_tag(self._storage, repo_address, tag_head)
 
+    def list_repo_heads(self) -> List[RepoHead]:
+        return base_repos.list_repo_heads(self._storage)
+
     def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
         base_repos.update_repo_last_run_at(
             self._storage,
             repo_address,
             last_run_at,
         )
 
@@ -256,7 +268,10 @@
         return self._storage.get_signed_download_url(object_key)
 
     def get_signed_upload_url(self, object_key: str) -> str:
         return self._storage.get_signed_upload_url(object_key)
 
     def get_configurator(self):
         return GCPConfigurator()
+
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_address, username, workflow_name)
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/compute.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/compute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import re
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional
 
 import google.api_core.exceptions
 from google.cloud import compute_v1
 from google.oauth2 import service_account
 
 from dstack import version
 from dstack.backend.aws.runners import _serialize_runner_yaml
 from dstack.backend.base.compute import Compute, choose_instance_type
 from dstack.backend.gcp import utils as gcp_utils
 from dstack.backend.gcp.config import GCPConfig
 from dstack.core.instance import InstanceType
 from dstack.core.job import Job, Requirements
 from dstack.core.request import RequestHead, RequestStatus
-from dstack.core.runners import Gpu, Resources, Runner
+from dstack.core.runners import Gpu, Resources
 
 DSTACK_INSTANCE_TAG = "dstack-runner-instance"
 
 
 _supported_accelerators = [
     {"accelerator_name": "nvidia-a100-80gb", "gpu_name": "A100", "memory_mb": 1024 * 80},
     {"accelerator_name": "nvidia-tesla-a100", "gpu_name": "A100", "memory_mb": 1024 * 40},
@@ -38,24 +38,26 @@
         self.instances_client = compute_v1.InstancesClient(credentials=self.credentials)
         self.images_client = compute_v1.ImagesClient(credentials=self.credentials)
         self.firewalls_client = compute_v1.FirewallsClient(credentials=self.credentials)
         self.machine_types_client = compute_v1.MachineTypesClient(credentials=self.credentials)
         self.accelerator_types_client = compute_v1.AcceleratorTypesClient(
             credentials=self.credentials
         )
+        self.zone_operations_client = compute_v1.ZoneOperationsClient(credentials=self.credentials)
 
     def get_request_head(self, job: Job, request_id: Optional[str]) -> RequestHead:
         if request_id is None:
             return RequestHead(
                 job_id=job.job_id,
                 status=RequestStatus.TERMINATED,
                 message="request_id is not specified",
             )
         instance_status = _get_instance_status(
-            client=self.instances_client,
+            instances_client=self.instances_client,
+            zone_operations_client=self.zone_operations_client,
             project_id=self.gcp_config.project_id,
             zone=self.gcp_config.zone,
             instance_name=request_id,
         )
         return RequestHead(
             job_id=job.job_id,
             status=instance_status,
@@ -93,14 +95,15 @@
                 zone=self.gcp_config.zone,
                 instance_type=instance_type,
             ),
             labels=_get_labels(
                 bucket=self.gcp_config.bucket_name,
                 job=job,
             ),
+            ssh_key_pub=job.ssh_key_pub,
         )
         return instance.name
 
     def terminate_instance(self, request_id: str):
         _terminate_instance(
             client=self.instances_client,
             gcp_config=self.gcp_config,
@@ -112,25 +115,39 @@
             client=self.instances_client,
             gcp_config=self.gcp_config,
             instance_name=request_id,
         )
 
 
 def _get_instance_status(
-    client: compute_v1.InstancesClient, project_id: str, zone: str, instance_name: str
+    instances_client: compute_v1.InstancesClient,
+    zone_operations_client: compute_v1.ZoneOperationsClient,
+    project_id: str,
+    zone: str,
+    instance_name: str,
 ) -> RequestStatus:
     get_instance_request = compute_v1.GetInstanceRequest(
         instance=instance_name,
         project=project_id,
         zone=zone,
     )
     try:
-        instance = client.get(get_instance_request)
+        instance = instances_client.get(get_instance_request)
     except google.api_core.exceptions.NotFound:
         return RequestStatus.TERMINATED
+    if instance.scheduling.provisioning_model == compute_v1.Scheduling.ProvisioningModel.SPOT.name:
+        list_operations_request = compute_v1.ListZoneOperationsRequest(
+            project=project_id,
+            zone=zone,
+            filter=f'(name = "{instance_name}") AND (operationType = "compute.instances.preempted")',
+        )
+        operations = zone_operations_client.list(list_operations_request)
+        if len(list(operations)) > 0:
+            return RequestStatus.NO_CAPACITY
+
     if instance.status in ["PROVISIONING", "STAGING", "RUNNING"]:
         return RequestStatus.RUNNING
     return RequestStatus.TERMINATED
 
 
 def _choose_instance_type(
     machine_types_client: compute_v1.MachineTypesClient,
@@ -411,17 +428,20 @@
 def _get_subnet_resource(region: str, subnet: str) -> str:
     return f"regions/{region}/subnetworks/{subnet}"
 
 
 def _get_labels(bucket: str, job: Job) -> Dict[str, str]:
     labels = {
         "owner": "dstack",
-        "dstack_bucket": bucket,
-        "dstack_repo": job.repo_address.path("-").replace(".", "-"),
     }
+    if gcp_utils.is_valid_label_value(bucket):
+        labels["dstack_bucket"] = bucket
+    dstack_repo = job.repo_address.path("-").lower().replace(".", "-")
+    if gcp_utils.is_valid_label_value(dstack_repo):
+        labels["dstack_repo"] = dstack_repo
     if job.local_repo_user_name is not None:
         dstack_user_name = job.local_repo_user_name.lower().replace(" ", "_")
         if gcp_utils.is_valid_label_value(dstack_user_name):
             labels["dstack_user_name"] = dstack_user_name
     return labels
 
 
@@ -436,14 +456,15 @@
     machine_type: str,
     instance_name: str,
     user_data_script: str,
     service_account: str,
     interruptible: bool,
     accelerators: List[compute_v1.AcceleratorConfig],
     labels: Dict[str, str],
+    ssh_key_pub: str,
 ) -> compute_v1.Instance:
     try:
         _create_firewall_rules(
             firewalls_client=firewalls_client,
             project_id=project_id,
             network=network,
         )
@@ -467,14 +488,15 @@
         disks=[disk],
         user_data_script=user_data_script,
         service_account=service_account,
         external_access=True,
         spot=interruptible,
         accelerators=accelerators,
         labels=labels,
+        ssh_key_pub=ssh_key_pub,
     )
     return instance
 
 
 def _disk_from_image(
     disk_type: str,
     disk_size_gb: int,
@@ -515,14 +537,15 @@
 
 def _create_instance(
     instances_client: compute_v1.InstancesClient,
     project_id: str,
     zone: str,
     instance_name: str,
     disks: List[compute_v1.AttachedDisk],
+    ssh_key_pub: str,
     machine_type: str = "n1-standard-1",
     network_link: str = "global/networks/default",
     subnetwork_link: str = None,
     internal_ip: str = None,
     external_access: bool = False,
     external_ipv4: str = None,
     accelerators: List[compute_v1.AcceleratorConfig] = None,
@@ -611,18 +634,18 @@
 
     if custom_hostname is not None:
         instance.hostname = custom_hostname
 
     if delete_protection:
         instance.deletion_protection = True
 
+    metadata_items = [compute_v1.Items(key="ssh-keys", value=f"root:{ssh_key_pub}")]
     if user_data_script is not None:
-        instance.metadata = compute_v1.Metadata(
-            items=[compute_v1.Items(key="user-data", value=user_data_script)]
-        )
+        metadata_items.append(compute_v1.Items(key="user-data", value=user_data_script))
+    instance.metadata = compute_v1.Metadata(items=metadata_items)
 
     if service_account is not None:
         instance.service_accounts = [
             compute_v1.ServiceAccount(
                 email=service_account,
                 scopes=["https://www.googleapis.com/auth/cloud-platform"],
             )
@@ -663,26 +686,22 @@
     Returns:
         A Firewall object.
     """
     firewall_rule = compute_v1.Firewall()
     firewall_rule.name = f"dstack-runner-allow-incoming-" + network.replace("/", "-")
     firewall_rule.direction = "INGRESS"
 
-    allowed_ports_tcp = compute_v1.Allowed()
-    allowed_ports_tcp.I_p_protocol = "tcp"
-    allowed_ports_tcp.ports = ["3000-4000"]
-
-    allowed_ports_udp = compute_v1.Allowed()
-    allowed_ports_udp.I_p_protocol = "udp"
-    allowed_ports_udp.ports = ["3000-4000"]
+    allowed_ssh_port = compute_v1.Allowed()
+    allowed_ssh_port.I_p_protocol = "tcp"
+    allowed_ssh_port.ports = ["22"]
 
-    firewall_rule.allowed = [allowed_ports_tcp, allowed_ports_udp]
+    firewall_rule.allowed = [allowed_ssh_port]
     firewall_rule.source_ranges = ["0.0.0.0/0"]
     firewall_rule.network = network
-    firewall_rule.description = "Allowing TCP/UDP traffic on ports 3000-4000 from Internet."
+    firewall_rule.description = "Allowing only SSH connections from Internet."
 
     firewall_rule.target_tags = [DSTACK_INSTANCE_TAG]
 
     operation = firewalls_client.insert(project=project_id, firewall_resource=firewall_rule)
     gcp_utils.wait_for_extended_operation(operation, "firewall rule creation")
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/config.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+import json
 import os
+from argparse import Namespace
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import yaml
 from google.cloud import compute_v1, exceptions, storage
 from google.oauth2 import service_account
 from rich.prompt import Confirm, Prompt
-from simple_term_menu import TerminalMenu
+from rich_argparse import RichHelpFormatter
 
-from dstack.cli.common import ask_choice, console
+from dstack.cli.common import ask_choice, console, is_termios_available
 from dstack.core.config import BackendConfig, Configurator, get_config_path
-from dstack.core.error import ConfigError
+from dstack.core.error import ConfigError, HubConfigError
+from dstack.hub.models import (
+    GCPProjectValues,
+    GCPVPCSubnetProjectElement,
+    GCPVPCSubnetProjectElementValue,
+    ProjectElement,
+    ProjectElementValue,
+)
 
 DEFAULT_GEOGRAPHIC_AREA = "North America"
 
-
 GCP_LOCATIONS = [
     {
         "name": "North America",
         "regions": [
             "northamerica-northeast1",
             "northamerica-northeast2",
             "us-central1",
@@ -131,37 +139,36 @@
             res["credentials_file"] = self.credentials_file
         return res
 
     def serialize_yaml(self) -> str:
         return yaml.dump(self.serialize())
 
     @classmethod
-    def deserialize(cls, data: Dict) -> Optional["GCPConfig"]:
-        if data.get("backend") != "gcp":
+    def deserialize(cls, config_data: Dict) -> Optional["GCPConfig"]:
+        if config_data.get("backend") != "gcp":
             raise ConfigError(f"Not a GCP config")
-
         try:
-            project_id = data["project"]
-            region = data["region"]
-            zone = data["zone"]
-            bucket_name = data["bucket"]
-            vpc = data["vpc"]
-            subnet = data["subnet"]
+            project_id = config_data["project"]
+            region = config_data["region"]
+            zone = config_data["zone"]
+            bucket_name = config_data["bucket"]
+            vpc = config_data["vpc"]
+            subnet = config_data["subnet"]
         except KeyError:
             raise ConfigError("Cannot load config")
 
-        credentials_file = data.get("credentials_file")
         return cls(
             project_id=project_id,
             region=region,
             zone=zone,
             bucket_name=bucket_name,
             vpc=vpc,
             subnet=subnet,
-            credentials_file=credentials_file,
+            credentials_file=config_data.get("credentials_file"),
+            credentials=config_data.get("credentials"),
         )
 
     @classmethod
     def deserialize_yaml(cls, yaml_content: str) -> "GCPConfig":
         content = yaml.load(yaml_content, yaml.FullLoader)
         if content is None:
             raise ConfigError("Cannot load config")
@@ -180,22 +187,186 @@
 
 
 class GCPConfigurator(Configurator):
     @property
     def name(self):
         return "gcp"
 
-    def get_config(self, data: Dict) -> BackendConfig:
-        return GCPConfig.deserialize(data=data)
+    def get_config_from_hub_config_data(self, config_data: Dict, auth_data: Dict) -> BackendConfig:
+        credentials = json.loads(auth_data["credentials"])
+        data = {
+            "backend": "gcp",
+            "credentials": credentials,
+            "project": credentials["project_id"],
+            "region": config_data["region"],
+            "zone": config_data["zone"],
+            "bucket": config_data["bucket_name"],
+            "vpc": config_data["vpc"],
+            "subnet": config_data["subnet"],
+        }
+        return GCPConfig.deserialize(data)
 
-    def parse_args(self, args: list = []):
-        pass
+    def register_parser(self, parser):
+        gcp_parser = parser.add_parser("gcp", help="", formatter_class=RichHelpFormatter)
+        gcp_parser.add_argument("--bucket", type=str, help="", required=True)
+        gcp_parser.add_argument("--project", type=str, help="", required=True)
+        gcp_parser.add_argument("--region", type=str, help="", required=True)
+        gcp_parser.add_argument("--zone", type=str, help="", required=True)
+        gcp_parser.add_argument("--vpc", type=str, help="", required=True)
+        gcp_parser.add_argument("--subnet", type=str, help="", required=True)
+        gcp_parser.set_defaults(func=self._command)
 
-    def configure_hub(self, data: Dict):
-        pass
+    def _command(self, args: Namespace):
+        config = GCPConfig(
+            project_id=args.project,
+            region=args.region,
+            zone=args.zone,
+            bucket_name=args.bucket,
+            subnet=args.subnet,
+            vpc=args.vpc,
+        )
+        config.save()
+        print(f"[grey58]OK[/]")
+
+    def configure_hub(self, config_data: Dict) -> GCPProjectValues:
+        try:
+            service_account_info = json.loads(config_data.get("credentials"))
+            self.credentials = service_account.Credentials.from_service_account_info(
+                info=service_account_info
+            )
+            storage_client = storage.Client(credentials=self.credentials)
+            storage_client.list_buckets(max_results=1)
+        except Exception:
+            raise HubConfigError(
+                "Credentials are not valid", code="invalid_credentials", fields=["credentials"]
+            )
+        project_values = GCPProjectValues()
+        project_values.area = self._get_hub_geographic_area(config_data.get("area"))
+        location = self._get_location(project_values.area.selected)
+        project_values.region, regions = self._get_hub_region(
+            location=location,
+            default_region=config_data.get("region"),
+        )
+        project_values.zone = self._get_hub_zone(
+            location=location,
+            region=regions.get(project_values.region.selected),
+            default_zone=config_data.get("zone"),
+        )
+        project_values.bucket_name = self._get_hub_buckets(
+            region=project_values.region.selected,
+            default_bucket=config_data.get("bucket_name"),
+        )
+        project_values.vpc_subnet = self._get_hub_vpc_subnet(
+            region=project_values.region.selected,
+            default_vpc=config_data.get("vpc"),
+            default_subnet=config_data.get("subnet"),
+        )
+        return project_values
+
+    def _get_hub_geographic_area(self, default_area: Optional[str]) -> ProjectElement:
+        area_names = sorted([l["name"] for l in GCP_LOCATIONS])
+        if default_area is None:
+            default_area = DEFAULT_GEOGRAPHIC_AREA
+        if default_area not in area_names:
+            raise HubConfigError(f"Invalid GCP area {default_area}")
+        element = ProjectElement(selected=default_area)
+        for area_name in area_names:
+            element.values.append(ProjectElementValue(value=area_name, label=area_name))
+        return element
+
+    def _get_hub_region(
+        self, location: Dict, default_region: Optional[str]
+    ) -> Tuple[ProjectElement, Dict]:
+        regions_client = compute_v1.RegionsClient(credentials=self.credentials)
+        regions = regions_client.list(project=self.credentials.project_id)
+        region_names = sorted(
+            [r.name for r in regions if r.name in location["regions"]],
+            key=lambda name: (name != location["default_region"], name),
+        )
+        if default_region is None:
+            default_region = region_names[0]
+        if default_region not in region_names:
+            raise HubConfigError(f"Invalid GCP region {default_region} in area {location['name']}")
+        element = ProjectElement(selected=default_region)
+        for region_name in region_names:
+            element.values.append(ProjectElementValue(value=region_name, label=region_name))
+        return element, {r.name: r for r in regions}
+
+    def _get_hub_zone(
+        self, location: Dict, region: compute_v1.Region, default_zone: Optional[str]
+    ) -> ProjectElement:
+        zone_names = sorted(
+            [self._get_resource_name(z) for z in region.zones],
+            key=lambda name: (name != location["default_zone"], name),
+        )
+        if default_zone is None:
+            default_zone = zone_names[0]
+        if default_zone not in zone_names:
+            raise HubConfigError(f"Invalid GCP zone {default_zone} in region {region.name}")
+        element = ProjectElement(selected=default_zone)
+        for zone_name in zone_names:
+            element.values.append(ProjectElementValue(value=zone_name, label=zone_name))
+        return element
+
+    def _get_hub_buckets(
+        self, region: str, default_bucket: Optional[str] = None
+    ) -> ProjectElement:
+        storage_client = storage.Client(credentials=self.credentials)
+        buckets = storage_client.list_buckets()
+        bucket_names = [bucket.name for bucket in buckets if bucket.location.lower() == region]
+        if default_bucket is not None and default_bucket not in bucket_names:
+            raise HubConfigError(
+                f"Invalid bucket {default_bucket} for region {region}",
+                code="invalid_bucket",
+                fields=["bucket_name"],
+            )
+        element = ProjectElement(selected=default_bucket)
+        for bucket_name in bucket_names:
+            element.values.append(ProjectElementValue(value=bucket_name, label=bucket_name))
+        return element
+
+    def _get_hub_vpc_subnet(
+        self,
+        region: str,
+        default_vpc: Optional[str],
+        default_subnet: Optional[str],
+    ) -> GCPVPCSubnetProjectElement:
+        if default_vpc is None:
+            default_vpc = "default"
+        if default_subnet is None:
+            default_subnet = "default"
+        no_preference_vpc_subnet = ("default", "default")
+        networks_client = compute_v1.NetworksClient(credentials=self.credentials)
+        networks = networks_client.list(project=self.credentials.project_id)
+        vpc_subnet_list = []
+        for network in networks:
+            for subnet in network.subnetworks:
+                subnet_region = self._get_subnet_region(subnet)
+                if subnet_region != region:
+                    continue
+                vpc_subnet_list.append((network.name, self._get_subnet_name(subnet)))
+        if (default_vpc, default_subnet) not in vpc_subnet_list:
+            raise HubConfigError(f"Invalid VPC subnet {default_vpc, default_subnet}")
+        if (default_vpc, default_subnet) != no_preference_vpc_subnet:
+            selected = f"{default_subnet} ({default_vpc})"
+        else:
+            selected = f"No preference (default)"
+        vpc_subnet_list = sorted(vpc_subnet_list, key=lambda t: t != no_preference_vpc_subnet)
+        element = GCPVPCSubnetProjectElement(selected=selected)
+        for vpc, subnet in vpc_subnet_list:
+            element.values.append(
+                GCPVPCSubnetProjectElementValue(
+                    vpc=vpc,
+                    subnet=subnet,
+                    label=f"{subnet} ({vpc})"
+                    if (subnet, vpc) != no_preference_vpc_subnet
+                    else f"No preference (default)",
+                )
+            )
+        return element
 
     def configure_cli(self):
         credentials_file = None
         region = None
         zone = None
         bucket_name = None
         vpc = None
@@ -310,31 +481,36 @@
             zone_names,
             zone_names,
             default_zone,
         )
         return zone
 
     def _ask_bucket(self, default_bucket: Optional[str]) -> str:
-        console.print(
-            "[sea_green3 bold]?[/sea_green3 bold] [bold]Choose storage bucket[/bold] "
-            "[gray46]Use arrows to move, type to filter[/gray46]"
-        )
         if default_bucket is None:
             default_bucket = f"dstack-{self.project_id}-{self.region}"
-        bucket_options = [f"Default [{default_bucket}]", "Custom..."]
-        bucket_menu = TerminalMenu(
-            bucket_options,
-            menu_cursor_style=["fg_red", "bold"],
-            menu_highlight_style=["fg_red", "bold"],
-            search_highlight_style=["fg_purple"],
-            raise_error_on_interrupt=True,
-        )
-        bucket_index = bucket_menu.show()
-        bucket_title = bucket_options[bucket_index].replace("[", "\\[")
-        console.print(f"[sea_green3 bold]✓[/sea_green3 bold] [grey74]{bucket_title}[/grey74]")
+        if is_termios_available:
+            from simple_term_menu import TerminalMenu
+
+            console.print(
+                "[sea_green3 bold]?[/sea_green3 bold] [bold]Choose storage bucket[/bold] "
+                "[gray46]Use arrows to move, type to filter[/gray46]"
+            )
+            bucket_options = [f"Default [{default_bucket}]", "Custom..."]
+            bucket_menu = TerminalMenu(
+                bucket_options,
+                menu_cursor_style=["fg_red", "bold"],
+                menu_highlight_style=["fg_red", "bold"],
+                search_highlight_style=["fg_purple"],
+                raise_error_on_interrupt=True,
+            )
+            bucket_index = bucket_menu.show()
+            bucket_title = bucket_options[bucket_index].replace("[", "\\[")
+            console.print(f"[sea_green3 bold]✓[/sea_green3 bold] [grey74]{bucket_title}[/grey74]")
+        else:
+            bucket_index = 1
         if bucket_index == 1:
             return self._ask_bucket_name(default_bucket)
         if self._validate_bucket(default_bucket):
             return default_bucket
         return self._ask_bucket_name(default_bucket)
 
     def _ask_bucket_name(self, default_bucket: Optional[str]) -> str:
@@ -380,14 +556,16 @@
 
         return True
 
     def _ask_vpc_subnet(
         self, default_vpc: Optional[str], default_subnet: Optional[str]
     ) -> Tuple[str, str]:
         no_preference_vpc_subnet = ("default", "default")
+        if default_vpc is None or default_subnet is None:
+            default_vpc, default_subnet = no_preference_vpc_subnet
         networks_client = compute_v1.NetworksClient(credentials=self.credentials)
         list_networks_request = compute_v1.ListNetworksRequest(project=self.project_id)
         networks = networks_client.list(list_networks_request)
         subnets = []
         for network in networks:
             for subnet in network.subnetworks:
                 subnet_region = self._get_subnet_region(subnet)
@@ -395,27 +573,29 @@
                     continue
                 subnets.append(
                     {
                         "vpc": network.name,
                         "subnet": self._get_subnet_name(subnet),
                     }
                 )
-        vpc_subnet_values = sorted(
+        vpc_subnets = sorted(
             [(s["vpc"], s["subnet"]) for s in subnets], key=lambda t: t != no_preference_vpc_subnet
         )
+        vpc_subnet_values = [f"{t[0]},{t[1]}" for t in vpc_subnets]
         vpc_subnet_labels = [
             f"{t[1]} [{t[0]}]" if t != no_preference_vpc_subnet else "Default [no preference]"
-            for t in vpc_subnet_values
+            for t in vpc_subnets
         ]
-        vpc, subnet = ask_choice(
+        vpc_subnet = ask_choice(
             "Choose VPC subnet",
             vpc_subnet_labels,
             vpc_subnet_values,
-            (default_vpc, default_subnet),
+            f"{default_vpc},{default_subnet}",
         )
+        vpc, subnet = vpc_subnet.split(",")
         return vpc, subnet
 
     def _get_resource_name(self, resource_path: str) -> str:
         return resource_path.rsplit(sep="/", maxsplit=1)[1]
 
     def _get_region_geographic_area(self, region: Optional[str]) -> Optional[str]:
         if region is None:
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/logs.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import time
-from typing import Generator, Optional
+from datetime import datetime
+from typing import Dict, Generator, Optional
 
 from google.cloud import logging
 from google.oauth2 import service_account
 
 from dstack.backend.base import jobs
 from dstack.backend.base.logs import fix_urls
 from dstack.backend.base.storage import Storage
+from dstack.core.job import Job
 from dstack.core.log_event import LogEvent, LogEventSource
 from dstack.core.repo import RepoAddress
 
 POLL_LOGS_ATTEMPTS = 5
 POLL_LOGS_WAIT_TIME = 2
 
 
@@ -23,44 +25,51 @@
         self.logging_client = logging.Client(project=project_id, credentials=credentials)
 
     def poll_logs(
         self,
         storage: Storage,
         repo_address: RepoAddress,
         run_name: str,
+        start_time: int,
     ) -> Generator[LogEvent, None, None]:
         log_name = _get_log_name(self.bucket_name, repo_address, run_name)
+        timestamp = datetime.fromtimestamp(start_time / 1000).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         logger = self.logging_client.logger(log_name)
+        jobs_cache = {}
         # Hack: It takes some time for logs to become available after runner writes them.
         # So we try reading logs multiple times.
         # The proper solution would be for the runner to ensure logs availability before marking job as Done.
         found_log = False
         for _ in range(POLL_LOGS_ATTEMPTS):
-            log_entries = logger.list_entries()
+            log_entries = logger.list_entries(filter_=f'timestamp>="{timestamp}"')
             for log_entry in log_entries:
                 found_log = True
-                yield _log_entry_to_log_event(storage, repo_address, log_entry)
+                yield _log_entry_to_log_event(storage, repo_address, log_entry, jobs_cache)
             if found_log:
                 break
             time.sleep(POLL_LOGS_WAIT_TIME)
 
 
 def _get_log_name(bucket_name: str, repo_address: RepoAddress, run_name) -> str:
     return f"dstack-jobs-{bucket_name}-{repo_address.path('-')}-{run_name}"
 
 
 def _log_entry_to_log_event(
     storage: Storage,
     repo_address: RepoAddress,
     log_entry: logging.LogEntry,
+    jobs_cache: Dict[str, Job],
 ) -> LogEvent:
     job_id = log_entry.payload["job_id"]
     log = log_entry.payload["log"]
-    job = jobs.get_job(storage, repo_address, job_id)
-    log = fix_urls(log.encode(), job).decode()
+    job = jobs_cache.get(job_id)
+    if job is None:
+        job = jobs.get_job(storage, repo_address, job_id)
+        jobs_cache[job_id] = job
+    log = fix_urls(log.encode(), job, {}).decode()
     timestamp = int(log_entry.timestamp.timestamp())
     return LogEvent(
         event_id=log_entry.insert_id,
         timestamp=timestamp,
         job_id=job_id,
         log_message=log,
         log_source=LogEventSource.STDOUT
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/storage.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/gcp/utils.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,9 +46,9 @@
 
     return result
 
 
 def is_valid_label_value(value: str) -> bool:
     if len(value) > 63:
         return False
-    m = re.match(r"^[\w\d_-]+$", value)
+    m = re.match(r"^[a-z\d_-]+$", value)
     return m is not None
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/hub/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dstack.backend.base import artifacts as base_artifacts
 from dstack.backend.hub.client import HubClient
 from dstack.backend.hub.config import HUBConfig, HubConfigurator
 from dstack.backend.hub.storage import HUBStorage
 from dstack.core.artifact import Artifact
 from dstack.core.config import BackendConfig
 from dstack.core.error import ConfigError
-from dstack.core.job import Job, JobHead
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
 from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 
 
@@ -33,14 +33,15 @@
         except ConfigError:
             self._loaded = False
 
     def _hub_client(self) -> HubClient:
         if self._client is None:
             self._client = HubClient(
                 url=self.backend_config.url,
+                project=self.backend_config.project,
                 token=self.backend_config.token,
             )
         return self._client
 
     @property
     def name(self):
         return "hub"
@@ -60,15 +61,15 @@
 
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         return self._hub_client().get_job(repo_address=repo_address, job_id=job_id)
 
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         return self._hub_client().list_jobs(repo_address=repo_address, run_name=run_name)
 
-    def run_job(self, job: Job):
+    def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
         self._hub_client().run_job(job=job)
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         self._hub_client().stop_job(repo_address=repo_address, job_id=job_id, abort=abort)
 
     def list_job_heads(
         self, repo_address: RepoAddress, run_name: Optional[str] = None
@@ -79,14 +80,15 @@
         self._hub_client().delete_job_head(repo_address=repo_address, job_id=job_id)
 
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         return self._hub_client().list_run_heads(
             repo_address=repo_address,
             run_name=run_name,
             include_request_heads=include_request_heads,
         )
 
@@ -112,22 +114,24 @@
         )
 
     def download_run_artifact_files(
         self,
         repo_address: RepoAddress,
         run_name: str,
         output_dir: Optional[str],
+        files_path: Optional[str] = None,
     ):
         # /{hub_name}/artifacts/download
         artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
             repo_address=repo_address,
             artifacts=artifacts,
             output_dir=output_dir,
+            files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
         repo_address: RepoAddress,
         job_id: str,
         artifact_name: str,
@@ -201,7 +205,12 @@
 
     def delete_secret(self, repo_address: RepoAddress, secret_name: str):
         # /{hub_name}/secrets/delete
         self._hub_client().delete_secret(repo_address=repo_address, secret_name=secret_name)
 
     def get_configurator(self):
         return HubConfigurator()
+
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
+        self._hub_client().delete_workflow_cache(
+            repo_address=repo_address, username=username, workflow_name=workflow_name
+        )
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/hub/client.py` & `dstack-0.7rc1/cli/dstack/backend/hub/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,67 +3,67 @@
 from urllib.parse import urlencode, urlparse, urlunparse
 
 import requests
 
 from dstack.core.artifact import Artifact
 from dstack.core.job import Job, JobHead
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
+from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 from dstack.hub.models import (
     AddTagPath,
     AddTagRun,
     JobsGet,
     JobsList,
     LinkUpload,
     PollLogs,
     ReposUpdate,
     RunsList,
+    SaveRepoCredentials,
     SecretAddUpdate,
     StopRunners,
+    UserRepoAddress,
 )
 
 
-def _url(url: str, additional_path: str, query: dict = {}):
+def _url(url: str, project: str, additional_path: str, query: dict = {}):
     unparse_url = urlparse(url=url)
-    new_path = unparse_url.path
-    if new_path.endswith("/"):
-        new_path = new_path[: len(new_path) - 1]
     if additional_path.startswith("/"):
         additional_path = additional_path[1:]
 
     new_url = urlunparse(
         (
             unparse_url.scheme,
             unparse_url.netloc,
-            f"{new_path}/{additional_path}",
+            f"/api/project/{project}/{additional_path}",
             None,
             urlencode(query=query),
             unparse_url.fragment,
         )
     )
     return new_url
 
 
 class HubClient:
-    def __init__(self, url: str, token: str):
+    def __init__(self, url: str, project: str, token: str):
         self.url = url
         self.token = token
+        self.project = project
 
     @staticmethod
-    def validate(url: str, token: str) -> bool:
-        url = _url(url=url, additional_path="/info")
+    def validate(url: str, project: str, token: str) -> bool:
+        url = _url(url=url, project=project, additional_path="/info")
         try:
             resp = requests.get(url=url, headers=HubClient._auth(token=token))
             if resp.ok:
                 print(resp.json())
                 return True
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return False
         except requests.ConnectionError:
             print(f"{url} connection refused")
         return False
 
     @staticmethod
@@ -77,169 +77,194 @@
         headers = HubClient._auth(token=self.token)
         headers["Content-type"] = "application/json"
         return headers
 
     def get_repos_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
         url = _url(
             url=self.url,
-            additional_path=f"/repos/credentials",
+            project=self.project,
+            additional_path=f"/repos/credentials/get",
         )
         try:
-            resp = requests.get(url=url, headers=self._headers(), data=repo_address.json())
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 json_data = resp.json()
-                return RepoCredentials(
-                    protocol=json_data["protocol"],
-                    private_key=json_data["private_key"],
-                    oauth_token=json_data["oauth_token"],
-                )
-            if resp.status_code == 401:
+                return RepoCredentials(**json_data)
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def save_repos_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
         url = _url(
             url=self.url,
-            additional_path=f"/repos/credentials",
+            project=self.project,
+            additional_path=f"/repos/credentials/save",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
-                data={
-                    "repo_address": repo_address.json(),
-                    "repo_credentials": repo_credentials.json(),
-                },
+                data=SaveRepoCredentials(
+                    repo_address=repo_address,
+                    repo_credentials=repo_credentials,
+                ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def create_run(self, repo_address: RepoAddress) -> str:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/runs/create",
         )
         try:
             resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 return resp.text
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return ""
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return ""
 
     def create_job(self, job: Job):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/jobs/create",
         )
         try:
             resp = requests.post(url=url, headers=self._headers(), data=job.json())
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def run_job(self, job: Job):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/runners/run",
         )
         try:
             resp = requests.post(url=url, headers=self._headers(), data=job.json())
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/runners/stop",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=StopRunners(
                     repo_address=repo_address,
                     job_id=job_id,
                     abort=abort,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/tags/{tag_name}",
         )
         try:
-            resp = requests.get(url=url, headers=self._headers(), data=repo_address.json())
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 return TagHead.parse_obj(resp.json())
-            if resp.status_code == 401:
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def list_tag_heads(self, repo_address: RepoAddress) -> Optional[List[TagHead]]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/tags/list/heads",
         )
         try:
-            resp = requests.get(url=url, headers=self._headers(), data=repo_address.json())
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 body = resp.json()
                 return [TagHead.parse_obj(tag) for tag in body]
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def add_tag_from_run(
         self,
         repo_address: RepoAddress,
         tag_name: str,
         run_name: str,
         run_jobs: Optional[List[Job]],
     ):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/tags/add/run",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=AddTagRun(
@@ -247,345 +272,393 @@
                     tag_name=tag_name,
                     run_name=run_name,
                     run_jobs=run_jobs,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def add_tag_from_local_dirs(
         self,
         repo_data: LocalRepoData,
         tag_name: str,
         local_dirs: List[str],
     ):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/tags/add/path",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=AddTagPath(
                     repo_data=repo_data,
                     tag_name=tag_name,
                     local_dirs=local_dirs,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/tags/{tag_head.tag_name}/delete",
         )
         try:
             resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/repos/update",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=ReposUpdate(
                     repo_address=repo_address,
                     last_run_at=last_run_at,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def list_job_heads(
         self, repo_address: RepoAddress, run_name: Optional[str] = None
     ) -> Optional[List[JobHead]]:
         query = {}
         if not (run_name is None):
             query["run_name"] = run_name
-        url = _url(url=self.url, additional_path=f"/jobs/list/heads", query=query)
+        url = _url(
+            url=self.url, project=self.project, additional_path=f"/jobs/list/heads", query=query
+        )
         try:
-            resp = requests.get(url=url, headers=self._headers(), data=repo_address.json())
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
             if resp.ok:
                 body = resp.json()
                 return [JobHead.parse_obj(job) for job in body]
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
     ) -> List[RunHead]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/runs/list",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=RunsList(
                     repo_address=repo_address,
                     run_name=run_name,
                     include_request_heads=include_request_heads,
                 ).json(),
             )
             if resp.ok:
                 body = resp.json()
                 return [RunHead.parse_obj(run) for run in body]
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return []
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return []
 
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/jobs/get",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=JobsGet(
                     repo_address=repo_address,
                     job_id=job_id,
                 ).json(),
             )
             if resp.ok:
                 json_data = resp.json()
                 return Job.parse_obj(json_data)
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/secrets/list",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=repo_address.json(),
             )
             if resp.ok:
                 json_data = resp.json()
                 return json_data
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return []
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return []
 
     def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
         url = _url(
             url=self.url,
-            additional_path=f"/secrets/get/{secret_name}",
+            project=self.project,
+            additional_path=f"/secrets/{secret_name}/get",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=repo_address.json(),
             )
             if resp.ok:
                 json_data = resp.json()
                 return Secret.parse_obj(json_data)
-            if resp.status_code == 401:
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def add_secret(self, repo_address: RepoAddress, secret: Secret):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/secrets/add",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=SecretAddUpdate(
                     repo_address=repo_address,
                     secret=secret,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def update_secret(self, repo_address: RepoAddress, secret: Secret):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/secrets/update",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=SecretAddUpdate(
                     repo_address=repo_address,
                     secret=secret,
                 ).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def delete_secret(self, repo_address: RepoAddress, secret_name: str):
         url = _url(
             url=self.url,
-            additional_path=f"/secrets/delete/{secret_name}",
+            project=self.project,
+            additional_path=f"/secrets/{secret_name}/delete",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=repo_address.json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/jobs/list",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=JobsList(repo_address=repo_address, run_name=run_name).json(),
             )
             if resp.ok:
                 job_data = resp.json()
                 return [Job.parse_obj(job) for job in job_data]
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return []
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return []
 
     def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/artifacts/list",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=JobsList(repo_address=repo_address, run_name=run_name).json(),
             )
             if resp.ok:
                 artifact_data = resp.json()
                 return [Artifact.parse_obj(artifact) for artifact in artifact_data]
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return []
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return []
 
     def delete_job_head(self, repo_address: RepoAddress, job_id: str):
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/jobs/delete",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=JobsGet(repo_address=repo_address, job_id=job_id).json(),
             )
             if resp.ok:
                 return None
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def poll_logs(
         self,
         repo_address: RepoAddress,
         job_heads: List[JobHead],
         start_time: int,
         attached: bool,
     ) -> Generator[LogEvent, None, None]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/logs/poll",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=PollLogs(
                     repo_address=repo_address,
                     job_heads=job_heads,
                     start_time=start_time,
                     attached=attached,
@@ -603,53 +676,83 @@
                             _braces -= 1
                         _body.append(b)
 
                         if _braces == 0:
                             json_data = json.loads(_body)
                             _body = bytearray()
                             yield LogEvent.parse_obj(json_data)
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def upload_file(self, dest_path: str) -> Optional[str]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/link/upload",
         )
         try:
             resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=LinkUpload(object_key=dest_path).json(),
             )
             if resp.ok:
                 return resp.text
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
 
     def download_file(self, dest_path: str) -> Optional[str]:
         url = _url(
             url=self.url,
+            project=self.project,
             additional_path=f"/link/download",
         )
         try:
-            resp = requests.get(
+            resp = requests.post(
                 url=url,
                 headers=self._headers(),
                 data=LinkUpload(object_key=dest_path).json(),
             )
             if resp.ok:
                 return resp.text
-            if resp.status_code == 401:
+            elif resp.status_code == 401:
                 print("Unauthorized. Please set correct token")
                 return None
+            else:
+                resp.raise_for_status()
         except requests.ConnectionError:
             print(f"{self.url} connection refused")
         return None
+
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
+        url = _url(
+            url=self.url,
+            project=self.project,
+            additional_path=f"/workflows/{workflow_name}/cache/delete",
+        )
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=UserRepoAddress(username=username, repo_address=repo_address).json(),
+            )
+            if resp.ok:
+                return
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/hub/config.py` & `dstack-0.7rc1/cli/dstack/backend/hub/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,122 @@
 import os
+from argparse import Namespace
 from pathlib import Path
-from typing import Any
-from urllib.parse import urlparse, urlunparse
+from typing import Any, Dict, Optional, Tuple
 
 import yaml
 from rich import print
 from rich.prompt import Prompt
+from rich_argparse import RichHelpFormatter
 
 from dstack.backend.hub.client import HubClient
 from dstack.core.config import BackendConfig, Configurator, get_config_path
 from dstack.core.error import ConfigError
 
 
 class HUBConfig(BackendConfig):
     NAME = "hub"
 
     def __init__(self):
         super().__init__()
         self.url = os.getenv("DSTACK_HUB_URL") or None
+        self.project = os.getenv("DSTACK_HUB_PROJECT") or None
         self.token = os.getenv("DSTACK_HUB_TOKEN") or None
 
     def load(self, path: Path = get_config_path()):
         if path.exists():
             with path.open() as f:
                 config_data = yaml.load(f, Loader=yaml.FullLoader)
                 if config_data.get("backend") != self.NAME:
                     raise ConfigError(f"It's not HUB config")
                 if config_data.get("url") is None:
                     raise ConfigError(f"For HUB backend:the URL field is required")
                 if config_data.get("token") is None:
                     raise ConfigError(f"For HUB backend:the token field is required")
+                if config_data.get("project") is None:
+                    raise ConfigError(f"For HUB backend:the project field is required")
                 self.url = config_data.get("url")
+                self.project = config_data.get("project")
                 self.token = config_data.get("token")
         else:
             raise ConfigError()
 
     def save(self, path: Path = get_config_path()):
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
-        unparse_url = urlparse(url=self.url)
-        new_path = unparse_url.path
-        if not new_path.endswith("/api/hub/"):
-            new_path = "/api/hub" + new_path
-
-        new_url = urlunparse(
-            (
-                unparse_url.scheme,
-                unparse_url.netloc,
-                new_path,
-                None,
-                None,
-                None,
-            )
-        )
         with path.open("w") as f:
             config_data = {
                 "backend": self.NAME,
-                "url": new_url,
+                "url": self.url,
+                "project": self.project,
                 "token": self.token,
             }
             yaml.dump(config_data, f)
 
 
 class HubConfigurator(Configurator):
     NAME = "hub"
 
-    def get_config(self, config: Any):
+    def get_config_from_hub_config_data(self, config_data: Any, auth_data: Dict) -> BackendConfig:
         pass
 
     def get_backend_client(self, config: Any):
         pass
 
     def configure_hub(self, config: Any):
         pass
 
-    def parse_args(self, args: list = []):
-        if len(args) % 2 != 0:
-            raise ConfigError("Arguments must be even")
-        config = HUBConfig()
-        for idx in range(0, len(args), 2):
-            arg = str(args[idx])
-            if arg.startswith("--"):
-                arg = arg[2:]
-            if hasattr(config, arg):
-                setattr(config, arg, args[idx + 1])
-        config.save()
-        print(f"[grey58]OK[/]")
-
     def configure_cli(self) -> HUBConfig:
         config = HUBConfig()
         try:
             config.load()
         except ConfigError:
             pass
         default_url = config.url
         default_token = config.token
+        default_project = config.project
 
         config.url, config.token = self.ask_new_param(
             default_url=default_url,
+            default_project=default_project,
             default_token=default_token,
         )
         config.save()
         print(f"[grey58]OK[/]")
 
-    def ask_new_param(self, default_url: str, default_token: str) -> (str, str):
+    def ask_new_param(
+        self, default_url: str, default_project: str, default_token: str
+    ) -> Tuple[str, str, str]:
         url = Prompt.ask(
             "[sea_green3 bold]?[/sea_green3 bold] [bold]Enter HUB URL[/bold]",
             default=default_url,
         )
+        project = Prompt.ask(
+            "[sea_green3 bold]?[/sea_green3 bold] [bold]Enter HUB project[/bold]",
+            default=default_project,
+        )
         token = Prompt.ask(
             "[sea_green3 bold]?[/sea_green3 bold] [bold]Enter HUB token[/bold]",
             default=default_token,
         )
-        if HubClient.validate(url=url, token=token):
-            return url, token
+        if HubClient.validate(url=url, project=project, token=token):
+            return url, project, token
         return self.ask_new_param(
             default_url=url,
+            default_project=project,
             default_token=token,
         )
+
+    def register_parser(self, parser):
+        hub_parser = parser.add_parser("hub", help="", formatter_class=RichHelpFormatter)
+        hub_parser.add_argument("--url", type=str, help="", required=True)
+        hub_parser.add_argument("--project", type=str, help="", required=True)
+        hub_parser.add_argument("--token", type=str, help="", required=True)
+        hub_parser.set_defaults(func=self._command)
+
+    def _command(self, args: Namespace):
+        config = HUBConfig()
+        config.url = args.url
+        config.project = args.project
+        config.token = args.token
+        config.save()
+        print(f"[grey58]OK[/]")
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/hub/storage.py` & `dstack-0.7rc1/cli/dstack/backend/hub/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/local/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
 from typing import Generator, List, Optional, Tuple
 
 from dstack.backend.base import Backend, BackendType
 from dstack.backend.base import artifacts as base_artifacts
+from dstack.backend.base import cache as base_cache
 from dstack.backend.base import jobs as base_jobs
 from dstack.backend.base import repos as base_repos
 from dstack.backend.base import runs as base_runs
 from dstack.backend.base import secrets as base_secrets
 from dstack.backend.base import tags as base_tags
 from dstack.backend.local import artifacts, logs
 from dstack.backend.local.compute import LocalCompute
 from dstack.backend.local.config import LocalConfig
 from dstack.backend.local.secrets import LocalSecretsManager
 from dstack.backend.local.storage import LocalStorage
 from dstack.core.artifact import Artifact
-from dstack.core.job import Job, JobHead
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
 from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 
 
@@ -50,16 +51,16 @@
 
     def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         return base_jobs.get_job(self._storage, repo_address, job_id)
 
     def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
         return base_jobs.list_jobs(self._storage, repo_address, run_name)
 
-    def run_job(self, job: Job):
-        base_jobs.run_job(self._storage, self._compute, job)
+    def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
+        base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         base_jobs.stop_job(self._storage, self._compute, repo_address, job_id, abort)
 
     def list_job_heads(
         self, repo_address: RepoAddress, run_name: Optional[str] = None
     ) -> List[JobHead]:
@@ -69,18 +70,23 @@
         base_jobs.delete_job_head(self._storage, repo_address, job_id)
 
     def list_run_heads(
         self,
         repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         job_heads = self.list_job_heads(repo_address, run_name)
         return base_runs.get_run_heads(
-            self._storage, self._compute, job_heads, include_request_heads
+            self._storage,
+            self._compute,
+            job_heads,
+            include_request_heads,
+            interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
         repo_address: RepoAddress,
         job_heads: List[JobHead],
         start_time: int,
@@ -94,21 +100,23 @@
         return base_artifacts.list_run_artifact_files(self._storage, repo_address, run_name)
 
     def download_run_artifact_files(
         self,
         repo_address: RepoAddress,
         run_name: str,
         output_dir: Optional[str],
+        files_path: Optional[str] = None,
     ):
         list_artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
             repo_address=repo_address,
             artifacts=list_artifacts,
             output_dir=output_dir,
+            files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
         repo_address: RepoAddress,
         job_id: str,
         artifact_name: str,
@@ -207,7 +215,10 @@
         )
 
     def get_artifacts_path(self, repo_address: RepoAddress) -> Path:
         return artifacts.get_artifacts_path(self.backend_config.path, repo_address)
 
     def get_configurator(self):
         pass
+
+    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_address, username, workflow_name)
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/compute.py` & `dstack-0.7rc1/cli/dstack/backend/local/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/config.py` & `dstack-0.7rc1/cli/dstack/backend/local/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/logs.py` & `dstack-0.7rc1/cli/dstack/backend/local/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,13 +82,14 @@
     storage: Storage,
     compute: Compute,
     repo_address: RepoAddress,
     job_heads: List[JobHead],
     start_time: int,
     attached: bool,
 ) -> Generator[LogEvent, None, None]:
+    jobs_cache = {}
     try:
         # Read log_file
         for event in events_loop(storage, compute, repo_address, job_heads):
-            yield render_log_message(storage, event, repo_address)
+            yield render_log_message(storage, event, repo_address, jobs_cache)
     except Exception as e:
         raise e
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/runners.py` & `dstack-0.7rc1/cli/dstack/backend/local/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/local/secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,15 @@
     cur = con.cursor()
     cur.execute("DELETE FROM KV WHERE secret_name=?", (key,))
     con.commit()
     con.close()
 
 
 def _check_db(db_filepath: str):
-    if not Path(db_filepath).exists():
-        Path(db_filepath).parent.mkdir(parents=True)
+    Path(db_filepath).parent.mkdir(exist_ok=True, parents=True)
     if not os.path.exists(db_filepath):
         con = sqlite3.connect(db_filepath)
         cur = con.cursor()
         cur.execute("""CREATE TABLE IF NOT EXISTS KV (secret_name TEXT, secret_string TEXT);""")
         con.commit()
         con.close()
```

### Comparing `dstack-0.2rc1/cli/dstack/backend/local/storage.py` & `dstack-0.7rc1/cli/dstack/backend/local/storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -63,14 +63,25 @@
 
     def upload_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         full_dest_path = os.path.join(self.root_path, dest_path)
         Path(full_dest_path).parent.mkdir(parents=True, exist_ok=True)
         shutil.copy2(source_path, full_dest_path)
         callback(os.path.getsize(source_path))
 
+    def delete_prefix(self, keys_prefix: str):
+        if keys_prefix.endswith("/"):
+            shutil.rmtree(Path(self.root_path) / keys_prefix, ignore_errors=True)
+        else:
+            prefix_path = Path(self.root_path) / keys_prefix
+            for file in prefix_path.parent.glob(f"{prefix_path.name}*"):
+                if file.is_dir():
+                    shutil.rmtree(file, ignore_errors=True)
+                else:
+                    file.unlink()
+
 
 def _list_objects(Root: str, Prefix: str, MaxKeys: Optional[int] = None) -> List[str]:
     prefix_path = Path.joinpath(Root, Prefix)
     parent_dir = prefix_path.parent
     file_prefix = prefix_path.name
     if not os.path.exists(parent_dir):
         return []
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 from argparse import Namespace, _SubParsersAction
 
 from rich_argparse import RichHelpFormatter
 
 from dstack.cli.updates import check_for_updates
 
 
@@ -16,15 +17,16 @@
             kwargs["help"] = self.description
         self._parser = parser.add_parser(
             self.name, add_help=False, formatter_class=RichHelpFormatter, **kwargs
         )
         self._parser.add_argument(
             "-h",
             "--help",
-            action="help",
+            action="store_true" if self.name == "run" else "help",
+            default=argparse.SUPPRESS,
             help="Show this help message and exit",
         )
         self._parser.set_defaults(func=self.__command)
 
     @property
     def name(self):
         return self.NAME
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/hub/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,44 +11,63 @@
 class HubCommand(BasicCommand):
     NAME = "hub"
     DESCRIPTION = None  # Hidden by default
 
     def __init__(self, parser):
         super(HubCommand, self).__init__(parser)
 
-    def hub_start(self, args: Namespace):
+    def _hub_start(self, args: Namespace):
         os.environ["DSTACK_HUB_HOST"] = args.host
         os.environ["DSTACK_HUB_PORT"] = str(args.port)
+        os.environ["DSTACK_HUB_LOG_LEVEL"] = args.log_level
         if args.token:
             os.environ["DSTACK_HUB_ADMIN_TOKEN"] = args.token
         uvicorn.run(
             "dstack.hub.main:app",
             host=args.host,
             port=args.port,
             reload=version.__version__ is None,
             log_level="error",
         )
 
     def register(self):
         subparsers = self._parser.add_subparsers()
-
         hub_parser = subparsers.add_parser(
-            "start", help="Start a hub server", formatter_class=RichHelpFormatter
+            "start",
+            help="Start a hub server",
+            formatter_class=RichHelpFormatter,
+            add_help=False,
+        )
+        hub_parser.add_argument(
+            "-h",
+            "--help",
+            action="help",
+            help="Show this help message and exit",
         )
-
         hub_parser.add_argument(
             "--host",
             metavar="HOST",
             type=str,
-            help="Bind socket to this host.  Default: 127.0.0.1",
+            help="Bind socket to this host. Defaults to 127.0.0.1",
             default="127.0.0.1",
         )
         hub_parser.add_argument(
             "-p",
             "--port",
             metavar="PORT",
             type=int,
-            help="Bind socket to this port. Default: 3000.",
+            help="Bind socket to this port. Defaults to 3000.",
             default=3000,
         )
+        hub_parser.add_argument(
+            "-l",
+            "--log-level",
+            metavar="LOG-LEVEL",
+            type=str,
+            help="",
+            default="ERROR",
+        )
         hub_parser.add_argument("--token", metavar="TOKEN", type=str, help="The admin user token")
-        hub_parser.set_defaults(func=self.hub_start)
+        hub_parser.set_defaults(func=self._hub_start)
+
+    def _command(self, args: Namespace):
+        self._parser.print_help()
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/logs/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 from argparse import Namespace
 
-from rich.table import Table
+from rich.prompt import Confirm
 
-from dstack.api.artifacts import list_artifacts_with_merged_backends
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
-from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
 from dstack.cli.common import console
 from dstack.core.error import check_config, check_git
-from dstack.utils.common import sizeof_fmt
 
 
-class LsCommand(BasicCommand):
-    NAME = "ls"
-    DESCRIPTION = "List artifacts"
+def _verb(abort: bool):
+    if abort:
+        return "Abort"
+    else:
+        return "Stop"
+
+
+class StopCommand(BasicCommand):
+    NAME = "stop"
+    DESCRIPTION = "Stop run(s)"
 
     def __init__(self, parser):
-        super(LsCommand, self).__init__(parser)
+        super(StopCommand, self).__init__(parser)
 
     def register(self):
         self._parser.add_argument(
-            "run_name_or_tag_name",
-            metavar="RUN | :TAG",
-            type=str,
-            help="A name of a run or a tag",
+            "run_name", metavar="RUN", type=str, nargs="?", help="A name of a run"
+        )
+        self._parser.add_argument(
+            "-a",
+            "--all",
+            help="Stop all unfinished runs",
+            dest="all",
+            action="store_true",
+        )
+        self._parser.add_argument(
+            "-x",
+            "--abort",
+            help="Don't wait for a graceful stop and abort the run immediately",
+            dest="abort",
+            action="store_true",
+        )
+        self._parser.add_argument(
+            "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
 
     @check_config
     @check_git
     def _command(self, args: Namespace):
-        table = Table(box=None)
-        table.add_column("ARTIFACT", style="bold", no_wrap=True)
-        table.add_column("FILE")
-        table.add_column("SIZE", style="dark_sea_green4")
-        table.add_column("BACKENDS", style="bold")
-
-        repo_data = load_repo_data()
-        backends = list_backends()
-        run_names = []
-        backends_run_name = []
-        for backend in backends:
-            try:
-                run_name, _ = get_tagged_run_name(repo_data, backend, args.run_name_or_tag_name)
-                run_names.append(run_name)
-                backends_run_name.append(backend)
-            except (TagNotFoundError, RunNotFoundError):
-                pass
-
-        if len(run_names) == 0:
-            console.print(f"Cannot find the run or tag '{args.run_name_or_tag_name}'")
+        if not args.run_name and not args.all:
+            console.print("Specify a run name or use --all to stop all workflows")
             exit(1)
-
-        artifacts = list_artifacts_with_merged_backends(
-            backends_run_name, load_repo_data(), run_names[0]
-        )
-        for artifact, backends in artifacts:
-            for i, file in enumerate(artifact.files):
-                table.add_row(
-                    artifact.name if i == 0 else "",
-                    file.filepath,
-                    sizeof_fmt(file.filesize_in_bytes),
-                    ", ".join(b.name for b in backends),
-                )
-        console.print(table)
+        if (
+            args.run_name
+            and (
+                args.yes or Confirm.ask(f"[red]{_verb(args.abort)} the run '{args.run_name}'?[/]")
+            )
+        ) or (args.all and (args.yes or Confirm.ask(f"[red]{_verb(args.abort)} all runs?[/]"))):
+            repo_data = load_repo_data()
+            found_run = False
+            for backend in list_backends():
+                job_heads = backend.list_job_heads(repo_data, args.run_name)
+                found_run = len(job_heads) > 0
+                for job_head in job_heads:
+                    if job_head.status.is_unfinished():
+                        backend.stop_job(repo_data, job_head.job_id, args.abort)
+            if args.run_name and not found_run:
+                console.print(f"Cannot find the run '{args.run_name}'")
+                exit(1)
+            console.print(f"[grey58]OK[/]")
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/pull/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/pull/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/push/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/push/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/run/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/run/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 from dstack.api.backend import get_backend_by_name, get_current_remote_backend, get_local_backend
 from dstack.api.logs import poll_logs
 from dstack.api.repo import load_repo_data
 from dstack.api.run import list_runs_with_merged_backends
 from dstack.backend.base import Backend
 from dstack.backend.base.logs import fix_urls
 from dstack.cli.commands import BasicCommand
+from dstack.cli.commands.run.ssh_tunnel import allocate_local_ports, run_ssh_tunnel
 from dstack.cli.common import console, print_runs
+from dstack.cli.config import BaseConfig
 from dstack.core.error import check_backend, check_config, check_git
-from dstack.core.job import JobHead, JobStatus
+from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.repo import RepoAddress
 from dstack.core.request import RequestStatus
+from dstack.core.userconfig import RepoUserConfig
 from dstack.utils.common import since
 
 __all__ = "RunCommand"
 
 POLL_PROVISION_RATE_SECS = 3
 
 POLL_FINISHED_STATE_RATE_SECS = 1
@@ -58,14 +61,19 @@
                 if workflows_file_path.name.endswith(".yaml") or workflows_file_path.name.endswith(
                     ".yml"
                 ):
                     workflows.extend(_load_workflows_from_file(workflows_file_path))
     return workflows
 
 
+def _read_ssh_key_pub(key_path: str) -> str:
+    path = Path(key_path)
+    return path.with_suffix(path.suffix + ".pub").read_text().strip("\n")
+
+
 def parse_run_args(
     args: Namespace,
 ) -> Tuple[str, List[str], Optional[str], Dict[str, Any]]:
     provider_args = args.args + args.unknown
     workflow_name = None
     workflow_data = {}
 
@@ -82,64 +90,72 @@
             sys.exit(f"No workflow or provider '{args.workflow_or_provider}' is found")
 
         provider_name = args.workflow_or_provider
 
     return provider_name, provider_args, workflow_name, workflow_data
 
 
-def poll_logs_ws(backend: Backend, repo_address: RepoAddress, job_head: JobHead):
-    job = backend.get_job(repo_address, job_head.job_id)
-
+def poll_logs_ws(backend: Backend, repo_address: RepoAddress, job: Job, ports: Dict[int, int]):
     def on_message(ws: WebSocketApp, message):
-        message = fix_urls(message, job)
+        message = fix_urls(message, job, ports, hostname="127.0.0.1")
         sys.stdout.buffer.write(message)
         sys.stdout.buffer.flush()
 
     def on_error(_: WebSocketApp, err: Exception):
         if isinstance(err, KeyboardInterrupt):
-            run_name = job_head.run_name
+            run_name = job.run_name
             if Confirm.ask(f"\n [red]Abort the run '{run_name}'?[/]"):
                 backend.stop_jobs(repo_address, run_name, abort=True)
                 console.print(f"[grey58]OK[/]")
             exit()
         else:
             console.print(err)
 
     def on_open(_: WebSocketApp):
         pass
 
     def on_close(_: WebSocketApp, close_status_code, close_msg):
         pass
 
-    url = f"ws://{job.host_name}:{job.env['WS_LOGS_PORT']}/logsws"
-    cursor.hide()
+    local_ws_logs_port = ports.get(int(job.env["WS_LOGS_PORT"]), int(job.env["WS_LOGS_PORT"]))
+    url = f"ws://127.0.0.1:{local_ws_logs_port}/logsws"
+    atty = sys.stdout.isatty()
+    if atty:
+        cursor.hide()
     _ws = websocket.WebSocketApp(
         url,
         on_message=on_message,
         on_error=on_error,
         on_open=on_open,
         on_close=on_close,
     )
     _ws.run_forever()
-    cursor.show()
+    if atty:
+        cursor.show()
 
     try:
         while True:
-            _job_head = backend.get_job(repo_address, job_head.job_id)
+            _job_head = backend.get_job(repo_address, job.job_id)
             run = backend.list_run_heads(repo_address, _job_head.run_name)[0]
             if run.status.is_finished():
                 break
             time.sleep(POLL_FINISHED_STATE_RATE_SECS)
     except KeyboardInterrupt:
         if Confirm.ask(f"\n [red]Abort the run '{job.run_name}'?[/]"):
             backend.stop_jobs(repo_address, job.run_name, abort=True)
             console.print(f"[grey58]OK[/]")
 
 
-def poll_run(repo_address: RepoAddress, job_heads: List[JobHead], backend: Backend):
+def poll_run(
+    repo_address: RepoAddress,
+    job_heads: List[JobHead],
+    backend: Backend,
+    ssh_key: Optional[str],
+    openssh_server: bool,
+):
     run_name = job_heads[0].run_name
     try:
         console.print()
         request_errors_printed = False
         downloading = False
         with Progress(
             TextColumn("[progress.description]{task.description}"),
@@ -173,20 +189,41 @@
                         progress.update(task, description=f"[dark_orange]No capacity[/]")
                         request_errors_printed = True
                 elif request_errors_printed:
                     progress.update(
                         task, description="Provisioning... It may take up to a minute."
                     )
                     request_errors_printed = False
-        console.print("Provisioning... It may take up to a minute. [green]✓[/]")
+
+        jobs = [backend.get_job(repo_address, job_head.job_id) for job_head in job_heads]
+        ports = {}
+        if backend.name != "local":
+            console.print("Starting SSH tunnel...")
+            ports = allocate_local_ports(jobs)
+            if not run_ssh_tunnel(
+                ssh_key, jobs[0].host_name, ports
+            ):  # todo: cleanup explicitly (stop tunnel)
+                console.print("[warning]Warning: failed to start SSH tunnel[/warning] [red]✗[/]")
+        else:
+            console.print("Provisioning... It may take up to a minute. [green]✓[/]")
         console.print()
         console.print("[grey58]To interrupt, press Ctrl+C.[/]")
         console.print()
+
+        if openssh_server:
+            ssh_port = jobs[0].ports[-1]
+            ssh_port = ports.get(ssh_port, ssh_port)
+            ssh_key_escaped = ssh_key.replace(" ", "\\ ")
+            console.print("To connect via SSH, use:")
+            console.print(f"  ssh -i {ssh_key_escaped} root@localhost -p {ssh_port}")
+            console.print()
+
+        run = backend.list_run_heads(repo_address, run_name)[0]
         if len(job_heads) == 1 and run and run.status == JobStatus.RUNNING:
-            poll_logs_ws(backend, repo_address, job_heads[0])
+            poll_logs_ws(backend, repo_address, jobs[0], ports)
         else:
             poll_logs(
                 backend,
                 repo_address,
                 job_heads,
                 since("1d"),
                 attach=True,
@@ -202,23 +239,25 @@
     NAME = "run"
     DESCRIPTION = "Run a workflow"
 
     def __init__(self, parser):
         super(RunCommand, self).__init__(parser)
 
     def register(self):
-        workflow_help = "A name of the workflow"
         workflows = _load_workflows()
-        if len(workflows) > 0:
-            workflow_help = "{" + ",".join(w["name"] for w in workflows if w.get("name")) + "}"
+        workflow_names = [w["name"] for w in workflows if w.get("name")]
+        provider_names = providers.get_provider_names()
+        workflow_or_provider_names = workflow_names + provider_names
+        workflow_help = "{" + ",".join(workflow_or_provider_names) + "}"
         self._parser.add_argument(
             "workflow_or_provider",
-            metavar="WORKFLOW",
+            metavar="WORKFLOW | PROVIDER",
             type=str,
             help=workflow_help,
+            choices=workflow_or_provider_names,
             nargs="?",
         )
         self._parser.add_argument(
             "--remote",
             metavar="BACKEND",
             nargs=argparse.ZERO_OR_MORE,
             help="",
@@ -238,25 +277,26 @@
             help="Do not poll for status update and logs",
             action="store_true",
         )
         self._parser.add_argument(
             "args",
             metavar="ARGS",
             nargs=argparse.ZERO_OR_MORE,
-            help="Override provider arguments",
+            help="Override workflow or provider arguments",
         )
 
     @check_config
     @check_git
     @check_backend
     def _command(self, args: Namespace):
         if not args.workflow_or_provider:
             self._parser.print_help()
             exit(1)
         try:
+            config = BaseConfig()
             repo_data = load_repo_data()
             backend = get_local_backend()
             if args.remote is not None:
                 if len(args.remote) == 0:
                     remote_backend = get_current_remote_backend()
                     if remote_backend is None:
                         console.print(f"No remote configured. Run `dstack config`.")
@@ -275,27 +315,55 @@
                 workflow_data,
             ) = parse_run_args(args)
             provider = providers.load_provider(provider_name)
             if hasattr(args, "help") and args.help:
                 provider.help(workflow_name)
                 sys.exit()
 
-            if backend.get_repo_credentials(repo_data):
-                run_name = backend.create_run(repo_data)
-                provider.load(backend, provider_args, workflow_name, workflow_data, run_name)
-                if args.tag_name:
-                    tag_head = backend.get_tag_head(repo_data, args.tag_name)
-                    if tag_head:
-                        backend.delete_tag_head(repo_data, tag_head)
-                jobs = provider.submit_jobs(backend, args.tag_name)
-                backend.update_repo_last_run_at(
-                    repo_data, last_run_at=int(round(time.time() * 1000))
-                )
-                print_runs(list_runs_with_merged_backends([backend], run_name=run_name))
-                if not args.detach:
-                    poll_run(repo_data, jobs, backend)
-            else:
+            repo_credentials = backend.get_repo_credentials(repo_data)
+            repo_user_config = config.read(
+                config.repos / f"{repo_data.path(delimiter='.')}.yaml",
+                RepoUserConfig,
+                non_empty=False,
+            )
+            if not repo_credentials:
                 sys.exit(f"Call `dstack init` first")
+            if not repo_user_config.ssh_key_path:
+                if (
+                    (backend.name != "local" and not args.detach)
+                    or workflow_data.get("ssh", False)
+                    or "--ssh" in provider_args
+                ):
+                    console.print("Call `dstack init` first")
+                    console.print("  [gray58]No valid SSH identity[/]")
+                    exit(1)
+            else:
+                workflow_data["ssh_key_pub"] = _read_ssh_key_pub(repo_user_config.ssh_key_path)
+
+            run_name = backend.create_run(repo_data)
+            provider.load(backend, provider_args, workflow_name, workflow_data, run_name)
+            if args.tag_name:
+                tag_head = backend.get_tag_head(repo_data, args.tag_name)
+                if tag_head:
+                    backend.delete_tag_head(repo_data, tag_head)
+            jobs = provider.submit_jobs(backend, args.tag_name)
+            backend.update_repo_last_run_at(repo_data, last_run_at=int(round(time.time() * 1000)))
+            runs_with_merged_backends = list_runs_with_merged_backends(
+                [backend], run_name=run_name
+            )
+            print_runs(runs_with_merged_backends)
+            run = runs_with_merged_backends[0][0]
+            if run.status == JobStatus.FAILED:
+                console.print("\nProvisioning failed\n")
+                exit(1)
+            if not args.detach:
+                poll_run(
+                    repo_data,
+                    jobs,
+                    backend,
+                    ssh_key=repo_user_config.ssh_key_path,
+                    openssh_server=provider.openssh_server,
+                )
         except ValidationError as e:
             sys.exit(
                 f"There a syntax error in one of the files inside the {os.getcwd()}/.dstack/workflows directory:\n\n{e}"
             )
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/secrets/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/prune/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,43 @@
-import sys
-from argparse import Namespace
-
-from rich import print
-from rich.prompt import Confirm
+import argparse
+from typing import List
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
+from dstack.backend.base import Backend
 from dstack.cli.commands import BasicCommand
+from dstack.cli.common import console
 from dstack.core.error import check_config, check_git
+from dstack.core.repo import LocalRepoData
 
 
-def _verb(abort: bool):
-    if abort:
-        return "Abort"
-    else:
-        return "Stop"
-
-
-class StopCommand(BasicCommand):
-    NAME = "stop"
-    DESCRIPTION = "Stop run(s)"
+class PruneCommand(BasicCommand):
+    NAME = "prune"
+    DESCRIPTION = "Prunes cache from the storage"
 
     def __init__(self, parser):
-        super(StopCommand, self).__init__(parser)
+        super().__init__(parser)
 
     def register(self):
-        self._parser.add_argument(
-            "run_name", metavar="RUN", type=str, nargs="?", help="A name of a run"
-        )
-        self._parser.add_argument(
-            "-a",
-            "--all",
-            help="Stop all unfinished runs",
-            dest="all",
-            action="store_true",
-        )
-        self._parser.add_argument(
-            "-x",
-            "--abort",
-            help="Don't wait for a graceful stop and abort the run immediately",
-            dest="abort",
-            action="store_true",
-        )
-        self._parser.add_argument(
-            "-y", "--yes", help="Don't ask for confirmation", action="store_true"
+        self._parser: argparse.ArgumentParser
+        subparsers = self._parser.add_subparsers(title="entities", dest="entity", required=True)
+
+        cache_cmd = subparsers.add_parser("cache", help="Workflow cache")
+        cache_cmd.add_argument(
+            "workflow", metavar="WORKFLOW", help="A workflow name to prune cache"
         )
+        cache_cmd.set_defaults(prune_action=self.prune_cache)
 
     @check_config
     @check_git
-    def _command(self, args: Namespace):
-        if (
-            args.run_name
-            and (
-                args.yes or Confirm.ask(f"[red]{_verb(args.abort)} the run '{args.run_name}'?[/]")
+    def _command(self, args: argparse.Namespace):
+        repo_data = load_repo_data()
+        backends = list_backends()
+        args.prune_action(args, backends, repo_data)
+
+    @staticmethod
+    def prune_cache(args: argparse.Namespace, backends: List[Backend], repo_data: LocalRepoData):
+        for backend in backends:
+            backend.delete_workflow_cache(
+                repo_data, repo_data.local_repo_user_email or "default", args.workflow
             )
-        ) or (args.all and (args.yes or Confirm.ask(f"[red]{_verb(args.abort)} all runs?[/]"))):
-            repo_data = load_repo_data()
-            for backend in list_backends():
-                job_heads = backend.list_job_heads(repo_data, args.run_name)
-                if job_heads:
-                    for job_head in job_heads:
-                        if job_head.status.is_unfinished():
-                            backend.stop_job(repo_data, job_head.job_id, args.abort)
-                    print(f"[grey58]OK[/]")
-                    return
-            sys.exit(f"Cannot find the run '{args.run_name}'")
-        else:
-            if not args.run_name and not args.all:
-                sys.exit("Specify a run name or use --all to stop all workflows")
+            console.print(f"[gray58]Cache pruned (backend: {backend.name})[/]")
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/common.py` & `dstack-0.7rc1/cli/dstack/cli/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
 from dstack.backend.base import Backend
 from dstack.core.job import JobStatus
 from dstack.core.request import RequestStatus
 from dstack.core.run import RunHead
 from dstack.utils.common import pretty_date
 
-_is_termios_available = find_spec("termios") is not None
+is_termios_available = find_spec("termios") is not None
 
 
 console = Console()
 
 
 def ask_choice(
     title: str,
     labels: List[str],
     values: List[str],
     selected_value: Optional[str],
     show_choices: Optional[bool] = None,
 ) -> str:
     if selected_value not in values:
         selected_value = None
-    if _is_termios_available:
+    if is_termios_available:
         from simple_term_menu import TerminalMenu
 
         console.print(
             f"[sea_green3 bold]?[/sea_green3 bold] [bold]{title}[/bold] "
             "[gray46]Use arrows to move, type to filter[/gray46]"
         )
         try:
@@ -47,15 +47,15 @@
             raise_error_on_interrupt=True,
         )
         chosen_menu_index = terminal_menu.show()
         chosen_menu_label = labels[chosen_menu_index].replace("[", "\\[")
         console.print(f"[sea_green3 bold]✓[/sea_green3 bold] [grey74]{chosen_menu_label}[/grey74]")
         return values[chosen_menu_index]
     else:
-        if len(values) < 6 and show_choices is None or show_choices is True:
+        if len(values) < 10 and show_choices is None or show_choices is True:
             return Prompt.ask(
                 prompt=f"[sea_green3 bold]?[/sea_green3 bold] [bold]{title}[/bold]",
                 choices=values,
                 default=selected_value,
             )
         else:
             value = Prompt.ask(
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/handlers.py` & `dstack-0.7rc1/cli/dstack/cli/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from dstack import version
 from dstack.cli.commands.config import ConfigCommand
+from dstack.cli.commands.cp import CpCommand
 from dstack.cli.commands.hub import HubCommand
 from dstack.cli.commands.init import InitCommand
 from dstack.cli.commands.logs import LogCommand
 from dstack.cli.commands.ls import LsCommand
+from dstack.cli.commands.prune import PruneCommand
 from dstack.cli.commands.ps import PSCommand
 from dstack.cli.commands.pull import PullCommand
 from dstack.cli.commands.push import PushCommand
 from dstack.cli.commands.rm import RMCommand
 from dstack.cli.commands.run import RunCommand
 from dstack.cli.commands.secrets import SecretCommand
 from dstack.cli.commands.stop import StopCommand
 from dstack.cli.commands.tags import TAGCommand
 
 commands_classes = [
     ConfigCommand,
+    CpCommand,
     InitCommand,
     LogCommand,
     LsCommand,
+    PruneCommand,
     PSCommand,
     PullCommand,
     PushCommand,
     RMCommand,
     RunCommand,
     SecretCommand,
     StopCommand,
```

### Comparing `dstack-0.2rc1/cli/dstack/cli/main.py` & `dstack-0.7rc1/cli/dstack/cli/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/cli/updates.py` & `dstack-0.7rc1/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/core/app.py` & `dstack-0.7rc1/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/core/artifact.py` & `dstack-0.7rc1/cli/dstack/core/artifact.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseModel
 
 from dstack.core.storage import StorageFile
 
 
 class ArtifactSpec(BaseModel):
     artifact_path: str
-    mount: bool
+    mount: bool = False
 
     def __str__(self) -> str:
         return f'ArtifactSpec(artifact_path="{self.artifact_path}", ' f"mount={self.mount})"
 
 
 class ArtifactHead(BaseModel):
     job_id: str
```

### Comparing `dstack-0.2rc1/cli/dstack/core/config.py` & `dstack-0.7rc1/cli/dstack/core/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
-import yaml
+from dstack.hub.models import ProjectValues
 
 
 def get_config_path():
     return Path.joinpath(get_dstack_dir(), "config.yaml")
 
 
 def get_dstack_dir():
     return Path.joinpath(Path.home(), ".dstack")
 
 
 class BackendConfig(ABC):
-
     credentials: Optional[Dict] = None
 
     @abstractmethod
     def save(self, path: Path = get_config_path()):
         pass
 
     @abstractmethod
@@ -34,17 +33,17 @@
         return self.NAME or ""
 
     @abstractmethod
     def configure_cli(self):
         pass
 
     @abstractmethod
-    def configure_hub(self, data: Dict):
+    def configure_hub(self, config_data: Dict) -> ProjectValues:
         pass
 
     @abstractmethod
-    def get_config(self, data: Dict) -> BackendConfig:
+    def get_config_from_hub_config_data(self, config_data: Dict, auth_data: Dict) -> BackendConfig:
         pass
 
     @abstractmethod
-    def parse_args(self, args: list = []):
+    def register_parser(self, parser):
         pass
```

### Comparing `dstack-0.2rc1/cli/dstack/core/job.py` & `dstack-0.7rc1/cli/dstack/core/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel
 
 from dstack.core.app import AppSpec
 from dstack.core.artifact import ArtifactSpec
+from dstack.core.cache import CacheSpec
 from dstack.core.dependents import DepSpec
 from dstack.core.repo import RepoAddress, RepoData
-from dstack.utils.common import _quoted
+from dstack.utils.common import _quoted, format_list
 
 
 class GpusRequirements(BaseModel):
     count: Optional[int] = None
     memory_mib: Optional[int] = None
     name: Optional[str] = None
 
@@ -81,14 +82,15 @@
         self.job_id = job_id
 
     def __str__(self) -> str:
         return f'JobRefId(job_id="{self.job_id}")'
 
 
 class JobStatus(Enum):
+    PENDING = "pending"
     SUBMITTED = "submitted"
     DOWNLOADING = "downloading"
     RUNNING = "running"
     UPLOADING = "uploading"
     STOPPING = "stopping"
     STOPPED = "stopped"
     ABORTING = "aborting"
@@ -142,14 +144,25 @@
             f"submitted_at={self.submitted_at}, "
             f"artifact_paths={artifact_paths}, "
             f"tag_name={_quoted(self.tag_name)}, "
             f"app_names={app_names})"
         )
 
 
+class RegistryAuth(BaseModel):
+    username: Optional[str] = None
+    password: Optional[str] = None
+
+    def __str__(self) -> str:
+        return f"RegistryCredentials(username={self.username}, password={self.password})"
+
+    def serialize(self) -> Dict[str, Any]:
+        return self.dict(exclude_none=True)
+
+
 def check_dict(element: Any, field: str):
     if type(element) == dict:
         return element.get(field)
     if hasattr(element, field):
         return getattr(element, field)
     return None
 
@@ -160,29 +173,34 @@
     run_name: str
     workflow_name: Optional[str]
     provider_name: str
     local_repo_user_name: Optional[str]
     local_repo_user_email: Optional[str]
     status: JobStatus
     submitted_at: int
+    submission_num: int = 1
     image_name: str
+    registry_auth: Optional[RegistryAuth]
     commands: Optional[List[str]]
+    entrypoint: Optional[List[str]]
     env: Optional[Dict[str, str]]
     working_dir: Optional[str]
     artifact_specs: Optional[List[ArtifactSpec]]
+    cache_specs: List[CacheSpec]
     port_count: Optional[int]
     ports: Optional[List[int]]
     host_name: Optional[str]
     requirements: Optional[Requirements]
     dep_specs: Optional[List[DepSpec]]
     master_job: Optional[JobRef]
     app_specs: Optional[List[AppSpec]]
     runner_id: Optional[str]
     request_id: Optional[str]
     tag_name: Optional[str]
+    ssh_key_pub: Optional[str]
 
     def __init__(self, **data: Any):
         # TODO Ugly style
         if type(data) == dict:
             if "repo_address" in data:
                 del data["repo_address"]
             if "artifact_paths" in data:
@@ -203,57 +221,48 @@
     def get_id(self) -> Optional[str]:
         return self.job_id
 
     def set_id(self, job_id: Optional[str]):
         self.job_id = job_id
 
     def __str__(self) -> str:
-        commands = (
-            ("[" + ", ".join(map(lambda a: _quoted(str(a)), self.commands)) + "]")
-            if self.commands
-            else None
-        )
-        artifact_specs = (
-            ("[" + ", ".join(map(lambda a: _quoted(str(a)), self.artifact_specs)) + "]")
-            if self.artifact_specs
-            else None
-        )
-        app_specs = (
-            ("[" + ", ".join(map(lambda a: str(a), self.app_specs)) + "]")
-            if self.app_specs
-            else None
-        )
-        dep_specs = (
-            ("[" + ", ".join(map(lambda d: str(d), self.dep_specs)) + "]")
-            if self.dep_specs
-            else None
-        )
+        commands = format_list(self.commands, formatter=lambda a: _quoted(str(a)))
+        entrypoint = format_list(self.entrypoint, formatter=lambda a: _quoted(str(a)))
+        artifact_specs = format_list(self.artifact_specs)
+        cache_specs = format_list(self.cache_specs or None)
+        app_specs = format_list(self.app_specs)
+        dep_specs = format_list(self.dep_specs)
+        ssk_key_pub = f"...{self.ssh_key_pub[-16:]}" if self.ssh_key_pub else None
         return (
             f'Job(job_id="{self.job_id}", repo_data={self.repo_data}, '
             f'run_name="{self.run_name}", workflow_name={_quoted(self.workflow_name)}, '
             f'provider_name="{self.provider_name}", '
             f"local_repo_user_name={_quoted(self.local_repo_user_name)}, "
             f"local_repo_user_email={_quoted(self.local_repo_user_email)}, "
             f"status=JobStatus.{self.status.name}, "
             f"submitted_at={self.submitted_at}, "
             f'image_name="{self.image_name}", '
+            f'registry_auth="{self.registry_auth}", '
             f"commands={commands}, "
+            f"entrypoint={entrypoint}, "
             f"env={self.env}, "
             f"working_dir={_quoted(self.working_dir)}, "
             f"port_count={self.port_count}, "
             f"ports={self.ports}, "
             f"host_name={_quoted(self.host_name)}, "
             f"artifact_specs={artifact_specs}, "
+            f"cache_specs={cache_specs}, "
             f"requirements={self.requirements}, "
             f"dep_specs={dep_specs}, "
             f"master_job={self.master_job}, "
             f"app_specs={app_specs}, "
             f"runner_id={_quoted(self.runner_id)}, "
             f"request_id={_quoted(self.request_id)}, "
-            f"tag_name={_quoted(self.tag_name)})"
+            f"tag_name={_quoted(self.tag_name)}"
+            f"ssh_key_pub={_quoted(ssk_key_pub)})"
         )
 
     def serialize(self) -> dict:
         deps = []
         if self.dep_specs:
             for dep in self.dep_specs:
                 deps.append(
@@ -274,29 +283,33 @@
                 )
         job_data = {
             "job_id": self.job_id,
             "repo_host_name": self.repo_address.repo_host_name,
             "repo_port": self.repo_address.repo_port or 0,
             "repo_user_name": self.repo_data.repo_user_name,
             "repo_name": self.repo_data.repo_name,
-            "repo_branch": self.repo_data.repo_branch,
-            "repo_hash": self.repo_data.repo_hash,
+            "repo_branch": self.repo_data.repo_branch or "",
+            "repo_hash": self.repo_data.repo_hash or "",
             "repo_diff": self.repo_data.repo_diff or "",
             "run_name": self.run_name,
             "workflow_name": self.workflow_name or "",
             "provider_name": self.provider_name,
             "local_repo_user_name": self.local_repo_user_name or "",
             "local_repo_user_email": self.local_repo_user_email or "",
             "status": self.status.value,
             "submitted_at": self.submitted_at,
+            "submission_num": self.submission_num,
             "image_name": self.image_name,
+            "registry_auth": self.registry_auth.serialize() if self.registry_auth else {},
             "commands": self.commands or [],
+            "entrypoint": self.entrypoint,
             "env": self.env or {},
             "working_dir": self.working_dir or "",
             "artifacts": artifacts,
+            "cache": [item.dict() for item in self.cache_specs],
             "port_count": self.port_count if self.port_count else 0,
             "ports": [str(port) for port in self.ports] if self.ports else [],
             "host_name": self.host_name or "",
             "requirements": self.requirements.serialize() if self.requirements else {},
             "deps": deps,
             "master_job_id": self.master_job.get_id() if self.master_job else "",
             "apps": [
@@ -309,14 +322,15 @@
                 for a in self.app_specs
             ]
             if self.app_specs
             else [],
             "runner_id": self.runner_id or "",
             "request_id": self.request_id or "",
             "tag_name": self.tag_name or "",
+            "ssh_key_pub": self.ssh_key_pub or "",
         }
         return job_data
 
     @staticmethod
     def unserialize(job_data: dict):
         _requirements = job_data.get("requirements")
         requirements = (
@@ -394,47 +408,54 @@
         job = Job(
             job_id=job_data["job_id"],
             repo_data=RepoData(
                 repo_host_name=job_data["repo_host_name"],
                 repo_port=job_data.get("repo_port") or None,
                 repo_user_name=job_data["repo_user_name"],
                 repo_name=job_data["repo_name"],
-                repo_branch=job_data["repo_branch"],
-                repo_hash=job_data["repo_hash"],
+                repo_branch=job_data["repo_branch"] or None,
+                repo_hash=job_data["repo_hash"] or None,
                 repo_diff=job_data["repo_diff"] or None,
             ),
             run_name=job_data["run_name"],
             workflow_name=job_data.get("workflow_name") or None,
             provider_name=job_data["provider_name"],
             local_repo_user_name=job_data.get("local_repo_user_name"),
             local_repo_user_email=job_data.get("local_repo_user_email") or None,
             status=JobStatus(job_data["status"]),
             submitted_at=job_data["submitted_at"],
+            submission_num=job_data.get("submission_num") or 1,
             image_name=job_data["image_name"],
+            registry_auth=RegistryAuth(**job_data.get("registry_auth", {})),
             commands=job_data.get("commands") or None,
+            entrypoint=job_data.get("entrypoint") or None,
             env=job_data["env"] or None,
             working_dir=job_data.get("working_dir") or None,
             artifact_specs=artifact_specs,
+            cache_specs=[CacheSpec(**item) for item in job_data.get("cache", [])],
             port_count=job_data.get("port_count") or None,
             ports=job_data.get("ports") or None,
             host_name=job_data.get("host_name") or None,
             requirements=requirements,
             dep_specs=dep_specs or None,
             master_job=master_job,
             app_specs=app_specs,
             runner_id=job_data.get("runner_id") or None,
             request_id=job_data.get("request_id") or None,
             tag_name=job_data.get("tag_name") or None,
+            ssh_key_pub=job_data.get("ssh_key_pub") or None,
         )
         return job
 
 
 class JobSpec(JobRef):
     image_name: str
+    registry_auth: Optional[RegistryAuth] = None
     commands: Optional[List[str]] = None
+    entrypoint: Optional[List[str]] = None
     env: Optional[Dict[str, str]] = None
     working_dir: Optional[str] = None
     artifact_specs: Optional[List[ArtifactSpec]] = None
     port_count: Optional[int] = None
     requirements: Optional[Requirements] = None
     master_job: Optional[JobRef] = None
     app_specs: Optional[List[AppSpec]] = None
@@ -442,32 +463,23 @@
     def get_id(self) -> Optional[str]:
         return self.job_id
 
     def set_id(self, job_id: Optional[str]):
         self.job_id = job_id
 
     def __str__(self) -> str:
-        commands = (
-            ("[" + ", ".join(map(lambda a: _quoted(str(a)), self.commands)) + "]")
-            if self.commands
-            else None
-        )
-        artifact_specs = (
-            ("[" + ", ".join(map(lambda a: str(a), self.artifact_specs)) + "]")
-            if self.artifact_specs
-            else None
-        )
-        app_specs = (
-            ("[" + ", ".join(map(lambda a: str(a), self.app_specs)) + "]")
-            if self.app_specs
-            else None
-        )
+        commands = format_list(self.commands, formatter=lambda a: _quoted(str(a)))
+        entrypoint = format_list(self.entrypoint, formatter=lambda a: _quoted(str(a)))
+        artifact_specs = format_list(self.artifact_specs)
+        app_specs = format_list(self.app_specs)
         return (
             f'JobSpec(job_id="{self.job_id}", image_name="{self.image_name}", '
+            f"registry_auth={self.registry_auth}, "
             f"commands={commands}, "
+            f"entrypoint={entrypoint}, "
             f"env={self.env}, "
             f"working_dir={_quoted(self.working_dir)}, "
             f"port_count={self.port_count}, "
             f"artifact_specs={artifact_specs}, "
             f"requirements={self.requirements}, "
             f"master_job={self.master_job}, "
             f"app_specs={app_specs})"
```

### Comparing `dstack-0.2rc1/cli/dstack/core/repo.py` & `dstack-0.7rc1/cli/dstack/core/repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,41 +56,38 @@
 
 
 class RepoCredentials(BaseModel):
     protocol: RepoProtocol
     private_key: Union[str, None]
     oauth_token: Union[str, None]
 
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
     def __str__(self) -> str:
         return (
             f"RepoCredentials(protocol=RepoProtocol.{self.protocol.name}, "
             f"private_key_length={len(self.private_key) if self.private_key else None}, "
             f"oauth_token={_quoted_masked(self.oauth_token)})"
         )
 
 
 class RepoData(RepoAddress):
-    repo_branch: str
-    repo_hash: str
+    repo_branch: Optional[str]
+    repo_hash: Optional[str]
     repo_diff: Union[str, None]
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     def __str__(self) -> str:
         return (
             f'RepoData(repo_host_name="{self.repo_host_name}", '
             f'repo_port={_quoted(self.repo_port)}", '
             f'repo_user_name="{self.repo_user_name}", '
             f'repo_name="{self.repo_name}", '
-            f'repo_branch="{self.repo_branch}", '
-            f'repo_hash="{self.repo_hash}", '
+            f'repo_branch="{_quoted(self.repo_branch)}", '
+            f'repo_hash="{_quoted(self.repo_hash)}", '
             f"repo_diff_length={len(self.repo_diff) if self.repo_diff else None})"
         )
 
 
 class LocalRepoData(RepoData):
     protocol: RepoProtocol
     identity_file: Union[str, None]
@@ -103,16 +100,16 @@
 
     def __str__(self) -> str:
         return (
             f'LocalRepoData(repo_host_name="{self.repo_host_name}", '
             f'repo_port={_quoted(self.repo_port)}", '
             f'repo_user_name="{self.repo_user_name}", '
             f'repo_name="{self.repo_name}", '
-            f'repo_branch="{self.repo_branch}", '
-            f'repo_hash="{self.repo_hash}", '
+            f'repo_branch="{_quoted(self.repo_branch)}", '
+            f'repo_hash="{_quoted(self.repo_hash)}", '
             f"repo_diff_length={len(self.repo_diff) if self.repo_diff else None}, "
             f"protocol=RepoProtocol.{self.protocol.name}, "
             f"identity_file={_quoted(self.identity_file)}, "
             f"oauth_token={_quoted_masked(self.oauth_token)},"
             f'local_repo_user_name="{_quoted(self.local_repo_user_name)}, '
             f"local_repo_user_email={_quoted(self.local_repo_user_email)})"
         )
```

### Comparing `dstack-0.2rc1/cli/dstack/core/request.py` & `dstack-0.7rc1/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/core/run.py` & `dstack-0.7rc1/cli/dstack/core/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/core/runners.py` & `dstack-0.7rc1/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/core/tag.py` & `dstack-0.7rc1/cli/dstack/core/tag.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack/hub/db/models.py` & `dstack-0.7rc1/cli/dstack/hub/db/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,53 @@
 from typing import List
 
-from sqlalchemy import Column, ForeignKey, Integer, String, Table
-from sqlalchemy.orm import Mapped, mapped_column, relationship
+from sqlalchemy import ForeignKey, Integer, MetaData, String
+from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 
-from dstack.hub.db import Database
+constraint_naming_convention = {
+    "ix": "ix_%(column_0_label)s",
+    "uq": "uq_%(table_name)s_%(column_0_name)s",
+    "ck": "ck_%(table_name)s_%(constraint_name)s",
+    "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
+    "pk": "pk_%(table_name)s",
+}
 
 
-class Base:
+class Base(DeclarativeBase):
+    metadata = MetaData(naming_convention=constraint_naming_convention)
+
     def __repr__(self) -> str:
         src = self.__class__.__name__
-        attr = [f"{key}= {val}" for (key, val) in self.__dict__.items() if not key.startwith("_")]
-        attr_string = ",".join(attr)
+        attr = [f"{key}={val}" for (key, val) in self.__dict__.items() if not key.startswith("_")]
+        attr_string = ", ".join(attr)
         return f"{src}({attr_string})"
 
 
-association_table_user_hub = Table(
-    "user_hub",
-    Database.Base.metadata,
-    Column("users_name", ForeignKey("users.name")),
-    Column("hub_name", ForeignKey("hubs.name")),
-)
-
-
-class Role(Base, Database.Base):
-    __tablename__ = "roles"
-
-    id: Mapped[int] = mapped_column(Integer, primary_key=True, autoincrement=True)
-    name: Mapped[str] = mapped_column(String(30))
-
-    def __repr__(self) -> str:
-        return super().__repr__()
-
-
-class User(Base, Database.Base):
+class User(Base):
     __tablename__ = "users"
 
-    name: Mapped[str] = mapped_column(String(30), primary_key=True)
+    name: Mapped[str] = mapped_column(String(50), primary_key=True)
     token: Mapped[str] = mapped_column(String(200))
-    role_id: Mapped[int] = mapped_column(ForeignKey("roles.id"))
-    hub_role: Mapped[Role] = relationship()
-
-    def __repr__(self) -> str:
-        return super().__repr__()
+    global_role: Mapped[str] = mapped_column(String(100))
 
 
-class Member(Base, Database.Base):
+class Member(Base):
     __tablename__ = "members"
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True, autoincrement=True)
-    hub_name: Mapped[str] = mapped_column(ForeignKey("hubs.name"))
+    project_name: Mapped[str] = mapped_column(ForeignKey("projects.name", ondelete="CASCADE"))
+    project: Mapped["Project"] = relationship()
 
-    user_name: Mapped[str] = mapped_column(ForeignKey("users.name"))
+    user_name: Mapped[str] = mapped_column(ForeignKey("users.name", ondelete="CASCADE"))
     user: Mapped[User] = relationship()
 
-    role_id: Mapped[int] = mapped_column(ForeignKey("roles.id"))
-    hub_role: Mapped[Role] = relationship()
-
-    def __repr__(self) -> str:
-        return super().__repr__()
+    project_role: Mapped[str] = mapped_column(String(100))
 
 
-class Hub(Base, Database.Base):
-    __tablename__ = "hubs"
+class Project(Base):
+    __tablename__ = "projects"
 
-    name: Mapped[str] = mapped_column(String(30), primary_key=True)
+    name: Mapped[str] = mapped_column(String(50), primary_key=True)
     backend: Mapped[str] = mapped_column(String(30))
     config: Mapped[str] = mapped_column(String(300))
     auth: Mapped[str] = mapped_column(String(300))
-    members: Mapped[List[Member]] = relationship(lazy="selectin")
-
-    def __repr__(self) -> str:
-        return super().__repr__()
-
-
-class Scope(Base, Database.Base):
-    __tablename__ = "scopes"
-
-    id: Mapped[int] = mapped_column(Integer, primary_key=True, autoincrement=True)
-    pattern: Mapped[str] = mapped_column(String(100), nullable=False)
-
-    def __repr__(self) -> str:
-        return super().__repr__()
+    members: Mapped[List[Member]] = relationship(back_populates="project", lazy="selectin")
```

### Comparing `dstack-0.2rc1/cli/dstack/hub/routers/link.py` & `dstack-0.7rc1/cli/dstack/hub/routers/link.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from fastapi import APIRouter, Depends
 from fastapi.responses import PlainTextResponse
-from fastapi.security import HTTPBearer
 
 from dstack.hub.models import LinkUpload
 from dstack.hub.routers.cache import get_backend
-from dstack.hub.routers.util import get_hub
-from dstack.hub.security.scope import Scope
+from dstack.hub.routers.util import get_project
+from dstack.hub.security.permissions import ProjectMember
 
-router = APIRouter(prefix="/api/hub", tags=["link"])
-
-security = HTTPBearer()
+router = APIRouter(prefix="/api/project", tags=["link"], dependencies=[Depends(ProjectMember())])
 
 
 @router.post(
-    "/{hub_name}/link/upload",
-    dependencies=[Depends(Scope("link:upload:write"))],
+    "/{project_name}/link/upload",
     response_model=str,
     response_class=PlainTextResponse,
 )
-async def link_upload(hub_name: str, body: LinkUpload):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+async def link_upload(project_name: str, body: LinkUpload):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     return backend.get_signed_upload_url(object_key=body.object_key)
 
 
-@router.get(
-    "/{hub_name}/link/download",
-    dependencies=[Depends(Scope("link:download:read"))],
+@router.post(
+    "/{project_name}/link/download",
     response_model=str,
     response_class=PlainTextResponse,
 )
-async def link_upload(hub_name: str, body: LinkUpload):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+async def link_upload(project_name: str, body: LinkUpload):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     return backend.get_signed_download_url(object_key=body.object_key)
```

### Comparing `dstack-0.2rc1/cli/dstack/hub/routers/logs.py` & `dstack-0.7rc1/cli/dstack/hub/routers/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from functools import partial
 from typing import Any, AsyncIterable, Callable, Coroutine, List, Mapping, Optional, Union
 
 import anyio
 from fastapi import APIRouter, Depends
-from fastapi.security import HTTPBearer
 from starlette.background import BackgroundTask
 from starlette.concurrency import iterate_in_threadpool
 from starlette.responses import Response
 from starlette.types import Receive
 from starlette.types import Scope as StarletteScope
 from starlette.types import Send
 
-from dstack.core.job import JobHead
-from dstack.core.repo import RepoAddress
 from dstack.hub.models import PollLogs
 from dstack.hub.routers.cache import get_backend
-from dstack.hub.routers.util import get_hub
-from dstack.hub.security.scope import Scope
+from dstack.hub.routers.util import get_project
+from dstack.hub.security.permissions import ProjectMember
 
-router = APIRouter(prefix="/api/hub", tags=["logs"])
-
-security = HTTPBearer()
+router = APIRouter(prefix="/api/project", tags=["logs"], dependencies=[Depends(ProjectMember())])
 
 
 class JSONStreamingResponse(Response):
     def __init__(
         self,
         content: Any,
         status_code: int = 200,
@@ -72,22 +67,21 @@
             task_group.start_soon(wrap, partial(self.stream_response, send))
             await wrap(partial(self.listen_for_disconnect, receive))
 
         if self.background is not None:
             await self.background()
 
 
-@router.get(
-    "/{hub_name}/logs/poll",
-    dependencies=[Depends(Scope("logs:poll:read"))],
+@router.post(
+    "/{project_name}/logs/poll",
     response_class=JSONStreamingResponse,
 )
-async def poll_logs(hub_name: str, body: PollLogs):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+async def poll_logs(project_name: str, body: PollLogs):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     return JSONStreamingResponse(
         content=backend.poll_logs(
             repo_address=body.repo_address,
             job_heads=body.job_heads,
             start_time=body.start_time,
             attached=body.attached,
         ),
```

### Comparing `dstack-0.2rc1/cli/dstack/hub/routers/tags.py` & `dstack-0.7rc1/cli/dstack/hub/routers/tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 from typing import List, Union
 
-from fastapi import APIRouter, Depends
-from fastapi.security import HTTPBearer
+from fastapi import APIRouter, Depends, HTTPException, status
 
 from dstack.core.repo import RepoAddress
 from dstack.core.tag import TagHead
 from dstack.hub.models import AddTagPath, AddTagRun
 from dstack.hub.routers.cache import get_backend
-from dstack.hub.routers.util import get_hub
-from dstack.hub.security.scope import Scope
+from dstack.hub.routers.util import error_detail, get_project
+from dstack.hub.security.permissions import ProjectMember
 
-router = APIRouter(prefix="/api/hub", tags=["tags"])
+router = APIRouter(prefix="/api/project", tags=["tags"], dependencies=[Depends(ProjectMember())])
 
-security = HTTPBearer()
 
-
-@router.get(
-    "/{hub_name}/tags/list/heads",
-    dependencies=[Depends(Scope("tags:list:read"))],
+@router.post(
+    "/{project_name}/tags/list/heads",
     response_model=List[TagHead],
 )
-async def list_heads_tags(hub_name: str, repo_address: RepoAddress):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+async def list_heads_tags(project_name: str, repo_address: RepoAddress):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     list_tag = backend.list_tag_heads(repo_address=repo_address)
     return list_tag
 
 
-@router.get(
-    "/{hub_name}/tags/{tag_name}",
-    dependencies=[Depends(Scope("tags:get:read"))],
+@router.post(
+    "/{project_name}/tags/{tag_name}",
     response_model=TagHead,
 )
-async def get_tags(hub_name: str, tag_name: str, repo_address: RepoAddress):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+async def get_tag(project_name: str, tag_name: str, repo_address: RepoAddress) -> TagHead:
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     tag = backend.get_tag_head(repo_address=repo_address, tag_name=tag_name)
+    if tag is None:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND, detail=error_detail("Tag not found")
+        )
     return tag
 
 
-@router.post(
-    "/{hub_name}/tags/{tag_name}/delete", dependencies=[Depends(Scope("tags:delete:write"))]
-)
-async def delete_tags(hub_name: str, tag_name: str, repo_address: RepoAddress):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+@router.post("/{project_name}/tags/{tag_name}/delete")
+async def delete_tag(project_name: str, tag_name: str, repo_address: RepoAddress):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     tag = backend.get_tag_head(repo_address=repo_address, tag_name=tag_name)
     backend.delete_tag_head(repo_address=repo_address, tag_head=tag)
 
 
-@router.post("/{hub_name}/tags/add/run", dependencies=[Depends(Scope("tags:add:write"))])
-async def add_tags(hub_name: str, body: AddTagRun):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+@router.post("/{project_name}/tags/add/run")
+async def add_tag_from_run(project_name: str, body: AddTagRun):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     backend.add_tag_from_run(
         repo_address=body.repo_address,
         tag_name=body.tag_name,
         run_name=body.run_name,
         run_jobs=body.run_jobs,
     )
 
 
-@router.post("/{hub_name}/tags/add/path", dependencies=[Depends(Scope("tags:add:write"))])
-async def add_tags(hub_name: str, body: AddTagPath):
-    hub = await get_hub(hub_name=hub_name)
-    backend = get_backend(hub)
+@router.post("/{project_name}/tags/add/path")
+async def add_tag_from_path(project_name: str, body: AddTagPath):
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
     backend.add_tag_from_local_dirs(
         repo_data=body.repo_data, tag_name=body.tag_name, local_dirs=body.local_dirs
     )
```

### Comparing `dstack-0.2rc1/cli/dstack/hub/routers/users.py` & `dstack-0.7rc1/cli/dstack/hub/routers/users.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,107 @@
+import re
 import uuid
-from typing import Dict, List
+from typing import List
 
 from fastapi import APIRouter, Depends, HTTPException, status
-from fastapi.security import HTTPBearer
-from fastapi.security.http import HTTPAuthorizationCredentials
 
-from dstack.hub.models import HubDelete, User, UserInfo
-from dstack.hub.repository.user import UserManager
-from dstack.hub.security.scope import Scope
+from dstack.hub.db.models import User
+from dstack.hub.models import DeleteUsers, UserInfo, UserInfoWithToken, UserPatch
+from dstack.hub.repository.users import UserManager
+from dstack.hub.routers.util import error_detail
+from dstack.hub.security.permissions import Authenticated, GlobalAdmin, raise_forbidden
+from dstack.hub.security.utils import ROLE_ADMIN
 
 router = APIRouter(prefix="/api/users", tags=["users"])
 
-security = HTTPBearer()
 
-
-@router.post("", response_model=User, dependencies=[Depends(Scope("users:info:read"))])
-async def users_create(body: User) -> User:
+@router.get("/list")
+async def list_users(user: User = Depends(Authenticated())) -> List[UserInfo]:
+    users = await UserManager.get_user_list()
+    project_users = []
+    for u in users:
+        if user.global_role == ROLE_ADMIN or user.name == u.name:
+            project_user = UserInfo(
+                user_name=u.name,
+                global_role=u.global_role,
+            )
+            project_users.append(project_user)
+    return project_users
+
+
+@router.post("")
+async def create_user(body: UserInfo, user: User = Depends(GlobalAdmin())) -> UserInfoWithToken:
+    if not re.match(r"^[a-zA-Z0-9]([_-](?![_-])|[a-zA-Z0-9]){1,18}[a-zA-Z0-9]$", body.user_name):
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST, detail=error_detail("Username is incorrect")
+        )
     user = await UserManager.get_user_by_name(name=body.user_name)
     if user is not None:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="User exists")
-    user = await UserManager.create(name=body.user_name, role=body.global_role)
-    return User(
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST, detail=error_detail("User exists")
+        )
+    user = await UserManager.create(name=body.user_name, global_role=body.global_role)
+    return UserInfoWithToken(
         user_name=user.name,
         token=user.token,
-        global_role=user.hub_role.name,
+        global_role=user.global_role,
     )
 
 
-@router.delete("", dependencies=[Depends(Scope("users:get:read"))])
-async def users_delete(body: HubDelete):
+@router.delete("")
+async def delete_users(body: DeleteUsers, user: User = Depends(GlobalAdmin())):
     for user_name in body.users:
-        user = await UserManager.get_user_by_name(name=user_name)
-        if user is None:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="User not exists")
+        user = await _get_user(user_name)
         await UserManager.remove(user)
 
 
-@router.get("/info", response_model=UserInfo, dependencies=[Depends(Scope("users:info:read"))])
-async def users_info(authorization: HTTPAuthorizationCredentials = Depends(security)) -> UserInfo:
-    user = await UserManager.get_user_by_token(authorization.credentials)
-    return UserInfo(user_name=user.name)
+@router.get("/info")
+async def get_my_user_info(user: User = Depends(Authenticated())) -> UserInfo:
+    return UserInfo(user_name=user.name, global_role=user.global_role)
 
 
-@router.get("/list", response_model=List[User], dependencies=[Depends(Scope("users:list:read"))])
-async def users_list() -> List[User]:
-    users = await UserManager.get_user_list()
-    hub_users = []
-    for user in users:
-        hub_user = User(
-            user_name=user.name,
-            token=user.token,
-            global_role=user.hub_role.name,
-        )
-        hub_users.append(hub_user)
-    return hub_users
-
-
-@router.get(
-    "/{user_name}/refresh-token",
-    response_model=User,
-    dependencies=[Depends(Scope("users:refresh:write"))],
-)
-async def users_get(user_name: str) -> User:
-    user = await UserManager.get_user_by_name(name=user_name)
+@router.post("/{user_name}/refresh-token")
+async def refresh_token(
+    user_name: str, user: User = Depends(Authenticated())
+) -> UserInfoWithToken:
+    user = await _get_user(user_name)
     user.token = str(uuid.uuid4())
     await UserManager.save(user)
-    return User(
+    return UserInfoWithToken(
         user_name=user.name,
         token=user.token,
-        global_role=user.hub_role.name,
+        global_role=user.global_role,
     )
 
 
-@router.get("/{user_name}", response_model=User, dependencies=[Depends(Scope("users:get:read"))])
-async def users_get(user_name: str) -> User:
-    user = await UserManager.get_user_by_name(name=user_name)
-    return User(
+@router.patch("/{user_name}")
+async def update_user(
+    user_name: str, body: UserPatch, user: User = Depends(GlobalAdmin())
+) -> UserInfoWithToken:
+    user = await _get_user(user_name)
+    await UserManager.save(user)
+    return UserInfoWithToken(
         user_name=user.name,
         token=user.token,
-        global_role=user.hub_role.name,
+        global_role=body.global_role,
+    )
+
+
+@router.get("/{user_name}")
+async def get_user(user_name: str, user: User = Depends(Authenticated())) -> UserInfoWithToken:
+    if user.global_role != ROLE_ADMIN and user.name != user_name:
+        raise_forbidden()
+    user_to_get = await UserManager.get_user_by_name(name=user_name)
+    return UserInfoWithToken(
+        user_name=user_to_get.name,
+        token=user_to_get.token,
+        global_role=user_to_get.global_role,
     )
+
+
+async def _get_user(user_name: str) -> User:
+    user = await UserManager.get_user_by_name(name=user_name)
+    if user is None:
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST, detail=error_detail("User does not exist")
+        )
+    return user
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/__init__.py` & `dstack-0.7rc1/cli/dstack/providers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import importlib
+import shlex
 import sys
-import time
 from abc import abstractmethod
 from argparse import ArgumentParser, Namespace
 from pkgutil import iter_modules
 from typing import Any, Dict, List, Optional, Union
 
-from jinja2 import Template
-
 from dstack.api.repo import load_repo_data
 from dstack.backend.base import Backend
+from dstack.core.cache import CacheSpec
 from dstack.core.job import (
     ArtifactSpec,
     DepSpec,
     GpusRequirements,
     Job,
     JobSpec,
     JobStatus,
     Requirements,
 )
 from dstack.core.repo import RepoAddress, RepoData
-from dstack.utils.common import _quoted
+from dstack.utils.common import _quoted, get_milliseconds_since_epoch
+from dstack.utils.interpolator import VariablesInterpolator
 
 DEFAULT_CPU = 2
 DEFAULT_MEM = "8GB"
 
 
 def _str_to_mib(s: str) -> int:
     ns = s.replace(" ", "").lower()
@@ -53,15 +53,19 @@
         self.provider_name: str = provider_name
         self.provider_data: Optional[Dict[str, Any]] = None
         self.provider_args: Optional[List[str]] = None
         self.workflow_name: Optional[str] = None
         self.run_as_provider: Optional[bool] = None
         self.run_name: Optional[str] = None
         self.dep_specs: Optional[List[DepSpec]] = None
+        self.cache_specs: List[CacheSpec] = []
+        self.ssh_key_pub: Optional[str] = None
+        self.openssh_server: bool = False
         self.loaded = False
+        self.home_dir: Optional[str] = None
 
     def __str__(self) -> str:
         return (
             f'Provider(name="{self.provider_name}", '
             f'workflow_data="{self.provider_data}", '
             f'workflow_name="{_quoted(self.workflow_name)}, '
             f'provider_name="{self.provider_name}", '
@@ -86,50 +90,38 @@
             sys.exit(
                 f"Python version `{python_version}` is not supported. "
                 f"Supported versions: {str(supported_python_versions)}."
             )
         return python_version
 
     def _inject_context(self):
-        class Args:
-            def __init__(self, args: List[str]) -> None:
-                super().__init__()
-                self.args = args
-
-            def __str__(self):
-                _str = ""
-                for arg in self.args:
-                    if _str:
-                        _str += " "
-                    if " " in arg:
-                        _str += '"' + arg.replace('"', '\\"') + '"'
-                    else:
-                        _str += arg
-                return _str
-
-        class Run:
-            def __init__(self, name: str, args: Args) -> None:
-                super().__init__()
-                self.name = name
-                self.args = args
-
-        run = Run(self.run_name, Args(self.provider_data.get("run_args") or []))
-        self.provider_data = self._inject_context_recursively(self.provider_data, run=run)
+        args = []
+        for arg in self.provider_data.get("run_args", []):
+            if " " in arg:
+                arg = '"%s"' % arg.replace('"', '\\"')
+            args.append(arg)
+
+        self.provider_data = self._inject_context_recursively(
+            VariablesInterpolator(
+                {"run": {"name": self.run_name, "args": " ".join(args)}}, skip=["secrets"]
+            ),
+            self.provider_data,
+        )
 
     @staticmethod
-    def _inject_context_recursively(obj: Any, **kwargs: Any) -> Any:
+    def _inject_context_recursively(interpolator: VariablesInterpolator, obj: Any) -> Any:
         if isinstance(obj, str):
-            return Template(obj, variable_start_string="${{").render(**kwargs)
+            return interpolator.interpolate(obj)
         elif isinstance(obj, dict):
             d = {}
             for k in obj:
-                d[k] = Provider._inject_context_recursively(obj[k], **kwargs)
+                d[k] = Provider._inject_context_recursively(interpolator, obj[k])
             return d
         elif isinstance(obj, list):
-            return [Provider._inject_context_recursively(item, **kwargs) for item in obj]
+            return [Provider._inject_context_recursively(interpolator, item) for item in obj]
         else:
             return obj
 
     def load(
         self,
         backend: Backend,
         provider_args: List[str],
@@ -138,17 +130,20 @@
         run_name: str,
     ):
         self.provider_args = provider_args
         self.workflow_name = workflow_name
         self.provider_data = provider_data
         self.run_as_provider = not workflow_name
         self.run_name = run_name
+        self.openssh_server = self.provider_data.get("ssh", False)
         self.parse_args()
         self._inject_context()
         self.dep_specs = self._dep_specs(backend)
+        self.cache_specs = self._cache_specs()
+        self.ssh_key_pub = self.provider_data.get("ssh_key_pub")
         self.loaded = True
 
     @abstractmethod
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
         return None
 
     def help(self, workflow_name: Optional[str]):
@@ -165,15 +160,14 @@
         parser.add_argument("-r", "--requirements", metavar="PATH", type=str)
         parser.add_argument("-e", "--env", action="append")
         parser.add_argument("-a", "--artifact", metavar="PATH", dest="artifacts", action="append")
         parser.add_argument("--dep", metavar="(:TAG | WORKFLOW)", dest="deps", action="append")
         parser.add_argument("-w", "--working-dir", metavar="PATH", type=str)
         group = parser.add_mutually_exclusive_group()
         group.add_argument("-i", "--interruptible", action="store_true")
-        group.add_argument("-l", "--local", action="store_true")
         parser.add_argument("--cpu", metavar="NUM", type=int)
         parser.add_argument("--memory", metavar="SIZE", type=str)
         parser.add_argument("--gpu", metavar="NUM", type=int)
         parser.add_argument("--gpu-name", metavar="NAME", type=str)
         parser.add_argument("--gpu-memory", metavar="SIZE", type=str)
         parser.add_argument("--shm-size", metavar="SIZE", type=str)
 
@@ -212,56 +206,57 @@
                 gpu["memory"] = args.gpu_memory
             if args.gpu_name:
                 gpu["name"] = args.gpu_name
         if args.shm_size:
             resources["shm_size"] = args.shm_size
         if args.interruptible:
             resources["interruptible"] = True
-        if args.local:
-            resources["local"] = True
         if unknown_args:
             self.provider_data["run_args"] = unknown_args
 
     def parse_args(self):
         pass
 
     def submit_jobs(self, backend: Backend, tag_name: str) -> List[Job]:
         if not self.loaded:
             raise Exception("The provider is not loaded")
         job_specs = self.create_job_specs()
         repo_data = load_repo_data()
         # [TODO] Handle master job
         jobs = []
         for i, job_spec in enumerate(job_specs):
-            submitted_at = int(round(time.time() * 1000))
             job = Job(
                 job_id=f"{self.run_name},{self.workflow_name or ''},{i}",
                 repo_data=repo_data,
                 run_name=self.run_name,
                 workflow_name=self.workflow_name or None,
                 provider_name=self.provider_name,
                 local_repo_user_name=repo_data.local_repo_user_name,
                 local_repo_user_email=repo_data.local_repo_user_email,
                 status=JobStatus.SUBMITTED,
-                submitted_at=submitted_at,
+                submitted_at=get_milliseconds_since_epoch(),
                 image_name=job_spec.image_name,
+                registry_auth=job_spec.registry_auth,
                 commands=job_spec.commands,
+                entrypoint=job_spec.entrypoint,
                 env=job_spec.env,
                 working_dir=job_spec.working_dir,
                 artifact_specs=job_spec.artifact_specs,
+                cache_specs=self.cache_specs,
                 port_count=job_spec.port_count,
                 ports=None,
                 host_name=None,
                 requirements=job_spec.requirements,
                 dep_specs=self.dep_specs,
                 master_job=job_spec.master_job,
                 app_specs=job_spec.app_specs,
                 runner_id=None,
                 request_id=None,
                 tag_name=tag_name,
+                ssh_key_pub=self.ssh_key_pub,
             )
             backend.submit_job(job)
             jobs.append(job)
         if tag_name:
             backend.add_tag_from_run(repo_data, tag_name, self.run_name, jobs)
         return jobs
 
@@ -270,34 +265,45 @@
             repo_data = load_repo_data()
             return [
                 self._parse_dep_spec(dep, backend, repo_data) for dep in self.provider_data["deps"]
             ]
         else:
             return None
 
-    def _artifact_specs(self) -> Optional[List[ArtifactSpec]]:
-        if self.provider_data.get("artifacts"):
-            return [self._parse_artifact_spec(a) for a in self.provider_data["artifacts"]]
-        else:
-            return None
-
-    @staticmethod
-    def _parse_artifact_spec(artifact: Union[dict, str]) -> ArtifactSpec:
-        def remove_prefix(text: str, prefix: str) -> str:
-            if text.startswith(prefix):
-                return text[len(prefix) :]
-            return text
+    def _validate_local_path(self, path: str) -> str:
+        if path == "~" or path.startswith("~/"):
+            if not self.home_dir:
+                raise KeyError("home_dir is not defined, local path can't start with ~")
+            home = self.home_dir.rstrip("/")
+            path = home if path == "~" else f"{home}/{path[len('~/'):]}"
+        while path.startswith("./"):
+            path = path[len("./") :]
+        if not path.startswith("/"):
+            pass  # todo: use self.working_dir
+        return path
 
-        if isinstance(artifact, str):
-            return ArtifactSpec(artifact_path=remove_prefix(artifact, "./"), mount=False)
-        else:
-            return ArtifactSpec(
-                artifact_path=remove_prefix(artifact["path"], "./"),
-                mount=artifact.get("mount") is True,
-            )
+    def _artifact_specs(self) -> Optional[List[ArtifactSpec]]:
+        artifact_specs = []
+        for item in self.provider_data.get("artifacts", []):
+            if isinstance(item, str):
+                item = {"artifact_path": item}
+            else:
+                item["artifact_path"] = item.pop("path")
+            item["artifact_path"] = self._validate_local_path(item["artifact_path"])
+            artifact_specs.append(ArtifactSpec(**item))
+        return artifact_specs or None
+
+    def _cache_specs(self) -> List[CacheSpec]:
+        cache_specs = []
+        for item in self.provider_data.get("cache", []):
+            if isinstance(item, str):
+                item = {"path": item}
+            item["path"] = self._validate_local_path(item["path"])
+            cache_specs.append(CacheSpec(**item))
+        return cache_specs
 
     @staticmethod
     def _parse_dep_spec(dep: Union[dict, str], backend: Backend, repo_data: RepoData) -> DepSpec:
         if isinstance(dep, str):
             mount = False
             if dep.startswith(":"):
                 tag_dep = True
@@ -383,14 +389,20 @@
     def _get_list_data(self, name: str) -> Optional[List[str]]:
         v = self.provider_data.get(name)
         if isinstance(v, str):
             return v.split("\n")
         else:
             return v
 
+    def _get_entrypoint(self) -> Optional[List[str]]:
+        v = self.provider_data.get("entrypoint")
+        if isinstance(v, str):
+            return shlex.split(v)
+        return v
+
     def _resources(self) -> Requirements:
         resources = Requirements()
         cpu = self.provider_data["resources"].get("cpu", DEFAULT_CPU)
         if not str(cpu).isnumeric():
             sys.exit("resources.cpu should be an integer")
         cpu = int(cpu)
         if cpu > 0:
@@ -402,41 +414,56 @@
             if str(gpu).isnumeric():
                 gpu = int(self.provider_data["resources"]["gpu"])
                 if gpu > 0:
                     resources.gpus = GpusRequirements(count=gpu)
             else:
                 gpu_count = 0
                 gpu_name = None
+                gpu_memory = None
                 if str(gpu.get("count")).isnumeric():
                     gpu_count = int(gpu.get("count"))
                 if gpu.get("name"):
                     gpu_name = gpu.get("name")
                     if not gpu_count:
                         gpu_count = 1
+                if gpu.get("memory"):
+                    gpu_memory = _str_to_mib(gpu.get("memory"))
+                    if not gpu_count:
+                        gpu_count = 1
                 if gpu_count:
-                    resources.gpus = GpusRequirements(count=gpu_count, name=gpu_name)
+                    resources.gpus = GpusRequirements(
+                        count=gpu_count, name=gpu_name, memory_mib=gpu_memory
+                    )
         for resource_name in self.provider_data["resources"]:
             if resource_name.endswith("/gpu") and len(resource_name) > 4:
                 if not str(self.provider_data["resources"][resource_name]).isnumeric():
                     sys.exit(f"resources.'{resource_name}' should be an integer")
                 gpu = int(self.provider_data["resources"][resource_name])
                 if gpu > 0:
                     resources.gpus = GpusRequirements(count=gpu, name=resource_name[:-4])
         if self.provider_data["resources"].get("shm_size"):
             resources.shm_size_mib = _str_to_mib(self.provider_data["resources"]["shm_size"])
         if self.provider_data["resources"].get("interruptible"):
             resources.interruptible = self.provider_data["resources"]["interruptible"]
-        if self.provider_data["resources"].get("local"):
-            resources.local = self.provider_data["resources"]["local"]
         return resources
 
     @staticmethod
     def _extend_commands_with_env(commands, env):
         commands.extend([f"export {e}={env[e] if env.get(e) else ''}" for e in env])
 
+    @staticmethod
+    def _extend_commands_with_openssh_server(commands: List[str], ssh_pub_key: str, port_idx: int):
+        commands.extend(
+            [
+                f'echo "{ssh_pub_key}" >> ~/.ssh/authorized_keys',
+                "ssh-keygen -A > /dev/null",
+                f"/usr/sbin/sshd -p $PORT_{port_idx}",
+            ]
+        )
+
 
 def get_provider_names() -> List[str]:
     return list(
         map(
             lambda m: m[1],
             filter(
                 lambda m: m.ispkg and not m[1].startswith("_"),
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/_torchrun/main.py` & `dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import argparse
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
-from dstack.jobs import GpusRequirements, JobSpec, Requirements
+from rich_argparse import RichHelpFormatter
+
+from dstack.backend.base import Backend
+from dstack.core.job import GpusRequirements, JobSpec, Requirements
 from dstack.providers import Provider
 
 
 class TorchrunProvider(Provider):
     def __init__(self):
         super().__init__("torchrun")
         self.script = None
@@ -17,34 +20,35 @@
         self.working_dir = None
         self.nodes = None
         self.resources = None
         self.args = None
 
     def load(
         self,
+        backend: Backend,
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
     ):
-        super().load(provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, provider_args, workflow_name, provider_data, run_name)
         self.script = self.provider_data.get("script") or self.provider_data.get("file")
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.nodes = self.provider_data.get("nodes") or 1
         self.resources = self._resources()
         self.args = self.provider_data.get("args")
 
     def _resources(self) -> Optional[Requirements]:
         resources = super()._resources()
         if resources.gpu is None:
-            resources.gpu = GpusRequirements(1)
+            resources.gpu = GpusRequirements(count=1)
         return resources
 
     def _image_name(self) -> str:
         cuda_is_required = self.resources and self.resources.gpus
         cuda_image_name = f"dstackai/miniforge:{self.python}-cuda-11.1"
         cpu_image_name = f"dstackai/miniforge:{self.python}"
         return cuda_image_name if cuda_is_required else cpu_image_name
@@ -98,15 +102,18 @@
                         requirements=self.resources,
                         master_job=master_job,
                     )
                 )
         return job_specs
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
         parser.add_argument("--nnodes", type=int, nargs="?")
         if not workflow_name:
             parser.add_argument("file", metavar="FILE", type=str)
             parser.add_argument("args", metavar="ARGS", nargs=argparse.ZERO_OR_MORE)
         return parser
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/bash/main.py` & `dstack-0.7rc1/cli/dstack/providers/bash/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,109 @@
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
+from rich_argparse import RichHelpFormatter
+
+from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class BashProvider(Provider):
     def __init__(self):
         super().__init__("bash")
         self.file = None
-        self.setup = None
         self.python = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
         self.ports = None
         self.commands = None
         self.image_name = None
+        self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
     ):
         super().load(backend, provider_args, workflow_name, provider_data, run_name)
-        self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.commands = self._get_list_data("commands")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.ports = self.provider_data.get("ports")
         self.resources = self._resources()
         self.image_name = self._image_name()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
+        parser.add_argument("--ssh", action="store_true", dest="openssh_server")
         parser.add_argument("-p", "--ports", metavar="PORT_COUNT", type=int)
         if not workflow_name:
             parser.add_argument("-c", "--command", type=str)
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
         if self.run_as_provider:
             self.provider_data["commands"] = [args.command]
         if args.ports:
             self.provider_data["ports"] = args.ports
+        if args.openssh_server:
+            self.openssh_server = True
 
     def create_job_specs(self) -> List[JobSpec]:
-        apps = None
-        if self.ports:
-            apps = []
-            for i in range(self.ports):
-                apps.append(
-                    AppSpec(
-                        port_index=i,
-                        app_name="bash" + (str(i) if self.ports > 1 else ""),
-                    )
+        apps = []
+        for i in range(self.ports or 0):
+            apps.append(
+                AppSpec(
+                    port_index=i,
+                    app_name="bash" + (str(i) if self.ports > 1 else ""),
                 )
+            )
+        if self.openssh_server:
+            apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
+                entrypoint=["/bin/bash", "-i", "-c"],
                 working_dir=self.working_dir,
                 artifact_specs=self.artifact_specs,
-                port_count=self.ports,
+                port_count=len(apps),
                 requirements=self.resources,
                 app_specs=apps,
             )
         ]
 
     def _image_name(self) -> str:
         cuda_is_required = self.resources and self.resources.gpus
-        cuda_image_name = f"dstackai/miniforge:{self.python}-cuda-11.1"
-        cpu_image_name = f"dstackai/miniforge:{self.python}"
+        cuda_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}-cuda-11.1"
+        cpu_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}"
         return cuda_image_name if cuda_is_required else cpu_image_name
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
-        if self.setup:
-            commands.extend(self.setup)
+        if self.openssh_server:
+            self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, self.ports or 0)
         commands.extend(self.commands)
         return commands
 
 
 def __provider__():
     return BashProvider()
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/code/main.py` & `dstack-0.7rc1/cli/dstack/providers/code/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import uuid
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
+from rich_argparse import RichHelpFormatter
+
+from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class CodeProvider(Provider):
@@ -16,14 +19,15 @@
         self.version = None
         self.requirements = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
         self.image_name = None
+        self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
@@ -36,60 +40,73 @@
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
+        parser.add_argument("--ssh", action="store_true", dest="openssh_server")
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
+        if args.openssh_server:
+            self.openssh_server = True
 
     def create_job_specs(self) -> List[JobSpec]:
         env = {}
         connection_token = uuid.uuid4().hex
         env["CONNECTION_TOKEN"] = connection_token
+        apps = [
+            AppSpec(
+                port_index=0,
+                app_name="code",
+                url_query_params={
+                    "tkn": connection_token,
+                },
+            )
+        ]
+        if self.openssh_server:
+            apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
+                entrypoint=["/bin/bash", "-i", "-c"],
                 env=env,
                 working_dir=self.working_dir,
                 artifact_specs=self.artifact_specs,
-                port_count=1,
+                port_count=len(apps),
                 requirements=self.resources,
-                app_specs=[
-                    AppSpec(
-                        port_index=0,
-                        app_name="code",
-                        url_query_params={
-                            "tkn": connection_token,
-                        },
-                    )
-                ],
+                app_specs=apps,
             )
         ]
 
     def _image_name(self) -> str:
         cuda_is_required = self.resources and self.resources.gpus
-        cuda_image_name = f"dstackai/miniforge:{self.python}-cuda-11.1"
-        cpu_image_name = f"dstackai/miniforge:{self.python}"
+        cuda_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}-cuda-11.1"
+        cpu_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}"
         return cuda_image_name if cuda_is_required else cpu_image_name
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
+        if self.openssh_server:
+            self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, 1)
         commands.extend(
             [
+                "pip install ipykernel -q",
                 "mkdir -p /tmp",
                 'if [ $(uname -m) = "aarch64" ]; then arch="arm64"; else arch="x64"; fi',
                 f"wget -q https://github.com/gitpod-io/openvscode-server/releases/download/"
                 f"openvscode-server-v{self.version}/openvscode-server-v{self.version}-linux-$arch.tar.gz -O "
                 f"/tmp/openvscode-server-v{self.version}-linux-$arch.tar.gz",
                 f"tar -xzf /tmp/openvscode-server-v{self.version}-linux-$arch.tar.gz -C /tmp",
                 f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --install-extension ms-python.python",
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/docker/main.py` & `dstack-0.7rc1/cli/dstack/providers/docker/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
+from rich_argparse import RichHelpFormatter
+
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class DockerProvider(Provider):
     def __init__(self):
         super().__init__("docker")
         self.image_name = None
-        self.setup = None
+        self.registry_auth = None
         self.commands = None
+        self.entrypoint = None
         self.artifact_specs = None
         self.env = None
         self.working_dir = None
         self.ports = None
         self.resources = None
 
     def load(
@@ -25,39 +28,48 @@
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
     ):
         super().load(backend, provider_args, workflow_name, provider_data, run_name)
         self.image_name = self.provider_data["image"]
-        self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
+        self.registry_auth = self.provider_data.get("registry_auth")
         self.commands = self._get_list_data("commands")
+        self.entrypoint = self._get_entrypoint()
+        if self.commands and self.entrypoint is None:  # commands not empty
+            self.entrypoint = ["/bin/sh", "-i", "-c"]
         self.artifact_specs = self._artifact_specs()
         self.env = self.provider_data.get("env")
         self.working_dir = self.provider_data.get("working_dir")
         self.ports = self.provider_data.get("ports")
         self.resources = self._resources()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
         parser.add_argument("-p", "--ports", type=int)
         if not workflow_name:
             parser.add_argument("image", metavar="IMAGE", type=str)
             parser.add_argument("-c", "--command", type=str)
+            parser.add_argument("-e", "--entrypoint", type=str)
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
         if self.run_as_provider:
             self.provider_data["image"] = args.image
             if args.command:
                 self.provider_data["commands"] = [args.command]
+            if args.entrypoint:
+                self.provider_data["entrypoint"] = args.entrypoint
         if args.ports:
             self.provider_data["ports"] = args.ports
 
     def create_job_specs(self) -> List[JobSpec]:
         apps = None
         if self.ports:
             apps = []
@@ -65,21 +77,21 @@
                 apps.append(
                     AppSpec(
                         port_index=i,
                         app_name="docker" + (i if self.ports > 1 else ""),
                     )
                 )
         commands = []
-        if self.setup:
-            commands.extend(self.setup)
         commands.extend(self.commands or [])
         return [
             JobSpec(
                 image_name=self.image_name,
+                registry_auth=self.registry_auth,
                 commands=commands,
+                entrypoint=self.entrypoint,
                 env=self.env,
                 working_dir=self.working_dir,
                 artifact_specs=self.artifact_specs,
                 port_count=self.ports,
                 requirements=self.resources,
                 app_specs=apps,
             )
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/lab/main.py` & `dstack-0.7rc1/cli/dstack/providers/lab/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import uuid
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
+from rich_argparse import RichHelpFormatter
+
+from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class LabProvider(Provider):
@@ -15,14 +18,15 @@
         self.python = None
         self.version = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
         self.image_name = None
+        self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
@@ -35,57 +39,69 @@
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
+        parser.add_argument("--ssh", action="store_true", dest="openssh_server")
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
+        if args.openssh_server:
+            self.openssh_server = True
 
     def create_job_specs(self) -> List[JobSpec]:
         env = {}
         token = uuid.uuid4().hex
         env["TOKEN"] = token
+        apps = [
+            AppSpec(
+                port_index=0,
+                app_name="lab",
+                url_path="lab",
+                url_query_params={"token": token},
+            )
+        ]
+        if self.openssh_server:
+            apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
+                entrypoint=["/bin/bash", "-i", "-c"],
                 env=env,
                 working_dir=self.working_dir,
                 artifact_specs=self.artifact_specs,
-                port_count=1,
+                port_count=len(apps),
                 requirements=self.resources,
-                app_specs=[
-                    AppSpec(
-                        port_index=0,
-                        app_name="lab",
-                        url_path="lab",
-                        url_query_params={"token": token},
-                    )
-                ],
+                app_specs=apps,
             )
         ]
 
     def _image_name(self) -> str:
         cuda_is_required = self.resources and self.resources.gpus
-        cuda_image_name = f"dstackai/miniforge:{self.python}-cuda-11.1"
-        cpu_image_name = f"dstackai/miniforge:{self.python}"
+        cuda_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}-cuda-11.1"
+        cpu_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}"
         return cuda_image_name if cuda_is_required else cpu_image_name
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
+        if self.openssh_server:
+            self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, 1)
         commands.extend(
             [
                 "conda install psutil -y",
                 "pip install jupyterlab" + (f"=={self.version}" if self.version else ""),
                 "pip install ipywidgets",
                 "jupyter nbextension enable --py widgetsnbextension",
                 "mkdir -p /root/.jupyter",
```

### Comparing `dstack-0.2rc1/cli/dstack/providers/notebook/main.py` & `dstack-0.7rc1/cli/dstack/providers/notebook/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import uuid
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Optional
 
+from rich_argparse import RichHelpFormatter
+
+from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class NotebookProvider(Provider):
@@ -15,14 +18,15 @@
         self.python = None
         self.version = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
         self.image_name = None
+        self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
@@ -35,56 +39,68 @@
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
-        parser = ArgumentParser(prog="dstack run " + (workflow_name or self.provider_name))
+        parser = ArgumentParser(
+            prog="dstack run " + (workflow_name or self.provider_name),
+            formatter_class=RichHelpFormatter,
+        )
         self._add_base_args(parser)
+        parser.add_argument("--ssh", action="store_true", dest="openssh_server")
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
+        if args.openssh_server:
+            self.openssh_server = True
 
     def create_job_specs(self) -> List[JobSpec]:
         env = {}
         token = uuid.uuid4().hex
         env["TOKEN"] = token
+        apps = [
+            AppSpec(
+                port_index=0,
+                app_name="notebook",
+                url_query_params={"token": token},
+            )
+        ]
+        if self.openssh_server:
+            apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
+                entrypoint=["/bin/bash", "-i", "-c"],
                 env=env,
                 working_dir=self.working_dir,
                 artifact_specs=self.artifact_specs,
-                port_count=1,
+                port_count=len(apps),
                 requirements=self.resources,
-                app_specs=[
-                    AppSpec(
-                        port_index=0,
-                        app_name="notebook",
-                        url_query_params={"token": token},
-                    )
-                ],
+                app_specs=apps,
             )
         ]
 
     def _image_name(self) -> str:
         cuda_is_required = self.resources and self.resources.gpus
-        cuda_image_name = f"dstackai/miniforge:{self.python}-cuda-11.1"
-        cpu_image_name = f"dstackai/miniforge:{self.python}"
+        cuda_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}-cuda-11.1"
+        cpu_image_name = f"dstackai/miniforge:py{self.python}-{version.miniforge_image}"
         return cuda_image_name if cuda_is_required else cpu_image_name
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
+        if self.openssh_server:
+            self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, 1)
         commands.extend(
             [
                 "conda install psutil -y",
                 "pip install jupyter" + (f"=={self.version}" if self.version else ""),
                 "mkdir -p /root/.jupyter",
                 'echo "c.NotebookApp.allow_root = True" > /root/.jupyter/jupyter_notebook_config.py',
                 "echo \"c.NotebookApp.allow_origin = '*'\" >> /root/.jupyter/jupyter_notebook_config.py",
```

### Comparing `dstack-0.2rc1/cli/dstack/utils/common.py` & `dstack-0.7rc1/cli/dstack/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import time
 from datetime import datetime, timedelta
 from typing import Any, Optional
 
 from botocore.utils import datetime2timestamp, parse_timestamp
 
 
 def _quoted(s: Optional[str]) -> str:
@@ -95,7 +96,17 @@
     return "%.1f%s%s" % (num, "Yi", suffix)
 
 
 def removeprefix(s: str, prefix: str) -> str:
     if s.startswith(prefix):
         return s[len(prefix) :]
     return s
+
+
+def get_milliseconds_since_epoch() -> int:
+    return int(round(time.time() * 1000))
+
+
+def format_list(items: Optional[list], *, formatter=str) -> Optional[str]:
+    if items is None:
+        return None
+    return "[{}]".format(", ".join(formatter(item) for item in items))
```

### Comparing `dstack-0.2rc1/cli/dstack/utils/random_names.py` & `dstack-0.7rc1/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.2rc1/cli/dstack.egg-info/PKG-INFO` & `dstack-0.7rc1/cli/dstack.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.2rc1
-Summary: Easy-to-run ML workflows on any cloud
+Version: 0.7rc1
+Summary: The hassle-free tool for managing ML workflows on any cloud platform.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,134 +20,147 @@
 <h1 align="center">
   <a target="_blank" href="https://dstack.ai">
     <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
   </a>
 </h1>
 
 <h4 align="center">
-Easy-to-run ML workflows on any cloud
+Automate your ML workflows on any cloud
 </h4>
 
 <p align="center">
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within teams. 
+The hassle-free tool for managing ML workflows on any cloud platform. 
 </p>
 
-[![Slack](https://img.shields.io/badge/slack-join%20community-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
+[![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://docs.dstack.ai" target="_blank"><b>Docs</b></a> • 
 <a href="https://docs.dstack.ai/quick-start"><b>Quick start</b></a> • 
-<a href="https://docs.dstack.ai/basics/hello-world" target="_blank"><b>Basics</b></a> • 
-<a href="https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ" target="_blank"><b>Slack</b></a> 
+<a href="https://docs.dstack.ai/playground" target="_blank"><b>Playground</b></a> •   
+<a href="https://docs.dstack.ai/setup"><b>Setup</b></a> • 
+<a href="https://docs.dstack.ai/usage/hello-world" target="_blank"><b>Usage</b></a>  • 
+<a href="https://docs.dstack.ai/examples/tensorboard" target="_blank"><b>Examples</b></a>
 </p>
 
 [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)](https://github.com/dstackai/dstack/commits/)
 [![PyPI - License](https://img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/dstackai/dstack/blob/master/LICENSE.md)
 
 </div>
 
-`dstack` is the most easy way to define ML workflows as code and run them either locally or remotely on any cloud.
+## What is dstack?
 
-### Highlighted features
+`dstack` is an open-source tool that automates ML workflows, enabling effective management on any cloud platform. 
 
-* Define ML workflows declaratively as code
-* Run workflows locally or remotely on any cloud (AWS, GCP, etc)
-* Use on-demand on spot instances conveniently
-* Save data, checkpoints, environments as artifacts and reuse them across workflows
-* No need to use custom Docker images or Kubernetes
+It empowers your team to prepare data, train, and fine-tune models using their preferred frameworks and dev
+environments without spending time on engineering and infrastructure.
 
-## Installation
+## Install the CLI
 
-Use pip to install the `dstack` CLI:
+Use `pip` to install `dstack`:
 
 ```shell
-pip install dstack --upgrade
+pip install dstack
 ```
 
-## Example
+## Configure a remote
 
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
+By default, workflows run locally. To run workflows remotely (e.g. in a configured cloud account),
+configure a remote using the `dstack config` command.
+
+```shell
+dstack config
+
+? Choose backend. Use arrows to move, type to filter
+> [aws]
+  [gcp]
+  [hub]
+```
+
+Choose [`hub`](https://docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and settings through a user
+interface while working in a team.
+
+For running remote workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/setup/aws.md)
+or [`gcp`](https://docs.dstack.ai/setup/gcp.md).
+
+## Define workflows
+
+Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
 
 ```yaml
 workflows:
-  - name: mnist-data
-    provider: bash
-    commands:
-      - pip install torchvision
-      - python mnist/mnist_data.py
-    artifacts:
-      - path: ./data
-
   - name: train-mnist
     provider: bash
-    deps:
-      - workflow: mnist-data
     commands:
       - pip install torchvision pytorch-lightning tensorboard
-      - python mnist/train_mnist.py
+      - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-YAML-defined workflows eliminate the need to modify code in your scripts, giving you the freedom to choose frameworks,
-experiment trackers, and cloud providers.
-
 ## Run locally
 
-Use the `dstack` CLI to run workflows locally:
+By default, workflows run locally on your machine.
 
 ```shell
-dstack run mnist-data
+dstack run train-mnist
+
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
+
+Provisioning... It may take up to a minute. ✓
+
+To interrupt, press Ctrl+C.
+
+GPU available: True, used: True
+
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
 ## Run remotely
 
-To run workflows remotely (e.g. in the cloud) or share artifacts outside your machine, 
-you must configure your remote settings using the `dstack config` command:
+To run a workflow remotely (e.g. in a configured cloud account), add the `--remote` flag to the `dstack run` command:
+
+The necessary hardware resources can be configured either via YAML or through arguments in the `dstack run` command, such
+as `--gpu` and `--gpu-name`.
 
 ```shell
-dstack config
-```
+dstack run train-mnist --remote --gpu 1
 
-This command will ask you to choose the type of backend (e.g. AWS), and the corresponding
-settings (e.g. the region where to run workflows, an S3 bucket where to store artifacts, etc).
+RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+turtle-1  train-mnist  now        Submitted       aws
 
-```shell
-Backend: aws
-AWS profile: default
-AWS region: eu-west-1
-S3 bucket: dstack-142421590066-eu-west-1
-EC2 subnet: none
-```
+Provisioning... It may take up to a minute. ✓
 
-For more details on how to configure a remote, check the [installation](https://docs.dstack.ai/installation/#configure-a-remote) guide.
+To interrupt, press Ctrl+C.
 
-Once a remote is configured, use the `--remote` flag with the `dstack run` command to run the 
-workflow in the configured cloud:
+GPU available: True, used: True
 
-```shell
-dstack run mnist-data --remote
+Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-You can configure the required resources to run the workflows either via the `resources` property in YAML
-or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`, etc:
+Upon running a workflow remotely, `dstack` automatically creates resources in the configured cloud account and destroys them
+once the workflow is complete.
 
-```shell
-dstack run train-mnist --remote --gpu 1
-```
+## Providers
+
+`dstack` supports multiple [providers](https://docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch interactive development environments and applications.
+
+## Artifacts
 
-When you run a workflow remotely, `dstack` automatically creates resources in the configured cloud,
-and releases them once the workflow is finished.
+`dstack` allows you to save output artifacts and conveniently reuse them across workflows.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Docs](https://docs.dstack.ai/)
-* [Installation](https://docs.dstack.ai/installation)
 * [Quick start](https://docs.dstack.ai/quick-start)
-* [Basics](https://docs.dstack.ai/basics/hello-world)
+* [Playground](https://github.com/dstackai/dstack-playground)
+* [Setup](https://docs.dstack.ai/setup)
+* [Usage](https://docs.dstack.ai/usage/hello-world)
+* [Examples](https://docs.dstack.ai/examples/tensorboard)
  
 ##  Licence
 
 [Mozilla Public License 2.0](LICENSE.md)
```

#### html2text {}

```diff
@@ -1,56 +1,61 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.2rc1 Summary: Easy-to-run ML
-workflows on any cloud Home-page: https://dstack.ai Author: Andrey Cheptsov
-Author-email: andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://
-github.com/dstackai/dstack Platform: UNKNOWN Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: Mozilla Public License 2.0
-(MPL 2.0) Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dstack Version: 0.7rc1 Summary: The hassle-free
+tool for managing ML workflows on any cloud platform. Home-page: https://
+dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
+UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
+UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE.md
                             ****** [dstack] ******
-                 *** Easy-to-run ML workflows on any cloud ***
-Define ML workflows as code and run via CLI. Use any cloud. Collaborate within
-                                    teams.
-        [![Slack](https://img.shields.io/badge/slack-join%20community-
+                *** Automate your ML workflows on any cloud ***
+     The hassle-free tool for managing ML workflows on any cloud platform.
+           [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
-                   Docs â¢ Quick_start â¢ Basics â¢ Slack
+     Docs â¢ Quick_start â¢ Playground â¢ Setup â¢ Usage â¢ Examples
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
-`dstack` is the most easy way to define ML workflows as code and run them
-either locally or remotely on any cloud. ### Highlighted features * Define ML
-workflows declaratively as code * Run workflows locally or remotely on any
-cloud (AWS, GCP, etc) * Use on-demand on spot instances conveniently * Save
-data, checkpoints, environments as artifacts and reuse them across workflows *
-No need to use custom Docker images or Kubernetes ## Installation Use pip to
-install the `dstack` CLI: ```shell pip install dstack --upgrade ``` ## Example
-Here's an example from the [Quick start](https://docs.dstack.ai/quick-start).
-```yaml workflows: - name: mnist-data provider: bash commands: - pip install
-torchvision - python mnist/mnist_data.py artifacts: - path: ./data - name:
-train-mnist provider: bash deps: - workflow: mnist-data commands: - pip install
-torchvision pytorch-lightning tensorboard - python mnist/train_mnist.py
-artifacts: - path: ./lightning_logs ``` YAML-defined workflows eliminate the
-need to modify code in your scripts, giving you the freedom to choose
-frameworks, experiment trackers, and cloud providers. ## Run locally Use the
-`dstack` CLI to run workflows locally: ```shell dstack run mnist-data ``` ##
-Run remotely To run workflows remotely (e.g. in the cloud) or share artifacts
-outside your machine, you must configure your remote settings using the `dstack
-config` command: ```shell dstack config ``` This command will ask you to choose
-the type of backend (e.g. AWS), and the corresponding settings (e.g. the region
-where to run workflows, an S3 bucket where to store artifacts, etc). ```shell
-Backend: aws AWS profile: default AWS region: eu-west-1 S3 bucket: dstack-
-142421590066-eu-west-1 EC2 subnet: none ``` For more details on how to
-configure a remote, check the [installation](https://docs.dstack.ai/
-installation/#configure-a-remote) guide. Once a remote is configured, use the
-`--remote` flag with the `dstack run` command to run the workflow in the
-configured cloud: ```shell dstack run mnist-data --remote ``` You can configure
-the required resources to run the workflows either via the `resources` property
-in YAML or the `dstack run` command's arguments, such as `--gpu`, `--gpu-name`,
-etc: ```shell dstack run train-mnist --remote --gpu 1 ``` When you run a
-workflow remotely, `dstack` automatically creates resources in the configured
-cloud, and releases them once the workflow is finished. ## More information For
-additional information and examples, see the following links: * [Docs](https://
-docs.dstack.ai/) * [Installation](https://docs.dstack.ai/installation) * [Quick
-start](https://docs.dstack.ai/quick-start) * [Basics](https://docs.dstack.ai/
-basics/hello-world) ## Licence [Mozilla Public License 2.0](LICENSE.md)
+## What is dstack? `dstack` is an open-source tool that automates ML workflows,
+enabling effective management on any cloud platform. It empowers your team to
+prepare data, train, and fine-tune models using their preferred frameworks and
+dev environments without spending time on engineering and infrastructure. ##
+Install the CLI Use `pip` to install `dstack`: ```shell pip install dstack ```
+## Configure a remote By default, workflows run locally. To run workflows
+remotely (e.g. in a configured cloud account), configure a remote using the
+`dstack config` command. ```shell dstack config ? Choose backend. Use arrows to
+move, type to filter > [aws] [gcp] [hub] ``` Choose [`hub`](https://
+docs.dstack.ai/setup/hub.md) if you prefer managing cloud credentials and
+settings through a user interface while working in a team. For running remote
+workflows with local cloud credentials, select [`aws`](https://docs.dstack.ai/
+setup/aws.md) or [`gcp`](https://docs.dstack.ai/setup/gcp.md). ## Define
+workflows Define ML workflows, their output artifacts, hardware requirements,
+and dependencies via YAML. ```yaml workflows: - name: train-mnist provider:
+bash commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run
+locally By default, workflows run locally on your machine. ```shell dstack run
+train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist
+now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` ## Run remotely To run a workflow remotely
+(e.g. in a configured cloud account), add the `--remote` flag to the `dstack
+run` command: The necessary hardware resources can be configured either via
+YAML or through arguments in the `dstack run` command, such as `--gpu` and `--
+gpu-name`. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW
+SUBMITTED STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws
+Provisioning... It may take up to a minute. â To interrupt, press Ctrl+C. GPU
+available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35,
+v_num=0] ``` Upon running a workflow remotely, `dstack` automatically creates
+resources in the configured cloud account and destroys them once the workflow
+is complete. ## Providers `dstack` supports multiple [providers](https://
+docs.dstack.ai/usage/providers) to set up environments, run scripts, and launch
+interactive development environments and applications. ## Artifacts `dstack`
+allows you to save output artifacts and conveniently reuse them across
+workflows. ## More information For additional information and examples, see the
+following links: * [Docs](https://docs.dstack.ai/) * [Quick start](https://
+docs.dstack.ai/quick-start) * [Playground](https://github.com/dstackai/dstack-
+playground) * [Setup](https://docs.dstack.ai/setup) * [Usage](https://
+docs.dstack.ai/usage/hello-world) * [Examples](https://docs.dstack.ai/examples/
+tensorboard) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.2rc1/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 cli/dstack/backend/aws/repos.py
 cli/dstack/backend/aws/runners.py
 cli/dstack/backend/aws/secrets.py
 cli/dstack/backend/aws/storage.py
 cli/dstack/backend/aws/utils.py
 cli/dstack/backend/base/__init__.py
 cli/dstack/backend/base/artifacts.py
+cli/dstack/backend/base/cache.py
 cli/dstack/backend/base/compute.py
 cli/dstack/backend/base/jobs.py
 cli/dstack/backend/base/logs.py
 cli/dstack/backend/base/repos.py
 cli/dstack/backend/base/runners.py
 cli/dstack/backend/base/runs.py
 cli/dstack/backend/base/secrets.py
@@ -55,74 +56,87 @@
 cli/dstack/backend/local/config.py
 cli/dstack/backend/local/logs.py
 cli/dstack/backend/local/runners.py
 cli/dstack/backend/local/secrets.py
 cli/dstack/backend/local/storage.py
 cli/dstack/cli/__init__.py
 cli/dstack/cli/common.py
+cli/dstack/cli/config.py
 cli/dstack/cli/handlers.py
 cli/dstack/cli/main.py
 cli/dstack/cli/updates.py
 cli/dstack/cli/commands/__init__.py
 cli/dstack/cli/commands/config/__init__.py
+cli/dstack/cli/commands/cp/__init__.py
 cli/dstack/cli/commands/hub/__init__.py
 cli/dstack/cli/commands/init/__init__.py
 cli/dstack/cli/commands/logs/__init__.py
 cli/dstack/cli/commands/ls/__init__.py
+cli/dstack/cli/commands/prune/__init__.py
 cli/dstack/cli/commands/ps/__init__.py
 cli/dstack/cli/commands/pull/__init__.py
 cli/dstack/cli/commands/push/__init__.py
 cli/dstack/cli/commands/rm/__init__.py
 cli/dstack/cli/commands/run/__init__.py
+cli/dstack/cli/commands/run/ssh_tunnel.py
 cli/dstack/cli/commands/secrets/__init__.py
 cli/dstack/cli/commands/stop/__init__.py
 cli/dstack/cli/commands/tags/__init__.py
 cli/dstack/core/__init__.py
 cli/dstack/core/app.py
 cli/dstack/core/artifact.py
+cli/dstack/core/cache.py
 cli/dstack/core/config.py
 cli/dstack/core/dependents.py
 cli/dstack/core/error.py
 cli/dstack/core/instance.py
 cli/dstack/core/job.py
 cli/dstack/core/log_event.py
 cli/dstack/core/repo.py
 cli/dstack/core/request.py
 cli/dstack/core/run.py
 cli/dstack/core/runners.py
 cli/dstack/core/secret.py
 cli/dstack/core/storage.py
 cli/dstack/core/tag.py
+cli/dstack/core/userconfig.py
 cli/dstack/hub/__init__.py
 cli/dstack/hub/main.py
+cli/dstack/hub/background/__init__.py
+cli/dstack/hub/background/tasks/__init__.py
+cli/dstack/hub/background/tasks/resubmit_jobs.py
 cli/dstack/hub/db/__init__.py
 cli/dstack/hub/db/migrate.py
 cli/dstack/hub/db/models.py
+cli/dstack/hub/migration/__init__.py
+cli/dstack/hub/migration/env.py
+cli/dstack/hub/migration/versions/3b900659c822_.py
+cli/dstack/hub/migration/versions/__init__.py
 cli/dstack/hub/models/__init__.py
 cli/dstack/hub/repository/__init__.py
-cli/dstack/hub/repository/hub.py
-cli/dstack/hub/repository/role.py
-cli/dstack/hub/repository/user.py
+cli/dstack/hub/repository/projects.py
+cli/dstack/hub/repository/users.py
 cli/dstack/hub/routers/__init__.py
 cli/dstack/hub/routers/artifacts.py
-cli/dstack/hub/routers/auth.py
 cli/dstack/hub/routers/cache.py
-cli/dstack/hub/routers/hub.py
 cli/dstack/hub/routers/jobs.py
 cli/dstack/hub/routers/link.py
 cli/dstack/hub/routers/logs.py
+cli/dstack/hub/routers/projects.py
 cli/dstack/hub/routers/repos.py
 cli/dstack/hub/routers/runners.py
 cli/dstack/hub/routers/runs.py
 cli/dstack/hub/routers/secrets.py
 cli/dstack/hub/routers/tags.py
 cli/dstack/hub/routers/users.py
 cli/dstack/hub/routers/util.py
+cli/dstack/hub/routers/workflows.py
 cli/dstack/hub/security/__init__.py
-cli/dstack/hub/security/scope.py
+cli/dstack/hub/security/permissions.py
+cli/dstack/hub/security/utils.py
 cli/dstack/providers/__init__.py
 cli/dstack/providers/_torchrun/__init__.py
 cli/dstack/providers/_torchrun/main.py
 cli/dstack/providers/bash/__init__.py
 cli/dstack/providers/bash/main.py
 cli/dstack/providers/code/__init__.py
 cli/dstack/providers/code/main.py
@@ -131,9 +145,26 @@
 cli/dstack/providers/lab/__init__.py
 cli/dstack/providers/lab/main.py
 cli/dstack/providers/notebook/__init__.py
 cli/dstack/providers/notebook/main.py
 cli/dstack/schemas/__init__.py
 cli/dstack/utils/__init__.py
 cli/dstack/utils/common.py
+cli/dstack/utils/interpolator.py
 cli/dstack/utils/random_names.py
-cli/tests/__init__.py
+cli/tests/__init__.py
+cli/tests/backend/__init__.py
+cli/tests/backend/base/__init__.py
+cli/tests/backend/base/test_logs.py
+cli/tests/hub/__init__.py
+cli/tests/hub/common.py
+cli/tests/hub/conftest.py
+cli/tests/hub/routers/__init__.py
+cli/tests/hub/routers/test_jobs.py
+cli/tests/hub/routers/test_projects.py
+cli/tests/hub/routers/test_users.py
+cli/tests/providers/__init__.py
+cli/tests/providers/test_local_path.py
+cli/tests/providers/docker/__init__.py
+cli/tests/providers/docker/test_entrypoint.py
+cli/tests/utils/__init__.py
+cli/tests/utils/test_interpolator.py
```

### Comparing `dstack-0.2rc1/setup.py` & `dstack-0.7rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,30 @@
     version=get_version(),
     author="Andrey Cheptsov",
     author_email="andrey@dstack.ai",
     package_dir={"": "cli"},
     packages=find_packages("cli"),
     package_data={
         "dstack.schemas": ["*.json"],
-        "dstack.hub": ["statics/*", "statics/**/*", "statics/**/**/*"],
+        "dstack.hub": [
+            "statics/*",
+            "statics/**/*",
+            "statics/**/**/*",
+        ],
     },
     include_package_data=True,
     scripts=[],
     entry_points={
         "console_scripts": ["dstack=dstack.cli.main:main"],
     },
     url="https://dstack.ai",
     project_urls={
         "Source": "https://github.com/dstackai/dstack",
     },
-    description="Easy-to-run ML workflows on any cloud",
+    description="The hassle-free tool for managing ML workflows on any cloud platform.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     install_requires=[
         "pyyaml",
         "requests",
         "gitpython",
@@ -64,29 +68,32 @@
         "git-url-parse",
         "rich",
         "rich-argparse",
         "fastapi",
         "starlette",
         "uvicorn",
         "pydantic",
-        "sqlalchemy",
+        "sqlalchemy[asyncio]>=2.0.0",
         "websocket-client",
         "cursor",
         "simple-term-menu",
         "py-cpuinfo",
         "psutil",
         "jinja2",
         "pygtail",
         "packaging",
         "google-auth>=2.3.0",  # indirect
         "google-cloud-storage>=2.0.0",
         "google-cloud-compute>=1.5.0",
         "google-cloud-secret-manager>=2.0.0",
         "google-cloud-logging>=2.0.0",
         "aiosqlite",
+        "apscheduler",
+        "alembic>=1.10.2",
+        "typing-extensions>=4.0.0",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3",
     ],
```

