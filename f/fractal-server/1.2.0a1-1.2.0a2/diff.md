# Comparing `tmp/fractal_server-1.2.0a1.tar.gz` & `tmp/fractal_server-1.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.0a1.tar", max compression
+gzip compressed data, was "fractal_server-1.2.0a2.tar", max compression
```

## Comparing `fractal_server-1.2.0a1.tar` & `fractal_server-1.2.0a2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a1/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a1/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a1/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-04-11 10:01:35.365476 fractal_server-1.2.0a1/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a1/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21405 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11632 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11398 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a1/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a1/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a1/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2341 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     7955 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    20869 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     4510 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0       16 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3690 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     9140 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    18186 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4327 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    39963 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9748 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7379 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a1/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a1/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a1/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a1/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a1/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a1/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    13217 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/config.py
--rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a1/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a1/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a1/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a1/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a1/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12796 2023-04-11 10:01:01.989872 fractal_server-1.2.0a1/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a1/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-04-11 10:01:35.365476 fractal_server-1.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a1/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a2/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a2/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a2/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-11 10:24:38.930920 fractal_server-1.2.0a2/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a2/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    21405 2023-04-11 10:24:00.715757 fractal_server-1.2.0a2/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    11632 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11398 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a2/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a2/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a2/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     7955 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    20869 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     4510 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3690 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     9140 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    18186 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4327 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    39963 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9748 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a2/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a2/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a2/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a2/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a2/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a2/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a2/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    13216 2023-04-11 10:24:11.691515 fractal_server-1.2.0a2/fractal_server/config.py
+-rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a2/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a2/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a2/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a2/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a2/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12796 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a2/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-11 10:24:38.930920 fractal_server-1.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a2/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a2/PKG-INFO
```

### Comparing `fractal_server-1.2.0a1/LICENSE` & `fractal_server-1.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/README.md` & `fractal_server-1.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/__main__.py` & `fractal_server-1.2.0a2/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/alembic.ini` & `fractal_server-1.2.0a2/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/api/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.0a2/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.0a2/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.0a2/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.0a2/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/db/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/job.py` & `fractal_server-1.2.0a2/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/project.py` & `fractal_server-1.2.0a2/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/security.py` & `fractal_server-1.2.0a2/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/state.py` & `fractal_server-1.2.0a2/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/task.py` & `fractal_server-1.2.0a2/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/models/workflow.py` & `fractal_server-1.2.0a2/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_common.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/runner/common.py` & `fractal_server-1.2.0a2/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/app/security/__init__.py` & `fractal_server-1.2.0a2/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.0a2/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.0a2/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/README.md` & `fractal_server-1.2.0a2/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/project.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/state.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/task.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/user.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.0a2/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.0a2/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/config.py` & `fractal_server-1.2.0a2/fractal_server/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
             if not self.FRACTAL_SLURM_CONFIG_FILE.exists():
                 raise FractalConfigurationError(
                     f"{info} but {str(self.FRACTAL_SLURM_CONFIG_FILE)} "
                     "is missing"
                 )
 
             # Check that FRACTAL_SLURM_CONFIG_FILE content is valid
-            from fractal_server.app.runnner._slurm._slurm_config import (
+            from fractal_server.app.runner._slurm._slurm_config import (
                 load_slurm_config_file,
             )
 
             _ = load_slurm_config_file(
                 config_path=self.FRACTAL_SLURM_CONFIG_FILE
             )
```

### Comparing `fractal_server-1.2.0a1/fractal_server/main.py` & `fractal_server-1.2.0a2/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/migrations/env.py` & `fractal_server-1.2.0a2/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.0a2/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.0a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.0a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.0a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/syringe.py` & `fractal_server-1.2.0a2/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/tasks/collection.py` & `fractal_server-1.2.0a2/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/fractal_server/utils.py` & `fractal_server-1.2.0a2/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a1/pyproject.toml` & `fractal_server-1.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.0a1"
+version = "1.2.0a2"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.0a1"
+current_version = "1.2.0a2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.0a1/setup.py` & `fractal_server-1.2.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.0a1',
+    'version': '1.2.0a2',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.0a1/PKG-INFO` & `fractal_server-1.2.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.0a1
+Version: 1.2.0a2
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

