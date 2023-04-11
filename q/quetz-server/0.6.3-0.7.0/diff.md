# Comparing `tmp/quetz-server-0.6.3.tar.gz` & `tmp/quetz-server-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quetz-server-0.6.3.tar", last modified: Wed Apr  5 07:06:25 2023, max compression
+gzip compressed data, was "quetz-server-0.7.0.tar", last modified: Tue Apr 11 08:48:50 2023, max compression
```

## Comparing `quetz-server-0.6.3.tar` & `quetz-server-0.7.0.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.811200 quetz-server-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 07:06:08.000000 quetz-server-0.6.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 07:06:08.000000 quetz-server-0.6.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 07:06:08.000000 quetz-server-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 07:06:08.000000 quetz-server-0.6.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-05 07:06:15.000000 quetz-server-0.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-05 07:06:08.000000 quetz-server-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-05 07:06:08.000000 quetz-server-0.6.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-05 07:06:08.000000 quetz-server-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-05 07:06:08.000000 quetz-server-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-05 07:06:25.811200 quetz-server-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-05 07:06:08.000000 quetz-server-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-05 07:06:08.000000 quetz-server-0.6.3/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-05 07:06:08.000000 quetz-server-0.6.3/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-05 07:06:08.000000 quetz-server-0.6.3/dev_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.791200 quetz-server-0.6.3/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/Dockerfile.jupyterhub
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/docker_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/grafana.env
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/graphana_datasources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/jupyterhub_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/postgres.conf
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/postgres.env
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/prometheus.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.791200 quetz-server-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.791200 quetz-server-0.6.3/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/assets/quetz_header.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.791200 quetz-server-0.6.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.795200 quetz-server-0.6.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/_static/quetz_favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/_static/quetz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.795200 quetz-server-0.6.3/docs/source/deploying/
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/authenticators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/frontend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/nginx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/deploying/workers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.795200 quetz-server-0.6.3/docs/source/qeps/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/qeps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/qeps/qep-001-user-permissions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.795200 quetz-server-0.6.3/docs/source/using/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/using/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-05 07:06:08.000000 quetz-server-0.6.3/docs/source/using/mirroring.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-05 07:06:08.000000 quetz-server-0.6.3/download-test-package.sh
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-05 07:06:08.000000 quetz-server-0.6.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-05 07:06:08.000000 quetz-server-0.6.3/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 07:06:08.000000 quetz-server-0.6.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-05 07:06:13.000000 quetz-server-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.799200 quetz-server-0.6.3/quetz/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-05 07:06:13.000000 quetz-server-0.6.3/quetz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.799200 quetz-server-0.6.3/quetz/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/jupyterhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authentication/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.799200 quetz-server-0.6.3/quetz/basic_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/basic_frontend/avatar.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/basic_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/basic_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/channel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/condainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    42490 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/database_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.799200 quetz-server-0.6.3/quetz/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/jobs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    56237 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.799200 quetz-server-0.6.3/quetz/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/metrics/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.803200 quetz-server-0.6.3/quetz/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.803200 quetz-server-0.6.3/quetz/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/a80fb051a659_create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/pkgstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/repo_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/rest_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.803200 quetz-server-0.6.3/quetz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/reindexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tasks/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.803200 quetz-server-0.6.3/quetz/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/templates/channeldata-index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/templates/subdir-index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/testing/mockups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_main_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/tests/authentification/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/authentification/test_auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/authentification/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/authentification/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/authentification/test_pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.787201 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.807200 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.811200 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/other-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/other-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/test-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/data/test-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_pkg_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_versionorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/tests/test_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz/versionorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.811200 quetz-server-0.6.3/quetz_db_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/LIBSOLV_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/conda.c
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/conda.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/quetz_pg.c
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 07:06:08.000000 quetz-server-0.6.3/quetz_db_ext/quetz_sqlite.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:06:25.811200 quetz-server-0.6.3/quetz_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 07:06:25.000000 quetz-server-0.6.3/quetz_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-05 07:06:25.811200 quetz-server-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 07:06:08.000000 quetz-server-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-11 08:48:41.000000 quetz-server-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 08:48:34.000000 quetz-server-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-11 08:48:34.000000 quetz-server-0.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-11 08:48:34.000000 quetz-server-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 08:48:34.000000 quetz-server-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-11 08:48:50.886885 quetz-server-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-11 08:48:34.000000 quetz-server-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 08:48:34.000000 quetz-server-0.7.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-11 08:48:34.000000 quetz-server-0.7.0/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-11 08:48:34.000000 quetz-server-0.7.0/dev_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/Dockerfile.jupyterhub
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/docker_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/grafana.env
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/graphana_datasources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/jupyterhub_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/postgres.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/postgres.env
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/prometheus.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/wait-for-postgres.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/assets/quetz_header.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/_static/quetz_favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/_static/quetz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/deploying/
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/authenticators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/frontend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/nginx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/workers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/qeps/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/qeps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/qeps/qep-001-user-permissions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/mirroring.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-11 08:48:34.000000 quetz-server-0.7.0/download-test-package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 08:48:34.000000 quetz-server-0.7.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-11 08:48:34.000000 quetz-server-0.7.0/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:48:34.000000 quetz-server-0.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-11 08:48:39.000000 quetz-server-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 08:48:39.000000 quetz-server-0.7.0/quetz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/jupyterhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/basic_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/avatar.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/channel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/condainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/database_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56922 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/a80fb051a659_create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/pkgstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/repo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/rest_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/reindexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/templates/channeldata-index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/templates/subdir-index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/mockups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_main_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/authentification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.866885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/other-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/other-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_pkg_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_versionorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/versionorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz_db_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/LIBSOLV_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/conda.c
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/conda.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/quetz_pg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/quetz_sqlite.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-11 08:48:50.886885 quetz-server-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:48:34.000000 quetz-server-0.7.0/setup.py
```

### Comparing `quetz-server-0.6.3/.pre-commit-config.yaml` & `quetz-server-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/CHANGELOG.md` & `quetz-server-0.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.7.0
+
+([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.3...bc0ac65796d14083ae587eba103d6d60250759ff))
+
+### Enhancements made
+
+- Add endpoints for health checks [#622](https://github.com/mamba-org/quetz/pull/622) ([@janjagusch](https://github.com/janjagusch))
+
+### Maintenance and upkeep improvements
+
+- Fix pyright errors [#621](https://github.com/mamba-org/quetz/pull/621) ([@janjagusch](https://github.com/janjagusch))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-04-05&to=2023-04-11&type=c))
+
+[@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-04-05..2023-04-11&type=Issues) | [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-04-05..2023-04-11&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.6.3
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.2...794eccb91e775e3ff3466839dbfe65a226926615))
 
 ### Bugs fixed
 
 - Cast starlette URL to str [#618](https://github.com/mamba-org/quetz/pull/618) ([@janjagusch](https://github.com/janjagusch))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-02-20&to=2023-04-05&type=c))
 
 [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-02-20..2023-04-05&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.6.2
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.1...daa8d07d62703601ca236fe4bfaaa23132f781dd))
 
 ### Bugs fixed
 
 - Fix unbound variables [#609](https://github.com/mamba-org/quetz/pull/609) ([@janjagusch](https://github.com/janjagusch))
```

### Comparing `quetz-server-0.6.3/CONTRIBUTING.md` & `quetz-server-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/Dockerfile` & `quetz-server-0.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/LICENSE` & `quetz-server-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/MANIFEST.in` & `quetz-server-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/PKG-INFO` & `quetz-server-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.6.3
+Version: 0.7.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.6.3 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.7.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.6.3/README.md` & `quetz-server-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/RELEASE.md` & `quetz-server-0.7.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/alembic.ini` & `quetz-server-0.7.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker/Dockerfile` & `quetz-server-0.7.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker/docker_config.toml` & `quetz-server-0.7.0/docker/docker_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker/jupyterhub_config.py` & `quetz-server-0.7.0/docker/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker/nginx.conf` & `quetz-server-0.7.0/docker/nginx.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker/postgres.conf` & `quetz-server-0.7.0/docker/postgres.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docker-compose.yml` & `quetz-server-0.7.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/Makefile` & `quetz-server-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/assets/quetz_header.png` & `quetz-server-0.7.0/docs/assets/quetz_header.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/make.bat` & `quetz-server-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/_static/quetz_favicon.ico` & `quetz-server-0.7.0/docs/source/_static/quetz_favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/_static/quetz_logo.png` & `quetz-server-0.7.0/docs/source/_static/quetz_logo.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/conf.py` & `quetz-server-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/authenticators.rst` & `quetz-server-0.7.0/docs/source/deploying/authenticators.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/configuration.rst` & `quetz-server-0.7.0/docs/source/deploying/configuration.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/database.rst` & `quetz-server-0.7.0/docs/source/deploying/database.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/migrations.rst` & `quetz-server-0.7.0/docs/source/deploying/migrations.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/nginx.rst` & `quetz-server-0.7.0/docs/source/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/deploying/workers.rst` & `quetz-server-0.7.0/docs/source/deploying/workers.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/index.rst` & `quetz-server-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/plugins.rst` & `quetz-server-0.7.0/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/qeps/qep-001-user-permissions.rst` & `quetz-server-0.7.0/docs/source/qeps/qep-001-user-permissions.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/using/basics.rst` & `quetz-server-0.7.0/docs/source/using/basics.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/docs/source/using/mirroring.rst` & `quetz-server-0.7.0/docs/source/using/mirroring.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/environment.yml` & `quetz-server-0.7.0/environment.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/init_db.py` & `quetz-server-0.7.0/init_db.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/pyproject.toml` & `quetz-server-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [tool.jupyter-releaser.options]
 check-imports = ["quetz"]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.tbump.version]
-current = "0.6.3"
+current = "0.7.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [[tool.tbump.field]]
 name = "channel"
```

### Comparing `quetz-server-0.6.3/quetz/authentication/auth_dao.py` & `quetz-server-0.7.0/quetz/authentication/auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/azuread.py` & `quetz-server-0.7.0/quetz/authentication/azuread.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/base.py` & `quetz-server-0.7.0/quetz/authentication/base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/github.py` & `quetz-server-0.7.0/quetz/authentication/github.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/gitlab.py` & `quetz-server-0.7.0/quetz/authentication/gitlab.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/google.py` & `quetz-server-0.7.0/quetz/authentication/google.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/jupyterhub.py` & `quetz-server-0.7.0/quetz/authentication/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/oauth2.py` & `quetz-server-0.7.0/quetz/authentication/oauth2.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/pam.py` & `quetz-server-0.7.0/quetz/authentication/pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authentication/registry.py` & `quetz-server-0.7.0/quetz/authentication/registry.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/authorization.py` & `quetz-server-0.7.0/quetz/authorization.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/basic_frontend/avatar.jpg` & `quetz-server-0.7.0/quetz/basic_frontend/avatar.jpg`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/basic_frontend/favicon.ico` & `quetz-server-0.7.0/quetz/basic_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/basic_frontend/index.html` & `quetz-server-0.7.0/quetz/basic_frontend/index.html`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/channel_data.py` & `quetz-server-0.7.0/quetz/channel_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/cli.py` & `quetz-server-0.7.0/quetz/cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/condainfo.py` & `quetz-server-0.7.0/quetz/condainfo.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/config.py` & `quetz-server-0.7.0/quetz/config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/dao.py` & `quetz-server-0.7.0/quetz/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from collections import defaultdict
 from datetime import date, datetime
 from itertools import groupby
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from sqlalchemy import and_, func, insert, or_
 from sqlalchemy.dialects.postgresql import insert as pg_insert
-from sqlalchemy.exc import IntegrityError
+from sqlalchemy.exc import IntegrityError, NoResultFound  # type: ignore
 from sqlalchemy.ext.compiler import compiles
-from sqlalchemy.orm import Query, Session, aliased, exc, joinedload
+from sqlalchemy.orm import Query, Session, aliased, joinedload
 from sqlalchemy.sql.expression import FunctionElement, Insert
 from sqlalchemy.types import DateTime
 
 from quetz import channel_data, errors, rest_models, versionorder
 from quetz.database_extensions import version_match
 from quetz.utils import apply_custom_query
 
@@ -189,21 +189,21 @@
 
     def rollback(self):
         self.db.rollback()
 
     def get_profile(self, user_id):
         try:
             return self.db.query(Profile).filter(Profile.user_id == user_id).one()
-        except exc.NoResultFound:
+        except NoResultFound:
             logger.error("User not found")
 
     def get_user(self, user_id):
         try:
             return self.db.query(User).filter(User.id == user_id).one()
-        except exc.NoResultFound:
+        except NoResultFound:
             logger.error("User not found")
 
     def get_users(self, skip: int, limit: int, q: str, order_by: str = 'username:asc'):
         query = (
             self.db.query(User)
             .filter(User.username.isnot(None))
             .filter(User.profile.has())
@@ -218,15 +218,15 @@
             query = _parse_sort_by(query, User, order_by)
 
         if limit < 0:
             return query.all()
 
         return get_paginated_result(query, skip, limit)
 
-    def get_user_by_username(self, username: str):
+    def get_user_by_username(self, username: str) -> Optional[User]:
         return (
             self.db.query(User)
             .filter(User.username == username)
             .options(joinedload(User.profile))
             .one_or_none()
         )
 
@@ -573,15 +573,15 @@
             query = _parse_sort_by(query, Channel, order_by)
 
         return query.all()
 
     def get_channel(self, channel_name: str) -> Optional[Channel]:
         return self.db.query(Channel).filter(Channel.name == channel_name).one_or_none()
 
-    def get_package(self, channel_name: str, package_name: str):
+    def get_package(self, channel_name: str, package_name: str) -> Optional[Package]:
         return (
             self.db.query(Package)
             .join(Channel)
             .filter(Channel.name == channel_name)
             .filter(Package.name == package_name)
             .one_or_none()
         )
@@ -617,14 +617,16 @@
             self.db.rollback()
             raise errors.DBError(str(exc))
 
         return package
 
     def update_package_channeldata(self, channel_name, package_name, channeldata):
         package = self.get_package(channel_name, package_name)
+        if package is None:
+            raise KeyError(f"Package '{package_name}' not found.")
         if package.channeldata:
             old_data = json.loads(package.channeldata)
         else:
             old_data = None
         data = channel_data.combine(old_data, channeldata)
         package.channeldata = json.dumps(data)
         package.url = data.get("home", "")
@@ -647,14 +649,16 @@
             .filter(ChannelMember.channel_name == channel_name)
             .filter(User.username == username)
             .one_or_none()
         )
 
     def create_channel_member(self, channel_name, new_member):
         user = self.get_user_by_username(new_member.username)
+        if user is None:
+            raise KeyError(f"User '{new_member.username}' not found.")
 
         member = ChannelMember(
             channel_name=channel_name, user_id=user.id, role=new_member.role
         )
 
         self.db.add(member)
         self.db.commit()
@@ -677,14 +681,16 @@
             .filter(PackageMember.package_name == package_name)
             .filter(User.username == username)
             .one_or_none()
         )
 
     def create_package_member(self, channel_name, package_name, new_member):
         user = self.get_user_by_username(new_member.username)
