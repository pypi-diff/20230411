# Comparing `tmp/sqlmesh-0.3.2.dev10.tar.gz` & `tmp/sqlmesh-0.3.2.dev11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.3.2.dev10.tar", last modified: Mon Apr 10 23:10:54 2023, max compression
+gzip compressed data, was "sqlmesh-0.3.2.dev11.tar", last modified: Tue Apr 11 02:49:26 2023, max compression
```

## Comparing `sqlmesh-0.3.2.dev10.tar` & `sqlmesh-0.3.2.dev11.tar`

### file list

```diff
@@ -1,678 +1,678 @@
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.938785 sqlmesh-0.3.2.dev10/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.882118 sqlmesh-0.3.2.dev10/.circleci/
--rw-r--r--   0 toby      (1000) toby      (1001)     2449 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/.circleci/config.yml
--rw-r--r--   0 toby      (1000) toby      (1001)     3730 2023-03-16 21:46:32.000000 sqlmesh-0.3.2.dev10/.circleci/continue_config.yml
--rw-r--r--   0 toby      (1000) toby      (1001)       66 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/.dockerignore
--rw-r--r--   0 toby      (1000) toby      (1001)     2195 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/.gitignore
--rw-r--r--   0 toby      (1000) toby      (1001)     1900 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/.pre-commit-config.yaml
--rw-r--r--   0 toby      (1000) toby      (1001)      234 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev10/.readthedocs.yaml
--rw-r--r--   0 toby      (1000) toby      (1001)      135 2023-02-17 21:21:31.000000 sqlmesh-0.3.2.dev10/Dockerfile.api
--rw-r--r--   0 toby      (1000) toby      (1001)      383 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/Dockerfile.app
--rw-r--r--   0 toby      (1000) toby      (1001)    11346 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev10/LICENSE
--rw-r--r--   0 toby      (1000) toby      (1001)     1855 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/Makefile
--rw-r--r--   0 toby      (1000) toby      (1001)     1975 2023-04-10 23:10:54.938785 sqlmesh-0.3.2.dev10/PKG-INFO
--rw-r--r--   0 toby      (1000) toby      (1001)     1250 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/README.md
--rw-r--r--   0 toby      (1000) toby      (1001)     1008 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docker-compose.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.882118 sqlmesh-0.3.2.dev10/docs/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.868784 sqlmesh-0.3.2.dev10/docs/_readthedocs/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.882118 sqlmesh-0.3.2.dev10/docs/_readthedocs/html/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev10/docs/_readthedocs/html/.keep
--rw-r--r--   0 toby      (1000) toby      (1001)     9981 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/comparisons.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.882118 sqlmesh-0.3.2.dev10/docs/concepts/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.882118 sqlmesh-0.3.2.dev10/docs/concepts/architecture/
--rw-r--r--   0 toby      (1000) toby      (1001)     1334 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/architecture/serialization.md
--rw-r--r--   0 toby      (1000) toby      (1001)     1113 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 toby      (1000) toby      (1001)     5915 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/audits.md
--rw-r--r--   0 toby      (1000) toby      (1001)     3866 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/environments.md
--rw-r--r--   0 toby      (1000) toby      (1001)     5914 2023-03-28 05:36:19.000000 sqlmesh-0.3.2.dev10/docs/concepts/glossary.md
--rw-r--r--   0 toby      (1000) toby      (1001)       13 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/hooks.md
--rw-r--r--   0 toby      (1000) toby      (1001)     3027 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/macros.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.885451 sqlmesh-0.3.2.dev10/docs/concepts/models/
--rw-r--r--   0 toby      (1000) toby      (1001)     9934 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/docs/concepts/models/model_kinds.md
--rw-r--r--   0 toby      (1000) toby      (1001)     7454 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/docs/concepts/models/overview.md
--rw-r--r--   0 toby      (1000) toby      (1001)     7171 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/docs/concepts/models/python_models.md
--rw-r--r--   0 toby      (1000) toby      (1001)     4938 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/docs/concepts/models/seed_models.md
--rw-r--r--   0 toby      (1000) toby      (1001)     5356 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/docs/concepts/models/sql_models.md
--rw-r--r--   0 toby      (1000) toby      (1001)     6631 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/overview.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.885451 sqlmesh-0.3.2.dev10/docs/concepts/plans/
--rw-r--r--   0 toby      (1000) toby      (1001)    43124 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 toby      (1000) toby      (1001)     8981 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/plans.md
--rw-r--r--   0 toby      (1000) toby      (1001)       37 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/concepts/team_development.md
--rw-r--r--   0 toby      (1000) toby      (1001)     5699 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev10/docs/concepts/tests.md
--rw-r--r--   0 toby      (1000) toby      (1001)      607 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/docs/development.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.885451 sqlmesh-0.3.2.dev10/docs/guides/
--rw-r--r--   0 toby      (1000) toby      (1001)     1953 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/guides/connections.md
--rw-r--r--   0 toby      (1000) toby      (1001)    10756 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/guides/models.md
--rw-r--r--   0 toby      (1000) toby      (1001)     2136 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/guides/projects.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.885451 sqlmesh-0.3.2.dev10/docs/guides/scheduling/
--rw-r--r--   0 toby      (1000) toby      (1001)   740917 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 toby      (1000) toby      (1001)   379880 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 toby      (1000) toby      (1001)     5648 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/guides/scheduling.md
--rw-r--r--   0 toby      (1000) toby      (1001)     1854 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev10/docs/guides/testing.md
--rw-r--r--   0 toby      (1000) toby      (1001)     5510 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/docs/index.md
--rw-r--r--   0 toby      (1000) toby      (1001)      290 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev10/docs/installation.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.885451 sqlmesh-0.3.2.dev10/docs/integrations/
--rw-r--r--   0 toby      (1000) toby      (1001)     2905 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/docs/integrations/airflow.md
--rw-r--r--   0 toby      (1000) toby      (1001)     7309 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/integrations/dbt.md
--rw-r--r--   0 toby      (1000) toby      (1001)    20383 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/integrations/engines.md
--rw-r--r--   0 toby      (1000) toby      (1001)      926 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/integrations/github.md
--rw-r--r--   0 toby      (1000) toby      (1001)      217 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/integrations/overview.md
--rw-r--r--   0 toby      (1000) toby      (1001)      665 2023-03-28 05:37:30.000000 sqlmesh-0.3.2.dev10/docs/prerequisites.md
--rw-r--r--   0 toby      (1000) toby      (1001)    10774 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/docs/quick_start.md
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/docs/reference/
--rw-r--r--   0 toby      (1000) toby      (1001)     5816 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/reference/cli.md
--rw-r--r--   0 toby      (1000) toby      (1001)    13240 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/reference/configuration.md
--rw-r--r--   0 toby      (1000) toby      (1001)     4091 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/reference/notebook.md
--rw-r--r--   0 toby      (1000) toby      (1001)     1127 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/reference/overview.md
--rw-r--r--   0 toby      (1000) toby      (1001)       14 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/reference/python.md
--rw-r--r--   0 toby      (1000) toby      (1001)       16 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev10/docs/release_notes.md
--rw-r--r--   0 toby      (1000) toby      (1001)      122 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev10/docs/requirements.txt
--rw-r--r--   0 toby      (1000) toby      (1001)     3249 2023-03-24 02:16:43.000000 sqlmesh-0.3.2.dev10/docs/sqlmesh.png
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/airflow/
--rw-r--r--   0 toby      (1000) toby      (1001)     1713 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/airflow/Dockerfile.template
--rw-r--r--   0 toby      (1000) toby      (1001)     2164 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/examples/airflow/Makefile
--rw-r--r--   0 toby      (1000) toby      (1001)      942 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/airflow/README.md
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/airflow/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/airflow/dags/
--rw-r--r--   0 toby      (1000) toby      (1001)      263 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3515 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 toby      (1000) toby      (1001)       12 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/airflow/requirements.txt
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/airflow/spark_conf/
--rw-r--r--   0 toby      (1000) toby      (1001)      872 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 toby      (1000) toby      (1001)      151 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/sushi/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/audits/
--rw-r--r--   0 toby      (1000) toby      (1001)      105 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/sushi/audits/items.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      119 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/sushi/audits/order_items.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      829 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi/config.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/data/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi/data/.keep
--rw-r--r--   0 toby      (1000) toby      (1001)      551 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/sushi/helper.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/hooks/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-24 20:49:57.000000 sqlmesh-0.3.2.dev10/examples/sushi/hooks/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev10/examples/sushi/macros/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      702 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/examples/sushi/macros/macros.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/models/
--rw-r--r--   0 toby      (1000) toby      (1001)      913 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      204 2023-03-15 23:16:28.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/customers.sql
--rw-r--r--   0 toby      (1000) toby      (1001)     1915 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/items.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1892 2023-03-31 16:25:38.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/order_items.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1646 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/orders.py
--rw-r--r--   0 toby      (1000) toby      (1001)      346 2023-03-23 20:16:10.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      413 2023-03-15 18:49:02.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      123 2023-03-15 18:49:02.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      688 2023-03-25 05:44:28.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      197 2023-02-09 00:05:32.000000 sqlmesh-0.3.2.dev10/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/seeds/
--rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-04-06 20:58:38.000000 sqlmesh-0.3.2.dev10/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.888784 sqlmesh-0.3.2.dev10/examples/sushi/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)     1459 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev10/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/
--rw-r--r--   0 toby      (1000) toby      (1001)       15 2023-02-17 20:36:09.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/.gitignore
--rw-r--r--   0 toby      (1000) toby      (1001)       41 2023-02-17 20:36:09.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/.user.yml
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/analyses/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-03-14 22:00:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/config.py
--rw-r--r--   0 toby      (1000) toby      (1001)      507 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)      941 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/
--rw-r--r--   0 toby      (1000) toby      (1001)     1125 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      182 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 toby      (1000) toby      (1001)      309 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      389 2023-01-31 00:48:11.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      752 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      186 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.868784 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)      663 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)      117 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       65 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)      783 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/
--rw-r--r--   0 toby      (1000) toby      (1001)     2327 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 toby      (1000) toby      (1001)    10472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 toby      (1000) toby      (1001)       97 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-01-31 00:48:11.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/snapshots/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/sushi_dbt/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev10/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/wursthall/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.872117 sqlmesh-0.3.2.dev10/examples/wursthall/audits/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.892118 sqlmesh-0.3.2.dev10/examples/wursthall/audits/db/
--rw-r--r--   0 toby      (1000) toby      (1001)      141 2023-01-31 18:47:10.000000 sqlmesh-0.3.2.dev10/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       66 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/config.yaml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/macros/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      618 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/models/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/models/db/
--rw-r--r--   0 toby      (1000) toby      (1001)      428 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      256 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 toby      (1000) toby      (1001)     3145 2023-02-16 00:04:17.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 toby      (1000) toby      (1001)      537 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1667 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 toby      (1000) toby      (1001)      120 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 toby      (1000) toby      (1001)     3419 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 toby      (1000) toby      (1001)      892 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.872117 sqlmesh-0.3.2.dev10/examples/wursthall/seeds/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/seeds/src/
--rw-r--r--   0 toby      (1000) toby      (1001)     7416 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/examples/wursthall/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)      888 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev10/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 toby      (1000) toby      (1001)      955 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev10/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 toby      (1000) toby      (1001)     2094 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev10/mkdocs.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/pdoc/
--rwxr-xr-x   0 toby      (1000) toby      (1001)     1153 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev10/pdoc/cli.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/pdoc/templates/
--rw-r--r--   0 toby      (1000) toby      (1001)      131 2022-12-24 00:47:59.000000 sqlmesh-0.3.2.dev10/pdoc/templates/module.html.jinja2
--rw-r--r--   0 toby      (1000) toby      (1001)      734 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/pytest.ini
--rw-r--r--   0 toby      (1000) toby      (1001)     1299 2023-04-10 23:10:54.938785 sqlmesh-0.3.2.dev10/setup.cfg
--rw-r--r--   0 toby      (1000) toby      (1001)     3038 2023-04-10 20:55:23.000000 sqlmesh-0.3.2.dev10/setup.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/sqlmesh/
--rw-r--r--   0 toby      (1000) toby      (1001)        3 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/.airflowignore
--rw-r--r--   0 toby      (1000) toby      (1001)     3676 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      175 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh/_version.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.898784 sqlmesh-0.3.2.dev10/sqlmesh/cli/
--rw-r--r--   0 toby      (1000) toby      (1001)      821 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/sqlmesh/cli/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4314 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/cli/example_project.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8938 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/cli/main.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1391 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/cli/options.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.898784 sqlmesh-0.3.2.dev10/sqlmesh/core/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      586 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/_typing.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.898784 sqlmesh-0.3.2.dev10/sqlmesh/core/audit/
--rw-r--r--   0 toby      (1000) toby      (1001)      449 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      896 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7947 2023-03-16 21:46:32.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.898784 sqlmesh-0.3.2.dev10/sqlmesh/core/config/
--rw-r--r--   0 toby      (1000) toby      (1001)      638 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4412 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/base.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1001 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 toby      (1000) toby      (1001)      940 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/common.py
--rw-r--r--   0 toby      (1000) toby      (1001)    18770 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/connection.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3355 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/loader.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1655 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/model.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5389 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/root.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8432 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 toby      (1000) toby      (1001)    29028 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/console.py
--rw-r--r--   0 toby      (1000) toby      (1001)      731 2023-04-04 18:31:51.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/constants.py
--rw-r--r--   0 toby      (1000) toby      (1001)    33798 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/context.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8612 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/context_diff.py
--rw-r--r--   0 toby      (1000) toby      (1001)    17626 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/dialect.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.902118 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/
--rw-r--r--   0 toby      (1000) toby      (1001)     2390 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      762 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 toby      (1000) toby      (1001)    28418 2023-04-08 02:15:51.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5339 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9365 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 toby      (1000) toby      (1001)      193 2023-02-06 21:22:35.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1730 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1971 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1398 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7713 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1181 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2658 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3678 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1815 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/environment.py
--rw-r--r--   0 toby      (1000) toby      (1001)      742 2023-02-09 00:05:32.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/hooks.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9362 2023-03-16 20:26:39.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/loader.py
--rw-r--r--   0 toby      (1000) toby      (1001)    18920 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/macros.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.902118 sqlmesh-0.3.2.dev10/sqlmesh/core/model/
--rw-r--r--   0 toby      (1000) toby      (1001)      546 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1300 2023-02-18 02:42:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/common.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2417 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/decorator.py
--rw-r--r--   0 toby      (1000) toby      (1001)    47553 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/definition.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7382 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/kind.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12622 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/meta.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2017 2023-03-15 20:40:06.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/model/seed.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2314 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.902118 sqlmesh-0.3.2.dev10/sqlmesh/core/plan/
--rw-r--r--   0 toby      (1000) toby      (1001)      191 2022-12-26 22:38:40.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)    23746 2023-04-10 16:54:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/plan/definition.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8075 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12174 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/renderer.py
--rw-r--r--   0 toby      (1000) toby      (1001)    15345 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/scheduler.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3730 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/
--rw-r--r--   0 toby      (1000) toby      (1001)      527 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1990 2023-03-23 22:56:23.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 toby      (1000) toby      (1001)    31253 2023-04-10 23:08:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 toby      (1000) toby      (1001)    19457 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/
--rw-r--r--   0 toby      (1000) toby      (1001)      692 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)    13080 2023-04-10 20:55:17.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12222 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 toby      (1000) toby      (1001)    19898 2023-04-10 23:08:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12062 2023-03-15 20:40:06.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/test.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1412 2022-12-24 00:49:07.000000 sqlmesh-0.3.2.dev10/sqlmesh/core/user.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/dbt/
--rw-r--r--   0 toby      (1000) toby      (1001)       79 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9319 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/adapter.py
--rw-r--r--   0 toby      (1000) toby      (1001)    15630 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 toby      (1000) toby      (1001)    10323 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/builtin.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1969 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/column.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/common.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3229 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/loader.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9390 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/model.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12372 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/package.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3530 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/profile.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4412 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/project.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1049 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/seed.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3145 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/source.py
--rw-r--r--   0 toby      (1000) toby      (1001)    11101 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/target.py
--rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/dbt/util.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/engines/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4437 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/commands.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3414 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      148 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2571 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.905451 sqlmesh-0.3.2.dev10/sqlmesh/integrations/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2210 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1726 2023-01-19 20:03:13.000000 sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1829 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 toby      (1000) toby      (1001)    13153 2023-03-15 19:11:52.000000 sqlmesh-0.3.2.dev10/sqlmesh/magics.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/migrations/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/migrations/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1749 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/py.typed
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-03 22:04:13.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4020 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8053 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3830 2023-04-10 15:56:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 toby      (1000) toby      (1001)    18799 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-16 20:39:23.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2132 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 toby      (1000) toby      (1001)      868 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8508 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.908785 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1341 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 toby      (1000) toby      (1001)     6307 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2549 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 toby      (1000) toby      (1001)      877 2023-01-31 18:47:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1211 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1340 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5222 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 toby      (1000) toby      (1001)    10922 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4400 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1292 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4139 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5006 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.912118 sqlmesh-0.3.2.dev10/sqlmesh/utils/
--rw-r--r--   0 toby      (1000) toby      (1001)     4326 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     8053 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/concurrency.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7530 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 toby      (1000) toby      (1001)      410 2022-12-30 17:58:00.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/conversions.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4329 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/dag.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7549 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/date.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1244 2023-02-06 16:57:04.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/errors.py
--rw-r--r--   0 toby      (1000) toby      (1001)    15800 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/jinja.py
--rw-r--r--   0 toby      (1000) toby      (1001)    15093 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 toby      (1000) toby      (1001)      888 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/pandas.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1609 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/pydantic.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1534 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/rich.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1301 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.895451 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/
--rw-r--r--   0 toby      (1000) toby      (1001)     1975 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 toby      (1000) toby      (1001)    19684 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 toby      (1000) toby      (1001)        1 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 toby      (1000) toby      (1001)      141 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 toby      (1000) toby      (1001)      780 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 toby      (1000) toby      (1001)       12 2023-04-10 23:10:54.000000 sqlmesh-0.3.2.dev10/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 toby      (1000) toby      (1001)    21020 2023-03-27 01:45:27.000000 sqlmesh-0.3.2.dev10/sqlmesh.svg
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.912118 sqlmesh-0.3.2.dev10/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      285 2023-02-07 20:56:25.000000 sqlmesh-0.3.2.dev10/tests/common_fixtures.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3773 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/conftest.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.912118 sqlmesh-0.3.2.dev10/tests/core/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/core/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12116 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1298 2023-02-06 23:52:05.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7171 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1281 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2613 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 toby      (1000) toby      (1001)     7155 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2340 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 toby      (1000) toby      (1001)     6270 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev10/tests/core/test_audit.py
--rw-r--r--   0 toby      (1000) toby      (1001)     6611 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/core/test_config.py
--rw-r--r--   0 toby      (1000) toby      (1001)      850 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/core/test_connection_config.py
--rw-r--r--   0 toby      (1000) toby      (1001)    10703 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/core/test_context.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2749 2023-02-18 02:42:33.000000 sqlmesh-0.3.2.dev10/tests/core/test_dialect.py
--rw-r--r--   0 toby      (1000) toby      (1001)      464 2022-12-30 17:58:00.000000 sqlmesh-0.3.2.dev10/tests/core/test_environment.py
--rw-r--r--   0 toby      (1000) toby      (1001)    25987 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/core/test_integration.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5760 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/core/test_macros.py
--rw-r--r--   0 toby      (1000) toby      (1001)    24586 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/core/test_model.py
--rw-r--r--   0 toby      (1000) toby      (1001)    14690 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/tests/core/test_plan.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3886 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/core/test_plan_evaluator.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4557 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/core/test_scheduler.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3531 2022-12-20 18:12:54.000000 sqlmesh-0.3.2.dev10/tests/core/test_schema_diff.py
--rw-r--r--   0 toby      (1000) toby      (1001)      857 2023-01-06 17:32:21.000000 sqlmesh-0.3.2.dev10/tests/core/test_seed.py
--rw-r--r--   0 toby      (1000) toby      (1001)    25050 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/core/test_snapshot.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9368 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 toby      (1000) toby      (1001)    21886 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/core/test_state_sync.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/dbt/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-16 06:26:19.000000 sqlmesh-0.3.2.dev10/tests/dbt/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      630 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/dbt/conftest.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2572 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/dbt/test_adapter.py
--rw-r--r--   0 toby      (1000) toby      (1001)    12387 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/dbt/test_config.py
--rw-r--r--   0 toby      (1000) toby      (1001)    15733 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/dbt/test_transformation.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/engines/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/engines/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/engines/spark/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/engines/spark/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)      357 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/engines/spark/conftest.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1503 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/tests/fixtures/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 toby      (1000) toby      (1001)     1055 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 toby      (1000) toby      (1001)    10264 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)      941 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 toby      (1000) toby      (1001)      334 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      389 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      863 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      196 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.915451 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)      663 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 toby      (1000) toby      (1001)      117 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 toby      (1000) toby      (1001)       65 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 toby      (1000) toby      (1001)     1155 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      108 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 toby      (1000) toby      (1001)      193 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 toby      (1000) toby      (1001)       41 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 toby      (1000) toby      (1001)      540 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 toby      (1000) toby      (1001)     1249 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 toby      (1000) toby      (1001)       42 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 toby      (1000) toby      (1001)     2327 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 toby      (1000) toby      (1001)    10472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/fixtures/migrations/
--rw-r--r--   0 toby      (1000) toby      (1001)     9823 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/fixtures/migrations/environments.json
--rw-r--r--   0 toby      (1000) toby      (1001)    25229 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev10/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/integrations/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/integrations/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/integrations/github/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/integrations/github/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/integrations/github/fixtures/
--rw-r--r--   0 toby      (1000) toby      (1001)      816 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 toby      (1000) toby      (1001)      477 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/schedulers/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/schedulers/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1414 2023-01-19 20:03:13.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.918785 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3866 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4280 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 toby      (1000) toby      (1001)     9673 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1226 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 toby      (1000) toby      (1001)     6043 2023-03-03 19:46:07.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5785 2023-03-03 19:46:07.000000 sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/tests/utils/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/utils/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3580 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/utils/test_concurrency.py
--rw-r--r--   0 toby      (1000) toby      (1001)     6430 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/utils/test_connection_pool.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1381 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/tests/utils/test_dag.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1818 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/utils/test_date.py
--rw-r--r--   0 toby      (1000) toby      (1001)      551 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/utils/test_filesystem.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5516 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/utils/test_jinja.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5790 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev10/tests/utils/test_metaprogramming.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2501 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/utils/test_pandas.py
--rw-r--r--   0 toby      (1000) toby      (1001)      518 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev10/tests/utils/test_pydantic.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1194 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/tests/utils/test_yaml.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/tests/web/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev10/tests/web/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)    14574 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/tests/web/test_main.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/web/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev10/web/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/web/client/
--rw-r--r--   0 toby      (1000) toby      (1001)     1104 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/.eslintrc.js
--rw-r--r--   0 toby      (1000) toby      (1001)       94 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/.gitignore
--rw-r--r--   0 toby      (1000) toby      (1001)      129 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/.prettierignore
--rw-r--r--   0 toby      (1000) toby      (1001)      403 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/.prettierrc.js
--rw-r--r--   0 toby      (1000) toby      (1001)     1076 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/index.html
--rw-r--r--   0 toby      (1000) toby      (1001)      330 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/orval.config.ts
--rw-r--r--   0 toby      (1000) toby      (1001)   403384 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/package-lock.json
--rw-r--r--   0 toby      (1000) toby      (1001)     2144 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/package.json
--rw-r--r--   0 toby      (1000) toby      (1001)     1608 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/playwright.config.ts
--rw-r--r--   0 toby      (1000) toby      (1001)       82 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/postcss.config.js
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/web/client/public/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/web/client/public/favicons/
--rw-r--r--   0 toby      (1000) toby      (1001)     2473 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev10/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/web/client/src/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.922118 sqlmesh-0.3.2.dev10/web/client/src/api/
--rw-r--r--   0 toby      (1000) toby      (1001)     1220 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev10/web/client/src/api/channels.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     4473 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/api/index.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     3247 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/api/instance.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/web/client/src/assets/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.925452 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 toby      (1000) toby      (1001)    74500 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    74524 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    74368 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    73964 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    68940 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    67284 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    74116 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    73916 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 toby      (1000) toby      (1001)    55004 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    56384 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    57104 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    62320 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    56652 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    61688 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    57680 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    53148 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    57060 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    56836 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    61460 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    52820 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    59176 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    63876 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    60768 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    81732 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    60992 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 toby      (1000) toby      (1001)    64792 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/context/
--rw-r--r--   0 toby      (1000) toby      (1001)     4198 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/context/context.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     3220 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/context/editor.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      922 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/context/fileTree.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     2661 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/context/plan.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     1562 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/context/theme.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/hooks/
--rw-r--r--   0 toby      (1000) toby      (1001)      308 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      817 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev10/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     9237 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/index.css
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.875451 sqlmesh-0.3.2.dev10/web/client/src/library/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.878784 sqlmesh-0.3.2.dev10/web/client/src/library/components/
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/banner/
--rw-r--r--   0 toby      (1000) toby      (1001)     1295 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/button/
--rw-r--r--   0 toby      (1000) toby      (1001)     4517 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/button/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)     3516 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/
--rw-r--r--   0 toby      (1000) toby      (1001)      856 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)      632 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/
--rw-r--r--   0 toby      (1000) toby      (1001)     1388 2023-03-23 18:30:18.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 toby      (1000) toby      (1001)     4232 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     8065 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     2694 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1990 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     9785 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     8257 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     3708 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.928785 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 toby      (1000) toby      (1001)     5880 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     3854 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     1538 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/
--rw-r--r--   0 toby      (1000) toby      (1001)    10822 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     6044 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     2967 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)      562 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/graph/
--rw-r--r--   0 toby      (1000) toby      (1001)     2961 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     3146 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/
--rw-r--r--   0 toby      (1000) toby      (1001)     3568 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     6011 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)    22356 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/input/
--rw-r--r--   0 toby      (1000) toby      (1001)     2087 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)      688 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/
--rw-r--r--   0 toby      (1000) toby      (1001)     2292 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     4637 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     8042 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/
--rw-r--r--   0 toby      (1000) toby      (1001)     1560 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1953 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1447 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/
--rw-r--r--   0 toby      (1000) toby      (1001)     7537 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     6775 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1312 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)    10223 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1178 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)    13993 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     9926 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)    10478 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     3444 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     2155 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     2634 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/progress/
--rw-r--r--   0 toby      (1000) toby      (1001)      713 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/root/
--rw-r--r--   0 toby      (1000) toby      (1001)      526 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1921 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)      443 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/splitPane/
--rw-r--r--   0 toby      (1000) toby      (1001)      788 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 toby      (1000) toby      (1001)      541 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/tasksProgress/
--rw-r--r--   0 toby      (1000) toby      (1001)     7318 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/tasksProgress/TasksProgress.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.932119 sqlmesh-0.3.2.dev10/web/client/src/library/components/toggle/
--rw-r--r--   0 toby      (1000) toby      (1001)     1453 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 toby      (1000) toby      (1001)     1197 2023-03-23 18:30:18.000000 sqlmesh-0.3.2.dev10/web/client/src/main.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/models/
--rw-r--r--   0 toby      (1000) toby      (1001)     1647 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/models/artifact.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     3472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/models/directory.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     4190 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev10/web/client/src/models/environment.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     1506 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/models/file.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      173 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/src/models/index.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      766 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/src/models/initial.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      200 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev10/web/client/src/routes.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)       35 2023-01-20 16:57:53.000000 sqlmesh-0.3.2.dev10/web/client/src/tests/setup.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      541 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev10/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/types/
--rw-r--r--   0 toby      (1000) toby      (1001)      467 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/types/enum.ts
--rw-r--r--   0 toby      (1000) toby      (1001)      137 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/client/src/types/index.d.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/utils/
--rw-r--r--   0 toby      (1000) toby      (1001)     4102 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/src/utils/index.spec.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     5246 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/utils/index.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/workers/
--rw-r--r--   0 toby      (1000) toby      (1001)      113 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/workers/index.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/src/workers/sqlglot/
--rw-r--r--   0 toby      (1000) toby      (1001)     1105 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev10/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1578 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     5926 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev10/web/client/tailwind.config.js
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/client/tests/
--rw-r--r--   0 toby      (1000) toby      (1001)      170 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/tests/initial.spec.ts
--rw-r--r--   0 toby      (1000) toby      (1001)     1141 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/tsconfig.json
--rw-r--r--   0 toby      (1000) toby      (1001)     1167 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/client/vite.config.ts
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/server/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev10/web/server/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.935452 sqlmesh-0.3.2.dev10/web/server/api/
--rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev10/web/server/api/__init__.py
-drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-10 23:10:54.938785 sqlmesh-0.3.2.dev10/web/server/api/endpoints/
--rw-r--r--   0 toby      (1000) toby      (1001)      710 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/__init__.py
--rw-r--r--   0 toby      (1000) toby      (1001)     4864 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/commands.py
--rw-r--r--   0 toby      (1000) toby      (1001)      819 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/context.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1858 2023-02-17 21:21:31.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/directories.py
--rw-r--r--   0 toby      (1000) toby      (1001)      708 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/environments.py
--rw-r--r--   0 toby      (1000) toby      (1001)      637 2023-02-16 00:04:17.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/events.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5528 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/files.py
--rw-r--r--   0 toby      (1000) toby      (1001)      969 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/models.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3806 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/api/endpoints/plan.py
--rw-r--r--   0 toby      (1000) toby      (1001)     3381 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/console.py
--rw-r--r--   0 toby      (1000) toby      (1001)     1374 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/main.py
--rw-r--r--   0 toby      (1000) toby      (1001)     5724 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/models.py
--rw-r--r--   0 toby      (1000) toby      (1001)      260 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev10/web/server/openapi.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2401 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev10/web/server/settings.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2114 2023-02-06 16:57:04.000000 sqlmesh-0.3.2.dev10/web/server/sse.py
--rw-r--r--   0 toby      (1000) toby      (1001)     2419 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev10/web/server/utils.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.735380 sqlmesh-0.3.2.dev11/.circleci/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2449 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/.circleci/config.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)     3730 2023-03-16 21:46:32.000000 sqlmesh-0.3.2.dev11/.circleci/continue_config.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)       66 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/.dockerignore
+-rw-r--r--   0 toby      (1000) toby      (1001)     2195 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/.gitignore
+-rw-r--r--   0 toby      (1000) toby      (1001)     1900 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/.pre-commit-config.yaml
+-rw-r--r--   0 toby      (1000) toby      (1001)      234 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev11/.readthedocs.yaml
+-rw-r--r--   0 toby      (1000) toby      (1001)      135 2023-02-17 21:21:31.000000 sqlmesh-0.3.2.dev11/Dockerfile.api
+-rw-r--r--   0 toby      (1000) toby      (1001)      383 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/Dockerfile.app
+-rw-r--r--   0 toby      (1000) toby      (1001)    11346 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev11/LICENSE
+-rw-r--r--   0 toby      (1000) toby      (1001)     1855 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/Makefile
+-rw-r--r--   0 toby      (1000) toby      (1001)     1975 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/PKG-INFO
+-rw-r--r--   0 toby      (1000) toby      (1001)     1250 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/README.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     1008 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docker-compose.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.722047 sqlmesh-0.3.2.dev11/docs/_readthedocs/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/_readthedocs/html/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev11/docs/_readthedocs/html/.keep
+-rw-r--r--   0 toby      (1000) toby      (1001)     9981 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/comparisons.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/concepts/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/concepts/architecture/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1334 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     1113 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     5915 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/audits.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     3866 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/environments.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     5914 2023-03-28 05:36:19.000000 sqlmesh-0.3.2.dev11/docs/concepts/glossary.md
+-rw-r--r--   0 toby      (1000) toby      (1001)       13 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/hooks.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     3027 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/macros.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/concepts/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)     9934 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     7454 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/docs/concepts/models/overview.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     7171 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/docs/concepts/models/python_models.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     4938 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/docs/concepts/models/seed_models.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     5356 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/docs/concepts/models/sql_models.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     6631 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/overview.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/concepts/plans/
+-rw-r--r--   0 toby      (1000) toby      (1001)    43124 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 toby      (1000) toby      (1001)     8981 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/plans.md
+-rw-r--r--   0 toby      (1000) toby      (1001)       37 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/concepts/team_development.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     5699 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev11/docs/concepts/tests.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      607 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/docs/development.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.738714 sqlmesh-0.3.2.dev11/docs/guides/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1953 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/guides/connections.md
+-rw-r--r--   0 toby      (1000) toby      (1001)    10756 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/guides/models.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     2136 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/guides/projects.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/docs/guides/scheduling/
+-rw-r--r--   0 toby      (1000) toby      (1001)   740917 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 toby      (1000) toby      (1001)   379880 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 toby      (1000) toby      (1001)     5648 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/guides/scheduling.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     1854 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev11/docs/guides/testing.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     5510 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/docs/index.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      290 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev11/docs/installation.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/docs/integrations/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2905 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/docs/integrations/airflow.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     7309 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/integrations/dbt.md
+-rw-r--r--   0 toby      (1000) toby      (1001)    20383 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/integrations/engines.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      926 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/integrations/github.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      217 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/integrations/overview.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      665 2023-03-28 05:37:30.000000 sqlmesh-0.3.2.dev11/docs/prerequisites.md
+-rw-r--r--   0 toby      (1000) toby      (1001)    10774 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/docs/quick_start.md
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/docs/reference/
+-rw-r--r--   0 toby      (1000) toby      (1001)     5816 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/reference/cli.md
+-rw-r--r--   0 toby      (1000) toby      (1001)    13240 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/reference/configuration.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     4091 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/reference/notebook.md
+-rw-r--r--   0 toby      (1000) toby      (1001)     1127 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/reference/overview.md
+-rw-r--r--   0 toby      (1000) toby      (1001)       14 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/reference/python.md
+-rw-r--r--   0 toby      (1000) toby      (1001)       16 2023-03-26 21:03:05.000000 sqlmesh-0.3.2.dev11/docs/release_notes.md
+-rw-r--r--   0 toby      (1000) toby      (1001)      122 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev11/docs/requirements.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)     3249 2023-03-24 02:16:43.000000 sqlmesh-0.3.2.dev11/docs/sqlmesh.png
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/airflow/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1713 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/airflow/Dockerfile.template
+-rw-r--r--   0 toby      (1000) toby      (1001)     2164 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/examples/airflow/Makefile
+-rw-r--r--   0 toby      (1000) toby      (1001)      942 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/airflow/README.md
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/airflow/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/airflow/dags/
+-rw-r--r--   0 toby      (1000) toby      (1001)      263 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3515 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 toby      (1000) toby      (1001)       12 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/airflow/requirements.txt
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/airflow/spark_conf/
+-rw-r--r--   0 toby      (1000) toby      (1001)      872 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 toby      (1000) toby      (1001)      151 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/sushi/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/sushi/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/sushi/audits/
+-rw-r--r--   0 toby      (1000) toby      (1001)      105 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/sushi/audits/items.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      119 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      829 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi/config.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.742047 sqlmesh-0.3.2.dev11/examples/sushi/data/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi/data/.keep
+-rw-r--r--   0 toby      (1000) toby      (1001)      551 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/sushi/helper.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.745380 sqlmesh-0.3.2.dev11/examples/sushi/hooks/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-24 20:49:57.000000 sqlmesh-0.3.2.dev11/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.745380 sqlmesh-0.3.2.dev11/examples/sushi/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-19 21:43:17.000000 sqlmesh-0.3.2.dev11/examples/sushi/macros/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      702 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/examples/sushi/macros/macros.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.745380 sqlmesh-0.3.2.dev11/examples/sushi/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)      913 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      204 2023-03-15 23:16:28.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/customers.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)     1915 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/items.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1892 2023-03-31 16:25:38.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/order_items.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1646 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/orders.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      346 2023-03-23 20:16:10.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      413 2023-03-15 18:49:02.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      123 2023-03-15 18:49:02.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      688 2023-04-11 02:47:01.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      197 2023-02-09 00:05:32.000000 sqlmesh-0.3.2.dev11/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.745380 sqlmesh-0.3.2.dev11/examples/sushi/seeds/
+-rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-04-06 20:58:38.000000 sqlmesh-0.3.2.dev11/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.745380 sqlmesh-0.3.2.dev11/examples/sushi/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1459 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev11/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/
+-rw-r--r--   0 toby      (1000) toby      (1001)       15 2023-02-17 20:36:09.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 toby      (1000) toby      (1001)       41 2023-02-17 20:36:09.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/analyses/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-03-14 22:00:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/config.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      507 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)      941 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1125 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      182 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)      309 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      389 2023-01-31 00:48:11.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      752 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      186 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.722047 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)      663 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)      117 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       65 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)      783 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.748714 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2327 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 toby      (1000) toby      (1001)    10472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 toby      (1000) toby      (1001)       97 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-01-31 00:48:11.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/sushi_dbt/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-08 23:52:34.000000 sqlmesh-0.3.2.dev11/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.725380 sqlmesh-0.3.2.dev11/examples/wursthall/audits/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/audits/db/
+-rw-r--r--   0 toby      (1000) toby      (1001)      141 2023-01-31 18:47:10.000000 sqlmesh-0.3.2.dev11/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       66 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/config.yaml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      618 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/models/db/
+-rw-r--r--   0 toby      (1000) toby      (1001)      428 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      256 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)     3145 2023-02-16 00:04:17.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      537 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1667 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      120 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)     3419 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      892 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.725380 sqlmesh-0.3.2.dev11/examples/wursthall/seeds/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/seeds/src/
+-rw-r--r--   0 toby      (1000) toby      (1001)     7416 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/examples/wursthall/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)      888 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev11/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 toby      (1000) toby      (1001)      955 2023-02-20 23:00:53.000000 sqlmesh-0.3.2.dev11/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 toby      (1000) toby      (1001)     2094 2023-03-31 16:15:00.000000 sqlmesh-0.3.2.dev11/mkdocs.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/pdoc/
+-rwxr-xr-x   0 toby      (1000) toby      (1001)     1153 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev11/pdoc/cli.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/pdoc/templates/
+-rw-r--r--   0 toby      (1000) toby      (1001)      131 2022-12-24 00:47:59.000000 sqlmesh-0.3.2.dev11/pdoc/templates/module.html.jinja2
+-rw-r--r--   0 toby      (1000) toby      (1001)      734 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/pytest.ini
+-rw-r--r--   0 toby      (1000) toby      (1001)     1299 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/setup.cfg
+-rw-r--r--   0 toby      (1000) toby      (1001)     3038 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/setup.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.752047 sqlmesh-0.3.2.dev11/sqlmesh/
+-rw-r--r--   0 toby      (1000) toby      (1001)        3 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/.airflowignore
+-rw-r--r--   0 toby      (1000) toby      (1001)     3676 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      175 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh/_version.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.755380 sqlmesh-0.3.2.dev11/sqlmesh/cli/
+-rw-r--r--   0 toby      (1000) toby      (1001)      821 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/sqlmesh/cli/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4314 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/cli/example_project.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8938 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/cli/main.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1391 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/cli/options.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.755380 sqlmesh-0.3.2.dev11/sqlmesh/core/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      586 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/_typing.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.755380 sqlmesh-0.3.2.dev11/sqlmesh/core/audit/
+-rw-r--r--   0 toby      (1000) toby      (1001)      449 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      896 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7947 2023-03-16 21:46:32.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.758714 sqlmesh-0.3.2.dev11/sqlmesh/core/config/
+-rw-r--r--   0 toby      (1000) toby      (1001)      638 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4412 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/base.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1001 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      940 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/common.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    18770 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/connection.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3355 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/loader.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1655 2023-02-08 21:20:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/model.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5389 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/root.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8432 2023-02-24 03:17:17.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    29028 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/console.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      731 2023-04-04 18:31:51.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/constants.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    33798 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/context.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8612 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/context_diff.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    17626 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/dialect.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.758714 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2390 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      762 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    28418 2023-04-08 02:15:51.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5339 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9365 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      193 2023-02-06 21:22:35.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1730 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1971 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1398 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7713 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1181 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2658 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3678 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1815 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/environment.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      742 2023-02-09 00:05:32.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/hooks.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9362 2023-04-11 02:42:27.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/loader.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    18920 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/macros.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.758714 sqlmesh-0.3.2.dev11/sqlmesh/core/model/
+-rw-r--r--   0 toby      (1000) toby      (1001)      546 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1300 2023-02-18 02:42:33.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/common.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2417 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    47553 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/definition.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7382 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/kind.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12622 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/meta.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2017 2023-03-15 20:40:06.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/model/seed.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2314 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.758714 sqlmesh-0.3.2.dev11/sqlmesh/core/plan/
+-rw-r--r--   0 toby      (1000) toby      (1001)      191 2022-12-26 22:38:40.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    23746 2023-04-11 02:42:27.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8075 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12174 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/renderer.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    15345 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/scheduler.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3730 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.758714 sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/
+-rw-r--r--   0 toby      (1000) toby      (1001)      527 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1990 2023-03-23 22:56:23.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    31253 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    19457 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/
+-rw-r--r--   0 toby      (1000) toby      (1001)      692 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    13080 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12222 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    19996 2023-04-11 02:49:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12062 2023-03-15 20:40:06.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/test.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1412 2022-12-24 00:49:07.000000 sqlmesh-0.3.2.dev11/sqlmesh/core/user.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/dbt/
+-rw-r--r--   0 toby      (1000) toby      (1001)       79 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9319 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    15630 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    10323 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1969 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/column.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/common.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3229 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/loader.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9390 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/model.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12372 2023-03-27 16:35:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/package.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3530 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/profile.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4412 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/project.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1049 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/seed.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3145 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/source.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    11101 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/target.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/dbt/util.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/engines/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4437 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/commands.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3414 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      148 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2571 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/integrations/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.762047 sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2210 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1726 2023-01-19 20:03:13.000000 sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1829 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    13153 2023-03-15 19:11:52.000000 sqlmesh-0.3.2.dev11/sqlmesh/magics.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.765381 sqlmesh-0.3.2.dev11/sqlmesh/migrations/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1749 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/py.typed
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.765381 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.765381 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-03 22:04:13.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4020 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8053 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3830 2023-04-10 15:56:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    18799 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.765381 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-16 20:39:23.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2132 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      868 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8508 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.765381 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1341 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     6307 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2549 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      877 2023-01-31 18:47:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1211 2023-01-24 00:56:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1340 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5222 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    10922 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4400 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1292 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4139 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5006 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.768714 sqlmesh-0.3.2.dev11/sqlmesh/utils/
+-rw-r--r--   0 toby      (1000) toby      (1001)     4326 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     8053 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7530 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      410 2022-12-30 17:58:00.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/conversions.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4329 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/dag.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7549 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/date.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1244 2023-02-06 16:57:04.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/errors.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    15800 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/jinja.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    15093 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      888 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/pandas.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1609 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1534 2023-01-27 21:05:52.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/rich.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1301 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.755380 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1975 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 toby      (1000) toby      (1001)    19684 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)        1 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)      141 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)      780 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)       12 2023-04-11 02:49:26.000000 sqlmesh-0.3.2.dev11/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 toby      (1000) toby      (1001)    21020 2023-03-27 01:45:27.000000 sqlmesh-0.3.2.dev11/sqlmesh.svg
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.768714 sqlmesh-0.3.2.dev11/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      285 2023-02-07 20:56:25.000000 sqlmesh-0.3.2.dev11/tests/common_fixtures.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3773 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/tests/conftest.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.768714 sqlmesh-0.3.2.dev11/tests/core/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/core/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12116 2023-03-17 20:39:00.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1298 2023-02-06 23:52:05.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7171 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1281 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2613 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     7155 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2340 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     6270 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev11/tests/core/test_audit.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     6611 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/core/test_config.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      850 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/core/test_connection_config.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    10703 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/tests/core/test_context.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2749 2023-02-18 02:42:33.000000 sqlmesh-0.3.2.dev11/tests/core/test_dialect.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      464 2022-12-30 17:58:00.000000 sqlmesh-0.3.2.dev11/tests/core/test_environment.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    25987 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/core/test_integration.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5760 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/core/test_macros.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    24586 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/core/test_model.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    14690 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/tests/core/test_plan.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3886 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4557 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/tests/core/test_scheduler.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3531 2022-12-20 18:12:54.000000 sqlmesh-0.3.2.dev11/tests/core/test_schema_diff.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      857 2023-01-06 17:32:21.000000 sqlmesh-0.3.2.dev11/tests/core/test_seed.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    25050 2023-04-10 16:50:33.000000 sqlmesh-0.3.2.dev11/tests/core/test_snapshot.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9368 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    21886 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/tests/core/test_state_sync.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/dbt/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-16 06:26:19.000000 sqlmesh-0.3.2.dev11/tests/dbt/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      630 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/dbt/conftest.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2572 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/dbt/test_adapter.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    12387 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/dbt/test_config.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    15733 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/dbt/test_transformation.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/engines/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/engines/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/engines/spark/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/engines/spark/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      357 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/engines/spark/conftest.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1503 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.728713 sqlmesh-0.3.2.dev11/tests/fixtures/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.728713 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)      291 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.728713 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1055 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 toby      (1000) toby      (1001)    10264 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)      941 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       80 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)      334 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      389 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      863 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      196 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.728713 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)      663 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.772048 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 toby      (1000) toby      (1001)      117 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)       65 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1155 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      108 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 toby      (1000) toby      (1001)      193 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 toby      (1000) toby      (1001)       41 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)      540 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)     1249 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 toby      (1000) toby      (1001)       42 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 toby      (1000) toby      (1001)       88 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2327 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 toby      (1000) toby      (1001)    10472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 toby      (1000) toby      (1001)     9746 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/fixtures/migrations/
+-rw-r--r--   0 toby      (1000) toby      (1001)     9823 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 toby      (1000) toby      (1001)    25229 2023-04-11 02:41:58.000000 sqlmesh-0.3.2.dev11/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/integrations/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/integrations/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/integrations/github/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/integrations/github/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/integrations/github/fixtures/
+-rw-r--r--   0 toby      (1000) toby      (1001)      816 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 toby      (1000) toby      (1001)      477 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/schedulers/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/schedulers/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1414 2023-01-19 20:03:13.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.775381 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3866 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4280 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     9673 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1226 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     6043 2023-03-03 19:46:07.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5785 2023-03-03 19:46:07.000000 sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/tests/utils/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/utils/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3580 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/utils/test_concurrency.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     6430 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/utils/test_connection_pool.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1381 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/tests/utils/test_dag.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1818 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/utils/test_date.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      551 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/utils/test_filesystem.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5516 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/utils/test_jinja.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5790 2023-03-06 22:53:34.000000 sqlmesh-0.3.2.dev11/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2501 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/utils/test_pandas.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      518 2022-12-05 20:35:22.000000 sqlmesh-0.3.2.dev11/tests/utils/test_pydantic.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1194 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/tests/utils/test_yaml.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/tests/web/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev11/tests/web/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)    14574 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/tests/web/test_main.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/web/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev11/web/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/web/client/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1104 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/.eslintrc.js
+-rw-r--r--   0 toby      (1000) toby      (1001)       94 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/.gitignore
+-rw-r--r--   0 toby      (1000) toby      (1001)      129 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/.prettierignore
+-rw-r--r--   0 toby      (1000) toby      (1001)      403 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/.prettierrc.js
+-rw-r--r--   0 toby      (1000) toby      (1001)     1076 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/index.html
+-rw-r--r--   0 toby      (1000) toby      (1001)      330 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/orval.config.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)   403384 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/package-lock.json
+-rw-r--r--   0 toby      (1000) toby      (1001)     2144 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/package.json
+-rw-r--r--   0 toby      (1000) toby      (1001)     1608 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/playwright.config.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)       82 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/postcss.config.js
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.732047 sqlmesh-0.3.2.dev11/web/client/public/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/web/client/public/favicons/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2473 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev11/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.778714 sqlmesh-0.3.2.dev11/web/client/src/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.782048 sqlmesh-0.3.2.dev11/web/client/src/api/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1220 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev11/web/client/src/api/channels.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     4473 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/api/index.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     3247 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/api/instance.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.732047 sqlmesh-0.3.2.dev11/web/client/src/assets/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.732047 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.782048 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    74500 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    74524 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    74368 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    73964 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    68940 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    67284 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    74116 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    73916 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    55004 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    56384 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    57104 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    62320 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    56652 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    61688 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    57680 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    53148 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    57060 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    56836 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    61460 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    52820 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    59176 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    63876 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    60768 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    81732 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    60992 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 toby      (1000) toby      (1001)    64792 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/context/
+-rw-r--r--   0 toby      (1000) toby      (1001)     4198 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/context/context.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     3220 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/context/editor.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      922 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/context/fileTree.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     2661 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/context/plan.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     1562 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/context/theme.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/hooks/
+-rw-r--r--   0 toby      (1000) toby      (1001)      308 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      817 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev11/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     9237 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/index.css
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.732047 sqlmesh-0.3.2.dev11/web/client/src/library/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.732047 sqlmesh-0.3.2.dev11/web/client/src/library/components/
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/library/components/banner/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1295 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/library/components/button/
+-rw-r--r--   0 toby      (1000) toby      (1001)     4517 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/library/components/button/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)     3516 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/
+-rw-r--r--   0 toby      (1000) toby      (1001)      856 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.785381 sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)      632 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1388 2023-03-23 18:30:18.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 toby      (1000) toby      (1001)     4232 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     8065 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     2694 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1990 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     9785 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     8257 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     3708 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 toby      (1000) toby      (1001)     5880 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     3854 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     1538 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/
+-rw-r--r--   0 toby      (1000) toby      (1001)    10822 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     6044 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     2967 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)      562 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/graph/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2961 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     3146 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/
+-rw-r--r--   0 toby      (1000) toby      (1001)     3568 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     6011 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)    22356 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/input/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2087 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)      688 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/
+-rw-r--r--   0 toby      (1000) toby      (1001)     2292 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     4637 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     8042 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1560 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1953 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1447 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.788715 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/
+-rw-r--r--   0 toby      (1000) toby      (1001)     7537 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     6775 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1312 2023-03-28 22:17:59.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)    10223 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1178 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)    13993 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     9926 2023-03-28 03:59:11.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)    10478 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     3444 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     2155 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     2634 2023-04-10 16:48:19.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/library/components/progress/
+-rw-r--r--   0 toby      (1000) toby      (1001)      713 2023-03-22 23:33:34.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/library/components/root/
+-rw-r--r--   0 toby      (1000) toby      (1001)      526 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1921 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)      247 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)      443 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/library/components/splitPane/
+-rw-r--r--   0 toby      (1000) toby      (1001)      788 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 toby      (1000) toby      (1001)      541 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/library/components/tasksProgress/
+-rw-r--r--   0 toby      (1000) toby      (1001)     7318 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/tasksProgress/TasksProgress.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/library/components/toggle/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1453 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 toby      (1000) toby      (1001)     1197 2023-03-23 18:30:18.000000 sqlmesh-0.3.2.dev11/web/client/src/main.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/models/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1647 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/models/artifact.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     3472 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/models/directory.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     4190 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev11/web/client/src/models/environment.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     1506 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/models/file.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      173 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/src/models/index.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      766 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/src/models/initial.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      200 2023-02-14 22:52:28.000000 sqlmesh-0.3.2.dev11/web/client/src/routes.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)       35 2023-01-20 16:57:53.000000 sqlmesh-0.3.2.dev11/web/client/src/tests/setup.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      541 2023-03-16 22:02:48.000000 sqlmesh-0.3.2.dev11/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/types/
+-rw-r--r--   0 toby      (1000) toby      (1001)      467 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/types/enum.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)      137 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/client/src/types/index.d.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/utils/
+-rw-r--r--   0 toby      (1000) toby      (1001)     4102 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     5246 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/utils/index.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/workers/
+-rw-r--r--   0 toby      (1000) toby      (1001)      113 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/workers/index.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/src/workers/sqlglot/
+-rw-r--r--   0 toby      (1000) toby      (1001)     1105 2023-04-03 18:38:25.000000 sqlmesh-0.3.2.dev11/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1578 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     5926 2023-03-24 21:34:25.000000 sqlmesh-0.3.2.dev11/web/client/tailwind.config.js
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.792048 sqlmesh-0.3.2.dev11/web/client/tests/
+-rw-r--r--   0 toby      (1000) toby      (1001)      170 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/tests/initial.spec.ts
+-rw-r--r--   0 toby      (1000) toby      (1001)     1141 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/tsconfig.json
+-rw-r--r--   0 toby      (1000) toby      (1001)     1167 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/client/vite.config.ts
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/web/server/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 23:05:37.000000 sqlmesh-0.3.2.dev11/web/server/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/web/server/api/
+-rw-r--r--   0 toby      (1000) toby      (1001)        0 2023-01-18 17:18:03.000000 sqlmesh-0.3.2.dev11/web/server/api/__init__.py
+drwxr-xr-x   0 toby      (1000) toby      (1001)        0 2023-04-11 02:49:26.795381 sqlmesh-0.3.2.dev11/web/server/api/endpoints/
+-rw-r--r--   0 toby      (1000) toby      (1001)      710 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     4864 2023-03-22 22:36:10.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/commands.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      819 2023-02-28 19:36:53.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/context.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1858 2023-02-17 21:21:31.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/directories.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      708 2023-03-02 20:21:25.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/environments.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      637 2023-02-16 00:04:17.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/events.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5528 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/files.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      969 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/models.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3806 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/api/endpoints/plan.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     3381 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/console.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     1374 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/main.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     5724 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/models.py
+-rw-r--r--   0 toby      (1000) toby      (1001)      260 2023-04-10 16:15:15.000000 sqlmesh-0.3.2.dev11/web/server/openapi.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2401 2023-03-14 17:51:18.000000 sqlmesh-0.3.2.dev11/web/server/settings.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2114 2023-02-06 16:57:04.000000 sqlmesh-0.3.2.dev11/web/server/sse.py
+-rw-r--r--   0 toby      (1000) toby      (1001)     2419 2023-03-22 22:09:21.000000 sqlmesh-0.3.2.dev11/web/server/utils.py
```

### Comparing `sqlmesh-0.3.2.dev10/.circleci/config.yml` & `sqlmesh-0.3.2.dev11/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/.circleci/continue_config.yml` & `sqlmesh-0.3.2.dev11/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/.gitignore` & `sqlmesh-0.3.2.dev11/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/.pre-commit-config.yaml` & `sqlmesh-0.3.2.dev11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/LICENSE` & `sqlmesh-0.3.2.dev11/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/Makefile` & `sqlmesh-0.3.2.dev11/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/PKG-INFO` & `sqlmesh-0.3.2.dev11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.3.2.dev10
+Version: 0.3.2.dev11
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sqlmesh-0.3.2.dev10/README.md` & `sqlmesh-0.3.2.dev11/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docker-compose.yml` & `sqlmesh-0.3.2.dev11/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/comparisons.md` & `sqlmesh-0.3.2.dev11/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/architecture/serialization.md` & `sqlmesh-0.3.2.dev11/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.3.2.dev11/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/audits.md` & `sqlmesh-0.3.2.dev11/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/environments.md` & `sqlmesh-0.3.2.dev11/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/glossary.md` & `sqlmesh-0.3.2.dev11/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/macros.md` & `sqlmesh-0.3.2.dev11/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/models/model_kinds.md` & `sqlmesh-0.3.2.dev11/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/models/overview.md` & `sqlmesh-0.3.2.dev11/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/models/python_models.md` & `sqlmesh-0.3.2.dev11/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/models/seed_models.md` & `sqlmesh-0.3.2.dev11/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/models/sql_models.md` & `sqlmesh-0.3.2.dev11/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/overview.md` & `sqlmesh-0.3.2.dev11/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.3.2.dev11/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/plans.md` & `sqlmesh-0.3.2.dev11/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/concepts/tests.md` & `sqlmesh-0.3.2.dev11/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/development.md` & `sqlmesh-0.3.2.dev11/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/connections.md` & `sqlmesh-0.3.2.dev11/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/models.md` & `sqlmesh-0.3.2.dev11/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/projects.md` & `sqlmesh-0.3.2.dev11/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.3.2.dev11/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.3.2.dev11/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/scheduling.md` & `sqlmesh-0.3.2.dev11/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/guides/testing.md` & `sqlmesh-0.3.2.dev11/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/index.md` & `sqlmesh-0.3.2.dev11/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/integrations/airflow.md` & `sqlmesh-0.3.2.dev11/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/integrations/dbt.md` & `sqlmesh-0.3.2.dev11/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/integrations/engines.md` & `sqlmesh-0.3.2.dev11/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/integrations/github.md` & `sqlmesh-0.3.2.dev11/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/prerequisites.md` & `sqlmesh-0.3.2.dev11/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/quick_start.md` & `sqlmesh-0.3.2.dev11/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/reference/cli.md` & `sqlmesh-0.3.2.dev11/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/reference/configuration.md` & `sqlmesh-0.3.2.dev11/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/reference/notebook.md` & `sqlmesh-0.3.2.dev11/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/reference/overview.md` & `sqlmesh-0.3.2.dev11/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/docs/sqlmesh.png` & `sqlmesh-0.3.2.dev11/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/airflow/Dockerfile.template` & `sqlmesh-0.3.2.dev11/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/airflow/Makefile` & `sqlmesh-0.3.2.dev11/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/airflow/README.md` & `sqlmesh-0.3.2.dev11/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.3.2.dev11/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.3.2.dev11/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/config.py` & `sqlmesh-0.3.2.dev11/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/helper.py` & `sqlmesh-0.3.2.dev11/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/macros/macros.py` & `sqlmesh-0.3.2.dev11/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/models/items.py` & `sqlmesh-0.3.2.dev11/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/models/order_items.py` & `sqlmesh-0.3.2.dev11/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/models/orders.py` & `sqlmesh-0.3.2.dev11/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.3.2.dev11/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.3.2.dev11/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/macros/macros.py` & `sqlmesh-0.3.2.dev11/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.3.2.dev11/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.3.2.dev11/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.3.2.dev11/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.3.2.dev11/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/models/src/shared.py` & `sqlmesh-0.3.2.dev11/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.3.2.dev11/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.3.2.dev11/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.3.2.dev11/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/mkdocs.yml` & `sqlmesh-0.3.2.dev11/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/pdoc/cli.py` & `sqlmesh-0.3.2.dev11/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/pytest.ini` & `sqlmesh-0.3.2.dev11/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/setup.cfg` & `sqlmesh-0.3.2.dev11/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/setup.py` & `sqlmesh-0.3.2.dev11/setup.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/cli/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/cli/example_project.py` & `sqlmesh-0.3.2.dev11/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/cli/main.py` & `sqlmesh-0.3.2.dev11/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/cli/options.py` & `sqlmesh-0.3.2.dev11/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/_typing.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/audit/definition.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/base.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/common.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/connection.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/loader.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/model.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/root.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/console.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/constants.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/context.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/context_diff.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/dialect.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/environment.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/hooks.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/loader.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/macros.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/common.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/decorator.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/definition.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/kind.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/meta.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/model/seed.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/notification_target.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/plan/definition.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/renderer.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/scheduler.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/schema_diff.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/snapshot/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,32 +464,36 @@
                         audits=audits,
                         cache=fingerprint_cache,
                     ).to_identifier(),
                 )
                 for name in _parents_from_model(model, models)
             )
 
