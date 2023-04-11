# Comparing `tmp/mitzu-0.5.8.tar.gz` & `tmp/mitzu-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.5.8.tar", max compression
+gzip compressed data, was "mitzu-0.5.9.tar", max compression
```

## Comparing `mitzu-0.5.8.tar` & `mitzu-0.5.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     1082 2023-03-17 16:50:46.251158 mitzu-0.5.8/LICENSE.txt
--rw-r--r--   0        0        0     7200 2023-03-17 16:50:46.251158 mitzu-0.5.8/README.md
--rw-r--r--   0        0        0     6148 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/.DS_Store
--rw-r--r--   0        0        0      860 2023-03-17 16:52:10.695433 mitzu-0.5.8/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1606 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      723 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3208 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39380 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1760 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/helper.py
--rw-r--r--   0        0        0    52530 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5347 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2068 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11435 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7124 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1367 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5372 2023-03-17 16:50:46.663159 mitzu-0.5.8/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1261 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13162 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1978 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     6202 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2261 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     2762 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4693 2023-03-17 16:50:46.667159 mitzu-0.5.8/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     7583 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/model.py
--rw-r--r--   0        0        0     2434 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     6433 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0     7561 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/admin_page.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15549 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4199 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21143 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9803 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    15020 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5299 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16185 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10086 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    11681 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1290 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1712 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4130 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     3932 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1319 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0     9839 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    12020 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10009 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35869 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9231 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     4900 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3323 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2065 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5423 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0     8922 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/storage.py
--rw-r--r--   0        0        0      666 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     3248 2023-03-17 16:50:46.671160 mitzu-0.5.8/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2914 2023-03-17 16:52:10.691433 mitzu-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 mitzu-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-24 13:47:41.090671 mitzu-0.5.9/LICENSE.txt
+-rw-r--r--   0        0        0     7200 2023-03-24 13:47:41.090671 mitzu-0.5.9/README.md
+-rw-r--r--   0        0        0     6148 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/.DS_Store
+-rw-r--r--   0        0        0      860 2023-03-24 13:48:44.543592 mitzu-0.5.9/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1606 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      723 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3208 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39380 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1760 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/helper.py
+-rw-r--r--   0        0        0    52530 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5347 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2068 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11435 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7124 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1367 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7547 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5372 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1261 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15067 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1963 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     6202 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     2349 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     2805 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8014 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/model.py
+-rw-r--r--   0        0        0     2434 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     6444 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0     7561 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/admin_page.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15549 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4199 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21143 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9803 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    15455 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5299 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    16185 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10086 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    11681 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1290 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1401 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1712 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4123 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     3932 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1319 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0     9839 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    12020 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0    10009 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1733 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35869 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9231 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     4900 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3308 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2065 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4710 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0     9534 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0      666 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/toast.py
+-rw-r--r--   0        0        0     3248 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2922 2023-03-24 13:48:44.539592 mitzu-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 mitzu-0.5.9/PKG-INFO
```

### Comparing `mitzu-0.5.8/LICENSE.txt` & `mitzu-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/README.md` & `mitzu-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/.DS_Store` & `mitzu-0.5.9/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/__init__.py` & `mitzu-0.5.9/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.5.8/mitzu/adapters/adapter_factory.py` & `mitzu-0.5.9/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/athena_adapter.py` & `mitzu-0.5.9/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/databricks_adapter.py` & `mitzu-0.5.9/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/file_adapter.py` & `mitzu-0.5.9/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/generic_adapter.py` & `mitzu-0.5.9/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/helper.py` & `mitzu-0.5.9/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/mysql_adapter.py` & `mitzu-0.5.9/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.5.9/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.5.9/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.5.9/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.5.9/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/adapters/trino_adapter.py` & `mitzu-0.5.9/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/helper.py` & `mitzu-0.5.9/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/model.py` & `mitzu-0.5.9/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/notebook/model_loader.py` & `mitzu-0.5.9/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/project_discovery.py` & `mitzu-0.5.9/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/project_serialization.py` & `mitzu-0.5.9/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/samples/__init__.py` & `mitzu-0.5.9/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/samples/data_ingestion.py` & `mitzu-0.5.9/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/samples/sample_data_generator.py` & `mitzu-0.5.9/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/serialization.py` & `mitzu-0.5.9/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/charts.py` & `mitzu-0.5.9/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/common.py` & `mitzu-0.5.9/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/labels.py` & `mitzu-0.5.9/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/plot.py` & `mitzu-0.5.9/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/titles.py` & `mitzu-0.5.9/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/tooltips.py` & `mitzu-0.5.9/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/transform_conv.py` & `mitzu-0.5.9/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/visualization/transform_retention.py` & `mitzu-0.5.9/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/.DS_Store` & `mitzu-0.5.9/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/explore_page.css` & `mitzu-0.5.9/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/favicon.ico` & `mitzu-0.5.9/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/logo.png` & `mitzu-0.5.9/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.5.9/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.5.9/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/auth/authorizer.py` & `mitzu-0.5.9/mitzu/webapp/auth/authorizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 import base64
 from typing import Any, Dict, Optional, List
 from urllib import parse
 from mitzu.helper import LOGGER
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.configs as configs
 import mitzu.webapp.service.user_service as U
