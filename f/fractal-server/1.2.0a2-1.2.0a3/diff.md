# Comparing `tmp/fractal_server-1.2.0a2.tar.gz` & `tmp/fractal_server-1.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.0a2.tar", max compression
+gzip compressed data, was "fractal_server-1.2.0a3.tar", max compression
```

## Comparing `fractal_server-1.2.0a2.tar` & `fractal_server-1.2.0a3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a2/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a2/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a2/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-04-11 10:24:38.930920 fractal_server-1.2.0a2/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a2/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a2/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21405 2023-04-11 10:24:00.715757 fractal_server-1.2.0a2/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11632 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11398 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a2/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a2/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a2/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2341 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     7955 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    20869 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     4510 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0       16 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3690 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     9140 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    18186 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4327 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    39963 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9748 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7379 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a2/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a2/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a2/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a2/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a2/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a2/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a2/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a2/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a2/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a2/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a2/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    13216 2023-04-11 10:24:11.691515 fractal_server-1.2.0a2/fractal_server/config.py
--rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a2/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a2/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a2/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a2/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a2/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-07 06:31:24.060647 fractal_server-1.2.0a2/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12796 2023-04-11 10:24:00.719757 fractal_server-1.2.0a2/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a2/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-04-11 10:24:38.930920 fractal_server-1.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a2/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a3/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a3/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a3/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-11 12:16:47.461555 fractal_server-1.2.0a3/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a3/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    21405 2023-04-11 12:05:25.621706 fractal_server-1.2.0a3/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    11632 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a3/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a3/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a3/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     7955 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    20869 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     4510 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3690 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8802 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    18306 2023-04-11 12:16:36.785569 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4327 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    39831 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9748 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a3/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a3/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a3/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a3/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a3/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a3/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    13216 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/config.py
+-rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a3/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a3/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a3/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a3/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a3/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a3/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12796 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a3/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-11 12:16:47.461555 fractal_server-1.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a3/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a3/PKG-INFO
```

### Comparing `fractal_server-1.2.0a2/LICENSE` & `fractal_server-1.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/README.md` & `fractal_server-1.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/__main__.py` & `fractal_server-1.2.0a3/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/alembic.ini` & `fractal_server-1.2.0a3/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/api/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.0a3/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.0a3/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.0a3/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.0a3/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/db/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/job.py` & `fractal_server-1.2.0a3/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/project.py` & `fractal_server-1.2.0a3/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/security.py` & `fractal_server-1.2.0a3/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/state.py` & `fractal_server-1.2.0a3/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/task.py` & `fractal_server-1.2.0a3/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/models/workflow.py` & `fractal_server-1.2.0a3/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_common.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_batching.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing import Optional
 
 
 class SlurmHeuristicsError(ValueError):
     pass
 
 