-            if new_snapshot == snapshot or new_snapshot in all_snapshots:
-                logger.debug(f"{snapshot.snapshot_id} is unchaged")
+            if new_snapshot == snapshot:
+                logger.debug(f"{new_snapshot.snapshot_id} is unchanged.")
+                continue
+            if new_snapshot.snapshot_id in all_snapshots:
+                logger.debug(f"{new_snapshot.snapshot_id} exists.")
                 continue
 
             snapshot_mapping[snapshot.snapshot_id] = new_snapshot
-            logger.debug(f"{snapshot.snapshot_id} mapped to {new_snapshot.snapshot_id}")
+            logger.debug(f"{snapshot.snapshot_id} mapped to {new_snapshot.snapshot_id}.")
 
         if not snapshot_mapping:
             logger.debug("No changes to snapshots detected.")
             return
 
         def map_data_versions(
             name: str, versions: t.Sequence[SnapshotDataVersion]
         ) -> t.Tuple[SnapshotDataVersion, ...]:
-            version_ids = [(version.snapshot_id(name), version) for version in versions]
+            version_ids = ((version.snapshot_id(name), version) for version in versions)
+
             return tuple(
-                snapshot_mapping.get(version_id, all_snapshots[version_id]).data_version
-                if version_id in all_snapshots
+                snapshot_mapping[version_id].data_version
+                if version_id in snapshot_mapping
                 else version
                 for version_id, version in version_ids
             )
 
         for from_snapshot_id, to_snapshot in snapshot_mapping.items():
             from_snapshot = all_snapshots[from_snapshot_id]
             to_snapshot.previous_versions = map_data_versions(
```

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/test.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/core/user.py` & `sqlmesh-0.3.2.dev11/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/adapter.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/builtin.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/column.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/common.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/loader.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/model.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/package.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/profile.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/project.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/seed.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/source.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/dbt/target.py` & `sqlmesh-0.3.2.dev11/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/engines/commands.py` & `sqlmesh-0.3.2.dev11/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/app.py` & `sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.3.2.dev11/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.3.2.dev11/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/magics.py` & `sqlmesh-0.3.2.dev11/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.3.2.dev11/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.3.2.dev11/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/__init__.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/concurrency.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/dag.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/date.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/errors.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/jinja.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/pandas.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/pydantic.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/rich.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh/utils/yaml.py` & `sqlmesh-0.3.2.dev11/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.3.2.dev11/sqlmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.3.2.dev10
+Version: 0.3.2.dev11
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.3.2.dev11/sqlmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.3.2.dev11/sqlmesh.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/sqlmesh.svg` & `sqlmesh-0.3.2.dev11/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/conftest.py` & `sqlmesh-0.3.2.dev11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.3.2.dev11/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_audit.py` & `sqlmesh-0.3.2.dev11/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_config.py` & `sqlmesh-0.3.2.dev11/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_connection_config.py` & `sqlmesh-0.3.2.dev11/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_context.py` & `sqlmesh-0.3.2.dev11/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_dialect.py` & `sqlmesh-0.3.2.dev11/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_integration.py` & `sqlmesh-0.3.2.dev11/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_macros.py` & `sqlmesh-0.3.2.dev11/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_model.py` & `sqlmesh-0.3.2.dev11/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_plan.py` & `sqlmesh-0.3.2.dev11/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_plan_evaluator.py` & `sqlmesh-0.3.2.dev11/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_scheduler.py` & `sqlmesh-0.3.2.dev11/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_schema_diff.py` & `sqlmesh-0.3.2.dev11/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_seed.py` & `sqlmesh-0.3.2.dev11/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_snapshot.py` & `sqlmesh-0.3.2.dev11/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.3.2.dev11/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/core/test_state_sync.py` & `sqlmesh-0.3.2.dev11/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/dbt/conftest.py` & `sqlmesh-0.3.2.dev11/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/dbt/test_adapter.py` & `sqlmesh-0.3.2.dev11/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/dbt/test_config.py` & `sqlmesh-0.3.2.dev11/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/dbt/test_transformation.py` & `sqlmesh-0.3.2.dev11/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/engines/spark/test_db_api.py` & `sqlmesh-0.3.2.dev11/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.3.2.dev11/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/migrations/environments.json` & `sqlmesh-0.3.2.dev11/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.3.2.dev11/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.3.2.dev11/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.3.2.dev11/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_concurrency.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_connection_pool.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_dag.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_date.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_filesystem.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_jinja.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_metaprogramming.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_pandas.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_pydantic.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/utils/test_yaml.py` & `sqlmesh-0.3.2.dev11/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/tests/web/test_main.py` & `sqlmesh-0.3.2.dev11/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/.eslintrc.js` & `sqlmesh-0.3.2.dev11/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/index.html` & `sqlmesh-0.3.2.dev11/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/package-lock.json` & `sqlmesh-0.3.2.dev11/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/package.json` & `sqlmesh-0.3.2.dev11/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/playwright.config.ts` & `sqlmesh-0.3.2.dev11/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/public/favicons/favicon.ico` & `sqlmesh-0.3.2.dev11/web/client/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/api/channels.ts` & `sqlmesh-0.3.2.dev11/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/api/index.ts` & `sqlmesh-0.3.2.dev11/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/api/instance.ts` & `sqlmesh-0.3.2.dev11/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.3.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/context/context.ts` & `sqlmesh-0.3.2.dev11/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/context/editor.ts` & `sqlmesh-0.3.2.dev11/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/context/fileTree.ts` & `sqlmesh-0.3.2.dev11/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/context/plan.ts` & `sqlmesh-0.3.2.dev11/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/context/theme.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.3.2.dev11/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/index.css` & `sqlmesh-0.3.2.dev11/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/tasksProgress/TasksProgress.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/tasksProgress/TasksProgress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/main.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/models/artifact.ts` & `sqlmesh-0.3.2.dev11/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/models/directory.ts` & `sqlmesh-0.3.2.dev11/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/models/environment.ts` & `sqlmesh-0.3.2.dev11/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/models/file.ts` & `sqlmesh-0.3.2.dev11/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/models/initial.ts` & `sqlmesh-0.3.2.dev11/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/tests/utils.tsx` & `sqlmesh-0.3.2.dev11/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/utils/index.spec.ts` & `sqlmesh-0.3.2.dev11/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/utils/index.ts` & `sqlmesh-0.3.2.dev11/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.3.2.dev11/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.3.2.dev11/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/tailwind.config.js` & `sqlmesh-0.3.2.dev11/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/tsconfig.json` & `sqlmesh-0.3.2.dev11/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/client/vite.config.ts` & `sqlmesh-0.3.2.dev11/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/__init__.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/commands.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/context.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/directories.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/environments.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/events.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/files.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/models.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/api/endpoints/plan.py` & `sqlmesh-0.3.2.dev11/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/console.py` & `sqlmesh-0.3.2.dev11/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/main.py` & `sqlmesh-0.3.2.dev11/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/models.py` & `sqlmesh-0.3.2.dev11/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/settings.py` & `sqlmesh-0.3.2.dev11/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/sse.py` & `sqlmesh-0.3.2.dev11/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.3.2.dev10/web/server/utils.py` & `sqlmesh-0.3.2.dev11/web/server/utils.py`

 * *Files identical despite different names*

