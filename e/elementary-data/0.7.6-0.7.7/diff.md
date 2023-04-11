# Comparing `tmp/elementary-data-0.7.6.tar.gz` & `tmp/elementary-data-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-nop81e3w/elementary-data-0.7.6.tar", last modified: Thu Mar 23 13:42:43 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-jrikyhh6/elementary-data-0.7.7.tar", last modified: Tue Apr 11 12:53:07 2023, max compression
```

## Comparing `elementary-data-0.7.6.tar` & `elementary-data-0.7.7.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-03-23 13:42:23.000000 elementary-data-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-03-23 13:42:23.000000 elementary-data-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    13858 2023-03-23 13:42:43.000000 elementary-data-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12999 2023-03-23 13:42:23.000000 elementary-data-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2333 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7387 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7909 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/sidebar/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/sidebar/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/sidebar/sidebar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5608 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10127 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7646 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/test_conn.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/operations/upload_source_freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-03-23 13:42:23.000000 elementary-data-0.7.6/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13858 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9291 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-23 13:42:42.000000 elementary-data-0.7.6/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-23 13:42:43.000000 elementary-data-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-03-23 13:42:23.000000 elementary-data-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8825 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:43.000000 elementary-data-0.7.6/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-03-23 13:42:23.000000 elementary-data-0.7.6/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-04-11 12:52:52.000000 elementary-data-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-11 12:52:52.000000 elementary-data-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14153 2023-04-11 12:53:07.000000 elementary-data-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13274 2023-04-11 12:52:52.000000 elementary-data-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      602 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/sidebar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19322 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6175 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10127 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7646 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/test_conn.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/upload_source_freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14153 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9291 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:53:07.000000 elementary-data-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-04-11 12:52:52.000000 elementary-data-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8825 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.7.6/LICENSE` & `elementary-data-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/PKG-INFO` & `elementary-data-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.6
+Version: 0.7.7
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: databricks
 Provides-Extra: spark
+Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
 <img alt="Logo" src="static/header_git.png"/ width="1000">
 </p>
 
 <h2 align="center">
@@ -195,12 +196,14 @@
 <a href="https://github.com/edbizarro"><img src="https://avatars.githubusercontent.com/u/84926?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/Chintanvpatel"><img src="https://avatars.githubusercontent.com/u/1384301?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.6 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.7 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.6.2 Description-Content-Type: text/markdown
 Provides-Extra: snowflake Provides-Extra: bigquery Provides-Extra: redshift
 Provides-Extra: postgres Provides-Extra: databricks Provides-Extra: spark