+        if user is None:
+            raise KeyError(f"User '{new_member.username}' not found.")
 
         member = PackageMember(
             channel_name=channel_name,
             package_name=package_name,
             user_id=user.id,
             role=new_member.role,
         )
@@ -953,15 +959,15 @@
         if limit < 0:
             return query.all()
         else:
             return get_paginated_result(query, skip, limit)
 
     def get_package_version_by_filename(
         self, channel_name: str, package_name: str, filename: str, platform: str
-    ):
+    ) -> Optional[PackageVersion]:
         query = (
             self.db.query(PackageVersion)
             .filter(PackageVersion.channel_name == channel_name)
             .filter(PackageVersion.package_name == package_name)
             .filter(PackageVersion.filename == filename)
             .filter(PackageVersion.platform == platform)
         )
```

### Comparing `quetz-server-0.6.3/quetz/database.py` & `quetz-server-0.7.0/quetz/database.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/database_extensions.py` & `quetz-server-0.7.0/quetz/database_extensions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/db_models.py` & `quetz-server-0.7.0/quetz/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/deps.py` & `quetz-server-0.7.0/quetz/deps.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/frontend.py` & `quetz-server-0.7.0/quetz/frontend.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/hooks.py` & `quetz-server-0.7.0/quetz/hooks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/api.py` & `quetz-server-0.7.0/quetz/jobs/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/dao.py` & `quetz-server-0.7.0/quetz/jobs/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/handlers.py` & `quetz-server-0.7.0/quetz/jobs/handlers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/models.py` & `quetz-server-0.7.0/quetz/jobs/models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/rest_models.py` & `quetz-server-0.7.0/quetz/jobs/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/jobs/runner.py` & `quetz-server-0.7.0/quetz/jobs/runner.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/main.py` & `quetz-server-0.7.0/quetz/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,19 @@
 
 
 @api_router.get("/dummylogin/{username}", tags=["dev"])
 def dummy_login(
     username: str, dao: Dao = Depends(get_dao), session=Depends(get_session)
 ):
     user = dao.get_user_by_username(username)
