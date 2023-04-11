# Comparing `tmp/fractal_server-1.2.0a0.tar.gz` & `tmp/fractal_server-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.0a0.tar", max compression
+gzip compressed data, was "fractal_server-1.2.0a1.tar", max compression
```

## Comparing `fractal_server-1.2.0a0.tar` & `fractal_server-1.2.0a1.tar`

### file list

```diff
@@ -1,114 +1,116 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a0/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a0/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a0/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-04-06 13:00:24.430287 fractal_server-1.2.0a0/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a0/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21429 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11656 2023-03-15 12:02:58.126238 fractal_server-1.2.0a0/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11423 2023-03-27 06:34:27.621724 fractal_server-1.2.0a0/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a0/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a0/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a0/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2415 2023-03-16 15:50:18.447564 fractal_server-1.2.0a0/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1118 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1103 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1279 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5549 2023-04-06 06:39:20.701034 fractal_server-1.2.0a0/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0     7979 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    20622 2023-04-06 06:39:20.701034 fractal_server-1.2.0a0/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     4558 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     8368 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_parsl/__init__.py
--rw-r--r--   0        0        0     1118 2022-11-02 11:51:16.318067 fractal_server-1.2.0a0/fractal_server/app/runner/_parsl/_functions.py
--rw-r--r--   0        0        0    12649 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_parsl/_setup.py
--rw-r--r--   0        0        0     9194 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     3833 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    25865 2023-04-06 06:39:20.701034 fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5947 2023-03-09 14:37:07.061177 fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     2329 2023-02-22 13:06:13.003243 fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/wait_thread.py
--rw-r--r--   0        0        0     9796 2023-03-27 12:29:48.791979 fractal_server-1.2.0a0/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7403 2023-03-17 07:37:58.062089 fractal_server-1.2.0a0/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a0/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a0/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a0/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a0/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a0/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a0/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a0/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a0/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a0/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a0/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a0/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a0/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a0/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a0/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a0/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a0/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a0/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a0/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12786 2023-04-06 06:39:20.701034 fractal_server-1.2.0a0/fractal_server/config.py
--rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a0/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a0/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a0/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a0/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a0/fractal_server/py.typed
--rw-r--r--   0        0        0     2810 2023-02-22 13:06:13.007243 fractal_server-1.2.0a0/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-06 12:56:07.781548 fractal_server-1.2.0a0/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12845 2023-03-15 12:02:58.126238 fractal_server-1.2.0a0/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a0/fractal_server/utils.py
--rw-r--r--   0        0        0     2668 2023-04-06 13:00:24.430287 fractal_server-1.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fractal_server-1.2.0a0/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a1/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a1/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a1/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-11 10:01:35.365476 fractal_server-1.2.0a1/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a1/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a1/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    21405 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    11632 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11398 2023-04-11 10:01:01.977872 fractal_server-1.2.0a1/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a1/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a1/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a1/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     7955 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    20869 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     4510 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3690 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     9140 2023-04-11 10:01:01.981872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    18186 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4327 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    39963 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9748 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a1/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a1/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a1/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a1/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a1/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a1/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a1/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a1/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a1/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a1/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    13217 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/config.py
+-rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a1/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a1/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a1/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a1/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a1/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 10:01:01.985872 fractal_server-1.2.0a1/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-07 06:31:24.060647 fractal_server-1.2.0a1/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12796 2023-04-11 10:01:01.989872 fractal_server-1.2.0a1/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a1/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-11 10:01:35.365476 fractal_server-1.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a1/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a1/PKG-INFO
```

### Comparing `fractal_server-1.2.0a0/LICENSE` & `fractal_server-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/README.md` & `fractal_server-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/__main__.py` & `fractal_server-1.2.0a1/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/alembic.ini` & `fractal_server-1.2.0a1/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/app/api/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.0a1/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.0a1/fractal_server/app/api/v1/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import logging
-from typing import List
 from typing import Optional
 from typing import Union
 
 from fastapi import APIRouter
 from fastapi import BackgroundTasks
 from fastapi import Depends
 from fastapi import HTTPException
@@ -124,19 +123,19 @@
         )
     return dict(dataset=dataset, project=project)
 
 
 # Main endpoints (no ID required)
 
 