-License-File: LICENSE
+Provides-Extra: all License-File: LICENSE
                                  width="1000">
          ***** Data observability for analytics & data engineers *****
 *** Monitor your data quality, operation and performance directly from your dbt
                                  project. ***
 [https://img.shields.io/badge/join-Slack-ff69b4] [https://img.shields.io/badge/
            docs-quickstart-orange] [License] left_text=Downloads"/>
   â­ï¸ Star the repo [static/star_github.png] â­ [Demo Â»](https://bit.ly/
```

### Comparing `elementary-data-0.7.6/README.md` & `elementary-data-0.7.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -170,12 +170,14 @@
 <a href="https://github.com/edbizarro"><img src="https://avatars.githubusercontent.com/u/84926?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/Chintanvpatel"><img src="https://avatars.githubusercontent.com/u/1384301?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `elementary-data-0.7.6/elementary/cli/cli.py` & `elementary-data-0.7.7/elementary/cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 click.echo(f.renderText("Elementary"))
 elementary.cli.upgrade.recommend_version_upgrade()
 
 logger = get_logger(__name__)
 
 
 def get_log_path(ctx):
-    file_path = Config.DEFAULT_FILES_PATH
+    target_path = Config.DEFAULT_TARGET_PATH
     try:
         ctx_args = ctx.args
         target_path_flag = "--target-path"
-        file_path = ctx_args[ctx_args.index(target_path_flag) + 1]
+        target_path = ctx_args[ctx_args.index(target_path_flag) + 1]
     finally:
-        os.makedirs(os.path.abspath(file_path), exist_ok=True)
-        return os.path.join(file_path, "edr.log")
+        os.makedirs(os.path.abspath(target_path), exist_ok=True)
+        return os.path.join(target_path, "edr.log")
 
 
 class ElementaryCLI(click.MultiCommand):
     _CMD_MAP = {
         "monitor": monitor,
         "report": report,
         "send-report": send_report,
```

### Comparing `elementary-data-0.7.6/elementary/cli/upgrade.py` & `elementary-data-0.7.7/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.7.7/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.7.7/elementary/clients/dbt/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.7.7/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/gcs/client.py` & `elementary-data-0.7.7/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/s3/client.py` & `elementary-data-0.7.7/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/slack/client.py` & `elementary-data-0.7.7/elementary/clients/slack/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/slack/schema.py` & `elementary-data-0.7.7/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.7.7/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/config/config.py` & `elementary-data-0.7.7/elementary/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
         "identifier": _IDENTIFIER_QUOTING,
     }
     _QUOTING_VALID_KEYS = set(_QUOTING_KEY_MAPPING.keys())
     _QUOTING_ENV_VARS = set(_QUOTING_KEY_MAPPING.values())
 
     DEFAULT_CONFIG_DIR = str(Path.home() / ".edr")
 
-    DEFAULT_FILES_PATH = os.getcwd() + "/edr_target"
+    DEFAULT_TARGET_PATH = os.getcwd() + "/edr_target"
 
     def __init__(
         self,
         config_dir: str = DEFAULT_CONFIG_DIR,
         profiles_dir: str = None,
         project_dir: str = None,
         profile_target: str = None,
         project_profile_target: str = None,
-        target_path: str = DEFAULT_FILES_PATH,
+        target_path: str = DEFAULT_TARGET_PATH,
         dbt_quoting: bool = None,
         update_bucket_website: bool = None,
         slack_webhook: str = None,
         slack_token: str = None,
         slack_channel_name: str = None,
         slack_group_alerts_by: str = None,
         timezone: str = None,
@@ -74,14 +74,15 @@
 
         self.target_dir = self._first_not_none(
             target_path,
             config.get("target-path"),
             os.getcwd(),
         )
         os.makedirs(os.path.abspath(self.target_dir), exist_ok=True)
+        os.environ["DBT_LOG_PATH"] = os.path.abspath(target_path)
 
         self.update_bucket_website = self._first_not_none(
             update_bucket_website,
             config.get("update_bucket_website"),
             False,
         )
```

### Comparing `elementary-data-0.7.6/elementary/exceptions/exceptions.py` & `elementary-data-0.7.7/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/alert.py` & `elementary-data-0.7.7/elementary/monitor/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/alerts.py` & `elementary-data-0.7.7/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.7.7/elementary/monitor/alerts/group_of_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/malformed.py` & `elementary-data-0.7.7/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/model.py` & `elementary-data-0.7.7/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.7.7/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/alerts/test.py` & `elementary-data-0.7.7/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.7.7/elementary/monitor/api/alerts/alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.7.7/elementary/monitor/api/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/filters/filters.py` & `elementary-data-0.7.7/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/filters/schema.py` & `elementary-data-0.7.7/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.7.7/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.7.7/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.7.7/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/models/models.py` & `elementary-data-0.7.7/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/models/schema.py` & `elementary-data-0.7.7/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/report/report.py` & `elementary-data-0.7.7/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/report/schema.py` & `elementary-data-0.7.7/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/selector/selector.py` & `elementary-data-0.7.7/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/sidebar/sidebar.py` & `elementary-data-0.7.7/elementary/monitor/api/sidebar/sidebar.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/tests/schema.py` & `elementary-data-0.7.7/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/api/tests/tests.py` & `elementary-data-0.7.7/elementary/monitor/api/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/cli.py` & `elementary-data-0.7.7/elementary/monitor/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Displayed in reverse order in --help.
 def common_options(cmd: str):
     def decorator(func):
         func = click.option(
             "--target-path",
             type=str,
-            default=Config.DEFAULT_FILES_PATH,
+            default=Config.DEFAULT_TARGET_PATH,
             help="Absolute target path for saving edr files such as logs and reports",
         )(func)
         func = click.option(
             "--disable-samples",
             type=bool,
             default=False,
             help="Disable sampling of data. Useful if your data contains PII.",
```

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,21 +119,35 @@
             return json.loads(latest_invocation)[0] if latest_invocation else {}
         except Exception as err:
             logger.error(f"Unable to get the latest invocation: {err}")
             self.tracking.record_internal_exception(err)
             return {}
 
     @staticmethod
-    def _check_dbt_package_compatibility(dbt_pkg_ver: str):
+    def _check_dbt_package_compatibility(dbt_pkg_ver: str) -> None:
         dbt_pkg_ver = version.parse(dbt_pkg_ver)
         py_pkg_ver = version.parse(package.get_package_version())
-        logger.info(
-            f"Checking compatibility between edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver})."
-        )
-        if (
-            dbt_pkg_ver.major != py_pkg_ver.major
-            or dbt_pkg_ver.minor != py_pkg_ver.minor
+        if dbt_pkg_ver.major > py_pkg_ver.major or (
+            dbt_pkg_ver.major == py_pkg_ver.major
+            and dbt_pkg_ver.minor > py_pkg_ver.minor
+        ):
+            logger.warning(
+                f"You are using incompatible versions between edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}).\n "
+                "To fix please run:\n"
+                "pip install --upgrade elementary-data\n",
+            )
+            return
+
+        if dbt_pkg_ver.major < py_pkg_ver.major or (
+            dbt_pkg_ver.major == py_pkg_ver.major
+            and dbt_pkg_ver.minor < py_pkg_ver.minor
         ):
             logger.warning(
                 f"You are using incompatible versions between edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}).\n "
-                "Please upgrade the major and minor versions to align.\n",
+                "To fix please update your packages.yml, and run:\n"
+                "dbt deps && dbt run --select elementary\n",
             )
+            return
+
+        logger.info(
+            f"edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}) are compatible :)"
+        )
```

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.7.7/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/README.md` & `elementary-data-0.7.7/elementary/monitor/dbt_project/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.7.7/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.7.7/elementary/monitor/dbt_project_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,51 +12,57 @@
 PATH = os.path.join(_MONITOR_DIR, "dbt_project")
 
 # Compatibility for previous dbt versions
 _MODULES_PATH = os.path.join(PATH, "dbt_modules")
 _PACKAGES_PATH = os.path.join(PATH, "dbt_packages")
 
 
-def get_elementary_package_path():
+def is_dbt_package_up_to_date() -> bool:
+    installed_version = _get_installed_dbt_package_version()
+    if installed_version is None:
+        return False
+
+    required_version = _get_required_dbt_package_version()
+    # We're using a non dbt Hub requirement, such as Git or local.
+    if not required_version:
+        return True
+
+    return installed_version == required_version
+
+
+def _get_elementary_package_path():
     package_path = os.path.join(_PACKAGES_PATH, _DBT_PACKAGE_NAME)
     if os.path.exists(package_path):
         return package_path
 
     legacy_package_path = os.path.join(_MODULES_PATH, _DBT_PACKAGE_NAME)
     if os.path.exists(legacy_package_path):
         return legacy_package_path
 
     return None
 
 
-def is_dbt_package_up_to_date() -> bool:
-    installed_version = get_installed_dbt_package_version()
-    if installed_version is None:
-        return False
-
-    required_version = get_required_dbt_package_version()
-    return installed_version == required_version
-
-
-def get_installed_dbt_package_version() -> Optional[str]:
-    package_path = get_elementary_package_path()
+def _get_installed_dbt_package_version() -> Optional[str]:
+    package_path = _get_elementary_package_path()
     if package_path is None:
         return None
 
     project_path = os.path.join(package_path, _DBT_PROJECT_FILENAME)
     if not os.path.exists(package_path):
         return None
 
     project_yaml_dict = OrderedYaml().load(project_path)
     return project_yaml_dict["version"]
 
 
-def get_required_dbt_package_version() -> Optional[str]:
+def _get_required_dbt_package_version() -> Optional[str]:
     packages_file_path = os.path.join(PATH, _PACKAGES_FILENAME)
     packages_yaml = OrderedYaml().load(packages_file_path)
 
-    for requirement in packages_yaml["packages"]:
-        package_name = requirement["package"].split("/")[-1]
+    for requirement in packages_yaml.get("packages", []):
+        package_id = requirement.get("package")
+        if not package_id:
+            continue
+        package_name = package_id.split("/")[-1]
         if package_name == _DBT_PACKAGE_NAME:
             return requirement["version"]
-
     return None
```

### Comparing `elementary-data-0.7.6/elementary/monitor/debug.py` & `elementary-data-0.7.7/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.7.7/elementary/monitor/fetchers/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/operations/cli.py` & `elementary-data-0.7.7/elementary/operations/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     "--profiles-dir",
     "-p",
     type=click.Path(exists=True),
     default=None,
     help="Which directory to look in for the profiles.yml file. "
     "If not set, edr will look in the current working directory first, then HOME/.dbt/",
 )
+@click.option(
+    "--target-path",
+    type=str,
+    default=Config.DEFAULT_TARGET_PATH,
+    help="Absolute target path for saving edr files such as logs and reports",
+)
 @click.pass_context
 def upload_source_freshness(ctx, **conf):
     """
     Upload the results of `dbt source freshness` to Elementary's schema.
     This is required in order to monitor and get alerts on source freshness failures.
     """
     config = Config(**conf)
```

### Comparing `elementary-data-0.7.6/elementary/operations/upload_source_freshness.py` & `elementary-data-0.7.7/elementary/operations/upload_source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.7.7/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/tracking/runner.py` & `elementary-data-0.7.7/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/tracking/tracking_interface.py` & `elementary-data-0.7.7/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/utils/cli_utils.py` & `elementary-data-0.7.7/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/utils/json_utils.py` & `elementary-data-0.7.7/elementary/utils/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         ret = sum_lists(ret)
     return list(set(ret))
 
 
 def list_of_lists_of_strings_to_comma_delimited_unique_strings(
     list_of_strings: List[List[str]], prefix: Optional[str] = None
 ) -> str:
+    list_of_strings = [x for x in list_of_strings if x]  # filter Nones and empty lists
     flat_list = sum_lists(list_of_strings)
     if prefix:
         flat_list = [append_prefix_if_missing(x, prefix) for x in flat_list]
     unique_strings = list(set(flat_list))
     return ", ".join(unique_strings)
```

### Comparing `elementary-data-0.7.6/elementary/utils/log.py` & `elementary-data-0.7.7/elementary/utils/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import sys
+from logging.handlers import RotatingFileHandler
 
 from elementary.utils.env_vars import is_debug
 
 
 class ColoredFormatter(logging.Formatter):
     YELLOW = "\x1b[33;20m"
     RED = "\x1b[31;20m"
@@ -21,33 +22,40 @@
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno, self.FORMAT)
         formatter = logging.Formatter(log_fmt, self.DATE_FORMAT)
         return formatter.format(record)
 
 
 FORMATTER = ColoredFormatter()
+MAX_BYTES_IN_FILE = 10 * 1024 * 1024
+ROTATION_BACKUP_COUNT = 4
 
 
 def get_console_handler():
     console_handler = logging.StreamHandler(sys.stdout)
     console_handler.setFormatter(FORMATTER)
     console_handler.setLevel(logging.DEBUG if is_debug() else logging.INFO)
     return console_handler
 
 
 def get_file_handler(files_target_path):
-    file_handler = logging.FileHandler(files_target_path, delay=True)
-    file_handler.setFormatter(FORMATTER)
-    file_handler.setLevel(logging.DEBUG)
-    return file_handler
+    rotation_handler = RotatingFileHandler(
+        files_target_path,
+        maxBytes=MAX_BYTES_IN_FILE,
+        backupCount=ROTATION_BACKUP_COUNT,
+        delay=True,
+    )
+    rotation_handler.setFormatter(FORMATTER)
+    rotation_handler.setLevel(logging.DEBUG)
+    return rotation_handler
 
 
 def get_logger(logger_name):
     logger = logging.getLogger(logger_name)
     logger.setLevel(logging.DEBUG)
     return logger
 
 
 def set_root_logger_handlers(logger_name, files_target_path):
     logger = logging.getLogger(logger_name)
-    logger.addHandler(get_file_handler(files_target_path))
     logger.addHandler(get_console_handler())
+    logger.addHandler(get_file_handler(files_target_path))
```

### Comparing `elementary-data-0.7.6/elementary/utils/ordered_yaml.py` & `elementary-data-0.7.7/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/utils/package.py` & `elementary-data-0.7.7/elementary/utils/package.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/utils/schema.py` & `elementary-data-0.7.7/elementary/utils/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary/utils/time.py` & `elementary-data-0.7.7/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.7.7/elementary_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.6
+Version: 0.7.7
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: databricks
 Provides-Extra: spark
+Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
 <img alt="Logo" src="static/header_git.png"/ width="1000">
 </p>
 
 <h2 align="center">
@@ -195,12 +196,14 @@
 <a href="https://github.com/edbizarro"><img src="https://avatars.githubusercontent.com/u/84926?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/Chintanvpatel"><img src="https://avatars.githubusercontent.com/u/1384301?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.6 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.7 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.6.2 Description-Content-Type: text/markdown
 Provides-Extra: snowflake Provides-Extra: bigquery Provides-Extra: redshift
 Provides-Extra: postgres Provides-Extra: databricks Provides-Extra: spark
-License-File: LICENSE
+Provides-Extra: all License-File: LICENSE
                                  width="1000">
          ***** Data observability for analytics & data engineers *****
 *** Monitor your data quality, operation and performance directly from your dbt
                                  project. ***
 [https://img.shields.io/badge/join-Slack-ff69b4] [https://img.shields.io/badge/
            docs-quickstart-orange] [License] left_text=Downloads"/>
   â­ï¸ Star the repo [static/star_github.png] â­ [Demo Â»](https://bit.ly/
```

### Comparing `elementary-data-0.7.6/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.7.7/elementary_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/setup.py` & `elementary-data-0.7.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 
 # The directory containing this file.
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file.
 README = (HERE / "README.md").read_text()
 
+ADAPTER_EXTRA_REQUIREMENTS = {
+    "snowflake": ["dbt-snowflake>=0.20,<2.0.0"],
+    "bigquery": ["dbt-bigquery>=0.20,<2.0.0"],
+    "redshift": ["dbt-redshift>=0.20,<2.0.0"],
+    "postgres": ["dbt-postgres>=0.20,<2.0.0"],
+    "databricks": ["dbt-databricks>=0.20,<2.0.0"],
+    "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
+}
+
+
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.7.6",
+    version="0.7.7",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
@@ -35,23 +45,19 @@
         "google-cloud-storage<3.0.0",
         "ruamel.yaml<1.0.0",
         "alive-progress<=2.3.1",
         "slack-sdk>=3.20.1,<4.0.0",
         "pytest-parametrization>=2022.2.1",
         "pydantic<2.0",
         "networkx>=2.3,<3",
-        "packaging>=20.9,<22.0",
+        "packaging>=20.9,<23.0",
     ],
     extras_require={
-        "snowflake": ["dbt-snowflake>=0.20,<2.0.0"],
-        "bigquery": ["dbt-bigquery>=0.20,<2.0.0"],
-        "redshift": ["dbt-redshift>=0.20,<2.0.0"],
-        "postgres": ["dbt-postgres>=0.20,<2.0.0"],
-        "databricks": ["dbt-databricks>=0.20,<2.0.0"],
-        "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
+        **ADAPTER_EXTRA_REQUIREMENTS,
+        "all": sum(ADAPTER_EXTRA_REQUIREMENTS.values(), []),
     },
     long_description_content_type="text/markdown",
     license="",
     url="https://github.com/elementary-data/elementary",
     author_email="or@elementary-data.com",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `elementary-data-0.7.6/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.7.7/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.7/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.7.7/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.7.7/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.7.7/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.7.7/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/group_alerts_by_table/utils.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.7.7/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/api/alerts/test_alerts_api.py` & `elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alerts_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.7/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.7.7/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.6/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.7.7/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*