+import mitzu.webapp.model as WM
 
 HOME_URL = os.getenv("HOME_URL", "http://localhost:8082")
 MITZU_WEBAPP_URL = os.getenv("MITZU_WEBAPP_URL", HOME_URL)
 JWT_ALGORITHM = "HS256"
+JWT_CLAIM_ROLE = "rol"
 
 
 @dataclass(frozen=True)
 class OAuthConfig:
     """
     Contains the minimal configuration for an OAuth backend.
 
@@ -182,39 +184,46 @@
             raise Exception(
                 f"Unexpected response: {resp.status_code}, {resp.content.decode('utf-8')}"
             )
 
         return resp.json()["id_token"]
 
     def _generate_new_token_for_identity(
-        self, identity: str, role: U.Role = U.Role.MEMBER
+        self, identity: str, role: WM.Role = WM.Role.MEMBER
     ) -> str:
         now = int(time.time())
         claims = {
             "iat": now - 10,
             "exp": now + self._config.session_timeout,
             "iss": "mitzu",
             "sub": identity,
-            "rol": role.value,
+            JWT_CLAIM_ROLE: role.value,
         }
         return jwt.encode(
             claims, key=self._config.token_signing_key, algorithm=JWT_ALGORITHM
         )
 
     def _validate_token(self, token: str) -> Optional[Dict]:
         try:
             claims = jwt.decode(
                 token, self._config.token_signing_key, algorithms=[JWT_ALGORITHM]
             )
-            if "rol" in claims.keys():
-                claims["rol"] = U.Role(claims["rol"])
+
+            if self._config.user_service is not None:
+                user_id = claims["sub"]
+                user = self._config.user_service.get_user_by_id(user_id)
+                if user is None:
+                    raise Exception("User not found")
+                claims[JWT_CLAIM_ROLE] = user.role
+            elif JWT_CLAIM_ROLE in claims.keys():
+                claims[JWT_CLAIM_ROLE] = WM.Role(claims[JWT_CLAIM_ROLE])
             else:
                 claims[
-                    "rol"
-                ] = U.Role.MEMBER  # backward compatibility with old sessions
+                    JWT_CLAIM_ROLE
+                ] = WM.Role.MEMBER  # backward compatibility with old sessions
             return claims
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def _validate_foreign_token(self, token) -> Optional[str]:
         if not self._config.token_validator:
@@ -225,23 +234,14 @@
                 return None
 
             user_email = decoded_token.get("email")
             if user_email is None:
                 LOGGER.warning("Email field is missing from the identity token")
                 return None
 
-            if (
-                self._config.allowed_email_domain is not None
-                and not user_email.endswith(self._config.allowed_email_domain)
-            ):
-                LOGGER.warning(
-                    f"User tried to login with not allowed email address: {user_email}"
-                )
-                return None
-
             return user_email
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def setup_authorizer(self, server: flask.Flask):
         @server.before_request
@@ -262,25 +262,59 @@
                             self._config.redirect_cookie_name, MITZU_WEBAPP_URL
                         )
 
                         user_email = self._validate_foreign_token(id_token)
                         if not user_email:
                             raise Exception("Unauthorized (Invalid jwt token)")
 
-                        token = self._generate_new_token_for_identity(user_email)
+                        if (
+                            self._config.allowed_email_domain is not None
+                            and not user_email.endswith(
+                                self._config.allowed_email_domain
+                            )
+                        ):
+                            raise Exception(
+                                f"User tried to login with not allowed email address: {user_email}"
+                            )
+
+                        user_role = WM.Role.MEMBER
+                        token_identity = user_email
+                        if (
+                            configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
+                            and self._config.user_service is not None
+                        ):
+                            user = self._config.user_service.get_user_by_email(
+                                user_email
+                            )
+                            if user is None:
+                                raise Exception(
+                                    f"User tried to login without having a local user: {user_email}"
+                                )
+                            user_role = user.role
+                            token_identity = user.id
+
+                        token = self._generate_new_token_for_identity(
+                            token_identity, role=user_role
+                        )
 
                         resp = self._redirect(redirect_url)
                         resp.set_cookie(self._config.token_cookie_name, token)
                         resp.set_cookie(
                             self._config.redirect_cookie_name, "", expires=0
                         )
                         return resp
                     except Exception as exc:
                         traceback.print_exception(type(exc), exc, exc.__traceback__)
                         LOGGER.warning(f"Failed to authenticate: {str(exc)}")
+                        if self._config.oauth and self._config.oauth.sign_out_url:
+                            resp = self._redirect(self._config.oauth.sign_out_url)
+                            resp.set_cookie(
+                                self._config.token_cookie_name, "", expires=0
+                            )
+                            return resp
                         return self._get_unauthenticated_response()
 
             auth_token = flask.request.cookies.get(self._config.token_cookie_name)
 
             if request.path == P.SIGN_OUT_URL:
                 if self._config.oauth and self._config.oauth.sign_out_url:
                     resp = self._redirect(self._config.oauth.sign_out_url)
@@ -308,41 +342,44 @@
                     return resp
 
             auth_token = flask.request.cookies.get(self._config.token_cookie_name)
             if auth_token is not None:
                 identity = self._validate_token(auth_token)
                 if identity is not None:
                     new_token = self._generate_new_token_for_identity(
-                        identity["sub"], role=identity["rol"]
+                        identity["sub"], role=identity[JWT_CLAIM_ROLE]
                     )
                     resp.set_cookie(self._config.token_cookie_name, new_token)
             return resp
 
     def is_request_authorized(self, request: flask.Request) -> bool:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         return auth_token is not None and self._validate_token(auth_token) is not None
 
-    def get_current_user_role(self, request: flask.Request) -> Optional[U.Role]:
+    def get_current_user_role(self, request: flask.Request) -> Optional[WM.Role]:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         if self._config.user_service is None:
-            return U.Role.MEMBER
+            return WM.Role.MEMBER
 
         if auth_token is None:
             return None
 
         claims = self._validate_token(auth_token)
-        if claims is None or "rol" not in claims.keys():
+        if claims is None or JWT_CLAIM_ROLE not in claims.keys():
             return None
 
-        return U.Role(claims["rol"])
+        return WM.Role(claims[JWT_CLAIM_ROLE])
 
     def login_local_user(self, email: str, password: str) -> bool:
         if self._config.user_service is None:
             raise ValueError("User service is not set for local auth")
 
+        if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
+            raise ValueError("Password login is not enabled, need to use SSO")
+
         user = self._config.user_service.get_user_by_email_and_password(email, password)
         if user is None:
             return False
 
         token = self._generate_new_token_for_identity(user.id, role=user.role)
         dash.callback_context.response.set_cookie(self._config.token_cookie_name, token)
         return True
```

### Comparing `mitzu-0.5.8/mitzu/webapp/auth/cognito.py` & `mitzu-0.5.9/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/auth/decorator.py` & `mitzu-0.5.9/mitzu/webapp/auth/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import flask
 from typing import cast
 import functools
 from dash.exceptions import PreventUpdate
 from dash.dcc import Location
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.paths as P
-import mitzu.webapp.service.user_service as US
+import mitzu.webapp.model as WM
 
 
 def restricted(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         dependencies: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
@@ -34,15 +34,15 @@
         )
 
         if dependencies.authorizer is not None:
             user_role = dependencies.authorizer.get_current_user_role(flask.request)
             if user_role is None:
                 raise PreventUpdate
 
-            if user_role != US.Role.ADMIN:
+            if user_role != WM.Role.ADMIN:
                 raise PreventUpdate
             else:
                 return func(*args, **kwargs)
         else:
             return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `mitzu-0.5.8/mitzu/webapp/auth/google.py` & `mitzu-0.5.9/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/cache.py` & `mitzu-0.5.9/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.5.9/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/configs.py` & `mitzu-0.5.9/mitzu/webapp/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 # auth
 AUTH_BACKEND = os.getenv("AUTH_BACKEND")
 AUTH_ALLOWED_EMAIL_DOMAIN = os.getenv("AUTH_ALLOWED_EMAIL_DOMAIN")
 AUTH_JWT_SECRET = os.getenv("AUTH_JWT_SECRET", "mitzu-dev-env")
 AUTH_SESSION_TIMEOUT = os.getenv("AUTH_SESSION_TIMEOUT", 7 * 24 * 60 * 60)
+AUTH_SSO_ONLY_FOR_LOCAL_USERS = bool(os.getenv("AUTH_SSO_ONLY_FOR_LOCAL_USERS", False))
 AUTH_ROOT_PASSWORD = os.getenv("AUTH_ROOT_PASSWORD", "test")
 AUTH_ROOT_USER_EMAIL = os.getenv("AUTH_ROOT_USER_EMAIL", "root@local")
 
 
 # cache
 CACHE_EXPIRATION = int(os.getenv("CACHE_EXPIRATION", "600"))
```

### Comparing `mitzu-0.5.8/mitzu/webapp/dependencies.py` & `mitzu-0.5.9/mitzu/webapp/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,31 @@
     def from_configs(cls, server: Flask) -> Dependencies:
         delegate_cache: C.MitzuCache
         if configs.STORAGE_REDIS_HOST is not None:
             delegate_cache = C.RedisMitzuCache()
         else:
             delegate_cache = C.DiskMitzuCache("cache")
         cache = C.RequestCache(delegate_cache)
+        storage = S.MitzuStorage(cache)
 
         authorizer = None
         oauth_config = None
         user_service = None
         if configs.AUTH_BACKEND == "cognito":
             from mitzu.webapp.auth.cognito import Cognito
 
             oauth_config = Cognito.get_config()
         elif configs.AUTH_BACKEND == "google":
             from mitzu.webapp.auth.google import GoogleOAuth
 
             oauth_config = GoogleOAuth.get_config()
 
-        elif configs.AUTH_BACKEND == "local":
+        elif configs.AUTH_BACKEND == "local" or configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
             user_service = U.UserService(
-                cache, root_password=configs.AUTH_ROOT_PASSWORD
+                storage, root_password=configs.AUTH_ROOT_PASSWORD
             )
 
         if oauth_config or user_service:
             auth_config = A.AuthConfig(
                 oauth=oauth_config,
                 token_validator=A.JWTTokenValidator.create_from_oauth_config(
                     oauth_config
@@ -70,15 +71,14 @@
         queue: C.MitzuCache
         if configs.QUEUE_REDIS_HOST is not None:
             queue = C.RedisMitzuCache()
         else:
             queue = C.DiskMitzuCache("queue")
 
         # Adding cache layer over storage
-        storage = S.MitzuStorage(cache)
         events_service = E.EventsService(storage)
 
         return Dependencies(
             authorizer=authorizer,
             cache=cache,
             storage=storage,
             queue=queue,
```

### Comparing `mitzu-0.5.8/mitzu/webapp/helper.py` & `mitzu-0.5.9/mitzu/webapp/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     component_type: bc.Component = dbc.Input,
     input_lg: int = 3,
     input_sm: int = 12,
     label_lg: int = 3,
     label_sm: int = 12,
     justify: Optional[str] = None,
     read_only: bool = False,
+    hidden: bool = False,
     **kwargs,
 ):
     if "size" not in kwargs and component_type not in [dbc.Checkbox, dcc.Dropdown]:
         kwargs["size"] = "sm"
     if (
         component_type in [dbc.Input, dbc.Textarea]
         and kwargs.get("placeholder") is None
@@ -125,14 +126,21 @@
         component_type = dbc.Input
         kwargs["readonly"] = True
         kwargs["disabled"] = True
         if "data" in kwargs.keys():
             del kwargs["data"]
     else:
         kwargs["id"] = {"type": index_type, "index": property}
+
+    if hidden:
+        kwargs["type"] = "hidden"
+        return component_type(
+            **kwargs,
+        )
+
     return dbc.Row(
         [
             dbc.Label(label_children, class_name="fw-bold", sm=label_sm, lg=label_lg),
             dbc.Col(
                 component_type(
                     **kwargs,
                 ),
```

### Comparing `mitzu-0.5.8/mitzu/webapp/model.py` & `mitzu-0.5.9/mitzu/webapp/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import List, Optional
 from uuid import uuid4
+from enum import Enum
 
 import mitzu.model as M
 import mitzu.visualization.common as C
 import mitzu.serialization as SE
 from mitzu.helper import create_unique_id
 
 
@@ -232,7 +233,32 @@
             name=name,
             id=self.id,
             created_at=self.created_at,
             last_updated_at=self.last_updated_at,
             dashboard_metrics=self.dashboard_metrics,
             owner=self.owner,
         )
+
+
+class Role(Enum):
+    ADMIN = "admin"
+    MEMBER = "member"
+
+    @classmethod
+    def all_values(cls):
+        return [
+            Role.ADMIN,
+            Role.MEMBER,
+        ]
+
+
+@dataclass
+class User:
+    """
+    Container class for describing a user
+    """
+
+    email: str
+    password_hash: str
+    password_salt: str
+    id: str = field(default_factory=create_unique_id)
+    role: Role = Role.MEMBER
```

### Comparing `mitzu-0.5.8/mitzu/webapp/navbar.py` & `mitzu-0.5.9/mitzu/webapp/navbar.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/offcanvas.py` & `mitzu-0.5.9/mitzu/webapp/offcanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     project_ids = dependencies.storage.list_projects()
     project_id = project_ids[0] if len(project_ids) > 0 else None
 
     show_users = False
     show_sign_out = False
     if dependencies.authorizer is not None:
         show_sign_out = True
-        show_users = dependencies.authorizer._config.oauth is None
+        show_users = dependencies.authorizer._config.user_service is not None
 
     res = dbc.Offcanvas(
         children=[
             dbc.Row(
                 [
                     dbc.Col(
                         dcc.Link(
```

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/admin_page.py` & `mitzu-0.5.9/mitzu/webapp/pages/admin_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.5.9/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/connections_page.py` & `mitzu-0.5.9/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.5.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/dashboards.py` & `mitzu-0.5.9/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/edit_user.py` & `mitzu-0.5.9/mitzu/webapp/pages/edit_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 )
 import dash_bootstrap_components as dbc
 import dash.development.base_component as bc
 import dash_mantine_components as dmc
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
-import mitzu.webapp.service.user_service as US
+import mitzu.webapp.model as WM
+import mitzu.webapp.configs as configs
 from mitzu.webapp.helper import create_form_property_input
 from mitzu.webapp.auth.decorator import (
     restricted_layout,
     restricted,
     restricted_for_admin,
 )
 from mitzu.webapp.webapp import MITZU_LOCATION
@@ -58,28 +59,28 @@
     logged_in_user_id = deps.authorizer.get_current_user_id()
     if logged_in_user_id is None:
         raise ValueError("Cannot determine logged in user id")
     logged_in_user = user_service.get_user_by_id(logged_in_user_id)
     if logged_in_user is None:
         raise ValueError("Logged in user is not found")
 
-    is_admin = deps.authorizer.get_current_user_role(flask.request) == US.Role.ADMIN
+    is_admin = deps.authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
     show_password_fields = user_id == "new"
     show_change_password = False
     show_delete_button = user_id != "new"
     if user_id is not None and user_id != "new":
         if user_id == "my-account":
             user_id = logged_in_user.id
 
         show_change_password = (
-            user_id == logged_in_user.id or logged_in_user.role == US.Role.ADMIN
+            user_id == logged_in_user.id or logged_in_user.role == WM.Role.ADMIN
         )
         user = user_service.get_user_by_id(user_id)
         show_delete_button = (
-            logged_in_user.role == US.Role.ADMIN
+            logged_in_user.role == WM.Role.ADMIN
             and user is not None
             and user.id != logged_in_user.id
         )
     else:
         user = None
 
     if user is None and user_id != "new":
@@ -121,37 +122,39 @@
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_ROLE,
                         icon_cls="bi bi-person-fill",
                         component_type=dmc.Select,
                         data=[
                             {"label": v.name.lower(), "value": v.value}
-                            for v in US.Role.all_values()
+                            for v in WM.Role.all_values()
                         ],
                         required=True,
-                        value=user.role if user is not None else US.Role.MEMBER.value,
+                        value=user.role if user is not None else WM.Role.MEMBER.value,
                         read_only=user_service.is_root_user(user_id),
                     ),
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_PASSWORD,
                         icon_cls="bi bi-key",
                         type="password",
                         required=True,
                         value="",
+                        hidden=configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS,
                     )
                     if show_password_fields
                     else None,
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_CONFIRM_PASSWORD,
                         icon_cls="bi bi-key",
                         type="password",
                         required=True,
                         value="",
+                        hidden=configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS,
                     )
                     if show_password_fields
                     else None,
                 ]
                 + (
                     [
                         html.Hr(),
@@ -227,14 +230,17 @@
                 ],
             ),
         ]
     )
 
 
 def change_password_form():
+    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
+        return []
+
     return [
         html.Hr(),
         create_form_property_input(
             index_type=INDEX_TYPE,
             property=PROP_PASSWORD,
             icon_cls="bi bi-key",
             type="password",
@@ -281,16 +287,23 @@
 def create_new_user(n_clicks: int, email="", role="", password="", confirm_password=""):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
     if user_service is None:
         raise ValueError("User service is not set")
 
+    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
+        # new user need a password other than empty string
+        from uuid import uuid4
+
+        password = str(uuid4())
+        confirm_password = password
+
     try:
-        user_service.new_user(email, password, confirm_password, role=US.Role(role))
+        user_service.new_user(email, password, confirm_password, role=WM.Role(role))
         return {
             SAVE_RESPONSE_CONTAINER: "User created!",
         }
     except Exception as e:
         return {
             SAVE_RESPONSE_CONTAINER: str(e),
         }
@@ -338,15 +351,15 @@
 
         if user_id == "my-account":
             user_id = logged_in_user_id
 
         if logged_in_user is None:
             raise Exception("User is not signed in")
 
-        if logged_in_user.role != US.Role.ADMIN and logged_in_user.id != user_id:
+        if logged_in_user.role != WM.Role.ADMIN and logged_in_user.id != user_id:
             raise Exception("User is not authorized to change this password")
 
         user_service.update_password(user_id, password, confirm_password)
         return {CHANGE_PASSWORD_RESPONSE_CONTAINER: "Password changed"}
     except Exception as e:
         return {
             CHANGE_PASSWORD_RESPONSE_CONTAINER: str(e),
@@ -386,15 +399,15 @@
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
         if logged_in_user_id is None:
             raise Exception("User is not signed in")
 
         if user_id == "my-account":
             user_id = logged_in_user_id
 
-        user_service.update_role(user_id, US.Role(role))
+        user_service.update_role(user_id, WM.Role(role))
         return {CHANGE_ROLE_RESPONSE_CONTAINER: "Role updated"}
     except Exception as e:
         return {
             CHANGE_ROLE_RESPONSE_CONTAINER: str(e),
         }
```

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/explore_project.py` & `mitzu-0.5.9/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/home.py` & `mitzu-0.5.9/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/login.py` & `mitzu-0.5.9/mitzu/webapp/pages/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,17 @@
                     )
                 ],
                 justify="center",
             ),
             html.Hr(),
             dbc.Row(
                 dbc.Col(
-                    login_with_local_users()
-                    if depenednecies.authorizer._config.user_service
-                    else login_with_oauth(),
+                    login_with_oauth()
+                    if depenednecies.authorizer._config.oauth
+                    else login_with_local_users(),
                     class_name="mt-5",
                 )
             ),
         ]
     )
```

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.5.9/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.5.9/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.5.9/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/manage_project.py` & `mitzu-0.5.9/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.5.9/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/paths.py` & `mitzu-0.5.9/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.5.9/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.5.9/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.5.9/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/projects_page.py` & `mitzu-0.5.9/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/pages/users.py` & `mitzu-0.5.9/mitzu/webapp/pages/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import dash.development.base_component as bc
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.service.user_service as user_service
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.helper import TBL_CLS, TBL_HEADER_CLS
 from mitzu.webapp.auth.decorator import restricted_layout
-import mitzu.webapp.service.user_service as US
+import mitzu.webapp.model as WM
 
 
 ADD_USER_BUTTON = "user_add_user"
 USERS_TABLE_ID = "users_table"
 USERS_TBL_BODY = "users_tbl_body"
 
 register_page(__name__, path=P.USERS_PATH, title="Mitzu - Users")
@@ -75,15 +75,15 @@
     if user_service is None:
         raise ValueError("User service is not set")
 
     authorizer = deps.authorizer
     if authorizer is None:
         raise ValueError("Authorizer is not set")
 
-    is_admin = authorizer.get_current_user_role(flask.request) == US.Role.ADMIN
+    is_admin = authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
 
     table = create_users_table(user_service)
 
     return html.Div(
         [
             NB.create_mitzu_navbar("users_list", []),
             dbc.Container(
```

### Comparing `mitzu-0.5.8/mitzu/webapp/service/events_service.py` & `mitzu-0.5.9/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/service/user_service.py` & `mitzu-0.5.9/mitzu/webapp/service/user_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,14 @@
 from typing import List, Optional, Tuple
-from dataclasses import dataclass, field
-from enum import Enum
 import random
 import string
-from mitzu.helper import create_unique_id
 import hashlib
-import mitzu.webapp.cache as C
+import mitzu.webapp.storage as S
 import mitzu.webapp.configs as configs
-
-
-class Role(Enum):
-    ADMIN = "admin"
-    MEMBER = "member"
-
-    @classmethod
-    def all_values(cls):
-        return [
-            Role.ADMIN,
-            Role.MEMBER,
-        ]
-
-
-@dataclass
-class User:
-    """
-    Container class for describing a user
-    """
-
-    email: str
-    password_hash: str
-    password_salt: str
-    id: str = field(default_factory=create_unique_id)
-    role: Role = Role.MEMBER
+import mitzu.webapp.model as WM
 
 
 class UserNotFoundException(Exception):
     """
     Raised when the user is not found in the local user store
     """
 
@@ -72,113 +45,104 @@
 
 
 class UserService:
     """
     UserService provides the a single API to manage users in the local user storage
     """
 
-    def __init__(self, cache: C.MitzuCache, root_password: Optional[str] = None):
-        self._cache = cache
+    def __init__(self, storage: S.MitzuStorage, root_password: Optional[str] = None):
+        self._storage = storage
 
         has_admin = False
         for user in self.list_users():
-            if user.role == Role.ADMIN:
+            if user.role == WM.Role.ADMIN:
                 has_admin = True
                 break
 
         if root_password and not has_admin:
             self.new_user(
                 configs.AUTH_ROOT_USER_EMAIL,
                 root_password,
                 root_password,
-                role=Role.ADMIN,
+                role=WM.Role.ADMIN,
             )
 
     def is_root_user(self, user_id: str) -> bool:
         user = self.get_user_by_id(user_id)
         return user is not None and user.email == configs.AUTH_ROOT_USER_EMAIL
 
-    def list_users(self) -> List[User]:
-        result = []
-        for key in self._cache.list_keys("users."):
-            result.append(self._cache.get(f"users.{key}"))
-        return result
+    def list_users(self) -> List[WM.User]:
+        return self._storage.list_users()
 
-    def get_user_by_id(self, user_id: str) -> Optional[User]:
-        return self._cache.get(f"users.{user_id}")
+    def get_user_by_id(self, user_id: str) -> Optional[WM.User]:
+        return self._storage.get_user_by_id(user_id)
 
-    def get_user_by_email(self, email: str) -> Optional[User]:
+    def get_user_by_email(self, email: str) -> Optional[WM.User]:
         for user in self.list_users():
             if user.email == email:
                 return user
         return None
 
-    def _store_user(self, user: User):
-        key = f"users.{user.id}"
-        if self._cache.get(key):
-            self._cache.clear(key)
-        self._cache.put(key, user)
-
     def update_password(self, user_id: str, password: str, password_confirmation: str):
         user = self.get_user_by_id(user_id)
         if user is None:
             raise UserNotFoundException()
 
         if password != password_confirmation:
             raise UserPasswordAndConfirmationDoNotMatch()
 
         hash, salt = self._get_password_hash_with_salt(password)
         user.password_hash = hash
         user.password_salt = salt
-        self._store_user(user)
+        self._storage.set_user(user)
 
-    def update_role(self, user_id: str, role: Role):
+    def update_role(self, user_id: str, role: WM.Role):
         user = self.get_user_by_id(user_id)
         if user is None:
             raise UserNotFoundException()
 
         if user.email == configs.AUTH_ROOT_USER_EMAIL:
             raise RootUserCannotBeChanged()
 
         user.role = role
-        self._store_user(user)
+        self._storage.set_user(user)
 
     def _get_password_hash_with_salt(self, password: str) -> Tuple[str, str]:
         salt = "".join(random.choice(string.printable) for i in range(10))
         password_to_hash = f"{password}:{salt}"
         hash = hashlib.sha256(password_to_hash.encode()).hexdigest()
         return (hash, salt)
 
     def new_user(
         self,
         email: str,
         password: str,
         password_confirmation: str,
-        role: Role = Role.MEMBER,
+        role: WM.Role = WM.Role.MEMBER,
     ) -> str:
         if self.get_user_by_email(email) is not None:
             raise UserAlreadyExists()
 
         if password != password_confirmation:
             raise UserPasswordAndConfirmationDoNotMatch()
 
         hash, salt = self._get_password_hash_with_salt(password)
 
-        user = User(
+        user = WM.User(
             email=email,
             password_hash=hash,
             password_salt=salt,
             role=role,
         )
-        self._store_user(user)
+        self._storage.set_user(user)
         return user.id
 
     def get_user_by_email_and_password(
         self, email: str, password: str
-    ) -> Optional[User]:
+    ) -> Optional[WM.User]:
         user = self.get_user_by_email(email)
         if user is None:
             return None
 
         password_to_hash = f"{password}:{user.password_salt}"
         hash = hashlib.sha256(password_to_hash.encode()).hexdigest()
         if hash == user.password_hash:
@@ -189,8 +153,8 @@
         user = self.get_user_by_id(user_id)
         if user is None:
             raise UserNotFoundException()
 
         if user.email == configs.AUTH_ROOT_USER_EMAIL:
             raise RootUserCannotBeChanged()
 
-        self._cache.clear(f"users.{user.id}")
+        self._storage.clear_user(user_id)
```

### Comparing `mitzu-0.5.8/mitzu/webapp/storage.py` & `mitzu-0.5.9/mitzu/webapp/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,7 +257,25 @@
         return dashboard
 
     def set_dashboard(self, dashboard_id: str, dashboard: WM.Dashboard):
         return self.mitzu_cache.put(DASHBOARD_PREFIX + dashboard_id, dashboard)
 
     def clear_dashboard(self, dashboard_id: str):
         return self.mitzu_cache.clear(DASHBOARD_PREFIX + dashboard_id)
+
+    def set_user(self, user: WM.User):
+        key = f"users.{user.id}"
+        if self.mitzu_cache.get(key):
+            self.mitzu_cache.clear(key)
+        self.mitzu_cache.put(key, user)
+
+    def get_user_by_id(self, user_id: str) -> Optional[WM.User]:
+        return self.mitzu_cache.get(f"users.{user_id}")
+
+    def list_users(self) -> List[WM.User]:
+        result = []
+        for key in self.mitzu_cache.list_keys("users."):
+            result.append(self.mitzu_cache.get(f"users.{key}"))
+        return result
+
+    def clear_user(self, user_id: str):
+        self.mitzu_cache.clear(f"users.{user_id}")
```

### Comparing `mitzu-0.5.8/mitzu/webapp/toast.py` & `mitzu-0.5.9/mitzu/webapp/toast.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/mitzu/webapp/webapp.py` & `mitzu-0.5.9/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.8/pyproject.toml` & `mitzu-0.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.5.8"
+version = "0.5.9"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
@@ -15,15 +15,15 @@
 pandas = "~1.3.5"
 plotly = "~5.5.0"
 sqlalchemy = {version="~1.4.31", extras=["asyncio"]}
 pyarrow = "~8.0.0"
 fastparquet = "~0.8.0"
 sqlparse = "^0.4.2"
 tqdm = "^4.64.1"
-cryptography= "==38.0.4"
+cryptography= ">=38.0.4,<39.1.0"
 requests = "^2.28.2"
 
 # Adapter extras
 psycopg2 = {version = "~2.9.3", optional=true}
 mysql-connector-python = {version = "~8.0.28", optional=true}
 trino = { version = "~0.313.0", optional=true, extras=["sqlalchemy"] }
 databricks-sql-connector = { version = "^2.0.2", optional=true}
```

### Comparing `mitzu-0.5.8/PKG-INFO` & `mitzu-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.5.8
+Version: 0.5.9
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: snowflake
 Provides-Extra: trinodwh
 Provides-Extra: webapp
 Requires-Dist: PyAthena (>=2.13.0,<3.0.0) ; extra == "athena"
 Requires-Dist: PyJWT[crypto] (>=2.4.0,<3.0.0) ; extra == "webapp"
-Requires-Dist: cryptography (==38.0.4)
+Requires-Dist: cryptography (>=38.0.4,<39.1.0)
 Requires-Dist: dash-bootstrap-components (>=1.2.0,<2.0.0) ; extra == "webapp"
 Requires-Dist: dash-draggable (>=0.1.2,<0.2.0) ; extra == "webapp"
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0) ; extra == "webapp"
 Requires-Dist: dash-mantine-components (>=0.11.1,<0.12.0) ; extra == "webapp"
 Requires-Dist: dash[celery,compress,diskcache] (>=2.6.0,<3.0.0) ; extra == "webapp"
 Requires-Dist: databricks-sql-connector (>=2.0.2,<3.0.0) ; extra == "databricks"
 Requires-Dist: fastparquet (>=0.8.0,<0.9.0)
```