-def _estimate_n_parallel_ftasks_per_script(
+def _estimate_parallel_tasks_per_job(
     *,
     cpus_per_task: int,
     mem_per_task: int,
     max_cpus_per_job: int,
     max_mem_per_job: int,
 ) -> int:
     """
@@ -50,18 +50,18 @@
     val_based_on_mem = max_mem_per_job // mem_per_task
     return min(val_based_on_cpus, val_based_on_mem)
 
 
 def heuristics(
     *,
     # Number of parallel components (always known)
-    n_ftasks_tot: int,
+    tot_tasks: int,
     # Optional WorkflowTask attributes:
-    n_ftasks_per_script: Optional[int] = None,
-    n_parallel_ftasks_per_script: Optional[int] = None,
+    tasks_per_job: Optional[int] = None,
+    parallel_tasks_per_job: Optional[int] = None,
     # Task requirements (multiple possible sources):
     cpus_per_task: int,
     mem_per_task: int,
     # Fractal configuration variables (soft/hard limits):
     target_cpus_per_job: int,
     max_cpus_per_job: int,
     target_mem_per_job: int,  # in MB
@@ -69,15 +69,15 @@
     target_num_jobs: int,
     max_num_jobs: int,
 ) -> tuple[int, int]:
     """
     Heuristically determine parameters for multi-task batching
 
     "In-job queues" refer to the case where
-    `n_parallel_ftasks_per_script<n_ftasks_per_script`, that is, where not all
+    `parallel_tasks_per_job<tasks_per_job`, that is, where not all
     tasks of a given SLURM job will be executed at the same time.
 
     This function goes through the following branches:
 
     1. Validate/fix parameters, if they are provided as input.
     2. Heuristically determine parameters based on the per-task resource
        requirements and on the target amount of per-job resources, without
@@ -87,22 +87,22 @@
        resorting to in-job queues.
     4. Heuristically determine parameters (based on the per-task resource
        requirements and on the maximum amount of per-job resources) and then
        introduce in-job queues to satisfy the hard constraint on the maximum
        number of jobs.
 
     Arguments:
-        n_ftasks_tot:
+        tot_tasks:
             Total number of elements to be processed (e.g. number of images in
             a OME-NGFF array).
-        n_ftasks_per_script:
-            If `n_ftasks_per_script` and `n_parallel_ftasks_per_script` are not
+        tasks_per_job:
+            If `tasks_per_job` and `parallel_tasks_per_job` are not
             `None`, validate/edit this choice.
-        n_parallel_ftasks_per_script:
-            If `n_ftasks_per_script` and `n_parallel_ftasks_per_script` are not
+        parallel_tasks_per_job:
+            If `tasks_per_job` and `parallel_tasks_per_job` are not
             `None`, validate/edit this choice.
         cpus_per_task:
             Number of CPUs needed for each parallel task.
         mem_per_task:
             Memory (in MB) needed for each parallel task.
         target_cpus_per_job:
             Optimal number of CPUs for each SLURM job.
@@ -113,21 +113,20 @@
         max_mem_per_job:
             Maximum amount of memory (in MB) for each SLURM job.
         target_num_jobs:
             Optimal total number of SLURM jobs for a given WorkflowTask.
         max_num_jobs:
             Maximum total number of SLURM jobs for a given WorkflowTask.
     Return:
-        Valid values of `n_ftasks_per_script` and
-        `n_parallel_ftasks_per_script`.
+        Valid values of `tasks_per_job` and `parallel_tasks_per_job`.
     """
     # Preliminary checks
-    if bool(n_ftasks_per_script) != bool(n_parallel_ftasks_per_script):
+    if bool(tasks_per_job) != bool(parallel_tasks_per_job):
         msg = (
-            "n_ftasks_per_script and n_parallel_ftasks_per_script must "
+            "tasks_per_job and parallel_tasks_per_job must "
             "be both set or both unset"
         )
         logging.error(msg)
         raise SlurmHeuristicsError(msg)
     if cpus_per_task > max_cpus_per_job:
         msg = (
             f"[heuristics] Requested {cpus_per_task=} "
@@ -140,96 +139,96 @@
             f"[heuristics] Requested {mem_per_task=} "
             f"but {max_mem_per_job=}."
         )
         logging.error(msg)
         raise SlurmHeuristicsError(msg)
 
     # Branch 1: validate/update given parameters
-    if n_ftasks_per_script and n_parallel_ftasks_per_script:
-        # Reduce n_parallel_ftasks_per_script if it exceeds n_ftasks_per_script
-        if n_parallel_ftasks_per_script > n_ftasks_per_script:
+    if tasks_per_job and parallel_tasks_per_job:
+        # Reduce parallel_tasks_per_job if it exceeds tasks_per_job
+        if parallel_tasks_per_job > tasks_per_job:
             logging.warning(
-                "[heuristics] Set n_parallel_ftasks_per_script="
-                f"n_ftasks_per_script={n_ftasks_per_script}"
+                "[heuristics] Set parallel_tasks_per_job="
+                f"tasks_per_job={tasks_per_job}"
             )
-            n_parallel_ftasks_per_script = n_ftasks_per_script
+            parallel_tasks_per_job = tasks_per_job
 
         # Check requested cpus_per_job
-        cpus_per_job = n_parallel_ftasks_per_script * cpus_per_task
+        cpus_per_job = parallel_tasks_per_job * cpus_per_task
         if cpus_per_job > target_cpus_per_job:
             logging.warning(
                 f"[heuristics] Requested {cpus_per_job=} "
                 f"but {target_cpus_per_job=}."
             )
         if cpus_per_job > max_cpus_per_job:
             msg = (
                 f"[heuristics] Requested {cpus_per_job=} "
                 f"but {max_cpus_per_job=}."
             )
             logging.error(msg)
             raise SlurmHeuristicsError(msg)
 
         # Check requested mem_per_job
-        mem_per_job = n_parallel_ftasks_per_script * mem_per_task
+        mem_per_job = parallel_tasks_per_job * mem_per_task
         if mem_per_job > target_mem_per_job:
             logging.warning(
                 f"[heuristics] Requested {mem_per_job=} "
                 f"but {target_mem_per_job=}."
             )
         if mem_per_job > max_mem_per_job:
             msg = (
                 f"[heuristics] Requested {mem_per_job=} "
                 f"but {max_mem_per_job=}."
             )
             logging.error(msg)
             raise SlurmHeuristicsError(msg)
 
         # Check number of jobs
-        num_jobs = math.ceil(n_ftasks_tot / n_ftasks_per_script)
+        num_jobs = math.ceil(tot_tasks / tasks_per_job)
         if num_jobs > target_num_jobs:
             logging.info(
                 f"[heuristics] Requested {num_jobs=} "
                 f"but {target_num_jobs=}."
             )
         if num_jobs > max_num_jobs:
             msg = f"[heuristics] Requested {num_jobs=} but {max_num_jobs=}."
             logging.error(msg)
             raise SlurmHeuristicsError(msg)
         logging.debug("[heuristics] Return from branch 1")
-        return (n_ftasks_per_script, n_parallel_ftasks_per_script)
+        return (tasks_per_job, parallel_tasks_per_job)
 
     # 2: Target-resources-based heuristics, without in-job queues
-    n_parallel_ftasks_per_script = _estimate_n_parallel_ftasks_per_script(
+    parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=target_cpus_per_job,
         max_mem_per_job=target_mem_per_job,
     )
-    n_ftasks_per_script = n_parallel_ftasks_per_script
-    num_jobs = math.ceil(n_ftasks_tot / n_ftasks_per_script)
+    tasks_per_job = parallel_tasks_per_job
+    num_jobs = math.ceil(tot_tasks / tasks_per_job)
     if num_jobs <= target_num_jobs:
         logging.debug("[heuristics] Return from branch 2")
-        return (n_ftasks_per_script, n_parallel_ftasks_per_script)
+        return (tasks_per_job, parallel_tasks_per_job)
 
     # Branch 3: Max-resources-based heuristics, without in-job queues
-    n_parallel_ftasks_per_script = _estimate_n_parallel_ftasks_per_script(
+    parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=max_cpus_per_job,
         max_mem_per_job=max_mem_per_job,
     )
-    n_ftasks_per_script = n_parallel_ftasks_per_script
-    num_jobs = math.ceil(n_ftasks_tot / n_ftasks_per_script)
+    tasks_per_job = parallel_tasks_per_job
+    num_jobs = math.ceil(tot_tasks / tasks_per_job)
     if num_jobs <= max_num_jobs:
         logging.debug("[heuristics] Return from branch 3")
-        return (n_ftasks_per_script, n_parallel_ftasks_per_script)
+        return (tasks_per_job, parallel_tasks_per_job)
 
     # Branch 4: Max-resources-based heuristics, with in-job queues
-    n_parallel_ftasks_per_script = _estimate_n_parallel_ftasks_per_script(
+    parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=max_cpus_per_job,
         max_mem_per_job=max_mem_per_job,
     )
-    n_ftasks_per_script = math.ceil(n_ftasks_tot / max_num_jobs)
+    tasks_per_job = math.ceil(tot_tasks / max_num_jobs)
     logging.debug("[heuristics] Return from branch 4")
-    return (n_ftasks_per_script, n_parallel_ftasks_per_script)
+    return (tasks_per_job, parallel_tasks_per_job)
```

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,32 +187,32 @@
 class SlurmConfig(BaseModel, extra=Extra.forbid):
     """
     Abstraction for SLURM parameters
 
     Part of the attributes map directly to some of the SLURM attribues (see
     https://slurm.schedmd.com/sbatch.html), e.g. `partition`. Other attributes
     are metaparameters which are needed in fractal-server to combine multiple
-    tasks in the same SLURM job (e.g. `n_parallel_ftasks_per_script` or
+    tasks in the same SLURM job (e.g. `parallel_tasks_per_job` or
     `max_num_jobs`).
 
     Attributes:
         partition: Corresponds to SLURM option.
         cpus_per_task: Corresponds to SLURM option.
         mem_per_task_MB: Corresponds to `mem` SLURM option.
         job_name: Corresponds to `name` SLURM option.
         constraint: Corresponds to SLURM option.
         gres: Corresponds to SLURM option.
         account: Corresponds to SLURM option.
         time: Corresponds to SLURM option (WARNING: not fully supported).
         prefix: Prefix of configuration lines in SLURM submission scripts.
         shebang_line: Shebang line for SLURM submission scripts.
         extra_lines: Additional lines to include in SLURM submission scripts.
-        n_ftasks_per_script: Number of tasks for each SLURM job.
-        n_parallel_ftasks_per_script: Number of tasks to run in parallel for
-                                      each SLURM job.
+        tasks_per_job: Number of tasks for each SLURM job.
+        parallel_tasks_per_job: Number of tasks to run in parallel for
+                                each SLURM job.
         target_cpus_per_job: Optimal number of CPUs to be requested in each
                              SLURM job.
         max_cpus_per_job: Maximum number of CPUs that can be requested in each
                           SLURM job.
         target_mem_per_job: Optimal amount of memory (in MB) to be requested in
                             each SLURM job.
         max_mem_per_job: Maximum amount of memory (in MB) that can be requested
@@ -237,16 +237,16 @@
     account: Optional[str] = None
 
     # Free-field attribute for extra lines to be added to the SLURM job
     # preamble
     extra_lines: Optional[list[str]] = Field(default_factory=list)
 
     # Metaparameters needed to combine multiple tasks in each SLURM job
-    n_ftasks_per_script: Optional[int] = None
-    n_parallel_ftasks_per_script: Optional[int] = None
+    tasks_per_job: Optional[int] = None
+    parallel_tasks_per_job: Optional[int] = None
     target_cpus_per_job: int
     max_cpus_per_job: int
     target_mem_per_job: int
     max_mem_per_job: int
     target_num_jobs: int
     max_num_jobs: int
 
@@ -287,42 +287,40 @@
         return sorted(script_lines, key=_sorting_function)
 
     def to_sbatch_preamble(self) -> list[str]:
         """
         Compile `SlurmConfig` object into the preamble of a SLURM submission
         script.
         """
-        if self.n_parallel_ftasks_per_script is None:
+        if self.parallel_tasks_per_job is None:
             raise ValueError(
                 "SlurmConfig.sbatch_preamble requires that "
-                f"{self.n_parallel_ftasks_per_script=} is not None."
+                f"{self.parallel_tasks_per_job=} is not None."
             )
         if self.extra_lines:
             if len(self.extra_lines) != len(set(self.extra_lines)):
                 raise ValueError(f"{self.extra_lines=} contains repetitions")
 
-        mem_per_job_MB = (
-            self.n_parallel_ftasks_per_script * self.mem_per_task_MB
-        )
+        mem_per_job_MB = self.parallel_tasks_per_job * self.mem_per_task_MB
         lines = [
             self.shebang_line,
             f"{self.prefix} --partition={self.partition}",
-            f"{self.prefix} --ntasks={self.n_parallel_ftasks_per_script}",
+            f"{self.prefix} --ntasks={self.parallel_tasks_per_job}",
             f"{self.prefix} --cpus-per-task={self.cpus_per_task}",
             f"{self.prefix} --mem={mem_per_job_MB}M",
         ]
         for key in ["job_name", "constraint", "gres", "time", "account"]:
             value = getattr(self, key)
             if value is not None:
                 # Handle the `time` parameter
-                if key == "time" and self.n_parallel_ftasks_per_script > 1:
+                if key == "time" and self.parallel_tasks_per_job > 1:
                     logging.warning(
                         "Ignore `#SBATCH --time=...` line (given: "
-                        f"{self.time=}) for n_parallel_ftasks_per_script>1"
-                        f" (given: {self.n_parallel_ftasks_per_script}), "
+                        f"{self.time=}) for parallel_tasks_per_job>1"
+                        f" (given: {self.parallel_tasks_per_job}), "
                         "since scaling of time with number of tasks is "
                         "not implemented."
                     )
                     continue
                 option = key.replace("_", "-")
                 lines.append(f"{self.prefix} --{option}={value}")
 
@@ -461,15 +459,19 @@
     logging.debug(
         "[get_slurm_config] WorkflowTask/Task meta attribute: "
         f"{wftask.overridden_meta=}"
     )
 
     # Incorporate slurm_env.default_slurm_config
     slurm_env = load_slurm_config_file(config_path=config_path)
-    slurm_dict = slurm_env.default_slurm_config.dict(exclude_unset=True)
+    slurm_dict = slurm_env.default_slurm_config.dict(
+        exclude_unset=True, exclude={"mem"}
+    )
+    if slurm_env.default_slurm_config.mem:
+        slurm_dict["mem_per_task_MB"] = slurm_env.default_slurm_config.mem
 
     # Incorporate slurm_env.batching_config
     for key, value in slurm_env.batching_config.dict().items():
         slurm_dict[key] = value
     logging.debug(
         "[get_slurm_config] Fractal SLURM configuration file: "
         f"{slurm_env.dict()=}"
@@ -481,17 +483,19 @@
     #    slurm_env which are not under the `needs_gpu` subgroup
     # 2. This block of definitions has lower priority than whatever comes next
     #    (i.e. from WorkflowTask.overridden_meta).
     needs_gpu = wftask.overridden_meta.get("needs_gpu", False)
     logging.debug(f"[get_slurm_config] {needs_gpu=}")
     if needs_gpu:
         for key, value in slurm_env.gpu_slurm_config.dict(
-            exclude_unset=True
+            exclude_unset=True, exclude={"mem"}
         ).items():
             slurm_dict[key] = value
+        if slurm_env.gpu_slurm_config.mem:
+            slurm_dict["mem_per_task_MB"] = slurm_env.gpu_slurm_config.mem
 
     # Number of CPUs per task, for multithreading
     if "cpus_per_task" in wftask.overridden_meta.keys():
         cpus_per_task = int(wftask.overridden_meta["cpus_per_task"])
         slurm_dict["cpus_per_task"] = cpus_per_task
 
     # Required memory per task, in MB
@@ -516,23 +520,21 @@
             "[get_slurm_config] Removing repeated elements "
             f"from {extra_lines=}."
         )
         extra_lines = list(set(extra_lines))
     slurm_dict["extra_lines"] = extra_lines
 
     # Job-batching parameters (if None, they will be determined heuristically)
-    n_ftasks_per_script = wftask.overridden_meta.get(
-        "n_ftasks_per_script", None
-    )
-    n_parallel_ftasks_per_script = wftask.overridden_meta.get(
-        "n_parallel_ftasks_per_script", None
+    tasks_per_job = wftask.overridden_meta.get("tasks_per_job", None)
+    parallel_tasks_per_job = wftask.overridden_meta.get(
+        "parallel_tasks_per_job", None
     )
 
-    slurm_dict["n_ftasks_per_script"] = n_ftasks_per_script
-    slurm_dict["n_parallel_ftasks_per_script"] = n_parallel_ftasks_per_script
+    slurm_dict["tasks_per_job"] = tasks_per_job
+    slurm_dict["parallel_tasks_per_job"] = parallel_tasks_per_job
 
     # Put everything together
     logging.debug(
         "[get_slurm_config] Now create a SlurmConfig object based "
         f"on {slurm_dict=}"
     )
     slurm_config = SlurmConfig(**slurm_dict)
```

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,16 +301,16 @@
         current_extra_lines = slurm_config.extra_lines or []
         slurm_config.extra_lines = (
             current_extra_lines + self.common_script_lines
         )
 
         # Adapt slurm_config to the fact that this is a single-task SlurmJob
         # instance
-        slurm_config.n_ftasks_per_script = 1
-        slurm_config.n_parallel_ftasks_per_script = 1
+        slurm_config.tasks_per_job = 1
+        slurm_config.parallel_tasks_per_job = 1
 
         fut = self._submit_job(
             fun,
             slurm_config=slurm_config,
             slurm_file_prefix=slurm_file_prefix,
             task_files=task_files,
             single_task_submission=True,
@@ -391,47 +391,45 @@
         )
 
         # Set file prefixes
         general_slurm_file_prefix = str(task_files.task_order)
 
         # Transform iterable into a list and count its elements
         list_args = list(iterable)
-        n_ftasks_tot = len(list_args)
+        tot_tasks = len(list_args)
 
         # Set/validate parameters for task batching
-        n_ftasks_per_script, n_parallel_ftasks_per_script = heuristics(
+        tasks_per_job, parallel_tasks_per_job = heuristics(
             # Number of parallel components (always known)
-            n_ftasks_tot=len(list_args),
+            tot_tasks=len(list_args),
             # Optional WorkflowTask attributes:
-            n_ftasks_per_script=slurm_config.n_ftasks_per_script,
-            n_parallel_ftasks_per_script=slurm_config.n_parallel_ftasks_per_script,  # noqa
+            tasks_per_job=slurm_config.tasks_per_job,
+            parallel_tasks_per_job=slurm_config.parallel_tasks_per_job,  # noqa
             # Task requirements (multiple possible sources):
             cpus_per_task=slurm_config.cpus_per_task,
             mem_per_task=slurm_config.mem_per_task_MB,
             # Fractal configuration variables (soft/hard limits):
             target_cpus_per_job=slurm_config.target_cpus_per_job,
             target_mem_per_job=slurm_config.target_mem_per_job,
             target_num_jobs=slurm_config.target_num_jobs,
             max_cpus_per_job=slurm_config.max_cpus_per_job,
             max_mem_per_job=slurm_config.max_mem_per_job,
             max_num_jobs=slurm_config.max_num_jobs,
         )
-        slurm_config.n_parallel_ftasks_per_script = (
-            n_parallel_ftasks_per_script
-        )
-        slurm_config.n_ftasks_per_script = n_ftasks_per_script
+        slurm_config.parallel_tasks_per_job = parallel_tasks_per_job
+        slurm_config.tasks_per_job = tasks_per_job
 
         # Divide arguments in batches of `n_tasks_per_script` tasks each
         args_batches = []
-        batch_size = n_ftasks_per_script
-        for ind_chunk in range(0, n_ftasks_tot, batch_size):
+        batch_size = tasks_per_job
+        for ind_chunk in range(0, tot_tasks, batch_size):
             args_batches.append(
                 list_args[ind_chunk : ind_chunk + batch_size]  # noqa
             )
-        if len(args_batches) != math.ceil(n_ftasks_tot / n_ftasks_per_script):
+        if len(args_batches) != math.ceil(tot_tasks / tasks_per_job):
             raise RuntimeError("Something wrong here while batching tasks")
 
         # Construct list of futures (one per SLURM job, i.e. one per batch)
         fs = []
         current_component_index = 0
         for ind_batch, batch in enumerate(args_batches):
             batch_size = len(batch)
@@ -996,22 +994,22 @@
         *,
         list_commands: list[str],
         slurm_out_path: str,
         slurm_err_path: str,
         slurm_config: SlurmConfig,
     ):
 
-        num_tasks_max_running = slurm_config.n_parallel_ftasks_per_script
+        num_tasks_max_running = slurm_config.parallel_tasks_per_job
         mem_per_task_MB = slurm_config.mem_per_task_MB
 
         # Set ntasks
         ntasks = min(len(list_commands), num_tasks_max_running)
         if len(list_commands) < num_tasks_max_running:
             ntasks = len(list_commands)
-            slurm_config.n_parallel_ftasks_per_script = ntasks
+            slurm_config.parallel_tasks_per_job = ntasks
             logging.info(
                 f"{len(list_commands)=} is smaller than "
                 f"{num_tasks_max_running=}. Setting {ntasks=}."
             )
 
         # Prepare SLURM preamble based on SlurmConfig object
         script_lines = slurm_config.to_sbatch_preamble()
```

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/runner/common.py` & `fractal_server-1.2.0a3/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/app/security/__init__.py` & `fractal_server-1.2.0a3/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.0a3/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.0a3/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/README.md` & `fractal_server-1.2.0a3/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/project.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/state.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/task.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/user.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.0a3/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.0a3/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/config.py` & `fractal_server-1.2.0a3/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/main.py` & `fractal_server-1.2.0a3/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/migrations/env.py` & `fractal_server-1.2.0a3/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.0a3/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.0a3/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.0a3/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.0a3/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/syringe.py` & `fractal_server-1.2.0a3/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/tasks/collection.py` & `fractal_server-1.2.0a3/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/fractal_server/utils.py` & `fractal_server-1.2.0a3/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a2/pyproject.toml` & `fractal_server-1.2.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.0a2"
+version = "1.2.0a3"
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
-current_version = "1.2.0a2"
+current_version = "1.2.0a3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.0a2/setup.py` & `fractal_server-1.2.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.0a2',
+    'version': '1.2.0a3',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.0a2/PKG-INFO` & `fractal_server-1.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