+    if user is None:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND,
+            detail=f"User '{username}' not found",
+        )
 
     logout(session)
     session["user_id"] = str(uuid.UUID(bytes=user.id))
 
     session["identity_provider"] = "dummy"
     return RedirectResponse("/")
 
@@ -435,14 +440,19 @@
 def delete_user(
     username: str,
     dao: Dao = Depends(get_dao),
     auth: authorization.Rules = Depends(get_rules),
 ):
     user = dao.get_user_by_username(username)
 
+    if not user or not user.profile:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND, detail=f"User {username} not found"
+        )
+
     auth.assert_delete_user(user.id)
     dao.delete_user(user.id)
 
 
 @api_router.get(
     "/users/{username}/role",
     response_model=rest_models.UserRole,
@@ -1102,14 +1112,19 @@
     db=Depends(get_db),
     auth: authorization.Rules = Depends(get_rules),
 ):
     version = dao.get_package_version_by_filename(
         channel_name, package_name, filename, platform
     )
 
+    if not version or not version.package:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND, detail="Package version not found"
+        )
+
     auth.assert_package_delete(version.package)
 
     if not version:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"package version {platform}/{filename} not found",
         )
@@ -1820,8 +1835,14 @@
     accept_encoding: Optional[str] = Header(None),
     session=Depends(get_remote_session),
     dao: Dao = Depends(get_dao),
 ):
     return serve_path("index.html", channel, accept_encoding, session, dao)
 
 