-@router.get("/", response_model=List[ProjectRead])
+@router.get("/", response_model=list[ProjectRead])
 async def get_list_project(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> List[Project]:
+) -> list[Project]:
     """
     Return list of projects user is member of
     """
     stm = (
         select(Project)
         .join(LinkUserProject)
         .where(LinkUserProject.user_id == user.id)
@@ -358,38 +357,38 @@
     db_dataset = Dataset(project_id=project_id, **dataset.dict())
     db.add(db_dataset)
     await db.commit()
     await db.refresh(db_dataset)
     return db_dataset
 
 
-@router.get("/{project_id}/workflows/", response_model=List[WorkflowRead])
+@router.get("/{project_id}/workflows/", response_model=list[WorkflowRead])
 async def get_workflow_list(
     project_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> Optional[List[WorkflowRead]]:
+) -> Optional[list[WorkflowRead]]:
     """
     Get list of workflows associated to the current project
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(Workflow).where(Workflow.project_id == project_id)
     res = await db.execute(stm)
     workflow_list = res.scalars().all()
     return workflow_list
 
 
-@router.get("/{project_id}/jobs/", response_model=List[ApplyWorkflowRead])
+@router.get("/{project_id}/jobs/", response_model=list[ApplyWorkflowRead])
 async def get_job_list(
     project_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> Optional[List[ApplyWorkflowRead]]:
+) -> Optional[list[ApplyWorkflowRead]]:
     """
     Get list of jobs associated to the current project
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(ApplyWorkflow).where(ApplyWorkflow.project_id == project_id)
@@ -520,22 +519,22 @@
     await db.commit()
     await db.refresh(db_resource)
     return db_resource
 
 
 @router.get(
     "/{project_id}/{dataset_id}/resources/",
-    response_model=List[ResourceRead],
+    response_model=list[ResourceRead],
 )
 async def get_resource(
     project_id: int,
     dataset_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> Optional[List[ResourceRead]]:
+) -> Optional[list[ResourceRead]]:
     """
     Get resources from a dataset
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(Resource).where(Resource.dataset_id == dataset_id)
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.0a1/fractal_server/app/api/v1/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import logging
 from copy import deepcopy  # noqa
 from pathlib import Path
 from shutil import copy as shell_copy
 from shutil import rmtree as shell_rmtree
 from tempfile import TemporaryDirectory
-from typing import List
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import BackgroundTasks
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
@@ -129,17 +128,17 @@
         await db.commit()
 
         # Delete corrupted package dir
         shell_rmtree(venv_path)
 
 
 async def _insert_tasks(
-    task_list: List[TaskCreate],
+    task_list: list[TaskCreate],
     db: AsyncSession,
-) -> List[Task]:
+) -> list[Task]:
     """
     Insert tasks into database
     """
     task_db_list = [Task.from_orm(t) for t in task_list]
     db.add_all(task_db_list)
     await db.commit()
     await asyncio.gather(*[db.refresh(t) for t in task_db_list])
@@ -281,19 +280,19 @@
     # not set; if so, we collect the current logs
     if verbose and not data.log:
         data.log = get_collection_log(data.venv_path)
         state.data = data.sanitised_dict()
     return state
 
 
-@router.get("/", response_model=List[TaskRead])
+@router.get("/", response_model=list[TaskRead])
 async def get_list_task(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> List[TaskRead]:
+) -> list[TaskRead]:
     """
     Get list of available tasks
     """
     stm = select(Task)
     res = await db.execute(stm)
     task_list = res.scalars().unique().fetchall()
     await asyncio.gather(*[db.refresh(t) for t in task_list])
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.0a1/fractal_server/app/api/v1/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 import asyncio
 from copy import deepcopy
 from typing import Optional
-from typing import Tuple
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from pydantic import UUID4
@@ -84,15 +83,15 @@
 
 async def _get_workflow_task_check_owner(
     *,
     workflow_id: int,
     workflow_task_id: int,
     user_id: UUID4,
     db: AsyncSession = Depends(get_db),
-) -> Tuple[WorkflowTask, Workflow]:
+) -> tuple[WorkflowTask, Workflow]:
     """
     Check that user has rights to access a Workflow and a WorkflowTask and
     return the WorkflowTask
 
     Raises:
         HTTPException(status_code=404_NOT_FOUND): If the WorkflowTask does not
                                                   exist
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/db/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/job.py` & `fractal_server-1.2.0a1/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/project.py` & `fractal_server-1.2.0a1/fractal_server/app/models/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 
 from pydantic import UUID4
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
@@ -42,48 +39,48 @@
         resource_list:
             (Mapper attribute)
 
     """
 
     id: Optional[int] = Field(default=None, primary_key=True)
     project_id: int = Field(foreign_key="project.id")
-    resource_list: List["Resource"] = Relationship(
+    resource_list: list["Resource"] = Relationship(
         sa_relationship_kwargs={
             "lazy": "selectin",
             "cascade": "all, delete-orphan",
         }
     )
-    meta: Dict[str, Any] = Field(sa_column=Column(JSON), default={})
+    meta: dict[str, Any] = Field(sa_column=Column(JSON), default={})
 
     class Config:
         arbitrary_types_allowed = True
 
     @property
-    def paths(self) -> List[Path]:
+    def paths(self) -> list[str]:
         return [r.path for r in self.resource_list]
 
 
 class Project(_ProjectBase, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
 
-    user_member_list: List[User] = Relationship(
+    user_member_list: list[User] = Relationship(
         link_model=LinkUserProject,
         sa_relationship_kwargs={
             "lazy": "selectin",
         },
     )
 
-    dataset_list: List[Dataset] = Relationship(
+    dataset_list: list[Dataset] = Relationship(
         sa_relationship_kwargs={
             "lazy": "selectin",
             "cascade": "all, delete-orphan",
         }
     )
 
-    workflow_list: List[Workflow] = Relationship(
+    workflow_list: list[Workflow] = Relationship(
         sa_relationship_kwargs={
             "lazy": "selectin",
             "cascade": "all, delete-orphan",
         },
     )
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/security.py` & `fractal_server-1.2.0a1/fractal_server/app/models/security.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Adapted from
 https://github.com/fastapi-users/fastapi-users-db-sqlmodel/blob/main/tests/conftest.py
 """
 import uuid
-from typing import List
 from typing import Optional
 
 from fastapi_users_db_sqlmodel import SQLModelBaseOAuthAccount
 from fastapi_users_db_sqlmodel import SQLModelBaseUserDB
 from pydantic import UUID4
 from sqlalchemy_utils import UUIDType
 from sqlmodel import Column
@@ -20,15 +19,15 @@
     id: UUID4 = Field(
         default_factory=uuid.uuid4,
         nullable=False,
         sa_column=Column(UUIDType(), primary_key=True),
     )
     slurm_user: Optional[str]
     cache_dir: Optional[str]
-    oauth_accounts: List["OAuthAccount"] = Relationship(
+    oauth_accounts: list["OAuthAccount"] = Relationship(
         back_populates="user",
         sa_relationship_kwargs={"lazy": "selectin", "cascade": "all, delete"},
     )
 
 
 class OAuthAccount(SQLModelBaseOAuthAccount, table=True):
     user_id: UUID4 = Field(foreign_key="user_oauth.id", nullable=False)
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/state.py` & `fractal_server-1.2.0a1/fractal_server/app/models/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 from typing import Any
-from typing import Dict
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 
@@ -24,13 +23,13 @@
     Attributes:
         id: Primary key
         data: Content of the `State`
         timestamp: Timestap of the `State`
     """
 
     id: Optional[int] = Field(default=None, primary_key=True)
-    data: Dict[str, Any] = Field(sa_column=Column(JSON), default={})
+    data: dict[str, Any] = Field(sa_column=Column(JSON), default={})
     timestamp: datetime = Field(
         default_factory=get_timestamp,
         nullable=False,
         sa_column=Column(DateTime(timezone=True)),
     )
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/task.py` & `fractal_server-1.2.0a1/fractal_server/app/models/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Any
-from typing import Dict
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 
 from ...common.schemas.task import _TaskBase
 
 
-class Task(_TaskBase, table=True):  # type: ignore
+class Task(_TaskBase, table=True):
     """
     Task model
 
     Attributes:
         id: Primary key
         command: TBD
         input_type: TBD
@@ -24,29 +23,22 @@
         name: inherited from `_TaskBase`
     """
 
     id: Optional[int] = Field(default=None, primary_key=True)
     command: str
     input_type: str
     output_type: str
-    default_args: Optional[Dict[str, Any]] = Field(
+    default_args: Optional[dict[str, Any]] = Field(
         sa_column=Column(JSON), default={}
     )
-    meta: Optional[Dict[str, Any]] = Field(sa_column=Column(JSON), default={})
+    meta: Optional[dict[str, Any]] = Field(sa_column=Column(JSON), default={})
 
     @property
     def parallelization_level(self) -> Optional[str]:
         try:
             return self.meta["parallelization_level"]
         except KeyError:
             return None
 
     @property
     def is_parallel(self) -> bool:
         return bool(self.parallelization_level)
-
-    @property
-    def executor(self) -> Optional[str]:
-        try:
-            return self.meta["executor"]
-        except KeyError:
-            return None
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/models/workflow.py` & `fractal_server-1.2.0a1/fractal_server/app/models/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import validator
 from sqlalchemy import Column
 from sqlalchemy.ext.orderinglist import ordering_list
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
 
 from ...common.schemas.workflow import _WorkflowBase
 from ...common.schemas.workflow import _WorkflowTaskBase
-from ...config import get_settings
-from ...syringe import Inject
 from ..db import AsyncSession
 from .task import Task
 
 
 class WorkflowTask(_WorkflowTaskBase, table=True):
     """
     A Task as part of a Workflow
@@ -52,16 +48,16 @@
         fields = {"parent": {"exclude": True}}
 
     id: Optional[int] = Field(default=None, primary_key=True)
 
     workflow_id: Optional[int] = Field(foreign_key="workflow.id")
     task_id: Optional[int] = Field(foreign_key="task.id")
     order: Optional[int]
-    meta: Optional[Dict[str, Any]] = Field(sa_column=Column(JSON))
-    args: Optional[Dict[str, Any]] = Field(sa_column=Column(JSON))
+    meta: Optional[dict[str, Any]] = Field(sa_column=Column(JSON))
+    args: Optional[dict[str, Any]] = Field(sa_column=Column(JSON))
     task: Task = Relationship(sa_relationship_kwargs=dict(lazy="selectin"))
 
     @validator("args")
     def validate_args(cls, value: dict = None):
         """
         Prevent fractal task reserved parameter names from entering args
 
@@ -99,25 +95,24 @@
         return self.task.is_parallel
 
     @property
     def parallelization_level(self) -> Union[str, None]:
         return self.task.parallelization_level
 
     @property
-    def executor(self) -> str:
-        try:
-            return self.meta["executor"]  # type: ignore
-        except (KeyError, TypeError):
-            if self.task.executor:
-                return self.task.executor
-            else:
-                settings = Inject(get_settings)
-                return settings.FRACTAL_RUNNER_DEFAULT_EXECUTOR
+    def overridden_meta(self) -> dict:
+        """
+        Return a combination of self.meta (higher priority) and self.task.meta
+        (lower priority) key-value pairs.
+        """
+        res = self.task.meta.copy() or {}
+        res.update(self.meta or {})
+        return res
 
-    def assemble_args(self, extra: Dict[str, Any] = None) -> dict:
+    def assemble_args(self, extra: dict[str, Any] = None) -> dict:
         """
         Merge of `extra` arguments and `self.arguments`.
 
         Returns
             full_args:
                 A dictionary consisting of the merge of `extra` and
                 `self.arguments`.
@@ -141,29 +136,29 @@
         task_list:
             List of associations to tasks.
     """
 
     id: Optional[int] = Field(default=None, primary_key=True)
     project_id: int = Field(foreign_key="project.id")
 
-    task_list: List["WorkflowTask"] = Relationship(
+    task_list: list["WorkflowTask"] = Relationship(
         sa_relationship_kwargs=dict(
             lazy="selectin",
             order_by="WorkflowTask.order",
             collection_class=ordering_list("order"),
             cascade="all, delete-orphan",
         ),
     )
 
     async def insert_task(
         self,
         task_id: int,
         *,
-        args: Optional[Dict[str, Any]] = None,
-        meta: Optional[Dict[str, Any]] = None,
+        args: Optional[dict[str, Any]] = None,
+        meta: Optional[dict[str, Any]] = None,
         order: Optional[int] = None,
         db: AsyncSession,
         commit: bool = True,
     ) -> WorkflowTask:
         """
         Insert a new WorkflowTask into Workflow.task_list
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 This module is the single entry point to the runner backend subsystem. Other
 subystems should only import this module and not its submodules or the
 individual backends.
 """
 import logging
 import os
 from pathlib import Path
-from typing import Dict
 from typing import Optional
 
 from ... import __VERSION__
 from ...config import get_settings
 from ...syringe import Inject
 from ...utils import get_timestamp
 from ...utils import set_logger
@@ -37,15 +36,15 @@
 from .common import close_job_logger
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import validate_workflow_compatibility  # noqa: F401
 
 
 _backends = {}
-_backend_errors: Dict[str, Exception] = {}
+_backend_errors: dict[str, Exception] = {}
 
 _backends["local"] = local_process_workflow
 
 try:
     from ._slurm import process_workflow as slurm_process_workflow
 
     _backends["slurm"] = slurm_process_workflow
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_common.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/_common.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,42 +10,52 @@
 import subprocess  # nosec
 from concurrent.futures import Executor
 from concurrent.futures import Future
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
 from shlex import split as shlex_split
-from typing import Any
 from typing import Callable
-from typing import Dict
 from typing import Generator
-from typing import List
 from typing import Optional
 
 from ...config import get_settings
 from ...syringe import Inject
 from ..models import WorkflowTask
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import TaskParameters
 from .common import write_args_file
 
 
 METADATA_FILENAME = "metadata.json"
 
 
+def no_op_submit_setup_call(
+    *,
+    wftask: WorkflowTask,
+    workflow_dir: Path,
+    workflow_dir_user: Path,
+    task_pars: TaskParameters,
+) -> dict:
+    """
+    Default (no-operation) interface of submit_setup_call.
+    """
+    return {}
+
+
 def sanitize_component(value: str) -> str:
     """
     Remove {" ", "/", "."} form a string, e.g. going from
     'plate.zarr/B/03/0' to 'plate_zarr_B_03_0'.
     """
     return value.replace(" ", "_").replace("/", "_").replace(".", "_")
 
 
-def _get_list_chunks(mylist: List, *, chunksize: Optional[int]) -> Generator:
+def _get_list_chunks(mylist: list, *, chunksize: Optional[int]) -> Generator:
     """
     Split a list into several chunks of maximum size `chunksize`. If
     `chunksize` is `None`, return a single chunk with the whole list.
 
     Arguments:
         mylist: The list to be splitted
         chunksize: The maximum size of each chunk
@@ -105,16 +115,17 @@
         component: Optional[str] = None,
     ):
         self.workflow_dir = workflow_dir
         self.workflow_dir_user = workflow_dir_user
         self.task_order = task_order
         self.component = component
 
-        if self.component:
-            component_safe = f"_par_{sanitize_component(self.component)}"
+        if self.component is not None:
+            component_safe = sanitize_component(str(self.component))
+            component_safe = f"_par_{component_safe}"
         else:
             component_safe = ""
 
         if self.task_order is not None:
             order = str(self.task_order)
         else:
             order = "task"
@@ -181,15 +192,15 @@
         raise JobExecutionError(
             info=f"Task failed with returncode={result.returncode}"
         )
 
 
 def call_single_task(
     *,
-    task: WorkflowTask,
+    wftask: WorkflowTask,
     task_pars: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
 ) -> TaskParameters:
     """
     Call a single task
 
@@ -206,15 +217,15 @@
 
     If the executor then impersonates another user (as in the
     `FractalSlurmExecutor`), this function is run by that user.  For this
     reason, it should not write any file to workflow_dir, or it may yield
     permission errors.
 
     Args:
-        task:
+        wftask:
             The workflow task to be called. This includes task specific
             arguments via the task.task.arguments attribute.
         task_pars:
             The parameters required to run the task which are not specific to
             the task, e.g., I/O paths.
         workflow_dir:
             The server-side working directory for workflow execution.
@@ -235,52 +246,52 @@
                             order and name.
         JobExecutionError: If the wrapped task raises a job-related error.
         RuntimeError: If the `workflow_dir` is falsy.
     """
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
-    workflow_files = get_task_file_paths(
+    task_files = get_task_file_paths(
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
-        task_order=task.order,
+        task_order=wftask.order,
     )
 
     # assemble full args
-    args_dict = task.assemble_args(extra=task_pars.dict())
+    args_dict = wftask.assemble_args(extra=task_pars.dict())
 
     # write args file
-    write_args_file(args_dict, path=workflow_files.args)
+    write_args_file(args_dict, path=task_files.args)
 
     # assemble full command
     cmd = (
-        f"{task.task.command} -j {workflow_files.args} "
-        f"--metadata-out {workflow_files.metadiff}"
+        f"{wftask.task.command} -j {task_files.args} "
+        f"--metadata-out {task_files.metadiff}"
     )
 
     try:
         _call_command_wrapper(
-            cmd, stdout=workflow_files.out, stderr=workflow_files.err
+            cmd, stdout=task_files.out, stderr=task_files.err
         )
     except TaskExecutionError as e:
-        e.workflow_task_order = task.order
-        e.workflow_task_id = task.id
-        e.task_name = task.task.name
+        e.workflow_task_order = wftask.order
+        e.workflow_task_id = wftask.id
+        e.task_name = wftask.task.name
         raise e
 
     # NOTE:
     # This assumes that the new metadata is printed to stdout
     # and nothing else outputs to stdout
-    with workflow_files.metadiff.open("r") as f_metadiff:
+    with task_files.metadiff.open("r") as f_metadiff:
         diff_metadata = json.load(f_metadiff)
     updated_metadata = task_pars.metadata.copy()
     updated_metadata.update(diff_metadata)
 
     # Assemble a Future[TaskParameter]
-    history = f"{task.task.name}"
+    history = f"{wftask.task.name}"
     try:
         updated_metadata["history"].append(history)
     except KeyError:
         updated_metadata["history"] = [history]
 
     out_task_parameters = TaskParameters(
         input_paths=[task_pars.output_path],
@@ -290,15 +301,15 @@
 
     return out_task_parameters
 
 
 def call_single_parallel_task(
     component: str,
     *,
-    task: WorkflowTask,
+    wftask: WorkflowTask,
     task_pars: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
 ) -> None:
     """
     Call a single instance of a parallel task
 
@@ -314,15 +325,15 @@
 
         If the executor then impersonates another user (as in the
         `FractalSlurmExecutor`), this function is run by that user.
 
     Args:
         component:
             The parallelisation parameter.
-        task:
+        wftask:
             The task to execute.
         task_pars:
             The parameters to pass on to the task.
         workflow_dir:
             The server-side working directory for workflow execution.
         workflow_dir_user:
             The user-side working directory for workflow execution (only
@@ -337,79 +348,77 @@
         RuntimeError: If the `workflow_dir` is falsy.
     """
     if not workflow_dir:
         raise RuntimeError
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
-    workflow_files = get_task_file_paths(
+    task_files = get_task_file_paths(
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
-        task_order=task.order,
+        task_order=wftask.order,
         component=component,
     )
 
     # assemble full args
     write_args_file(
         task_pars.dict(),
-        task.arguments,
+        wftask.arguments,
         dict(component=component),
-        path=workflow_files.args,
+        path=task_files.args,
     )
 
     # assemble full command
     cmd = (
-        f"{task.task.command} -j {workflow_files.args} "
-        f"--metadata-out {workflow_files.metadiff}"
+        f"{wftask.task.command} -j {task_files.args} "
+        f"--metadata-out {task_files.metadiff}"
     )
 
     try:
         _call_command_wrapper(
-            cmd, stdout=workflow_files.out, stderr=workflow_files.err
+            cmd, stdout=task_files.out, stderr=task_files.err
         )
     except TaskExecutionError as e:
-        e.workflow_task_order = task.order
-        e.workflow_task_id = task.id
-        e.task_name = task.task.name
+        e.workflow_task_order = wftask.order
+        e.workflow_task_id = wftask.id
+        e.task_name = wftask.task.name
         raise e
 
 
 def call_parallel_task(
     *,
     executor: Executor,
-    task: WorkflowTask,
+    wftask: WorkflowTask,
     task_pars_depend: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
-    submit_setup_call: Callable[
-        [WorkflowTask, TaskParameters, Path, Path], Dict[str, Any]
-    ] = lambda task, task_pars, workflow_dir, workflow_dir_user: {},
+    submit_setup_call: Callable = no_op_submit_setup_call,
 ) -> Future:  # py3.9 Future[TaskParameters]:
     """
     Collect results from the parallel instances of a parallel task
 
     Prepare and submit for execution all the single calls of a parallel task,
     and return a single future with the TaskParameters to be passed on to the
     next task.  Note that the configuration variable
-    [`FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW`](../../../../../configuration/#fractal_server.config.Settings.FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW)
+    [`FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW`](../../../../../configuration/#fractal_server.config.Settings.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW)
     may affect the internal behavior of this function.
 
     **Note**: This function returns a future which already has
     `out_future.done()=True` (that is, this function is blocking and it
     returns only after the task is over). The reason for returning a future
     instead of a `TaskParameter` object is for compatibility with the output of
     `executor.submit(call_single_task, ...)`.
 
     Args:
         executor:
             The `concurrent.futures.Executor`-compatible executor that will
             run the task.
-        task:
+        wftask:
             The parallel task to run.
-        task_pars_depend_future:
+        task_pars_depend:
             The task parameters to be passed on to the parallel task.
         workflow_dir:
             The server-side working directory for workflow execution.
         workflow_dir_user:
             The user-side working directory for workflow execution (only
             relevant for multi-user executors).
         submit_setup_call:
@@ -421,52 +430,60 @@
             A future that resolves in the output task parameters of the
             parallel task execution, ready to be passed on to the next task.
     """
 
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
-    component_list = task_pars_depend.metadata[task.parallelization_level]
+    component_list = task_pars_depend.metadata[wftask.parallelization_level]
+
+    # Backend-specific configuration
+    extra_setup = submit_setup_call(
+        wftask=wftask,
+        task_pars=task_pars_depend,
+        workflow_dir=workflow_dir,
+        workflow_dir_user=workflow_dir_user,
+    )
 
     # Preliminary steps
     partial_call_task = partial(
         call_single_parallel_task,
-        task=task,
+        wftask=wftask,
         task_pars=task_pars_depend,
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
     )
-    extra_setup = submit_setup_call(
-        task, task_pars_depend, workflow_dir, workflow_dir_user
-    )
 
-    # Depending on FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW, either submit all
-    # tasks at once or in smaller chunks.  Note that `for _ in map_iter: pass`
-    # explicitly calls the .result() method for each future, and therefore is
-    # blocking until the task are complete.
+    # Depending on FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW, either submit
+    # all tasks at once or in smaller chunks.  Note that `for _ in map_iter:
+    # pass` explicitly calls the .result() method for each future, and
+    # therefore is blocking until the task are complete.
     settings = Inject(get_settings)
-    FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW = (
-        settings.FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW
-    )
+    max_parallel_tasks = None
+    if settings.FRACTAL_RUNNER_BACKEND == "local":
+        max_parallel_tasks = (
+            settings.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW
+        )
     # Prepare generator of component chunks (this is just a single item if
-    # FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW is None)
+    # FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW is None)
     component_chunks_generator = _get_list_chunks(
-        component_list, chunksize=FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW
+        component_list,
+        chunksize=max_parallel_tasks,
     )
     for component_chunk in component_chunks_generator:
         # Submit this chunk of tasks for execution
         map_iter = executor.map(
             partial_call_task, component_chunk, **extra_setup
         )
         # Wait for execution of this chunk of tasks
         for _ in map_iter:
             pass  # noqa: 701
 
     # Assemble a Future[TaskParameter]
-    history = f"{task.task.name}: {component_list}"
+    history = f"{wftask.task.name}: {component_list}"
     try:
         task_pars_depend.metadata["history"].append(history)
     except KeyError:
         task_pars_depend.metadata["history"] = [history]
 
     out_task_parameters = TaskParameters(
         input_paths=[task_pars_depend.output_path],
@@ -478,21 +495,19 @@
     out_future.set_result(out_task_parameters)
     return out_future
 
 
 def recursive_task_submission(
     *,
     executor: Executor,
-    task_list: List[WorkflowTask],
+    task_list: list[WorkflowTask],
     task_pars: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
-    submit_setup_call: Callable[
-        [WorkflowTask, TaskParameters, Path, Path], Dict[str, Any]
-    ] = lambda task, task_pars, workflow_dir, workflow_dir_user: {},
+    submit_setup_call: Callable = no_op_submit_setup_call,
     logger_name: str,
 ) -> Future:
     """
     Recursively submit a list of tasks
 
     This recursive function schedules a workflow task list in the correct
     order, making sure to resolve dependency before proceeding to the next
@@ -527,23 +542,23 @@
         submit_setup_call:
             An optional function that computes configuration parameters for
             the executor.
         logger_name:
             Name of the logger
 
     Returns:
-        this_task_future:
+        this_wftask_future:
             a future that results to the task parameters which constitute the
             input of the following task in the list.
     """
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
     try:
-        *dependencies, this_task = task_list
+        *dependencies, this_wftask = task_list
     except ValueError:
         # step 0: return future containing original task_pars
         pseudo_future: Future = Future()
         pseudo_future.set_result(task_pars)
         return pseudo_future
 
     logger = logging.getLogger(logger_name)
@@ -560,47 +575,48 @@
     )
     # Wait for dependencies to be complete (NOTE: this is not necessary if we
     # explicitly wait for the result of executor.submit(call_single_task, ...),
     # see below
     task_pars_depend = task_pars_depend_future.result()
 
     logger.info(
-        f"SUBMIT {this_task.order}-th task "
-        f'(name="{this_task.task.name}", executor={this_task.executor}).'
+        f'SUBMIT {this_wftask.order}-th task (name="{this_wftask.task.name}")'
     )
-    if this_task.is_parallel:
+    if this_wftask.is_parallel:
         # NOTE: call_parallel_task is blocking, i.e. the returned future always
-        # has `this_task_future.done() = True`
-        this_task_future = call_parallel_task(
+        # has `this_wftask_future.done() = True`
+        this_wftask_future = call_parallel_task(
             executor=executor,
-            task=this_task,
+            wftask=this_wftask,
             task_pars_depend=task_pars_depend,
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
             submit_setup_call=submit_setup_call,
         )
     else:
         # NOTE: executor.submit(call_single_task, ...) is non-blocking, i.e.
-        # the returned future may have `this_task_future.done() = False`
+        # the returned future may have `this_wftask_future.done() = False`
         extra_setup = submit_setup_call(
-            this_task, task_pars, workflow_dir, workflow_dir_user
+            wftask=this_wftask,
+            task_pars=task_pars,
+            workflow_dir=workflow_dir,
+            workflow_dir_user=workflow_dir_user,
         )
-        this_task_future = executor.submit(
+        this_wftask_future = executor.submit(
             call_single_task,
-            task=this_task,
+            wftask=this_wftask,
             task_pars=task_pars_depend,
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
             **extra_setup,
         )
         # Wait for the future result (blocking)
-        this_task_future.result()
+        this_wftask_future.result()
     logger.info(
-        f"END    {this_task.order}-th task "
-        f'(name="{this_task.task.name}", executor={this_task.executor}).'
+        f'END    {this_wftask.order}-th task (name="{this_wftask.task.name}")'
     )
 
     # Write most recent metadata to METADATA_FILENAME
     with open(workflow_dir / METADATA_FILENAME, "w") as f:
-        json.dump(this_task_future.result().metadata, f, indent=2)
+        json.dump(this_wftask_future.result().metadata, f, indent=2)
 
-    return this_task_future
+    return this_wftask_future
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/_local/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 [ThreadPoolExecutor](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor)
 to run tasks in several threads. Incidentally, it also represents the reference
 implementation for a backend.
 """
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 
 from ...models import Workflow
 from .._common import recursive_task_submission
 from ..common import async_wrap
 from ..common import TaskParameters
 
 
 def _process_workflow(
     *,
     workflow: Workflow,
-    input_paths: List[Path],
+    input_paths: list[Path],
     output_path: Path,
-    input_metadata: Dict[str, Any],
+    input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Internal processing routine
 
     Schedules the workflow using a ThreadPoolExecutor.
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
     for the call signature.
@@ -54,23 +52,23 @@
     output_dataset_metadata = output_task_pars.metadata
     return output_dataset_metadata
 
 
 async def process_workflow(
     *,
     workflow: Workflow,
-    input_paths: List[Path],
+    input_paths: list[Path],
     output_path: Path,
-    input_metadata: Dict[str, Any],
+    input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     slurm_user: Optional[str] = None,
     worker_init: Optional[str] = None,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Run a workflow
 
     This function is responsible for running a workflow on some input data,
     saving the output and taking care of any exception raised during the run.
 
     NOTE: This is the `local` backend's public interface, which also works as
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,295 +1,323 @@
-# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
-# University of Zurich
-#
-# Original authors:
-# Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
-# Tommaso Comparin <tommaso.comparin@exact-lab.it>
-#
-# This file is part of Fractal and was originally developed by eXact lab S.r.l.
-# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
-# Institute for Biomedical Research and Pelkmans Lab from the University of
-# Zurich.
 """
-Slurm Bakend
+Common utilities and routines for runner backends (public API)
 
-This backend runs fractal workflows in a SLURM cluster using Clusterfutures
-Executor objects.
+This module includes utilities and routines that are of use to implement
+runner backends but that should also be exposed to the other components of
+`Fractal Server`.
 """
+import asyncio
 import json
+import os
+from functools import partial
+from functools import wraps
+from json import JSONEncoder
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
+from typing import Callable
 from typing import Optional
-from typing import Union
 
 from pydantic import BaseModel
-from pydantic import Field
 
-from ....config import get_settings
-from ....syringe import Inject
-from ...models import Workflow
-from ...models import WorkflowTask
-from .._common import get_task_file_paths
-from .._common import recursive_task_submission
-from ..common import async_wrap
-from ..common import TaskParameters
-from .executor import FractalSlurmExecutor
+from ...utils import close_logger as close_job_logger  # noqa F401
+from ..models import Dataset
+from ..models import Project
+from ..models.workflow import Workflow
 
 
-class SlurmConfig(BaseModel):
+class TaskExecutionError(RuntimeError):
     """
-    Abstraction for SLURM executor parameters
+    Forwards errors occurred during the execution of a task
 
-    This class wraps options for the `sbatch` command. Attribute `xxx` maps to
-    the `--xxx` option of `sbatch`.
-    Cf. [sbatch documentation](https://slurm.schedmd.com/sbatch.html)
-
-    Note that options containing hyphens ('-') need be aliased to attribute
-    names with underscores ('-').
+    This error wraps and forwards errors occurred during the execution of
+    tasks, when the exit code is larger than 0 (i.e. the error took place
+    within the task). This error also adds information that is useful to track
+    down and debug the failing task within a workflow.
 
     Attributes:
-        partition: TBD
-        time: TBD
-        mem: TBD
-        cpus_per_task: TBD
-        account: TBD
-        extra_lines: TBD
-    """
+        workflow_task_id:
+            ID of the workflow task that failed.
+        workflow_task_order:
+            Order of the task within the workflow.
+        task_name:
+            Human readable name of the failing task.
+    """
+
+    workflow_task_id: Optional[int] = None
+    workflow_task_order: Optional[int] = None
+    task_name: Optional[str] = None
+
+    def __init__(
+        self,
+        *args,
+        workflow_task_id: Optional[int] = None,
+        workflow_task_order: Optional[int] = None,
+        task_name: Optional[str] = None,
+    ):
+        super().__init__(*args)
+        self.workflow_task_id = workflow_task_id
+        self.workflow_task_order = workflow_task_order
+        self.task_name = task_name
+
+
+class JobExecutionError(RuntimeError):
+    """
+    Forwards errors in the execution of a task that are due to external factors
+
+    This error wraps and forwards errors occurred during the execution of
+    tasks, but related to external factors like:
+
+    1. A negative exit code (e.g. because the task received a TERM or KILL
+       signal);
+    2. An error on the executor side (e.g. the SLURM executor could not
+       find the pickled file with task output).
 
-    class Config:
-        allow_population_by_field_name = True
+    This error also adds information that is useful to track down and debug the
+    failing task within a workflow.
 
-    partition: str
-    time: Optional[str]
-    mem: Optional[str]
-    cpus_per_task: Optional[str] = Field(alias="cpus-per-task")
-    account: Optional[str]
-    extra_lines: Optional[List[str]] = Field(default_factory=list)
+    Attributes:
+        info:
+            A free field for additional information
+        cmd_file:
+            Path to the file of the command that was executed (e.g. a SLURM
+            submission script).
+        stdout_file:
+            Path to the file with the command stdout
+        stderr_file:
+            Path to the file with the command stderr
+    """
+
+    cmd_file: Optional[str] = None
+    stdout_file: Optional[str] = None
+    stderr_file: Optional[str] = None
+    info: Optional[str] = None
+
+    def __init__(
+        self,
+        *args,
+        cmd_file: Optional[str] = None,
+        stdout_file: Optional[str] = None,
+        stderr_file: Optional[str] = None,
+        info: Optional[str] = None,
+    ):
+        super().__init__(*args)
+        self.cmd_file = cmd_file
+        self.stdout_file = stdout_file
+        self.stderr_file = stderr_file
+        self.info = info
 
-    def to_sbatch(self, prefix="#SBATCH "):
+    def _read_file(self, filepath: str) -> str:
         """
-        Transform the class attributes into the preamble block of a script to
-        be submitted via `sbatch`
+        Return the content of a text file, and handle the cases where it is
+        empty or missing
         """
-        dic = self.dict(
-            exclude_none=True, by_alias=True, exclude={"extra_lines"}
-        )
-        sbatch_lines = []
-        for k, v in dic.items():
-            sbatch_lines.append(f"{prefix}--{k}={v}")
-        sbatch_lines.extend(self.extra_lines)
-        return sbatch_lines
+        if os.path.exists(filepath):
+            with open(filepath, "r") as f:
+                content = f.read()
+                if content:
+                    return f"Content of {filepath}:\n{content}"
+                else:
+                    return f"File {filepath} is empty\n"
+        else:
+            return f"File {filepath} is missing\n"
+
+    def assemble_error(self) -> str:
+        """
+        Read the files that are specified in attributes, and combine them in an
+        error message.
+        """
+        if self.cmd_file:
+            content = self._read_file(self.cmd_file)
+            cmd_content = f"COMMAND:\n{content}\n\n"
+        else:
+            cmd_content = ""
+        if self.stdout_file:
+            content = self._read_file(self.stdout_file)
+            out_content = f"STDOUT:\n{content}\n\n"
+        else:
+            out_content = ""
+        if self.stderr_file:
+            content = self._read_file(self.stderr_file)
+            err_content = f"STDERR:\n{content}\n\n"
+        else:
+            err_content = ""
+
+        content = f"{cmd_content}{out_content}{err_content}"
+        if self.info:
+            content = f"{content}ADDITIONAL INFO:\n{self.info}\n\n"
 
+        if not content:
+            content = str(self)
+        message = f"JobExecutionError\n\n{content}"
+        return message
 
-class SlurmConfigError(ValueError):
+
+class TaskParameterEncoder(JSONEncoder):
     """
-    Slurm configuration error
+    Convenience JSONEncoder that serialises `Path`s as strings
     """
 
-    pass
+    def default(self, value):
+        if isinstance(value, Path):
+            return value.as_posix()
+        return JSONEncoder.default(self, value)
 
 
-def load_slurm_config(
-    config_path: Optional[Path] = None,
-) -> Dict[str, SlurmConfig]:
+class TaskParameters(BaseModel):
     """
-    Parse slurm configuration file
+    Wrapper for task input parameters
 
-    The configuration file can contain multiple SLURM configurations in JSON
-    format. This functions deserialises all the configurations and returns
-    them in the form of SlurmConfig objects.
+    Instances of this class are used to pass parameters from the output of a
+    task to the input of the next one.
 
-    Args:
-        config_path:
-            The path to the configuration file. If not provided, it is read
-            from Fractal settings.
+    Attributes:
+        input_paths:
+            Input paths as derived by the input dataset.
+        output_paths:
+            Output path as derived from the output dataset.
+        metadata:
+            Dataset metadata, as found in the input dataset or as updated by
+            the previous task.
+    """
 
-    Raises:
-        SlurmConfigError: if any exeception was raised in reading or
-                          deserialising the configuration file.
+    input_paths: list[Path]
+    output_path: Path
+    metadata: dict[str, Any]
 
-    Returns:
-        config_dict:
-            Dictionary whose keys are the configuration identifiers and whose
-            values are SlurmConfig objects.
-    """
-    if not config_path:
-        settings = Inject(get_settings)
-        config_path = settings.FRACTAL_SLURM_CONFIG_FILE
-    try:
-        with config_path.open("r") as f:  # type: ignore
-            raw_data = json.load(f)
-
-        # coerce
-        config_dict = {
-            config_key: SlurmConfig(**raw_data[config_key])
-            for config_key in raw_data
-        }
-    except FileNotFoundError:
-        raise SlurmConfigError(f"Configuration file not found: {config_path}")
-    except Exception as e:
-        raise SlurmConfigError(
-            f"Could not read slurm configuration file: {config_path}"
-            f"\nOriginal error: {repr(e)}"
-        )
-    return config_dict
+    class Config:
+        arbitrary_types_allowed = True
+        extra = "forbid"
 
 
-def set_slurm_config(
-    task: WorkflowTask,
-    task_pars: TaskParameters,
-    workflow_dir: Path,
-    workflow_dir_user: Path,
-) -> Dict[str, Any]:
+async def auto_output_dataset(
+    *,
+    project: Project,
+    input_dataset: Dataset,
+    workflow: Workflow,
+    overwrite_input: bool = False,
+) -> Dataset:
     """
-    Collect SLURM configuration parameters
+    Determine the output dataset if it was not provided explicitly
 
-    Inject SLURM configuration for single task execution.
+    Only datasets containing exactly one path can be used as output.
 
-    For now, this is the reference implementation for argument
-    `submit_setup_call` of
-    [fractal_server.app.runner._common.recursive_task_submission][]
+    Note: This routine is still a stub.
 
     Args:
-        task:
-            Task for which the sbatch script is to be assembled
-        task_pars:
-            Task parameters to be passed to the task
-        workflow_dir:
-            Server-owned directory to store all task-execution-related relevant
-            files (inputs, outputs, errors, and all meta files related to the
-            job execution). Note: users cannot write directly to this folder.
-        workflow_dir_user:
-            User-side directory with the same scope as `workflow_dir`, and
-            where a user can write.
+        project:
+            The project that contains the input and output datasets.
+        input_dataset:
+            The input dataset.
+        workflow:
+            The workflow to be applied to the input dataset.
+        overwrite_input:
+            Whether it is allowed to overwrite the input dataset with the
+            output data.
 
     Raises:
-        SlurmConfigError: if the slurm-configuration file does not contain the
-                          required config
+        ValueError: If the input dataset is to be overwritten and it provides
+                    more than one path.
 
     Returns:
-        submit_setup_dict:
-            A dictionary that will be passed on to
-            `FractalSlurmExecutor.submit` and `FractalSlurmExecutor.map`, so
-            as to set extra options in the sbatch script.
-    """
-    config_dict = load_slurm_config()
-    try:
-        config = config_dict[task.executor]
-    except KeyError:
-        raise SlurmConfigError(f"Configuration not found: {task.executor}")
-
-    additional_setup_lines = config.to_sbatch()
-    additional_setup_lines.append(
-        f"#SBATCH --job-name {task.task.name.replace(' ', '_')}"
-    )
-
-    # From https://slurm.schedmd.com/sbatch.html: Beginning with 22.05, srun
-    # will not inherit the --cpus-per-task value requested by salloc or sbatch.
-    # It must be requested again with the call to srun or set with the
-    # SRUN_CPUS_PER_TASK environment variable if desired for the task(s).
-    if config.cpus_per_task:
-        additional_setup_lines.append(
-            f"export SRUN_CPUS_PER_TASK={config.cpus_per_task}"
+        output_dataset:
+            the output dataset
+    """
+    if overwrite_input and not input_dataset.read_only:
+        input_paths = input_dataset.paths
+        if len(input_paths) != 1:
+            raise ValueError(
+                "Cannot determine output dataset "
+                "with more than one input path."
+            )
+        output_dataset = input_dataset
+    else:
+        raise NotImplementedError(
+            "Cannot determine ouput dataset with "
+            f"{overwrite_input=} and {input_dataset.read_only=}"
         )
 
-    task_files = get_task_file_paths(
-        workflow_dir=workflow_dir,
-        workflow_dir_user=workflow_dir_user,
-        task_order=task.order,
-    )
-    return dict(
-        additional_setup_lines=additional_setup_lines,
-        job_file_prefix=task_files.file_prefix,
-    )
+    return output_dataset
 
 
-def _process_workflow(
+def validate_workflow_compatibility(
     *,
+    input_dataset: Dataset,
     workflow: Workflow,
-    input_paths: List[Path],
-    output_path: Path,
-    input_metadata: Dict[str, Any],
-    logger_name: str,
-    workflow_dir: Path,
-    workflow_dir_user: Path,
-    slurm_user: Optional[str] = None,
-    worker_init: Optional[Union[str, List[str]]] = None,
-) -> Dict[str, Any]:
-    """
-    Internal processing routine for the SLURM backend
-
-    This function initialises the a FractalSlurmExecutor, setting logging,
-    workflow working dir and user to impersonate. It then schedules the
-    workflow tasks and returns the output dataset metadata.
+    output_dataset: Optional[Dataset] = None,
+):
+    """
+    Check compatibility of workflow and input / ouptut dataset
+    """
+    if (
+        workflow.input_type != "Any"
+        and workflow.input_type != input_dataset.type
+    ):
+        raise TypeError(
+            f"Incompatible types `{workflow.input_type}` of workflow "
+            f"`{workflow.name}` and `{input_dataset.type}` of dataset "
+            f"`{input_dataset.name}`"
+        )
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    if not output_dataset:
+        if input_dataset.read_only:
+            raise ValueError("Input dataset is read-only")
+        else:
+            input_paths = input_dataset.paths
+            if len(input_paths) != 1:
+                # Only single input can be safely transformed in an output
+                raise ValueError(
+                    "Cannot determine output path: multiple input "
+                    "paths to overwrite"
+                )
+            else:
+                output_path = input_paths[0]
+    else:
+
+        if len(output_dataset.paths) != 1:
+            raise ValueError(
+                "Cannot determine output path: Multiple paths in dataset."
+            )
+        else:
+            output_path = output_dataset.paths[0]
+    return output_path
 
-    Returns:
-        output_dataset_metadata: Metadata of the output dataset
+
+def async_wrap(func: Callable) -> Callable:
     """
+    Wrap a synchronous callable in an async task
 
-    if not slurm_user:
-        raise RuntimeError(
-            "slurm_user argument is required, for slurm backend"
-        )
+    Ref: [issue #140](https://github.com/fractal-analytics-platform/fractal-server/issues/140)
+    and [this StackOverflow answer](https://stackoverflow.com/q/43241221/19085332).
 
-    if isinstance(worker_init, str):
-        worker_init = worker_init.split("\n")
+    Returns:
+        async_wrapper:
+            A factory that allows wrapping a blocking callable within a
+            coroutine.
+    """  # noqa: E501
 
-    with FractalSlurmExecutor(
-        debug=True,
-        keep_logs=True,
-        slurm_user=slurm_user,
-        working_dir=workflow_dir,
-        working_dir_user=workflow_dir_user,
-        common_script_lines=worker_init,
-    ) as executor:
-        output_task_pars_fut = recursive_task_submission(
-            executor=executor,
-            task_list=workflow.task_list,
-            task_pars=TaskParameters(
-                input_paths=input_paths,
-                output_path=output_path,
-                metadata=input_metadata,
-            ),
-            workflow_dir=workflow_dir,
-            workflow_dir_user=workflow_dir_user,
-            submit_setup_call=set_slurm_config,
-            logger_name=logger_name,
-        )
-    output_task_pars = output_task_pars_fut.result()
-    output_dataset_metadata = output_task_pars.metadata
-    return output_dataset_metadata
+    @wraps(func)
+    async def async_wrapper(*args, loop=None, executor=None, **kwargs):
+        if loop is None:
+            loop = asyncio.get_event_loop()
+        pfunc = partial(func, *args, **kwargs)
+        return await loop.run_in_executor(executor, pfunc)
 
+    return async_wrapper
 
-async def process_workflow(
-    *,
-    workflow: Workflow,
-    input_paths: List[Path],
-    output_path: Path,
-    input_metadata: Dict[str, Any],
-    logger_name: str,
-    workflow_dir: Path,
-    workflow_dir_user: Optional[Path] = None,
-    slurm_user: Optional[str] = None,
-    worker_init: Optional[str] = None,
-) -> Dict[str, Any]:
-    """
-    Process workflow (SLURM backend public interface)
-
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
-    """
-    output_dataset_metadata = await async_wrap(_process_workflow)(
-        workflow=workflow,
-        input_paths=input_paths,
-        output_path=output_path,
-        input_metadata=input_metadata,
-        logger_name=logger_name,
-        workflow_dir=workflow_dir,
-        workflow_dir_user=workflow_dir_user,
-        slurm_user=slurm_user,
-        worker_init=worker_init,
-    )
-    return output_dataset_metadata
+
+def write_args_file(*args: dict[str, Any], path: Path):
+    """
+    Merge arbitrary dictionaries and write to file
+
+    Args:
+        *args:
+            One or more dictionaries that will be merged into one respecting
+            the order with which they are passed in, i.e., last in overrides
+            previous ones.
+        path:
+            Destination for serialised file.
+    """
+    out = {}
+    for d in args:
+        out.update(d)
+    with open(path, "w") as f:
+        json.dump(out, f, cls=TaskParameterEncoder, indent=4)
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 This module provides a set of tools similar to `subprocess.run`, `glob.glob` or
 `os.path.exists`, but extended so that they can be executed on behalf of
 another user. Note that this requires appropriate sudo permissions.
 """
 import logging
 import shlex
 import subprocess  # nosec
-from typing import List
 from typing import Optional
+from typing import Sequence
 
 
 def _run_command_as_user(
     *,
     cmd: str,
     user: Optional[str] = None,
-    encoding: str = "utf-8",
+    encoding: Optional[str] = "utf-8",
     check: bool = False,
 ) -> subprocess.CompletedProcess:
     """
     Use `sudo -u` to impersonate another user and run a command
 
     Arguments:
         cmd: Command to be run
@@ -87,15 +87,15 @@
 
     cmd = f"mkdir -p {folder}"
     _run_command_as_user(cmd=cmd, user=user, check=True)
 
 
 def _glob_as_user(
     *, folder: str, user: str, startswith: Optional[str] = None
-) -> List[str]:
+) -> list[str]:
     """
     Run `ls` in a folder (as a user) and filter results
 
     Execute `ls` on a folder (impersonating a user, if `user` is not `None`)
     and select results that start with `startswith` (if not `None`).
 
     Arguments:
@@ -109,18 +109,38 @@
     if startswith:
         output = [f for f in output if f.startswith(startswith)]
     return output
 
 
 def _path_exists_as_user(*, path: str, user: Optional[str] = None) -> bool:
     """
-    Impersonate a user and check if `filepath` exists via `ls`
+    Impersonate a user and check if `path` exists via `ls`
 
     Arguments:
         path: Absolute file/folder path
         user: If not `None`, user to be impersonated
     """
     res = _run_command_as_user(cmd=f"ls {path}", user=user)
     if res.returncode == 0:
         return True
     else:
         return False
+
+
+def _multiple_paths_exist_as_user(
+    *,
+    paths: Sequence[str],
+    user: Optional[str] = None,
+) -> bool:
+    """
+    Impersonate a user and check if some paths exists via `ls`
+
+    Arguments:
+        paths: Absolute file/folder path
+        user: If not `None`, user to be impersonated
+    """
+    paths_string = " ".join(paths)
+    res = _run_command_as_user(cmd=f"ls {paths_string}", user=user)
+    if res.returncode == 0:
+        return True
+    else:
+        return False
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,16 @@
 This module provides a simple self-standing script that executes arbitrary
 python code received via pickled files on a cluster node.
 """
 import argparse
 import logging
 import os
 import sys
-from typing import Dict
-from typing import List
 from typing import Literal
 from typing import Optional
-from typing import Tuple
 from typing import Type
 from typing import Union
 
 import cloudpickle
 
 from fractal_server import __VERSION__
 
@@ -42,34 +39,34 @@
         exc_type_name: Name of the exception type
         tb: TBD
         args: TBD
         kwargs: TBD
     """
 
     def __init__(
-        self, exc_type: Type[BaseException], tb: List[str], *args, **kwargs
+        self, exc_type: Type[BaseException], tb: str, *args, **kwargs
     ):
         self.exc_type_name: str = exc_type.__name__
-        self.tb: List[str] = tb
+        self.tb: str = tb
         self.args = args
-        self.kwargs: Dict = kwargs
+        self.kwargs: dict = kwargs
 
 
 class FractalVersionMismatch(RuntimeError):
     """
     Custom exception for version mismatch
     """
 
     pass
 
 
 def _check_versions_mismatch(
-    server_versions: Dict[
+    server_versions: dict[
         Literal["python", "fractal_server", "cloudpickle"],
-        Union[str, Tuple[int]],
+        Union[str, tuple[int]],
     ]
 ):
     """
     Compare the server {python,cloudpickle,fractal_server} versions with the
     ones available to the current worker
 
     Arguments:
@@ -85,15 +82,15 @@
     server_python_version = server_versions["python"]
     worker_python_version = sys.version_info[:3]
     if worker_python_version != server_python_version:
         # FIXME: turn this into an error, after fixing a broader CI issue, see
         # https://github.com/fractal-analytics-platform/fractal-server/issues/375
         logging.critical(
             f"{server_python_version=} but {worker_python_version=}. "
-            "Note that cloudpickle is not guaranteed to correctly load "
+            "cloudpickle is not guaranteed to correctly load "
             "pickle files created with different python versions. "
             "Note, however, that if you reached this line it means that "
             "the pickle file was likely loaded correctly."
         )
 
     server_cloudpickle_version = server_versions["cloudpickle"]
     worker_cloudpickle_version = cloudpickle.__version__
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/runner/_slurm/wait_thread.py` & `fractal_server-1.2.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,90 @@
-import logging
 import traceback
 
 from cfut import FileWaitThread
 from cfut import slurm
 
-from ._subprocess_run_as_user import _path_exists_as_user
+from ._subprocess_run_as_user import _multiple_paths_exist_as_user
 
 
 class FractalFileWaitThread(FileWaitThread):
     """
-    Overrides the original clusterfutures.FileWaitThread, so that the
-    file-existence check can be replaced with the custom `_does_file_exist`
-    method.
+    Overrides the original clusterfutures.FileWaitThread, so that:
+
+    1. Each jobid in the waiting list is associated to a tuple of filenames,
+       rather than a single one.
+    2. The file-existence check can be replaced with the custom
+       `_does_file_exist` method. This also requires a `slurm_user` attribute.
 
     The function is copied from clusterfutures 0.5. Original Copyright: 2022
     Adrian Sampson, released under the MIT licence
 
     Note: in principle we could avoid the definition of
     `FractalFileWaitThread`, and pack all this code in
     `FractalSlurmWaitThread`.
     """
 
     def __init__(self, *args, **kwargs):
+        """
+        Changed from clusterfutures:
+        * Additional attribute `slurm_user`
+        """
+
         super().__init__(*args, **kwargs)
         self.slurm_user: str
 
+    def wait(
+        self,
+        *,
+        filenames: tuple[str, ...],
+        jobid: str,
+    ):
+        """
+        Add a a new job (filenames and callback value, that is, SLURM job ID)
+        to the set of files being waited upon.
+
+        Changed from clusterfutures:
+        * Replaced `filename` with `filenames`
+        """
+        with self.lock:
+            self.waiting[filenames] = jobid
+
     def check(self, i):
         """
         Do one check for completed jobs
 
-        The `i` parameter allows subclasses like `SlurmWaitThread` to do
+        Note: the `i` parameter allows subclasses like `SlurmWaitThread` to do
         something on every Nth check.
+
+        Changed from clusterfutures:
+        * Check file exitence via `_path_exists_as_user` instead of using `os`.
+        * For each item in `self.waiting`, check simultaneous existence of
+          multiple files.
         """
         # Poll for each file.
-        for filename in list(self.waiting):
-            if _path_exists_as_user(path=filename, user=self.slurm_user):
-                logging.info(
-                    f"[FractalFileWaitThread.check] {filename} exists"
-                )
-                self.callback(self.waiting[filename])
-                del self.waiting[filename]
+        for filenames in list(self.waiting):
+            all_files_exist = _multiple_paths_exist_as_user(
+                paths=filenames, user=self.slurm_user
+            )
+            if all_files_exist:
+                self.callback(self.waiting[filenames])
+                del self.waiting[filenames]
 
 
 class FractalSlurmWaitThread(FractalFileWaitThread):
     """
     Replaces the original clusterfutures.SlurmWaitThread, to inherit from
     FractalFileWaitThread instead of FileWaitThread.
 
     The function is copied from clusterfutures 0.5. Original Copyright: 2022
     Adrian Sampson, released under the MIT licence
+
+
+    Changed from clusterfutures:
+    * Rename `id_to_filename` to `id_to_filenames`
     """
 
     slurm_poll_interval = 30
 
     def check(self, i):
         super().check(i)
         if i % (self.slurm_poll_interval // self.interval) == 0:
@@ -62,11 +94,11 @@
                 # Don't abandon completion checking if jobs_finished errors
                 traceback.print_exc()
                 return
 
             if not finished_jobs:
                 return
 
-            id_to_filename = {v: k for (k, v) in self.waiting.items()}
+            id_to_filenames = {v: k for (k, v) in self.waiting.items()}
             for finished_id in finished_jobs:
                 self.callback(finished_id)
-                self.waiting.pop(id_to_filename[finished_id])
+                self.waiting.pop(id_to_filenames[finished_id])
```

### Comparing `fractal_server-1.2.0a0/fractal_server/app/security/__init__.py` & `fractal_server-1.2.0a1/fractal_server/app/security/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 Then, for each OAuth client defined in the Fractal Settings configuration, it
 registers the client and the relative routes.
 
 All routes are registerd under the `auth/` prefix.
 """
 import uuid
 from typing import AsyncGenerator
-from typing import List
 from typing import Optional
 from typing import Union
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import status
@@ -159,15 +158,15 @@
 ):
     """
     Return current user
     """
     return user
 
 
-@auth_router.get("/userlist", response_model=List[UserRead])
+@auth_router.get("/userlist", response_model=list[UserRead])
 async def list_users(
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_db),
 ):
     """
     Return list of all users
     """
```

### Comparing `fractal_server-1.2.0a0/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.0a1/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.0a1/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/README.md` & `fractal_server-1.2.0a1/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/project.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/state.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/task.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/user.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.0a1/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.0a1/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/config.py` & `fractal_server-1.2.0a1/fractal_server/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # Tommaso Comparin <tommaso.comparin@exact-lab.it>
 # Marco Franzon <marco.franzon@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
+import logging
 import shutil
 from os import environ
 from os import getenv
 from os.path import abspath
 from pathlib import Path
-from typing import List
 from typing import Literal
 from typing import Optional
 from typing import TypeVar
 
 from dotenv import load_dotenv
 from pydantic import BaseModel
 from pydantic import BaseSettings
@@ -95,15 +95,15 @@
     production deployments be marked as such to trigger server hardening.
     """
 
     ###########################################################################
     # AUTH
     ###########################################################################
 
-    OAUTH_CLIENTS: List[OAuthClient] = Field(default_factory=list)
+    OAUTH_CLIENTS: list[OAuthClient] = Field(default_factory=list)
 
     # JWT TOKEN
     JWT_EXPIRE_SECONDS: int = 180
     JWT_SECRET_KEY: Optional[str]
 
     # COOKIE TOKEN
     COOKIE_EXPIRE_SECONDS: int = 86400
@@ -241,33 +241,26 @@
     FRACTAL_LOGGING_LEVEL: int = 30
     """
     Logging verbosity for main Fractal logger (`30` means `WARNING` - see
     [logging
     levels](https://docs.python.org/3/library/logging.html#logging-levels)).
     """
 
-    FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW: Optional[int] = None
+    FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW: Optional[int] = None
     """
     Maximum number of components that a parallel task may process
-    simultaneously. If `None`, no limit is set.
+    simultaneously, for the [local backend](../internals/runners/local/).  If
+    `None`, no limit is set.
+
+    Intended use case: Reduce memory requirements of a workflow by capping the
+    number of tasks running in parallel.
 
     Note: this limit concerns a single task in a single workflow execution, but
     it does **not** limit the global (i.e. across workflow executions) number
     of components processed simultaneously.
-
-    Intended use cases:
-
-    1. When using the [local backend](../internals/runners/local/), reduce
-    memory requirements of a workflow by capping the number of tasks running in
-    parallel.
-    2. When using the [SLURM backend](../internals/runners/slurm/), reduce the
-    number of SLURM jobs that are submitted at the same time for a given
-    workflow; this is e.g. to avoid `AssocMaxSubmitJobLimit` errors related to
-    the [`MaxSubmitJobs` SLURM
-    limit](https://slurm.schedmd.com/resource_limits.html#assoc).
     """
 
     FRACTAL_SLURM_CONFIG_FILE: Optional[Path]
     """
     Path of JSON file with configuration for the SLURM backend.
     """
 
@@ -344,35 +337,57 @@
             FRACTAL_RUNNER_BACKEND: str = Field()
             if FRACTAL_RUNNER_BACKEND == "slurm":
                 FRACTAL_SLURM_CONFIG_FILE: Path
 
         StrictSettings(**self.dict())
 
         # Check that some variables are allowed
-        if isinstance(self.FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW, int):
-            if self.FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW < 1:
+        if isinstance(self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW, int):
+            if self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW < 1:
                 raise FractalConfigurationError(
-                    f"{self.FRACTAL_RUNNER_MAX_TASKS_PER_WORKFLOW=} "
+                    f"{self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW=} "
                     "not allowed"
                 )
 
+        if (
+            self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW
+            and self.FRACTAL_RUNNER_BACKEND != "local"
+        ):
+            logging.warning(
+                "FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW is set to "
+                f"{self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW}, but "
+                f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND} is "
+                "the local backend."
+            )
+
         if self.FRACTAL_RUNNER_BACKEND == "slurm":
             info = f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND}"
 
             # Check that FRACTAL_SLURM_CONFIG_FILE exists
             if not self.FRACTAL_SLURM_CONFIG_FILE.exists():
                 raise FractalConfigurationError(
                     f"{info} but {str(self.FRACTAL_SLURM_CONFIG_FILE)} "
                     "is missing"
                 )
+
+            # Check that FRACTAL_SLURM_CONFIG_FILE content is valid
+            from fractal_server.app.runnner._slurm._slurm_config import (
+                load_slurm_config_file,
+            )
+
+            _ = load_slurm_config_file(
+                config_path=self.FRACTAL_SLURM_CONFIG_FILE
+            )
+
             # Check that sbatch command is available
             if not shutil.which("sbatch"):
                 raise FractalConfigurationError(
                     f"{info} but sbatch command not found."
                 )
+
             # Check that squeue command is available
             if not shutil.which("squeue"):
                 raise FractalConfigurationError(
                     f"{info} but squeue command not found."
                 )
```

### Comparing `fractal_server-1.2.0a0/fractal_server/main.py` & `fractal_server-1.2.0a1/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/migrations/env.py` & `fractal_server-1.2.0a1/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.0a1/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.0a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.0a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.0a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/fractal_server/syringe.py` & `fractal_server-1.2.0a1/fractal_server/syringe.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     24
     >>> Inject.pop(foo)
     >>> bar()
     42
 """
 from typing import Any
 from typing import Callable
-from typing import Dict
 from typing import TypeVar
 
 
 T = TypeVar("T")
 _instance_count = 0
 
 
@@ -51,15 +50,15 @@
     This is a private class that is never directly instantiated.
 
     Attributes:
         _dependencies:
             The dependency directory
     """
 
-    _dependencies: Dict[Any, Any] = {}
+    _dependencies: dict[Any, Any] = {}
 
     def __init__(self):
         global _instance_count
         if _instance_count == 1:
             raise RuntimeError("You must only instance this class once")
         _instance_count += 1
```

### Comparing `fractal_server-1.2.0a0/fractal_server/tasks/collection.py` & `fractal_server-1.2.0a1/fractal_server/tasks/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 """
 import json
 import logging
 import shutil
 import sys
 from io import IOBase
 from pathlib import Path
-from typing import List
 from typing import Optional
-from typing import Tuple
 from typing import Union
 from zipfile import ZipFile
 
 from pydantic import root_validator
 
 from ..common.schemas import ManifestV1
 from ..common.schemas import TaskCollectPip
@@ -160,15 +158,15 @@
             return f"pip:{self.pip_package_version}"
 
     def check(self):
         if not self.version:
             raise ValueError("Version is not set or cannot be determined")
 
 
-def _package_from_path(wheel_path: Path) -> Tuple[str, str]:
+def _package_from_path(wheel_path: Path) -> tuple[str, str]:
     """
     Extract package name and version from package files such as wheel files.
     """
     wheel_filename = wheel_path.name
     package, version, *_rest = wheel_filename.split("-")
     return package, version
 
@@ -255,15 +253,15 @@
 
 
 async def create_package_environment_pip(
     *,
     task_pkg: _TaskCollectPip,
     venv_path: Path,
     logger_name: str,
-) -> List[TaskCreate]:
+) -> list[TaskCreate]:
     """
     Create environment and install package
     """
     logger = logging.getLogger(logger_name)
     try:
         logger.debug("Creating venv and installing package")
 
@@ -306,15 +304,15 @@
     return manifest
 
 
 def load_manifest(
     package_root: Path,
     python_bin: Path,
     source: str,
-) -> List[TaskCreate]:
+) -> list[TaskCreate]:
 
     manifest_file = package_root / "__FRACTAL_MANIFEST__.json"
     manifest = read_manifest(manifest_file)
 
     task_list = []
     for t in manifest.task_list:
         task_executable = package_root / t.executable
@@ -330,15 +328,15 @@
 
 
 async def _create_venv_install_package(
     *,
     task_pkg: _TaskCollectPip,
     path: Path,
     logger_name: str,
-) -> Tuple[Path, Path]:
+) -> tuple[Path, Path]:
     """Create venv and install package
 
     Args:
         path: the directory in which to create the environment
         task_pkg: object containing the different metadata required to install
             the package
```

### Comparing `fractal_server-1.2.0a0/fractal_server/utils.py` & `fractal_server-1.2.0a1/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a0/pyproject.toml` & `fractal_server-1.2.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.0a0"
+version = "1.2.0a1"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -21,15 +21,15 @@
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
 fastapi-users-db-sqlmodel = "^0.2.0"
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
 
-clusterfutures = { version = "^0.5", optional = true }
+clusterfutures = { version = "^0.5", optional = true}
 
 asyncpg = { version = "^0.27.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
 
 [tool.poetry.extras]
 slurm = ["clusterfutures"]
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.0a0"
+current_version = "1.2.0a1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -93,12 +93,12 @@
 [tool.poetry.scripts]
 fractalctl = "fractal_server.__main__:run"
 
 [tool.coverage.run]
 branch = true
 parallel = true
 relative_files = true
-omit = ["tests/*", "fractal_server/app/runner/_parsl/*", "fractal_server/common/tests/*"]
+omit = ["tests/*", "fractal_server/common/tests/*"]
 
 [[tool.mypy.overrides]]
 module = ["devtools", "uvicorn", "sqlalchemy_utils"]
 ignore_missing_imports = true
```

### Comparing `fractal_server-1.2.0a0/setup.py` & `fractal_server-1.2.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
  'fractal_server.app',
  'fractal_server.app.api',
  'fractal_server.app.api.v1',
  'fractal_server.app.db',
  'fractal_server.app.models',
  'fractal_server.app.runner',
  'fractal_server.app.runner._local',
- 'fractal_server.app.runner._parsl',
  'fractal_server.app.runner._slurm',
  'fractal_server.app.security',
  'fractal_server.common',
  'fractal_server.common.schemas',
  'fractal_server.common.tests',
  'fractal_server.migrations',
  'fractal_server.migrations.versions',
@@ -41,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.0a0',
+    'version': '1.2.0a1',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.0a0/PKG-INFO` & `fractal_server-1.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