+@app.get("/health/ready", status_code=status.HTTP_200_OK)
+@app.get("/health/live", status_code=status.HTTP_200_OK)
+def is_ready_live(task: Task = Depends(get_tasks_worker)):
+    return {}
+
+
 frontend.register(app)
```

### Comparing `quetz-server-0.6.3/quetz/metrics/api.py` & `quetz-server-0.7.0/quetz/metrics/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/metrics/db_models.py` & `quetz-server-0.7.0/quetz/metrics/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/metrics/middleware.py` & `quetz-server-0.7.0/quetz/metrics/middleware.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/metrics/rest_models.py` & `quetz-server-0.7.0/quetz/metrics/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/metrics/tasks.py` & `quetz-server-0.7.0/quetz/metrics/tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/metrics/view.py` & `quetz-server-0.7.0/quetz/metrics/view.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/env.py` & `quetz-server-0.7.0/quetz/migrations/env.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py` & `quetz-server-0.7.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py` & `quetz-server-0.7.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/30241b33d849_add_task_pending_state.py` & `quetz-server-0.7.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py` & `quetz-server-0.7.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/3c3288034362_add_channel_metadata.py` & `quetz-server-0.7.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py` & `quetz-server-0.7.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py` & `quetz-server-0.7.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py` & `quetz-server-0.7.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py` & `quetz-server-0.7.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/98c04a65df4a_register_mirrors.py` & `quetz-server-0.7.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py` & `quetz-server-0.7.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/a80fb051a659_create_tables.py` & `quetz-server-0.7.0/quetz/migrations/versions/a80fb051a659_create_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py` & `quetz-server-0.7.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py` & `quetz-server-0.7.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py` & `quetz-server-0.7.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py` & `quetz-server-0.7.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py` & `quetz-server-0.7.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py` & `quetz-server-0.7.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/pkgstores.py` & `quetz-server-0.7.0/quetz/pkgstores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/repo_data.py` & `quetz-server-0.7.0/quetz/repo_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/rest_models.py` & `quetz-server-0.7.0/quetz/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tasks/common.py` & `quetz-server-0.7.0/quetz/tasks/common.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tasks/indexing.py` & `quetz-server-0.7.0/quetz/tasks/indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tasks/mirror.py` & `quetz-server-0.7.0/quetz/tasks/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,14 +455,18 @@
         try:
             package = dao.create_package(
                 channel_name, package_data, user_id, role=authorization.OWNER
             )
         except DBError:
             # package already exists so skip it so we retrieve and update it
             package = dao.get_package(channel_name, package_name)
+            if not package:
+                raise KeyError(
+                    f"Package '{package_name}' not found in channel {channel_name}"
+                )
             package.description = description
             package.summary = summary
         package.url = metadata.get("home", "")
         package.platforms = ":".join(metadata.get("subdirs", []))
         package.channeldata = json.dumps(metadata)
         dao.db.commit()
```

### Comparing `quetz-server-0.6.3/quetz/tasks/reindexing.py` & `quetz-server-0.7.0/quetz/tasks/reindexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tasks/workers.py` & `quetz-server-0.7.0/quetz/tasks/workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     else:
         db = get_session(config.sqlalchemy_database_url)
         close_session = True
 
     user_id: Optional[str]
     if task_id:
         task = db.query(Task).filter(Task.id == task_id).one_or_none()
+        if not task:
+            raise KeyError(f"Task '{task_id}' not found")
         # take extra arguments from job definition
         if task.job.extra_args:
             job_extra_args = json.loads(task.job.extra_args)
             kwargs.update(job_extra_args)
         if task.job.owner_id:
             user_id = str(uuid.UUID(bytes=task.job.owner_id))
         else:
```

### Comparing `quetz-server-0.6.3/quetz/templates/channeldata-index.html.j2` & `quetz-server-0.7.0/quetz/templates/channeldata-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/templates/subdir-index.html.j2` & `quetz-server-0.7.0/quetz/templates/subdir-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/testing/fixtures.py` & `quetz-server-0.7.0/quetz/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/testing/mockups.py` & `quetz-server-0.7.0/quetz/testing/mockups.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/testing/utils.py` & `quetz-server-0.7.0/quetz/testing/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/conftest.py` & `quetz-server-0.7.0/quetz/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_api_keys.py` & `quetz-server-0.7.0/quetz/tests/api/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_channels.py` & `quetz-server-0.7.0/quetz/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_main.py` & `quetz-server-0.7.0/quetz/tests/api/test_main.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_main_packages.py` & `quetz-server-0.7.0/quetz/tests/api/test_main_packages.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_metrics.py` & `quetz-server-0.7.0/quetz/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/api/test_users.py` & `quetz-server-0.7.0/quetz/tests/api/test_users.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/authentification/test_auth_dao.py` & `quetz-server-0.7.0/quetz/tests/authentification/test_auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/authentification/test_base.py` & `quetz-server-0.7.0/quetz/tests/authentification/test_base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/authentification/test_oauth.py` & `quetz-server-0.7.0/quetz/tests/authentification/test_oauth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/authentification/test_pam.py` & `quetz-server-0.7.0/quetz/tests/authentification/test_pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/conftest.py` & `quetz-server-0.7.0/quetz/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/data/other-package-0.1-0.tar.bz2` & `quetz-server-0.7.0/quetz/tests/data/other-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/data/other-package-0.2-0.tar.bz2` & `quetz-server-0.7.0/quetz/tests/data/other-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/data/test-package-0.1-0.tar.bz2` & `quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/data/test-package-0.1-0_copy.tar.bz2` & `quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/data/test-package-0.2-0.tar.bz2` & `quetz-server-0.7.0/quetz/tests/data/test-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_auth.py` & `quetz-server-0.7.0/quetz/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_cli.py` & `quetz-server-0.7.0/quetz/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_config.py` & `quetz-server-0.7.0/quetz/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_dao.py` & `quetz-server-0.7.0/quetz/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_indexing.py` & `quetz-server-0.7.0/quetz/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_jobs.py` & `quetz-server-0.7.0/quetz/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_mirror.py` & `quetz-server-0.7.0/quetz/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_pkg_stores.py` & `quetz-server-0.7.0/quetz/tests/test_pkg_stores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_tasks.py` & `quetz-server-0.7.0/quetz/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_versionorder.py` & `quetz-server-0.7.0/quetz/tests/test_versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/tests/test_workers.py` & `quetz-server-0.7.0/quetz/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/utils.py` & `quetz-server-0.7.0/quetz/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz/versionorder.py` & `quetz-server-0.7.0/quetz/versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/CMakeLists.txt` & `quetz-server-0.7.0/quetz_db_ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/LIBSOLV_LICENSE.txt` & `quetz-server-0.7.0/quetz_db_ext/LIBSOLV_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/conda.c` & `quetz-server-0.7.0/quetz_db_ext/conda.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/conda.h` & `quetz-server-0.7.0/quetz_db_ext/conda.h`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/quetz_pg.c` & `quetz-server-0.7.0/quetz_db_ext/quetz_pg.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_db_ext/quetz_sqlite.c` & `quetz-server-0.7.0/quetz_db_ext/quetz_sqlite.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/quetz_server.egg-info/PKG-INFO` & `quetz-server-0.7.0/quetz_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.6.3
+Version: 0.7.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.6.3 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.7.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.6.3/quetz_server.egg-info/SOURCES.txt` & `quetz-server-0.7.0/quetz_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 quetz/tests/__init__.py
 quetz/tests/conftest.py
 quetz/tests/test_auth.py
 quetz/tests/test_cli.py
 quetz/tests/test_config.py
 quetz/tests/test_dao.py
 quetz/tests/test_db_models.py
+quetz/tests/test_health.py
 quetz/tests/test_indexing.py
 quetz/tests/test_jobs.py
 quetz/tests/test_mirror.py
 quetz/tests/test_pkg_stores.py
 quetz/tests/test_tasks.py
 quetz/tests/test_versionorder.py
 quetz/tests/test_workers.py
```

### Comparing `quetz-server-0.6.3/quetz_server.egg-info/requires.txt` & `quetz-server-0.7.0/quetz_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.6.3/setup.cfg` & `quetz-server-0.7.0/setup.cfg`

 * *Files identical despite different names*

