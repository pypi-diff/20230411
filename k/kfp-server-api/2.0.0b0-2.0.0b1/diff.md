# Comparing `tmp/kfp-server-api-2.0.0b0.tar.gz` & `tmp/kfp-server-api-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-server-api-2.0.0b0.tar", last modified: Wed Feb  8 18:19:09 2023, max compression
+gzip compressed data, was "kfp-server-api-2.0.0b1.tar", last modified: Tue Apr 11 20:46:53 2023, max compression
```

## Comparing `kfp-server-api-2.0.0b0.tar` & `kfp-server-api-2.0.0b1.tar`

### file list

```diff
@@ -1,145 +1,131 @@
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.300895 kfp-server-api-2.0.0b0/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    11357 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/LICENSE
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      446 2023-02-08 18:19:09.300895 kfp-server-api-2.0.0b0/PKG-INFO
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    13744 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/README.md
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.284895 kfp-server-api-2.0.0b0/kfp_server_api/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5435 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/__init__.py
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.288895 kfp-server-api-2.0.0b0/kfp_server_api/api/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      738 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/__init__.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     6214 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/auth_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    36215 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/experiment_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5358 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/healthz_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    56843 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/pipeline_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    14338 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/pipeline_upload_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    37131 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/recurring_run_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    11806 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/report_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    60827 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/run_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7057 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api/visualization_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    26257 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/api_client.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    13316 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/configuration.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3795 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/exceptions.py
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.292895 kfp-server-api-2.0.0b0/kfp_server_api/models/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4341 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/__init__.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3874 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_parameter.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7063 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_pipeline.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     8922 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_pipeline_version.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2913 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_relationship.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3997 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_key.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4909 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_reference.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3054 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_type.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4513 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3391 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/api_url.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2926 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/authorize_request_resources.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2939 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/authorize_request_verb.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5603 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/googlerpc_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3379 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_int_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3387 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_long_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3403 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_string_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7241 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_any.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3533 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_list_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2831 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_null_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3522 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_struct.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7513 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2908 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/recurring_run_mode.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3623 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_artifact_list.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4999 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_cron_schedule.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     8164 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_experiment.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2999 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_experiment_storage_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3616 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_filter.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3616 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_get_healthz_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5673 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_experiments_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5922 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5687 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_pipelines_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5803 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5361 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_runs_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5544 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_periodic_schedule.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     8024 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    15062 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_task_detail.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     8131 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     9872 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_version.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    10093 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_predicate.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3250 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_predicate_operation.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3903 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_read_artifact_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    18403 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_recurring_run.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2956 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_recurring_run_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    17689 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_run.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5847 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_run_details.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2971 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_run_storage_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4587 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_runtime_config.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3157 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_runtime_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4949 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_runtime_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4447 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_trigger.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3547 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_url.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7294 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_visualization.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2961 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_visualization_type.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)    12327 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/kfp_server_api/rest.py
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.288895 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      446 2023-02-08 18:19:09.000000 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/PKG-INFO
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5425 2023-02-08 18:19:09.000000 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/SOURCES.txt
--rw-r-----   0 ablai    (1040775) primarygroup (89939)        1 2023-02-08 18:19:09.000000 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/dependency_links.txt
--rw-r-----   0 ablai    (1040775) primarygroup (89939)       48 2023-02-08 18:19:09.000000 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/requires.txt
--rw-r-----   0 ablai    (1040775) primarygroup (89939)       15 2023-02-08 18:19:09.000000 kfp-server-api-2.0.0b0/kfp_server_api.egg-info/top_level.txt
--rw-r-----   0 ablai    (1040775) primarygroup (89939)       69 2023-02-08 18:19:09.300895 kfp-server-api-2.0.0b0/setup.cfg
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1197 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/setup.py
-drwxr-x---   0 ablai    (1040775) primarygroup (89939)        0 2023-02-08 18:19:09.300895 kfp-server-api-2.0.0b0/test/
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1423 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_parameter.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1784 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_pipeline.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2390 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_pipeline_version.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1399 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_relationship.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1464 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_resource_key.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1703 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_resource_reference.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1401 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_resource_type.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1592 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1335 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_api_url.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      849 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_auth_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1511 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_authorize_request_resources.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1456 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_authorize_request_verb.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2074 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_experiment_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1660 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_googlerpc_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      911 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_healthz_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2447 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_pipeline_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1043 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_pipeline_upload_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1506 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_predicate_int_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1518 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_predicate_long_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1540 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_predicate_string_values.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1419 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_protobuf_any.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2787 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_protobuf_list_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1423 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_protobuf_null_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2235 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_protobuf_struct.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3325 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_protobuf_value.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1412 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_recurring_run_mode.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2090 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_recurring_run_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      997 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_report_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2416 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_run_service_api.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1524 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_artifact_list.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1686 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_cron_schedule.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1734 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_experiment.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1557 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_experiment_storage_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2288 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_filter.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1547 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_get_healthz_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2140 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_list_experiments_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3852 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_list_pipeline_versions_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2478 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_list_pipelines_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5556 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_list_recurring_runs_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     7443 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_list_runs_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1741 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_periodic_schedule.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2022 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     4128 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_task_detail.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1863 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_task_executor_detail.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3229 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_version.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2265 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_predicate.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1511 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_predicate_operation.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1565 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_read_artifact_response.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     5928 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_recurring_run.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1513 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_recurring_run_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     8640 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_run.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     3993 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_run_details.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1480 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_run_storage_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2870 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_runtime_config.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1445 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_runtime_state.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1991 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_runtime_status.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     2119 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_trigger.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1379 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_url.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1613 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_visualization.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)     1500 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_v2beta1_visualization_type.py
--rw-r-----   0 ablai    (1040775) primarygroup (89939)      931 2023-02-08 18:18:39.000000 kfp-server-api-2.0.0b0/test/test_visualization_service_api.py
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11357 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/LICENSE
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      446 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/PKG-INFO
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    13256 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/README.md
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:52.997935 kfp-server-api-2.0.0b1/kfp_server_api/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5053 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/__init__.py
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.001936 kfp-server-api-2.0.0b1/kfp_server_api/api/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      738 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/__init__.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     6214 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/auth_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    36215 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/experiment_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5358 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/healthz_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    57807 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    14031 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_upload_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    37131 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/recurring_run_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11806 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/report_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    54490 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/run_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7057 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/visualization_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    26257 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/api_client.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    13316 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/configuration.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3795 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/exceptions.py
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.005936 kfp-server-api-2.0.0b1/kfp_server_api/models/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3959 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/__init__.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2926 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_resources.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2939 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_verb.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5603 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/googlerpc_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4512 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/pipeline_task_detail_child_task.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3379 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_int_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3387 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_long_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3403 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_string_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7241 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_any.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3533 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_list_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2831 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_null_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3522 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_struct.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7513 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2908 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/recurring_run_mode.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3623 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_artifact_list.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4999 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_cron_schedule.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8164 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2999 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment_storage_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3616 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_filter.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3616 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_get_healthz_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5673 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_experiments_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5922 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5687 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipelines_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5803 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5361 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_runs_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5544 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_periodic_schedule.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8024 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    17041 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_detail.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8131 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11265 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4853 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version_reference.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    10093 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3250 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate_operation.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3903 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_read_artifact_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    19559 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2956 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    18809 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5847 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_details.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2971 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_storage_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4587 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_config.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3157 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4949 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4447 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_trigger.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3547 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_url.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7294 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2961 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization_type.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)    12327 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/rest.py
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:52.997935 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      446 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/PKG-INFO
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5009 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/SOURCES.txt
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)        1 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/dependency_links.txt
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)       48 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/requires.txt
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)       15 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/top_level.txt
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)       69 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/setup.cfg
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1197 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/setup.py
+drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/test/
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      849 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_auth_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1511 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_authorize_request_resources.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1456 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_authorize_request_verb.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2074 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_experiment_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1660 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_googlerpc_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      911 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_healthz_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2447 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1600 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_task_detail_child_task.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1043 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_upload_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1506 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_int_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1518 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_long_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1540 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_string_values.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1419 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_protobuf_any.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2787 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_list_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1423 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_protobuf_null_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2235 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_struct.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3325 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_value.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1412 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_recurring_run_mode.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2090 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_recurring_run_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      997 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_report_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2416 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_run_service_api.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1524 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_artifact_list.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1686 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_cron_schedule.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1734 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_experiment.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1557 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_experiment_storage_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2288 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_filter.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1547 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_get_healthz_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2140 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_experiments_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3900 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipeline_versions_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2478 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipelines_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5806 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_recurring_runs_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8087 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_runs_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1741 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_periodic_schedule.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2022 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4402 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_detail.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1863 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_executor_detail.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3269 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1657 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version_reference.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2265 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_predicate.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1511 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_predicate_operation.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1565 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_read_artifact_response.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     6154 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1513 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     9212 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4315 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run_details.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1480 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run_storage_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2870 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_config.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1445 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_state.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1991 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_status.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2119 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_trigger.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1379 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_url.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1613 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_visualization.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1500 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_visualization_type.py
+-rw-r-----   0 lingqinggan (973760) primarygroup (89939)      931 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_visualization_service_api.py
```

### Comparing `kfp-server-api-2.0.0b0/LICENSE` & `kfp-server-api-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/README.md` & `kfp-server-api-2.0.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kfp-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.0-beta.0
-- Package version: 2.0.0-beta.0
+- API version: 2.0.0-beta.1
+- Package version: 2.0.0-beta.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -120,40 +120,32 @@
 *RecurringRunServiceApi* | [**delete_recurring_run**](docs/RecurringRunServiceApi.md#delete_recurring_run) | **DELETE** /apis/v2beta1/recurringruns/{recurring_run_id} | Deletes a recurring run.
 *RecurringRunServiceApi* | [**disable_recurring_run**](docs/RecurringRunServiceApi.md#disable_recurring_run) | **POST** /apis/v2beta1/recurringruns/{recurring_run_id}:disable | Stops a recurring run and all its associated runs. The recurring run is not deleted.
 *RecurringRunServiceApi* | [**enable_recurring_run**](docs/RecurringRunServiceApi.md#enable_recurring_run) | **POST** /apis/v2beta1/recurringruns/{recurring_run_id}:enable | Restarts a recurring run that was previously stopped. All runs associated with the  recurring run will continue.
 *RecurringRunServiceApi* | [**get_recurring_run**](docs/RecurringRunServiceApi.md#get_recurring_run) | **GET** /apis/v2beta1/recurringruns/{recurring_run_id} | Finds a specific recurring run by ID.
 *RecurringRunServiceApi* | [**list_recurring_runs**](docs/RecurringRunServiceApi.md#list_recurring_runs) | **GET** /apis/v2beta1/recurringruns | Finds all recurring runs given experiment and namespace.  If experiment ID is not specified, find all recurring runs across all experiments.
 *ReportServiceApi* | [**report_scheduled_workflow**](docs/ReportServiceApi.md#report_scheduled_workflow) | **POST** /apis/v2beta1/scheduledworkflows | 
 *ReportServiceApi* | [**report_workflow**](docs/ReportServiceApi.md#report_workflow) | **POST** /apis/v2beta1/workflows | 
-*RunServiceApi* | [**archive_run**](docs/RunServiceApi.md#archive_run) | **POST** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:archive | Archives a run in an experiment given by run ID and experiment ID.
-*RunServiceApi* | [**create_run**](docs/RunServiceApi.md#create_run) | **POST** /apis/v2beta1/experiments/{experiment_id}/runs | Creates a new run in an experiment specified by experiment ID.  If experiment ID is not specified, the run is created in the default experiment.
-*RunServiceApi* | [**delete_run**](docs/RunServiceApi.md#delete_run) | **DELETE** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id} | Deletes a run in an experiment given by run ID and experiment ID.
-*RunServiceApi* | [**get_run**](docs/RunServiceApi.md#get_run) | **GET** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id} | Finds a specific run by ID.
-*RunServiceApi* | [**list_runs**](docs/RunServiceApi.md#list_runs) | **GET** /apis/v2beta1/experiments/{experiment_id}/runs | Finds all runs in an experiment given by experiment ID.  If experiment id is not specified, finds all runs across all experiments.
-*RunServiceApi* | [**read_artifact**](docs/RunServiceApi.md#read_artifact) | **GET** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id}/nodes/{node_id}/artifacts/{artifact_name}:read | Finds artifact data in a run.
-*RunServiceApi* | [**retry_run**](docs/RunServiceApi.md#retry_run) | **POST** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:retry | Re-initiates a failed or terminated run.
-*RunServiceApi* | [**terminate_run**](docs/RunServiceApi.md#terminate_run) | **POST** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:terminate | Terminates an active run.
-*RunServiceApi* | [**unarchive_run**](docs/RunServiceApi.md#unarchive_run) | **POST** /apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:unarchive | Restores an archived run in an experiment given by run ID and experiment ID.
+*RunServiceApi* | [**archive_run**](docs/RunServiceApi.md#archive_run) | **POST** /apis/v2beta1/runs/{run_id}:archive | Archives a run in an experiment given by run ID and experiment ID.
+*RunServiceApi* | [**create_run**](docs/RunServiceApi.md#create_run) | **POST** /apis/v2beta1/runs | Creates a new run in an experiment specified by experiment ID.  If experiment ID is not specified, the run is created in the default experiment.
+*RunServiceApi* | [**delete_run**](docs/RunServiceApi.md#delete_run) | **DELETE** /apis/v2beta1/runs/{run_id} | Deletes a run in an experiment given by run ID and experiment ID.
+*RunServiceApi* | [**get_run**](docs/RunServiceApi.md#get_run) | **GET** /apis/v2beta1/runs/{run_id} | Finds a specific run by ID.
+*RunServiceApi* | [**list_runs**](docs/RunServiceApi.md#list_runs) | **GET** /apis/v2beta1/runs | Finds all runs in an experiment given by experiment ID.  If experiment id is not specified, finds all runs across all experiments.
+*RunServiceApi* | [**read_artifact**](docs/RunServiceApi.md#read_artifact) | **GET** /apis/v2beta1/runs/{run_id}/nodes/{node_id}/artifacts/{artifact_name}:read | Finds artifact data in a run.
+*RunServiceApi* | [**retry_run**](docs/RunServiceApi.md#retry_run) | **POST** /apis/v2beta1/runs/{run_id}:retry | Re-initiates a failed or terminated run.
+*RunServiceApi* | [**terminate_run**](docs/RunServiceApi.md#terminate_run) | **POST** /apis/v2beta1/runs/{run_id}:terminate | Terminates an active run.
+*RunServiceApi* | [**unarchive_run**](docs/RunServiceApi.md#unarchive_run) | **POST** /apis/v2beta1/runs/{run_id}:unarchive | Restores an archived run in an experiment given by run ID and experiment ID.
 *VisualizationServiceApi* | [**create_visualization_v1**](docs/VisualizationServiceApi.md#create_visualization_v1) | **POST** /apis/v2beta1/visualizations/{namespace} | 
 
 
 ## Documentation For Models
 
- - [ApiParameter](docs/ApiParameter.md)
- - [ApiPipeline](docs/ApiPipeline.md)
- - [ApiPipelineVersion](docs/ApiPipelineVersion.md)
- - [ApiRelationship](docs/ApiRelationship.md)
- - [ApiResourceKey](docs/ApiResourceKey.md)
- - [ApiResourceReference](docs/ApiResourceReference.md)
- - [ApiResourceType](docs/ApiResourceType.md)
- - [ApiStatus](docs/ApiStatus.md)
- - [ApiUrl](docs/ApiUrl.md)
  - [AuthorizeRequestResources](docs/AuthorizeRequestResources.md)
  - [AuthorizeRequestVerb](docs/AuthorizeRequestVerb.md)
  - [GooglerpcStatus](docs/GooglerpcStatus.md)
+ - [PipelineTaskDetailChildTask](docs/PipelineTaskDetailChildTask.md)
  - [PredicateIntValues](docs/PredicateIntValues.md)
  - [PredicateLongValues](docs/PredicateLongValues.md)
  - [PredicateStringValues](docs/PredicateStringValues.md)
  - [ProtobufAny](docs/ProtobufAny.md)
  - [ProtobufListValue](docs/ProtobufListValue.md)
  - [ProtobufNullValue](docs/ProtobufNullValue.md)
  - [ProtobufStruct](docs/ProtobufStruct.md)
@@ -171,14 +163,15 @@
  - [V2beta1ListRecurringRunsResponse](docs/V2beta1ListRecurringRunsResponse.md)
  - [V2beta1ListRunsResponse](docs/V2beta1ListRunsResponse.md)
  - [V2beta1PeriodicSchedule](docs/V2beta1PeriodicSchedule.md)
  - [V2beta1Pipeline](docs/V2beta1Pipeline.md)
  - [V2beta1PipelineTaskDetail](docs/V2beta1PipelineTaskDetail.md)
  - [V2beta1PipelineTaskExecutorDetail](docs/V2beta1PipelineTaskExecutorDetail.md)
  - [V2beta1PipelineVersion](docs/V2beta1PipelineVersion.md)
+ - [V2beta1PipelineVersionReference](docs/V2beta1PipelineVersionReference.md)
  - [V2beta1Predicate](docs/V2beta1Predicate.md)
  - [V2beta1PredicateOperation](docs/V2beta1PredicateOperation.md)
  - [V2beta1ReadArtifactResponse](docs/V2beta1ReadArtifactResponse.md)
  - [V2beta1RecurringRun](docs/V2beta1RecurringRun.md)
  - [V2beta1RecurringRunStatus](docs/V2beta1RecurringRunStatus.md)
  - [V2beta1Run](docs/V2beta1Run.md)
  - [V2beta1RunDetails](docs/V2beta1RunDetails.md)
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/__init__.py` & `kfp-server-api-2.0.0b1/kfp_server_api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.0.0-beta.0"
+__version__ = "2.0.0-beta.1"
 
 # import apis into sdk package
 from kfp_server_api.api.auth_service_api import AuthServiceApi
 from kfp_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
@@ -32,26 +32,18 @@
 from kfp_server_api.configuration import Configuration
 from kfp_server_api.exceptions import OpenApiException
 from kfp_server_api.exceptions import ApiTypeError
 from kfp_server_api.exceptions import ApiValueError
 from kfp_server_api.exceptions import ApiKeyError
 from kfp_server_api.exceptions import ApiException
 # import models into sdk package
-from kfp_server_api.models.api_parameter import ApiParameter
-from kfp_server_api.models.api_pipeline import ApiPipeline
-from kfp_server_api.models.api_pipeline_version import ApiPipelineVersion
-from kfp_server_api.models.api_relationship import ApiRelationship
-from kfp_server_api.models.api_resource_key import ApiResourceKey
-from kfp_server_api.models.api_resource_reference import ApiResourceReference
-from kfp_server_api.models.api_resource_type import ApiResourceType
-from kfp_server_api.models.api_status import ApiStatus
-from kfp_server_api.models.api_url import ApiUrl
 from kfp_server_api.models.authorize_request_resources import AuthorizeRequestResources
 from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb
 from kfp_server_api.models.googlerpc_status import GooglerpcStatus
+from kfp_server_api.models.pipeline_task_detail_child_task import PipelineTaskDetailChildTask
 from kfp_server_api.models.predicate_int_values import PredicateIntValues
 from kfp_server_api.models.predicate_long_values import PredicateLongValues
 from kfp_server_api.models.predicate_string_values import PredicateStringValues
 from kfp_server_api.models.protobuf_any import ProtobufAny
 from kfp_server_api.models.protobuf_list_value import ProtobufListValue
 from kfp_server_api.models.protobuf_null_value import ProtobufNullValue
 from kfp_server_api.models.protobuf_struct import ProtobufStruct
@@ -69,14 +61,15 @@
 from kfp_server_api.models.v2beta1_list_recurring_runs_response import V2beta1ListRecurringRunsResponse
 from kfp_server_api.models.v2beta1_list_runs_response import V2beta1ListRunsResponse
 from kfp_server_api.models.v2beta1_periodic_schedule import V2beta1PeriodicSchedule
 from kfp_server_api.models.v2beta1_pipeline import V2beta1Pipeline
 from kfp_server_api.models.v2beta1_pipeline_task_detail import V2beta1PipelineTaskDetail
 from kfp_server_api.models.v2beta1_pipeline_task_executor_detail import V2beta1PipelineTaskExecutorDetail
 from kfp_server_api.models.v2beta1_pipeline_version import V2beta1PipelineVersion
+from kfp_server_api.models.v2beta1_pipeline_version_reference import V2beta1PipelineVersionReference
 from kfp_server_api.models.v2beta1_predicate import V2beta1Predicate
 from kfp_server_api.models.v2beta1_predicate_operation import V2beta1PredicateOperation
 from kfp_server_api.models.v2beta1_read_artifact_response import V2beta1ReadArtifactResponse
 from kfp_server_api.models.v2beta1_recurring_run import V2beta1RecurringRun
 from kfp_server_api.models.v2beta1_recurring_run_status import V2beta1RecurringRunStatus
 from kfp_server_api.models.v2beta1_run import V2beta1Run
 from kfp_server_api.models.v2beta1_run_details import V2beta1RunDetails
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/__init__.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/auth_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/experiment_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/healthz_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/pipeline_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,25 +158,27 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_pipeline_version(self, pipeline_id, **kwargs):  # noqa: E501
+    def create_pipeline_version(self, pipeline_id, body, **kwargs):  # noqa: E501
         """Adds a pipeline version to the specified pipeline ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline_version(pipeline_id, async_req=True)
+        >>> thread = api.create_pipeline_version(pipeline_id, body, async_req=True)
         >>> result = thread.get()
 
         :param pipeline_id: Required input. ID of the parent pipeline. (required)
         :type pipeline_id: str
+        :param body: Required input. Pipeline version ID to be created. (required)
+        :type body: V2beta1PipelineVersion
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -184,27 +186,29 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V2beta1PipelineVersion
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_pipeline_version_with_http_info(pipeline_id, **kwargs)  # noqa: E501
+        return self.create_pipeline_version_with_http_info(pipeline_id, body, **kwargs)  # noqa: E501
 
-    def create_pipeline_version_with_http_info(self, pipeline_id, **kwargs):  # noqa: E501
+    def create_pipeline_version_with_http_info(self, pipeline_id, body, **kwargs):  # noqa: E501
         """Adds a pipeline version to the specified pipeline ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline_version_with_http_info(pipeline_id, async_req=True)
+        >>> thread = api.create_pipeline_version_with_http_info(pipeline_id, body, async_req=True)
         >>> result = thread.get()
 
         :param pipeline_id: Required input. ID of the parent pipeline. (required)
         :type pipeline_id: str
+        :param body: Required input. Pipeline version ID to be created. (required)
+        :type body: V2beta1PipelineVersion
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -219,15 +223,16 @@
                  returns the request thread.
         :rtype: tuple(V2beta1PipelineVersion, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'pipeline_id'
+            'pipeline_id',
+            'body'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -242,14 +247,18 @@
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'pipeline_id' is set
         if self.api_client.client_side_validation and ('pipeline_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['pipeline_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `pipeline_id` when calling `create_pipeline_version`")  # noqa: E501
+        # verify the required parameter 'body' is set
+        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
+                                                        local_var_params['body'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `body` when calling `create_pipeline_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'pipeline_id' in local_var_params:
             path_params['pipeline_id'] = local_var_params['pipeline_id']  # noqa: E501
 
@@ -257,18 +266,24 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
             '/apis/v2beta1/pipelines/{pipeline_id}/versions', 'POST',
             path_params,
             query_params,
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/pipeline_upload_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_upload_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ApiPipeline
+        :rtype: V2beta1Pipeline
         """
         kwargs['_return_http_data_only'] = True
         return self.upload_pipeline_with_http_info(uploadfile, **kwargs)  # noqa: E501
 
     def upload_pipeline_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
         """upload_pipeline  # noqa: E501
 
@@ -99,15 +99,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ApiPipeline, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V2beta1Pipeline, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'uploadfile',
             'name',
@@ -171,15 +171,15 @@
             '/apis/v2beta1/pipelines/upload', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ApiPipeline',  # noqa: E501
+            response_type='V2beta1Pipeline',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -196,29 +196,27 @@
         :type uploadfile: file
         :param name:
         :type name: str
         :param pipelineid:
         :type pipelineid: str
         :param description:
         :type description: str
-        :param namespace:
-        :type namespace: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ApiPipelineVersion
+        :rtype: V2beta1PipelineVersion
         """
         kwargs['_return_http_data_only'] = True
         return self.upload_pipeline_version_with_http_info(uploadfile, **kwargs)  # noqa: E501
 
     def upload_pipeline_version_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
         """upload_pipeline_version  # noqa: E501
 
@@ -232,16 +230,14 @@
         :type uploadfile: file
         :param name:
         :type name: str
         :param pipelineid:
         :type pipelineid: str
         :param description:
         :type description: str
-        :param namespace:
-        :type namespace: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -250,25 +246,24 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ApiPipelineVersion, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V2beta1PipelineVersion, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'uploadfile',
             'name',
             'pipelineid',
-            'description',
-            'namespace'
+            'description'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -295,16 +290,14 @@
         query_params = []
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
             query_params.append(('name', local_var_params['name']))  # noqa: E501
         if 'pipelineid' in local_var_params and local_var_params['pipelineid'] is not None:  # noqa: E501
             query_params.append(('pipelineid', local_var_params['pipelineid']))  # noqa: E501
         if 'description' in local_var_params and local_var_params['description'] is not None:  # noqa: E501
             query_params.append(('description', local_var_params['description']))  # noqa: E501
-        if 'namespace' in local_var_params and local_var_params['namespace'] is not None:  # noqa: E501
-            query_params.append(('namespace', local_var_params['namespace']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
         if 'uploadfile' in local_var_params:
             local_var_files['uploadfile'] = local_var_params['uploadfile']  # noqa: E501
@@ -325,14 +318,14 @@
             '/apis/v2beta1/pipelines/upload_version', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ApiPipelineVersion',  # noqa: E501
+            response_type='V2beta1PipelineVersion',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/recurring_run_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/report_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/run_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/run_service_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,25 +32,23 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def archive_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def archive_run(self, run_id, **kwargs):  # noqa: E501
         """Archives a run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.archive_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be archived. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -60,27 +58,25 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.archive_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.archive_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def archive_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def archive_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Archives a run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.archive_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be archived. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -97,15 +93,14 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -117,28 +112,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method archive_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `archive_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `archive_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
@@ -150,40 +139,38 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:archive', 'POST',
+            '/apis/v2beta1/runs/{run_id}:archive', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_run(self, experiment_id, body, **kwargs):  # noqa: E501
+    def create_run(self, body, **kwargs):  # noqa: E501
         """Creates a new run in an experiment specified by experiment ID.  If experiment ID is not specified, the run is created in the default experiment.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_run(experiment_id, body, async_req=True)
+        >>> thread = api.create_run(body, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param body: Run to be created. (required)
         :type body: V2beta1Run
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -193,27 +180,25 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V2beta1Run
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_run_with_http_info(experiment_id, body, **kwargs)  # noqa: E501
+        return self.create_run_with_http_info(body, **kwargs)  # noqa: E501
 
-    def create_run_with_http_info(self, experiment_id, body, **kwargs):  # noqa: E501
+    def create_run_with_http_info(self, body, **kwargs):  # noqa: E501
         """Creates a new run in an experiment specified by experiment ID.  If experiment ID is not specified, the run is created in the default experiment.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_run_with_http_info(experiment_id, body, async_req=True)
+        >>> thread = api.create_run_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param body: Run to be created. (required)
         :type body: V2beta1Run
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -230,15 +215,14 @@
                  returns the request thread.
         :rtype: tuple(V2beta1Run, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'body'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -250,28 +234,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `create_run`")  # noqa: E501
         # verify the required parameter 'body' is set
         if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
                                                         local_var_params['body'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `body` when calling `create_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -287,42 +265,42 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs', 'POST',
+            '/apis/v2beta1/runs', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V2beta1Run',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def delete_run(self, run_id, **kwargs):  # noqa: E501
         """Deletes a run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.delete_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be deleted. (required)
         :type run_id: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -330,29 +308,29 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.delete_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def delete_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def delete_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Deletes a run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.delete_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be deleted. (required)
         :type run_id: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -367,16 +345,16 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
-            'run_id'
+            'run_id',
+            'experiment_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -387,32 +365,28 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method delete_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `delete_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `delete_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
+        if 'experiment_id' in local_var_params and local_var_params['experiment_id'] is not None:  # noqa: E501
+            query_params.append(('experiment_id', local_var_params['experiment_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -420,42 +394,42 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}', 'DELETE',
+            '/apis/v2beta1/runs/{run_id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def get_run(self, run_id, **kwargs):  # noqa: E501
         """Finds a specific run by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.get_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be retrieved. (required)
         :type run_id: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -463,29 +437,29 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V2beta1Run
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.get_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def get_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def get_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Finds a specific run by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.get_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be retrieved. (required)
         :type run_id: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -500,16 +474,16 @@
                  returns the request thread.
         :rtype: tuple(V2beta1Run, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
-            'run_id'
+            'run_id',
+            'experiment_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -520,32 +494,28 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method get_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `get_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `get_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
+        if 'experiment_id' in local_var_params and local_var_params['experiment_id'] is not None:  # noqa: E501
+            query_params.append(('experiment_id', local_var_params['experiment_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -553,42 +523,42 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}', 'GET',
+            '/apis/v2beta1/runs/{run_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V2beta1Run',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_runs(self, experiment_id, **kwargs):  # noqa: E501
+    def list_runs(self, **kwargs):  # noqa: E501
         """Finds all runs in an experiment given by experiment ID.  If experiment id is not specified, finds all runs across all experiments.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_runs(experiment_id, async_req=True)
+        >>> thread = api.list_runs(async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. If empty, response includes runs across all experiments. (required)
-        :type experiment_id: str
         :param namespace: Optional input field. Filters based on the namespace.
         :type namespace: str
+        :param experiment_id: The ID of the parent experiment. If empty, response includes runs across all experiments.
+        :type experiment_id: str
         :param page_token: A page token to request the next page of results. The token is acquired from the nextPageToken field of the response from the previous ListRuns call or can be omitted when fetching the first page.
         :type page_token: str
         :param page_size: The number of runs to be listed per page. If there are more runs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
         :type page_size: int
         :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" (Example, \"name asc\" or \"id desc\"). Ascending by default.
         :type sort_by: str
         :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
@@ -604,29 +574,29 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V2beta1ListRunsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_runs_with_http_info(experiment_id, **kwargs)  # noqa: E501
+        return self.list_runs_with_http_info(**kwargs)  # noqa: E501
 
-    def list_runs_with_http_info(self, experiment_id, **kwargs):  # noqa: E501
+    def list_runs_with_http_info(self, **kwargs):  # noqa: E501
         """Finds all runs in an experiment given by experiment ID.  If experiment id is not specified, finds all runs across all experiments.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_runs_with_http_info(experiment_id, async_req=True)
+        >>> thread = api.list_runs_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. If empty, response includes runs across all experiments. (required)
-        :type experiment_id: str
         :param namespace: Optional input field. Filters based on the namespace.
         :type namespace: str
+        :param experiment_id: The ID of the parent experiment. If empty, response includes runs across all experiments.
+        :type experiment_id: str
         :param page_token: A page token to request the next page of results. The token is acquired from the nextPageToken field of the response from the previous ListRuns call or can be omitted when fetching the first page.
         :type page_token: str
         :param page_size: The number of runs to be listed per page. If there are more runs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
         :type page_size: int
         :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" (Example, \"name asc\" or \"id desc\"). Ascending by default.
         :type sort_by: str
         :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
@@ -649,16 +619,16 @@
                  returns the request thread.
         :rtype: tuple(V2beta1ListRunsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'namespace',
+            'experiment_id',
             'page_token',
             'page_size',
             'sort_by',
             'filter'
         ]
         all_params.extend(
             [
@@ -673,28 +643,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method list_runs" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `list_runs`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
 
         query_params = []
         if 'namespace' in local_var_params and local_var_params['namespace'] is not None:  # noqa: E501
             query_params.append(('namespace', local_var_params['namespace']))  # noqa: E501
+        if 'experiment_id' in local_var_params and local_var_params['experiment_id'] is not None:  # noqa: E501
+            query_params.append(('experiment_id', local_var_params['experiment_id']))  # noqa: E501
         if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
             query_params.append(('page_token', local_var_params['page_token']))  # noqa: E501
         if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
             query_params.append(('page_size', local_var_params['page_size']))  # noqa: E501
         if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
             query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
         if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
@@ -710,46 +676,46 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs', 'GET',
+            '/apis/v2beta1/runs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V2beta1ListRunsResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read_artifact(self, experiment_id, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
+    def read_artifact(self, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
         """Finds artifact data in a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_artifact(experiment_id, run_id, node_id, artifact_name, async_req=True)
+        >>> thread = api.read_artifact(run_id, node_id, artifact_name, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: ID of the run. (required)
         :type run_id: str
         :param node_id: ID of the running node. (required)
         :type node_id: str
         :param artifact_name: Name of the artifact. (required)
         :type artifact_name: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -757,33 +723,33 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V2beta1ReadArtifactResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_artifact_with_http_info(experiment_id, run_id, node_id, artifact_name, **kwargs)  # noqa: E501
+        return self.read_artifact_with_http_info(run_id, node_id, artifact_name, **kwargs)  # noqa: E501
 
-    def read_artifact_with_http_info(self, experiment_id, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
+    def read_artifact_with_http_info(self, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
         """Finds artifact data in a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_artifact_with_http_info(experiment_id, run_id, node_id, artifact_name, async_req=True)
+        >>> thread = api.read_artifact_with_http_info(run_id, node_id, artifact_name, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: ID of the run. (required)
         :type run_id: str
         :param node_id: ID of the running node. (required)
         :type node_id: str
         :param artifact_name: Name of the artifact. (required)
         :type artifact_name: str
+        :param experiment_id: The ID of the parent experiment.
+        :type experiment_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -798,18 +764,18 @@
                  returns the request thread.
         :rtype: tuple(V2beta1ReadArtifactResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'run_id',
             'node_id',
-            'artifact_name'
+            'artifact_name',
+            'experiment_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -820,18 +786,14 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read_artifact" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `read_artifact`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `read_artifact`")  # noqa: E501
         # verify the required parameter 'node_id' is set
         if self.api_client.client_side_validation and ('node_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['node_id'] is None):  # noqa: E501
@@ -840,24 +802,24 @@
         if self.api_client.client_side_validation and ('artifact_name' not in local_var_params or  # noqa: E501
                                                         local_var_params['artifact_name'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `artifact_name` when calling `read_artifact`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
         if 'node_id' in local_var_params:
             path_params['node_id'] = local_var_params['node_id']  # noqa: E501
         if 'artifact_name' in local_var_params:
             path_params['artifact_name'] = local_var_params['artifact_name']  # noqa: E501
 
         query_params = []
+        if 'experiment_id' in local_var_params and local_var_params['experiment_id'] is not None:  # noqa: E501
+            query_params.append(('experiment_id', local_var_params['experiment_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -865,40 +827,38 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}/nodes/{node_id}/artifacts/{artifact_name}:read', 'GET',
+            '/apis/v2beta1/runs/{run_id}/nodes/{node_id}/artifacts/{artifact_name}:read', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V2beta1ReadArtifactResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retry_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def retry_run(self, run_id, **kwargs):  # noqa: E501
         """Re-initiates a failed or terminated run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.retry_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.retry_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be retried. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -908,27 +868,25 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.retry_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.retry_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def retry_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def retry_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Re-initiates a failed or terminated run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.retry_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.retry_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be retried. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -945,15 +903,14 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -965,28 +922,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method retry_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `retry_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `retry_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
@@ -998,40 +949,38 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:retry', 'POST',
+            '/apis/v2beta1/runs/{run_id}:retry', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def terminate_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def terminate_run(self, run_id, **kwargs):  # noqa: E501
         """Terminates an active run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.terminate_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.terminate_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be terminated. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1041,27 +990,25 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.terminate_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.terminate_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def terminate_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def terminate_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Terminates an active run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.terminate_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.terminate_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be terminated. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1078,15 +1025,14 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1098,28 +1044,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method terminate_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `terminate_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `terminate_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
@@ -1131,40 +1071,38 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:terminate', 'POST',
+            '/apis/v2beta1/runs/{run_id}:terminate', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def unarchive_run(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def unarchive_run(self, run_id, **kwargs):  # noqa: E501
         """Restores an archived run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unarchive_run(experiment_id, run_id, async_req=True)
+        >>> thread = api.unarchive_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be restored. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1174,27 +1112,25 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.unarchive_run_with_http_info(experiment_id, run_id, **kwargs)  # noqa: E501
+        return self.unarchive_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def unarchive_run_with_http_info(self, experiment_id, run_id, **kwargs):  # noqa: E501
+    def unarchive_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
         """Restores an archived run in an experiment given by run ID and experiment ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unarchive_run_with_http_info(experiment_id, run_id, async_req=True)
+        >>> thread = api.unarchive_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param experiment_id: The ID of the parent experiment. (required)
-        :type experiment_id: str
         :param run_id: The ID of the run to be restored. (required)
         :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1211,15 +1147,14 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'experiment_id',
             'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1231,28 +1166,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method unarchive_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'experiment_id' is set
-        if self.api_client.client_side_validation and ('experiment_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['experiment_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `experiment_id` when calling `unarchive_run`")  # noqa: E501
         # verify the required parameter 'run_id' is set
         if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['run_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `run_id` when calling `unarchive_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'experiment_id' in local_var_params:
-            path_params['experiment_id'] = local_var_params['experiment_id']  # noqa: E501
         if 'run_id' in local_var_params:
             path_params['run_id'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
@@ -1264,15 +1193,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v2beta1/experiments/{experiment_id}/runs/{run_id}:unarchive', 'POST',
+            '/apis/v2beta1/runs/{run_id}:unarchive', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api/visualization_service_api.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api/visualization_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/api_client.py` & `kfp-server-api-2.0.0b1/kfp_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0-beta.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.0-beta.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/configuration.py` & `kfp-server-api-2.0.0b1/kfp_server_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.0-beta.0\n"\
-               "SDK Package Version: 2.0.0-beta.0".\
+               "Version of the API: 2.0.0-beta.1\n"\
+               "SDK Package Version: 2.0.0-beta.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/exceptions.py` & `kfp-server-api-2.0.0b1/kfp_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/__init__.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
-from kfp_server_api.models.api_parameter import ApiParameter
-from kfp_server_api.models.api_pipeline import ApiPipeline
-from kfp_server_api.models.api_pipeline_version import ApiPipelineVersion
-from kfp_server_api.models.api_relationship import ApiRelationship
-from kfp_server_api.models.api_resource_key import ApiResourceKey
-from kfp_server_api.models.api_resource_reference import ApiResourceReference
-from kfp_server_api.models.api_resource_type import ApiResourceType
-from kfp_server_api.models.api_status import ApiStatus
-from kfp_server_api.models.api_url import ApiUrl
 from kfp_server_api.models.authorize_request_resources import AuthorizeRequestResources
 from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb
 from kfp_server_api.models.googlerpc_status import GooglerpcStatus
+from kfp_server_api.models.pipeline_task_detail_child_task import PipelineTaskDetailChildTask
 from kfp_server_api.models.predicate_int_values import PredicateIntValues
 from kfp_server_api.models.predicate_long_values import PredicateLongValues
 from kfp_server_api.models.predicate_string_values import PredicateStringValues
 from kfp_server_api.models.protobuf_any import ProtobufAny
 from kfp_server_api.models.protobuf_list_value import ProtobufListValue
 from kfp_server_api.models.protobuf_null_value import ProtobufNullValue
 from kfp_server_api.models.protobuf_struct import ProtobufStruct
@@ -47,14 +39,15 @@
 from kfp_server_api.models.v2beta1_list_recurring_runs_response import V2beta1ListRecurringRunsResponse
 from kfp_server_api.models.v2beta1_list_runs_response import V2beta1ListRunsResponse
 from kfp_server_api.models.v2beta1_periodic_schedule import V2beta1PeriodicSchedule
 from kfp_server_api.models.v2beta1_pipeline import V2beta1Pipeline
 from kfp_server_api.models.v2beta1_pipeline_task_detail import V2beta1PipelineTaskDetail
 from kfp_server_api.models.v2beta1_pipeline_task_executor_detail import V2beta1PipelineTaskExecutorDetail
 from kfp_server_api.models.v2beta1_pipeline_version import V2beta1PipelineVersion
+from kfp_server_api.models.v2beta1_pipeline_version_reference import V2beta1PipelineVersionReference
 from kfp_server_api.models.v2beta1_predicate import V2beta1Predicate
 from kfp_server_api.models.v2beta1_predicate_operation import V2beta1PredicateOperation
 from kfp_server_api.models.v2beta1_read_artifact_response import V2beta1ReadArtifactResponse
 from kfp_server_api.models.v2beta1_recurring_run import V2beta1RecurringRun
 from kfp_server_api.models.v2beta1_recurring_run_status import V2beta1RecurringRunStatus
 from kfp_server_api.models.v2beta1_run import V2beta1Run
 from kfp_server_api.models.v2beta1_run_details import V2beta1RunDetails
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_parameter.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/pipeline_task_detail_child_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,94 +14,98 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiParameter(object):
+class PipelineTaskDetailChildTask(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'value': 'str'
+        'task_id': 'str',
+        'pod_name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'value': 'value'
+        'task_id': 'task_id',
+        'pod_name': 'pod_name'
     }
 
-    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
-        """ApiParameter - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, task_id=None, pod_name=None, local_vars_configuration=None):  # noqa: E501
+        """PipelineTaskDetailChildTask - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._value = None
+        self._task_id = None
+        self._pod_name = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if value is not None:
-            self.value = value
+        if task_id is not None:
+            self.task_id = task_id
+        if pod_name is not None:
+            self.pod_name = pod_name
 
     @property
-    def name(self):
-        """Gets the name of this ApiParameter.  # noqa: E501
+    def task_id(self):
+        """Gets the task_id of this PipelineTaskDetailChildTask.  # noqa: E501
 
+        System-generated ID of a task.  # noqa: E501
 
-        :return: The name of this ApiParameter.  # noqa: E501
+        :return: The task_id of this PipelineTaskDetailChildTask.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._task_id
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ApiParameter.
+    @task_id.setter
+    def task_id(self, task_id):
+        """Sets the task_id of this PipelineTaskDetailChildTask.
 
+        System-generated ID of a task.  # noqa: E501
 
-        :param name: The name of this ApiParameter.  # noqa: E501
-        :type name: str
+        :param task_id: The task_id of this PipelineTaskDetailChildTask.  # noqa: E501
+        :type task_id: str
         """
 
-        self._name = name
+        self._task_id = task_id
 
     @property
-    def value(self):
-        """Gets the value of this ApiParameter.  # noqa: E501
+    def pod_name(self):
+        """Gets the pod_name of this PipelineTaskDetailChildTask.  # noqa: E501
 
+        Name of the corresponding pod assigned by the orchestration engine. Also known as node_id.  # noqa: E501
 
-        :return: The value of this ApiParameter.  # noqa: E501
+        :return: The pod_name of this PipelineTaskDetailChildTask.  # noqa: E501
         :rtype: str
         """
-        return self._value
+        return self._pod_name
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this ApiParameter.
+    @pod_name.setter
+    def pod_name(self, pod_name):
+        """Sets the pod_name of this PipelineTaskDetailChildTask.
 
+        Name of the corresponding pod assigned by the orchestration engine. Also known as node_id.  # noqa: E501
 
-        :param value: The value of this ApiParameter.  # noqa: E501
-        :type value: str
+        :param pod_name: The pod_name of this PipelineTaskDetailChildTask.  # noqa: E501
+        :type pod_name: str
         """
 
-        self._value = value
+        self._pod_name = pod_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +133,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiParameter):
+        if not isinstance(other, PipelineTaskDetailChildTask):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiParameter):
+        if not isinstance(other, PipelineTaskDetailChildTask):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_pipeline.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,197 +14,205 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiPipeline(object):
+class V2beta1Pipeline(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
-        'created_at': 'datetime',
-        'name': 'str',
+        'pipeline_id': 'str',
+        'display_name': 'str',
         'description': 'str',
-        'parameters': 'list[ApiParameter]',
-        'error': 'str'
+        'created_at': 'datetime',
+        'namespace': 'str',
+        'error': 'GooglerpcStatus'
     }
 
     attribute_map = {
-        'id': 'id',
-        'created_at': 'created_at',
-        'name': 'name',
+        'pipeline_id': 'pipeline_id',
+        'display_name': 'display_name',
         'description': 'description',
-        'parameters': 'parameters',
+        'created_at': 'created_at',
+        'namespace': 'namespace',
         'error': 'error'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, error=None, local_vars_configuration=None):  # noqa: E501
-        """ApiPipeline - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, pipeline_id=None, display_name=None, description=None, created_at=None, namespace=None, error=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1Pipeline - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._created_at = None
-        self._name = None
+        self._pipeline_id = None
+        self._display_name = None
         self._description = None
-        self._parameters = None
+        self._created_at = None
+        self._namespace = None
         self._error = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if created_at is not None:
-            self.created_at = created_at
-        if name is not None:
-            self.name = name
+        if pipeline_id is not None:
+            self.pipeline_id = pipeline_id
+        if display_name is not None:
+            self.display_name = display_name
         if description is not None:
             self.description = description
-        if parameters is not None:
-            self.parameters = parameters
+        if created_at is not None:
+            self.created_at = created_at
+        if namespace is not None:
+            self.namespace = namespace
         if error is not None:
             self.error = error
 
     @property
-    def id(self):
-        """Gets the id of this ApiPipeline.  # noqa: E501
+    def pipeline_id(self):
+        """Gets the pipeline_id of this V2beta1Pipeline.  # noqa: E501
 
+        Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
-        :return: The id of this ApiPipeline.  # noqa: E501
+        :return: The pipeline_id of this V2beta1Pipeline.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._pipeline_id
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ApiPipeline.
+    @pipeline_id.setter
+    def pipeline_id(self, pipeline_id):
+        """Sets the pipeline_id of this V2beta1Pipeline.
 
+        Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
-        :param id: The id of this ApiPipeline.  # noqa: E501
-        :type id: str
+        :param pipeline_id: The pipeline_id of this V2beta1Pipeline.  # noqa: E501
+        :type pipeline_id: str
         """
 
-        self._id = id
+        self._pipeline_id = pipeline_id
 
     @property
-    def created_at(self):
-        """Gets the created_at of this ApiPipeline.  # noqa: E501
+    def display_name(self):
+        """Gets the display_name of this V2beta1Pipeline.  # noqa: E501
 
+        Required input field. Pipeline name provided by user.  # noqa: E501
 
-        :return: The created_at of this ApiPipeline.  # noqa: E501
-        :rtype: datetime
+        :return: The display_name of this V2beta1Pipeline.  # noqa: E501
+        :rtype: str
         """
-        return self._created_at
+        return self._display_name
 
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this ApiPipeline.
+    @display_name.setter
+    def display_name(self, display_name):
+        """Sets the display_name of this V2beta1Pipeline.
 
+        Required input field. Pipeline name provided by user.  # noqa: E501
 
-        :param created_at: The created_at of this ApiPipeline.  # noqa: E501
-        :type created_at: datetime
+        :param display_name: The display_name of this V2beta1Pipeline.  # noqa: E501
+        :type display_name: str
         """
 
-        self._created_at = created_at
+        self._display_name = display_name
 
     @property
-    def name(self):
-        """Gets the name of this ApiPipeline.  # noqa: E501
+    def description(self):
+        """Gets the description of this V2beta1Pipeline.  # noqa: E501
 
+        Optional input field. A short description of the pipeline.  # noqa: E501
 
-        :return: The name of this ApiPipeline.  # noqa: E501
+        :return: The description of this V2beta1Pipeline.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._description
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ApiPipeline.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this V2beta1Pipeline.
 
+        Optional input field. A short description of the pipeline.  # noqa: E501
 
-        :param name: The name of this ApiPipeline.  # noqa: E501
-        :type name: str
+        :param description: The description of this V2beta1Pipeline.  # noqa: E501
+        :type description: str
         """
 
-        self._name = name
+        self._description = description
 
     @property
-    def description(self):
-        """Gets the description of this ApiPipeline.  # noqa: E501
+    def created_at(self):
+        """Gets the created_at of this V2beta1Pipeline.  # noqa: E501
 
+        Output. Creation time of the pipeline.  # noqa: E501
 
-        :return: The description of this ApiPipeline.  # noqa: E501
-        :rtype: str
+        :return: The created_at of this V2beta1Pipeline.  # noqa: E501
+        :rtype: datetime
         """
-        return self._description
+        return self._created_at
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this ApiPipeline.
+    @created_at.setter
+    def created_at(self, created_at):
+        """Sets the created_at of this V2beta1Pipeline.
 
+        Output. Creation time of the pipeline.  # noqa: E501
 
-        :param description: The description of this ApiPipeline.  # noqa: E501
-        :type description: str
+        :param created_at: The created_at of this V2beta1Pipeline.  # noqa: E501
+        :type created_at: datetime
         """
 
-        self._description = description
+        self._created_at = created_at
 
     @property
-    def parameters(self):
-        """Gets the parameters of this ApiPipeline.  # noqa: E501
+    def namespace(self):
+        """Gets the namespace of this V2beta1Pipeline.  # noqa: E501
 
+        Input. A namespace this pipeline belongs to. Causes error if user is not authorized to access the specified namespace. If not specified in CreatePipeline, default namespace is used.  # noqa: E501
 
-        :return: The parameters of this ApiPipeline.  # noqa: E501
-        :rtype: list[ApiParameter]
+        :return: The namespace of this V2beta1Pipeline.  # noqa: E501
+        :rtype: str
         """
-        return self._parameters
+        return self._namespace
 
-    @parameters.setter
-    def parameters(self, parameters):
-        """Sets the parameters of this ApiPipeline.
+    @namespace.setter
+    def namespace(self, namespace):
+        """Sets the namespace of this V2beta1Pipeline.
 
+        Input. A namespace this pipeline belongs to. Causes error if user is not authorized to access the specified namespace. If not specified in CreatePipeline, default namespace is used.  # noqa: E501
 
-        :param parameters: The parameters of this ApiPipeline.  # noqa: E501
-        :type parameters: list[ApiParameter]
+        :param namespace: The namespace of this V2beta1Pipeline.  # noqa: E501
+        :type namespace: str
         """
 
-        self._parameters = parameters
+        self._namespace = namespace
 
     @property
     def error(self):
-        """Gets the error of this ApiPipeline.  # noqa: E501
+        """Gets the error of this V2beta1Pipeline.  # noqa: E501
 
-        In case any error happens retrieving a pipeline field, only pipeline ID and the error message is returned. Client has the flexibility of choosing how to handle error. This is especially useful during listing call.  # noqa: E501
 
-        :return: The error of this ApiPipeline.  # noqa: E501
-        :rtype: str
+        :return: The error of this V2beta1Pipeline.  # noqa: E501
+        :rtype: GooglerpcStatus
         """
         return self._error
 
     @error.setter
     def error(self, error):
-        """Sets the error of this ApiPipeline.
+        """Sets the error of this V2beta1Pipeline.
 
-        In case any error happens retrieving a pipeline field, only pipeline ID and the error message is returned. Client has the flexibility of choosing how to handle error. This is especially useful during listing call.  # noqa: E501
 
-        :param error: The error of this ApiPipeline.  # noqa: E501
-        :type error: str
+        :param error: The error of this V2beta1Pipeline.  # noqa: E501
+        :type error: GooglerpcStatus
         """
 
         self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -235,18 +243,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiPipeline):
+        if not isinstance(other, V2beta1Pipeline):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiPipeline):
+        if not isinstance(other, V2beta1Pipeline):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_relationship.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_null_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiRelationship(object):
+class ProtobufNullValue(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN_RELATIONSHIP = "UNKNOWN_RELATIONSHIP"
-    OWNER = "OWNER"
-    CREATOR = "CREATOR"
+    NULL_VALUE = "NULL_VALUE"
 
-    allowable_values = [UNKNOWN_RELATIONSHIP, OWNER, CREATOR]  # noqa: E501
+    allowable_values = [NULL_VALUE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +42,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """ApiRelationship - a model defined in OpenAPI"""  # noqa: E501
+        """ProtobufNullValue - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +82,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiRelationship):
+        if not isinstance(other, ProtobufNullValue):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiRelationship):
+        if not isinstance(other, ProtobufNullValue):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_key.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_get_healthz_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,96 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiResourceKey(object):
+class V2beta1GetHealthzResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'type': 'ApiResourceType',
-        'id': 'str'
+        'multi_user': 'bool'
     }
 
     attribute_map = {
-        'type': 'type',
-        'id': 'id'
+        'multi_user': 'multi_user'
     }
 
-    def __init__(self, type=None, id=None, local_vars_configuration=None):  # noqa: E501
-        """ApiResourceKey - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, multi_user=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1GetHealthzResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
-        self._id = None
+        self._multi_user = None
         self.discriminator = None
 
-        if type is not None:
-            self.type = type
-        if id is not None:
-            self.id = id
+        if multi_user is not None:
+            self.multi_user = multi_user
 
     @property
-    def type(self):
-        """Gets the type of this ApiResourceKey.  # noqa: E501
+    def multi_user(self):
+        """Gets the multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
 
+        Returns if KFP in multi-user mode  # noqa: E501
 
-        :return: The type of this ApiResourceKey.  # noqa: E501
-        :rtype: ApiResourceType
+        :return: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._type
+        return self._multi_user
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ApiResourceKey.
+    @multi_user.setter
+    def multi_user(self, multi_user):
+        """Sets the multi_user of this V2beta1GetHealthzResponse.
 
+        Returns if KFP in multi-user mode  # noqa: E501
 
-        :param type: The type of this ApiResourceKey.  # noqa: E501
-        :type type: ApiResourceType
+        :param multi_user: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
+        :type multi_user: bool
         """
 
-        self._type = type
-
-    @property
-    def id(self):
-        """Gets the id of this ApiResourceKey.  # noqa: E501
-
-        The ID of the resource that referred to.  # noqa: E501
-
-        :return: The id of this ApiResourceKey.  # noqa: E501
-        :rtype: str
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ApiResourceKey.
-
-        The ID of the resource that referred to.  # noqa: E501
-
-        :param id: The id of this ApiResourceKey.  # noqa: E501
-        :type id: str
-        """
-
-        self._id = id
+        self._multi_user = multi_user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -131,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiResourceKey):
+        if not isinstance(other, V2beta1GetHealthzResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiResourceKey):
+        if not isinstance(other, V2beta1GetHealthzResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_reference.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,122 +14,122 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiResourceReference(object):
+class V2beta1RuntimeStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'key': 'ApiResourceKey',
-        'name': 'str',
-        'relationship': 'ApiRelationship'
+        'update_time': 'datetime',
+        'state': 'V2beta1RuntimeState',
+        'error': 'GooglerpcStatus'
     }
 
     attribute_map = {
-        'key': 'key',
-        'name': 'name',
-        'relationship': 'relationship'
+        'update_time': 'update_time',
+        'state': 'state',
+        'error': 'error'
     }
 
-    def __init__(self, key=None, name=None, relationship=None, local_vars_configuration=None):  # noqa: E501
-        """ApiResourceReference - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, update_time=None, state=None, error=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1RuntimeStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._key = None
-        self._name = None
-        self._relationship = None
+        self._update_time = None
+        self._state = None
+        self._error = None
         self.discriminator = None
 
-        if key is not None:
-            self.key = key
-        if name is not None:
-            self.name = name
-        if relationship is not None:
-            self.relationship = relationship
+        if update_time is not None:
+            self.update_time = update_time
+        if state is not None:
+            self.state = state
+        if error is not None:
+            self.error = error
 
     @property
-    def key(self):
-        """Gets the key of this ApiResourceReference.  # noqa: E501
+    def update_time(self):
+        """Gets the update_time of this V2beta1RuntimeStatus.  # noqa: E501
 
+        Update time of this state.  # noqa: E501
 
-        :return: The key of this ApiResourceReference.  # noqa: E501
-        :rtype: ApiResourceKey
+        :return: The update_time of this V2beta1RuntimeStatus.  # noqa: E501
+        :rtype: datetime
         """
-        return self._key
+        return self._update_time
 
-    @key.setter
-    def key(self, key):
-        """Sets the key of this ApiResourceReference.
+    @update_time.setter
+    def update_time(self, update_time):
+        """Sets the update_time of this V2beta1RuntimeStatus.
 
+        Update time of this state.  # noqa: E501
 
-        :param key: The key of this ApiResourceReference.  # noqa: E501
-        :type key: ApiResourceKey
+        :param update_time: The update_time of this V2beta1RuntimeStatus.  # noqa: E501
+        :type update_time: datetime
         """
 
-        self._key = key
+        self._update_time = update_time
 
     @property
-    def name(self):
-        """Gets the name of this ApiResourceReference.  # noqa: E501
+    def state(self):
+        """Gets the state of this V2beta1RuntimeStatus.  # noqa: E501
 
-        The name of the resource that referred to.  # noqa: E501
 
-        :return: The name of this ApiResourceReference.  # noqa: E501
-        :rtype: str
+        :return: The state of this V2beta1RuntimeStatus.  # noqa: E501
+        :rtype: V2beta1RuntimeState
         """
-        return self._name
+        return self._state
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ApiResourceReference.
+    @state.setter
+    def state(self, state):
+        """Sets the state of this V2beta1RuntimeStatus.
 
-        The name of the resource that referred to.  # noqa: E501
 
-        :param name: The name of this ApiResourceReference.  # noqa: E501
-        :type name: str
+        :param state: The state of this V2beta1RuntimeStatus.  # noqa: E501
+        :type state: V2beta1RuntimeState
         """
 
-        self._name = name
+        self._state = state
 
     @property
-    def relationship(self):
-        """Gets the relationship of this ApiResourceReference.  # noqa: E501
+    def error(self):
+        """Gets the error of this V2beta1RuntimeStatus.  # noqa: E501
 
 
-        :return: The relationship of this ApiResourceReference.  # noqa: E501
-        :rtype: ApiRelationship
+        :return: The error of this V2beta1RuntimeStatus.  # noqa: E501
+        :rtype: GooglerpcStatus
         """
-        return self._relationship
+        return self._error
 
-    @relationship.setter
-    def relationship(self, relationship):
-        """Sets the relationship of this ApiResourceReference.
+    @error.setter
+    def error(self, error):
+        """Sets the error of this V2beta1RuntimeStatus.
 
 
-        :param relationship: The relationship of this ApiResourceReference.  # noqa: E501
-        :type relationship: ApiRelationship
+        :param error: The error of this V2beta1RuntimeStatus.  # noqa: E501
+        :type error: GooglerpcStatus
         """
 
-        self._relationship = relationship
+        self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -157,18 +157,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiResourceReference):
+        if not isinstance(other, V2beta1RuntimeStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiResourceReference):
+        if not isinstance(other, V2beta1RuntimeStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_resource_type.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,32 +14,31 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiResourceType(object):
+class V2beta1VisualizationType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN_RESOURCE_TYPE = "UNKNOWN_RESOURCE_TYPE"
-    EXPERIMENT = "EXPERIMENT"
-    JOB = "JOB"
-    PIPELINE = "PIPELINE"
-    PIPELINE_VERSION = "PIPELINE_VERSION"
-    NAMESPACE = "NAMESPACE"
+    ROC_CURVE = "ROC_CURVE"
+    TFDV = "TFDV"
+    TFMA = "TFMA"
+    TABLE = "TABLE"
+    CUSTOM = "CUSTOM"
 
-    allowable_values = [UNKNOWN_RESOURCE_TYPE, EXPERIMENT, JOB, PIPELINE, PIPELINE_VERSION, NAMESPACE]  # noqa: E501
+    allowable_values = [ROC_CURVE, TFDV, TFMA, TABLE, CUSTOM]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -47,15 +46,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """ApiResourceType - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1VisualizationType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -87,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiResourceType):
+        if not isinstance(other, V2beta1VisualizationType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiResourceType):
+        if not isinstance(other, V2beta1VisualizationType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_status.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_struct.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,120 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiStatus(object):
+class ProtobufStruct(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'error': 'str',
-        'code': 'int',
-        'details': 'list[ProtobufAny]'
+        'fields': 'dict(str, ProtobufValue)'
     }
 
     attribute_map = {
-        'error': 'error',
-        'code': 'code',
-        'details': 'details'
+        'fields': 'fields'
     }
 
-    def __init__(self, error=None, code=None, details=None, local_vars_configuration=None):  # noqa: E501
-        """ApiStatus - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, fields=None, local_vars_configuration=None):  # noqa: E501
+        """ProtobufStruct - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._error = None
-        self._code = None
-        self._details = None
+        self._fields = None
         self.discriminator = None
 
-        if error is not None:
-            self.error = error
-        if code is not None:
-            self.code = code
-        if details is not None:
-            self.details = details
+        if fields is not None:
+            self.fields = fields
 
     @property
-    def error(self):
-        """Gets the error of this ApiStatus.  # noqa: E501
+    def fields(self):
+        """Gets the fields of this ProtobufStruct.  # noqa: E501
 
+        Unordered map of dynamically typed values.  # noqa: E501
 
-        :return: The error of this ApiStatus.  # noqa: E501
-        :rtype: str
+        :return: The fields of this ProtobufStruct.  # noqa: E501
+        :rtype: dict(str, ProtobufValue)
         """
-        return self._error
+        return self._fields
 
-    @error.setter
-    def error(self, error):
-        """Sets the error of this ApiStatus.
+    @fields.setter
+    def fields(self, fields):
+        """Sets the fields of this ProtobufStruct.
 
+        Unordered map of dynamically typed values.  # noqa: E501
 
-        :param error: The error of this ApiStatus.  # noqa: E501
-        :type error: str
+        :param fields: The fields of this ProtobufStruct.  # noqa: E501
+        :type fields: dict(str, ProtobufValue)
         """
 
-        self._error = error
-
-    @property
-    def code(self):
-        """Gets the code of this ApiStatus.  # noqa: E501
-
-
-        :return: The code of this ApiStatus.  # noqa: E501
-        :rtype: int
-        """
-        return self._code
-
-    @code.setter
-    def code(self, code):
-        """Sets the code of this ApiStatus.
-
-
-        :param code: The code of this ApiStatus.  # noqa: E501
-        :type code: int
-        """
-
-        self._code = code
-
-    @property
-    def details(self):
-        """Gets the details of this ApiStatus.  # noqa: E501
-
-
-        :return: The details of this ApiStatus.  # noqa: E501
-        :rtype: list[ProtobufAny]
-        """
-        return self._details
-
-    @details.setter
-    def details(self, details):
-        """Sets the details of this ApiStatus.
-
-
-        :param details: The details of this ApiStatus.  # noqa: E501
-        :type details: list[ProtobufAny]
-        """
-
-        self._details = details
+        self._fields = fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -155,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiStatus):
+        if not isinstance(other, ProtobufStruct):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiStatus):
+        if not isinstance(other, ProtobufStruct):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/api_url.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ApiUrl(object):
+class V2beta1Url(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -37,41 +37,43 @@
     }
 
     attribute_map = {
         'pipeline_url': 'pipeline_url'
     }
 
     def __init__(self, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
-        """ApiUrl - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1Url - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pipeline_url = None
         self.discriminator = None
 
         if pipeline_url is not None:
             self.pipeline_url = pipeline_url
 
     @property
     def pipeline_url(self):
-        """Gets the pipeline_url of this ApiUrl.  # noqa: E501
+        """Gets the pipeline_url of this V2beta1Url.  # noqa: E501
 
+        URL of the pipeline version definition.  # noqa: E501
 
-        :return: The pipeline_url of this ApiUrl.  # noqa: E501
+        :return: The pipeline_url of this V2beta1Url.  # noqa: E501
         :rtype: str
         """
         return self._pipeline_url
 
     @pipeline_url.setter
     def pipeline_url(self, pipeline_url):
-        """Sets the pipeline_url of this ApiUrl.
+        """Sets the pipeline_url of this V2beta1Url.
 
+        URL of the pipeline version definition.  # noqa: E501
 
-        :param pipeline_url: The pipeline_url of this ApiUrl.  # noqa: E501
+        :param pipeline_url: The pipeline_url of this V2beta1Url.  # noqa: E501
         :type pipeline_url: str
         """
 
         self._pipeline_url = pipeline_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -103,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiUrl):
+        if not isinstance(other, V2beta1Url):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiUrl):
+        if not isinstance(other, V2beta1Url):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/authorize_request_resources.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_resources.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/authorize_request_verb.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_verb.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/googlerpc_status.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_int_values.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_int_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_long_values.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_long_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/predicate_string_values.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_string_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_any.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_list_value.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_list_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_null_value.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/recurring_run_mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ProtobufNullValue(object):
+class RecurringRunMode(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    NULL_VALUE = "NULL_VALUE"
+    MODE_UNSPECIFIED = "MODE_UNSPECIFIED"
+    ENABLE = "ENABLE"
+    DISABLE = "DISABLE"
 
-    allowable_values = [NULL_VALUE]  # noqa: E501
+    allowable_values = [MODE_UNSPECIFIED, ENABLE, DISABLE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -42,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """ProtobufNullValue - a model defined in OpenAPI"""  # noqa: E501
+        """RecurringRunMode - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -82,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProtobufNullValue):
+        if not isinstance(other, RecurringRunMode):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProtobufNullValue):
+        if not isinstance(other, RecurringRunMode):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_struct.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ProtobufStruct(object):
+class V2beta1Filter(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'fields': 'dict(str, ProtobufValue)'
+        'predicates': 'list[V2beta1Predicate]'
     }
 
     attribute_map = {
-        'fields': 'fields'
+        'predicates': 'predicates'
     }
 
-    def __init__(self, fields=None, local_vars_configuration=None):  # noqa: E501
-        """ProtobufStruct - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, predicates=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1Filter - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._fields = None
+        self._predicates = None
         self.discriminator = None
 
-        if fields is not None:
-            self.fields = fields
+        if predicates is not None:
+            self.predicates = predicates
 
     @property
-    def fields(self):
-        """Gets the fields of this ProtobufStruct.  # noqa: E501
+    def predicates(self):
+        """Gets the predicates of this V2beta1Filter.  # noqa: E501
 
-        Unordered map of dynamically typed values.  # noqa: E501
+        All predicates are AND-ed when this filter is applied.  # noqa: E501
 
-        :return: The fields of this ProtobufStruct.  # noqa: E501
-        :rtype: dict(str, ProtobufValue)
+        :return: The predicates of this V2beta1Filter.  # noqa: E501
+        :rtype: list[V2beta1Predicate]
         """
-        return self._fields
+        return self._predicates
 
-    @fields.setter
-    def fields(self, fields):
-        """Sets the fields of this ProtobufStruct.
+    @predicates.setter
+    def predicates(self, predicates):
+        """Sets the predicates of this V2beta1Filter.
 
-        Unordered map of dynamically typed values.  # noqa: E501
+        All predicates are AND-ed when this filter is applied.  # noqa: E501
 
-        :param fields: The fields of this ProtobufStruct.  # noqa: E501
-        :type fields: dict(str, ProtobufValue)
+        :param predicates: The predicates of this V2beta1Filter.  # noqa: E501
+        :type predicates: list[V2beta1Predicate]
         """
 
-        self._fields = fields
+        self._predicates = predicates
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProtobufStruct):
+        if not isinstance(other, V2beta1Filter):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProtobufStruct):
+        if not isinstance(other, V2beta1Filter):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/protobuf_value.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/recurring_run_mode.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class RecurringRunMode(object):
+class V2beta1RecurringRunStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    MODE_UNSPECIFIED = "MODE_UNSPECIFIED"
-    ENABLE = "ENABLE"
-    DISABLE = "DISABLE"
+    STATUS_UNSPECIFIED = "STATUS_UNSPECIFIED"
+    ENABLED = "ENABLED"
+    DISABLED = "DISABLED"
 
-    allowable_values = [MODE_UNSPECIFIED, ENABLE, DISABLE]  # noqa: E501
+    allowable_values = [STATUS_UNSPECIFIED, ENABLED, DISABLED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """RecurringRunMode - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RecurringRunStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RecurringRunMode):
+        if not isinstance(other, V2beta1RecurringRunStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RecurringRunMode):
+        if not isinstance(other, V2beta1RecurringRunStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_artifact_list.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_artifact_list.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_cron_schedule.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_experiment.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_experiment_storage_state.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_filter.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_read_artifact_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,70 +14,73 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1Filter(object):
+class V2beta1ReadArtifactResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'predicates': 'list[V2beta1Predicate]'
+        'data': 'str'
     }
 
     attribute_map = {
-        'predicates': 'predicates'
+        'data': 'data'
     }
 
-    def __init__(self, predicates=None, local_vars_configuration=None):  # noqa: E501
-        """V2beta1Filter - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, data=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1ReadArtifactResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._predicates = None
+        self._data = None
         self.discriminator = None
 
-        if predicates is not None:
-            self.predicates = predicates
+        if data is not None:
+            self.data = data
 
     @property
-    def predicates(self):
-        """Gets the predicates of this V2beta1Filter.  # noqa: E501
+    def data(self):
+        """Gets the data of this V2beta1ReadArtifactResponse.  # noqa: E501
 
-        All predicates are AND-ed when this filter is applied.  # noqa: E501
+        Byte array of the artifact content.  # noqa: E501
 
-        :return: The predicates of this V2beta1Filter.  # noqa: E501
-        :rtype: list[V2beta1Predicate]
+        :return: The data of this V2beta1ReadArtifactResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._predicates
+        return self._data
 
-    @predicates.setter
-    def predicates(self, predicates):
-        """Sets the predicates of this V2beta1Filter.
+    @data.setter
+    def data(self, data):
+        """Sets the data of this V2beta1ReadArtifactResponse.
 
-        All predicates are AND-ed when this filter is applied.  # noqa: E501
+        Byte array of the artifact content.  # noqa: E501
 
-        :param predicates: The predicates of this V2beta1Filter.  # noqa: E501
-        :type predicates: list[V2beta1Predicate]
+        :param data: The data of this V2beta1ReadArtifactResponse.  # noqa: E501
+        :type data: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                data is not None and not re.search(r'^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', data)):  # noqa: E501
+            raise ValueError(r"Invalid value for `data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
-        self._predicates = predicates
+        self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +108,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1Filter):
+        if not isinstance(other, V2beta1ReadArtifactResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1Filter):
+        if not isinstance(other, V2beta1ReadArtifactResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_get_healthz_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,71 +14,56 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1GetHealthzResponse(object):
+class V2beta1PredicateOperation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    OPERATION_UNSPECIFIED = "OPERATION_UNSPECIFIED"
+    EQUALS = "EQUALS"
+    NOT_EQUALS = "NOT_EQUALS"
+    GREATER_THAN = "GREATER_THAN"
+    GREATER_THAN_EQUALS = "GREATER_THAN_EQUALS"
+    LESS_THAN = "LESS_THAN"
+    LESS_THAN_EQUALS = "LESS_THAN_EQUALS"
+    IN = "IN"
+    IS_SUBSTRING = "IS_SUBSTRING"
+
+    allowable_values = [OPERATION_UNSPECIFIED, EQUALS, NOT_EQUALS, GREATER_THAN, GREATER_THAN_EQUALS, LESS_THAN, LESS_THAN_EQUALS, IN, IS_SUBSTRING]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'multi_user': 'bool'
     }
 
     attribute_map = {
-        'multi_user': 'multi_user'
     }
 
-    def __init__(self, multi_user=None, local_vars_configuration=None):  # noqa: E501
-        """V2beta1GetHealthzResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """V2beta1PredicateOperation - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._multi_user = None
         self.discriminator = None
 
-        if multi_user is not None:
-            self.multi_user = multi_user
-
-    @property
-    def multi_user(self):
-        """Gets the multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-
-        Returns if KFP in multi-user mode  # noqa: E501
-
-        :return: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-        :rtype: bool
-        """
-        return self._multi_user
-
-    @multi_user.setter
-    def multi_user(self, multi_user):
-        """Sets the multi_user of this V2beta1GetHealthzResponse.
-
-        Returns if KFP in multi-user mode  # noqa: E501
-
-        :param multi_user: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-        :type multi_user: bool
-        """
-
-        self._multi_user = multi_user
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -105,18 +90,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1GetHealthzResponse):
+        if not isinstance(other, V2beta1PredicateOperation):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1GetHealthzResponse):
+        if not isinstance(other, V2beta1PredicateOperation):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_experiments_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_pipelines_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_recurring_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_list_runs_response.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_periodic_schedule.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,205 +14,177 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1Pipeline(object):
+class V2beta1Visualization(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'pipeline_id': 'str',
-        'display_name': 'str',
-        'description': 'str',
-        'created_at': 'datetime',
-        'namespace': 'str',
-        'error': 'GooglerpcStatus'
+        'type': 'V2beta1VisualizationType',
+        'source': 'str',
+        'arguments': 'str',
+        'html': 'str',
+        'error': 'str'
     }
 
     attribute_map = {
-        'pipeline_id': 'pipeline_id',
-        'display_name': 'display_name',
-        'description': 'description',
-        'created_at': 'created_at',
-        'namespace': 'namespace',
+        'type': 'type',
+        'source': 'source',
+        'arguments': 'arguments',
+        'html': 'html',
         'error': 'error'
     }
 
-    def __init__(self, pipeline_id=None, display_name=None, description=None, created_at=None, namespace=None, error=None, local_vars_configuration=None):  # noqa: E501
-        """V2beta1Pipeline - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, type=None, source=None, arguments=None, html=None, error=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1Visualization - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._pipeline_id = None
-        self._display_name = None
-        self._description = None
-        self._created_at = None
-        self._namespace = None
+        self._type = None
+        self._source = None
+        self._arguments = None
+        self._html = None
         self._error = None
         self.discriminator = None
 
-        if pipeline_id is not None:
-            self.pipeline_id = pipeline_id
-        if display_name is not None:
-            self.display_name = display_name
-        if description is not None:
-            self.description = description
-        if created_at is not None:
-            self.created_at = created_at
-        if namespace is not None:
-            self.namespace = namespace
+        if type is not None:
+            self.type = type
+        if source is not None:
+            self.source = source
+        if arguments is not None:
+            self.arguments = arguments
+        if html is not None:
+            self.html = html
         if error is not None:
             self.error = error
 
     @property
-    def pipeline_id(self):
-        """Gets the pipeline_id of this V2beta1Pipeline.  # noqa: E501
+    def type(self):
+        """Gets the type of this V2beta1Visualization.  # noqa: E501
 
-        Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
-        :return: The pipeline_id of this V2beta1Pipeline.  # noqa: E501
-        :rtype: str
+        :return: The type of this V2beta1Visualization.  # noqa: E501
+        :rtype: V2beta1VisualizationType
         """
-        return self._pipeline_id
+        return self._type
 
-    @pipeline_id.setter
-    def pipeline_id(self, pipeline_id):
-        """Sets the pipeline_id of this V2beta1Pipeline.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this V2beta1Visualization.
 
-        Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
-        :param pipeline_id: The pipeline_id of this V2beta1Pipeline.  # noqa: E501
-        :type pipeline_id: str
+        :param type: The type of this V2beta1Visualization.  # noqa: E501
+        :type type: V2beta1VisualizationType
         """
 
-        self._pipeline_id = pipeline_id
+        self._type = type
 
     @property
-    def display_name(self):
-        """Gets the display_name of this V2beta1Pipeline.  # noqa: E501
+    def source(self):
+        """Gets the source of this V2beta1Visualization.  # noqa: E501
 
-        Required input field. Pipeline name provided by user.  # noqa: E501
+        Path pattern of input data to be used during generation of visualizations. This is required when creating the pipeline through CreateVisualization API.  # noqa: E501
 
-        :return: The display_name of this V2beta1Pipeline.  # noqa: E501
+        :return: The source of this V2beta1Visualization.  # noqa: E501
         :rtype: str
         """
-        return self._display_name
+        return self._source
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this V2beta1Pipeline.
+    @source.setter
+    def source(self, source):
+        """Sets the source of this V2beta1Visualization.
 
-        Required input field. Pipeline name provided by user.  # noqa: E501
+        Path pattern of input data to be used during generation of visualizations. This is required when creating the pipeline through CreateVisualization API.  # noqa: E501
 
-        :param display_name: The display_name of this V2beta1Pipeline.  # noqa: E501
-        :type display_name: str
+        :param source: The source of this V2beta1Visualization.  # noqa: E501
+        :type source: str
         """
 
-        self._display_name = display_name
+        self._source = source
 
     @property
-    def description(self):
-        """Gets the description of this V2beta1Pipeline.  # noqa: E501
+    def arguments(self):
+        """Gets the arguments of this V2beta1Visualization.  # noqa: E501
 
-        Optional input field. A short description of the pipeline.  # noqa: E501
+        Variables to be used during generation of a visualization. This should be provided as a JSON string. This is required when creating the pipeline through CreateVisualization API.  # noqa: E501
 
-        :return: The description of this V2beta1Pipeline.  # noqa: E501
+        :return: The arguments of this V2beta1Visualization.  # noqa: E501
         :rtype: str
         """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this V2beta1Pipeline.
-
-        Optional input field. A short description of the pipeline.  # noqa: E501
-
-        :param description: The description of this V2beta1Pipeline.  # noqa: E501
-        :type description: str
-        """
-
-        self._description = description
-
-    @property
-    def created_at(self):
-        """Gets the created_at of this V2beta1Pipeline.  # noqa: E501
-
-        Output. Creation time of the pipeline.  # noqa: E501
-
-        :return: The created_at of this V2beta1Pipeline.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._created_at
+        return self._arguments
 
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this V2beta1Pipeline.
+    @arguments.setter
+    def arguments(self, arguments):
+        """Sets the arguments of this V2beta1Visualization.
 
-        Output. Creation time of the pipeline.  # noqa: E501
+        Variables to be used during generation of a visualization. This should be provided as a JSON string. This is required when creating the pipeline through CreateVisualization API.  # noqa: E501
 
-        :param created_at: The created_at of this V2beta1Pipeline.  # noqa: E501
-        :type created_at: datetime
+        :param arguments: The arguments of this V2beta1Visualization.  # noqa: E501
+        :type arguments: str
         """
 
-        self._created_at = created_at
+        self._arguments = arguments
 
     @property
-    def namespace(self):
-        """Gets the namespace of this V2beta1Pipeline.  # noqa: E501
+    def html(self):
+        """Gets the html of this V2beta1Visualization.  # noqa: E501
 
-        Input. A namespace this pipeline belongs to. Causes error if user is not authorized to access the specified namespace. If not specified in CreatePipeline, default namespace is used.  # noqa: E501
+        Output. Generated visualization html.  # noqa: E501
 
-        :return: The namespace of this V2beta1Pipeline.  # noqa: E501
+        :return: The html of this V2beta1Visualization.  # noqa: E501
         :rtype: str
         """
-        return self._namespace
+        return self._html
 
-    @namespace.setter
-    def namespace(self, namespace):
-        """Sets the namespace of this V2beta1Pipeline.
+    @html.setter
+    def html(self, html):
+        """Sets the html of this V2beta1Visualization.
 
-        Input. A namespace this pipeline belongs to. Causes error if user is not authorized to access the specified namespace. If not specified in CreatePipeline, default namespace is used.  # noqa: E501
+        Output. Generated visualization html.  # noqa: E501
 
-        :param namespace: The namespace of this V2beta1Pipeline.  # noqa: E501
-        :type namespace: str
+        :param html: The html of this V2beta1Visualization.  # noqa: E501
+        :type html: str
         """
 
-        self._namespace = namespace
+        self._html = html
 
     @property
     def error(self):
-        """Gets the error of this V2beta1Pipeline.  # noqa: E501
+        """Gets the error of this V2beta1Visualization.  # noqa: E501
 
+        In case any error happens when generating visualizations, only visualization ID and the error message are returned. Client has the flexibility of choosing how to handle the error.  # noqa: E501
 
-        :return: The error of this V2beta1Pipeline.  # noqa: E501
-        :rtype: GooglerpcStatus
+        :return: The error of this V2beta1Visualization.  # noqa: E501
+        :rtype: str
         """
         return self._error
 
     @error.setter
     def error(self, error):
-        """Sets the error of this V2beta1Pipeline.
+        """Sets the error of this V2beta1Visualization.
 
+        In case any error happens when generating visualizations, only visualization ID and the error message are returned. Client has the flexibility of choosing how to handle the error.  # noqa: E501
 
-        :param error: The error of this V2beta1Pipeline.  # noqa: E501
-        :type error: GooglerpcStatus
+        :param error: The error of this V2beta1Visualization.  # noqa: E501
+        :type error: str
         """
 
         self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -243,18 +215,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1Pipeline):
+        if not isinstance(other, V2beta1Visualization):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1Pipeline):
+        if not isinstance(other, V2beta1Visualization):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_detail.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         'executor_detail': 'V2beta1PipelineTaskExecutorDetail',
         'state': 'V2beta1RuntimeState',
         'execution_id': 'str',
         'error': 'GooglerpcStatus',
         'inputs': 'dict(str, V2beta1ArtifactList)',
         'outputs': 'dict(str, V2beta1ArtifactList)',
         'parent_task_id': 'str',
-        'state_history': 'list[V2beta1RuntimeStatus]'
+        'state_history': 'list[V2beta1RuntimeStatus]',
+        'pod_name': 'str',
+        'child_tasks': 'list[PipelineTaskDetailChildTask]'
     }
 
     attribute_map = {
         'run_id': 'run_id',
         'task_id': 'task_id',
         'display_name': 'display_name',
         'create_time': 'create_time',
@@ -59,18 +61,20 @@
         'executor_detail': 'executor_detail',
         'state': 'state',
         'execution_id': 'execution_id',
         'error': 'error',
         'inputs': 'inputs',
         'outputs': 'outputs',
         'parent_task_id': 'parent_task_id',
-        'state_history': 'state_history'
+        'state_history': 'state_history',
+        'pod_name': 'pod_name',
+        'child_tasks': 'child_tasks'
     }
 
-    def __init__(self, run_id=None, task_id=None, display_name=None, create_time=None, start_time=None, end_time=None, executor_detail=None, state=None, execution_id=None, error=None, inputs=None, outputs=None, parent_task_id=None, state_history=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, run_id=None, task_id=None, display_name=None, create_time=None, start_time=None, end_time=None, executor_detail=None, state=None, execution_id=None, error=None, inputs=None, outputs=None, parent_task_id=None, state_history=None, pod_name=None, child_tasks=None, local_vars_configuration=None):  # noqa: E501
         """V2beta1PipelineTaskDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._run_id = None
         self._task_id = None
@@ -82,14 +86,16 @@
         self._state = None
         self._execution_id = None
         self._error = None
         self._inputs = None
         self._outputs = None
         self._parent_task_id = None
         self._state_history = None
+        self._pod_name = None
+        self._child_tasks = None
         self.discriminator = None
 
         if run_id is not None:
             self.run_id = run_id
         if task_id is not None:
             self.task_id = task_id
         if display_name is not None:
@@ -112,14 +118,18 @@
             self.inputs = inputs
         if outputs is not None:
             self.outputs = outputs
         if parent_task_id is not None:
             self.parent_task_id = parent_task_id
         if state_history is not None:
             self.state_history = state_history
+        if pod_name is not None:
+            self.pod_name = pod_name
+        if child_tasks is not None:
+            self.child_tasks = child_tasks
 
     @property
     def run_id(self):
         """Gets the run_id of this V2beta1PipelineTaskDetail.  # noqa: E501
 
         ID of the parent run.  # noqa: E501
 
@@ -297,26 +307,26 @@
 
         self._state = state
 
     @property
     def execution_id(self):
         """Gets the execution_id of this V2beta1PipelineTaskDetail.  # noqa: E501
 
-        Execution metadata of a task.  # noqa: E501
+        Execution id of the corresponding entry in ML metadata store.  # noqa: E501
 
         :return: The execution_id of this V2beta1PipelineTaskDetail.  # noqa: E501
         :rtype: str
         """
         return self._execution_id
 
     @execution_id.setter
     def execution_id(self, execution_id):
         """Sets the execution_id of this V2beta1PipelineTaskDetail.
 
-        Execution metadata of a task.  # noqa: E501
+        Execution id of the corresponding entry in ML metadata store.  # noqa: E501
 
         :param execution_id: The execution_id of this V2beta1PipelineTaskDetail.  # noqa: E501
         :type execution_id: str
         """
 
         self._execution_id = execution_id
 
@@ -429,14 +439,60 @@
 
         :param state_history: The state_history of this V2beta1PipelineTaskDetail.  # noqa: E501
         :type state_history: list[V2beta1RuntimeStatus]
         """
 
         self._state_history = state_history
 
+    @property
+    def pod_name(self):
+        """Gets the pod_name of this V2beta1PipelineTaskDetail.  # noqa: E501
+
+        Name of the corresponding pod assigned by the orchestration engine. Also known as node_id.  # noqa: E501
+
+        :return: The pod_name of this V2beta1PipelineTaskDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._pod_name
+
+    @pod_name.setter
+    def pod_name(self, pod_name):
+        """Sets the pod_name of this V2beta1PipelineTaskDetail.
+
+        Name of the corresponding pod assigned by the orchestration engine. Also known as node_id.  # noqa: E501
+
+        :param pod_name: The pod_name of this V2beta1PipelineTaskDetail.  # noqa: E501
+        :type pod_name: str
+        """
+
+        self._pod_name = pod_name
+
+    @property
+    def child_tasks(self):
+        """Gets the child_tasks of this V2beta1PipelineTaskDetail.  # noqa: E501
+
+        Sequence of dependen tasks.  # noqa: E501
+
+        :return: The child_tasks of this V2beta1PipelineTaskDetail.  # noqa: E501
+        :rtype: list[PipelineTaskDetailChildTask]
+        """
+        return self._child_tasks
+
+    @child_tasks.setter
+    def child_tasks(self, child_tasks):
+        """Sets the child_tasks of this V2beta1PipelineTaskDetail.
+
+        Sequence of dependen tasks.  # noqa: E501
+
+        :param child_tasks: The child_tasks of this V2beta1PipelineTaskDetail.  # noqa: E501
+        :type child_tasks: list[PipelineTaskDetailChildTask]
+        """
+
+        self._child_tasks = child_tasks
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_pipeline_version.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,41 +35,44 @@
     openapi_types = {
         'pipeline_id': 'str',
         'pipeline_version_id': 'str',
         'display_name': 'str',
         'description': 'str',
         'created_at': 'datetime',
         'package_url': 'V2beta1Url',
+        'code_source_url': 'str',
         'pipeline_spec': 'ProtobufStruct',
         'error': 'GooglerpcStatus'
     }
 
     attribute_map = {
         'pipeline_id': 'pipeline_id',
         'pipeline_version_id': 'pipeline_version_id',
         'display_name': 'display_name',
         'description': 'description',
         'created_at': 'created_at',
         'package_url': 'package_url',
+        'code_source_url': 'code_source_url',
         'pipeline_spec': 'pipeline_spec',
         'error': 'error'
     }
 
-    def __init__(self, pipeline_id=None, pipeline_version_id=None, display_name=None, description=None, created_at=None, package_url=None, pipeline_spec=None, error=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pipeline_id=None, pipeline_version_id=None, display_name=None, description=None, created_at=None, package_url=None, code_source_url=None, pipeline_spec=None, error=None, local_vars_configuration=None):  # noqa: E501
         """V2beta1PipelineVersion - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pipeline_id = None
         self._pipeline_version_id = None
         self._display_name = None
         self._description = None
         self._created_at = None
         self._package_url = None
+        self._code_source_url = None
         self._pipeline_spec = None
         self._error = None
         self.discriminator = None
 
         if pipeline_id is not None:
             self.pipeline_id = pipeline_id
         if pipeline_version_id is not None:
@@ -78,14 +81,16 @@
             self.display_name = display_name
         if description is not None:
             self.description = description
         if created_at is not None:
             self.created_at = created_at
         if package_url is not None:
             self.package_url = package_url
+        if code_source_url is not None:
+            self.code_source_url = code_source_url
         if pipeline_spec is not None:
             self.pipeline_spec = pipeline_spec
         if error is not None:
             self.error = error
 
     @property
     def pipeline_id(self):
@@ -220,14 +225,37 @@
         :param package_url: The package_url of this V2beta1PipelineVersion.  # noqa: E501
         :type package_url: V2beta1Url
         """
 
         self._package_url = package_url
 
     @property
+    def code_source_url(self):
+        """Gets the code_source_url of this V2beta1PipelineVersion.  # noqa: E501
+
+        Input. Optional. The URL to the code source of the pipeline version. The code is usually the Python definition of the pipeline and potentially related the component definitions. This allows users to trace back to how the pipeline YAML was created.  # noqa: E501
+
+        :return: The code_source_url of this V2beta1PipelineVersion.  # noqa: E501
+        :rtype: str
+        """
+        return self._code_source_url
+
+    @code_source_url.setter
+    def code_source_url(self, code_source_url):
+        """Sets the code_source_url of this V2beta1PipelineVersion.
+
+        Input. Optional. The URL to the code source of the pipeline version. The code is usually the Python definition of the pipeline and potentially related the component definitions. This allows users to trace back to how the pipeline YAML was created.  # noqa: E501
+
+        :param code_source_url: The code_source_url of this V2beta1PipelineVersion.  # noqa: E501
+        :type code_source_url: str
+        """
+
+        self._code_source_url = code_source_url
+
+    @property
     def pipeline_spec(self):
         """Gets the pipeline_spec of this V2beta1PipelineVersion.  # noqa: E501
 
 
         :return: The pipeline_spec of this V2beta1PipelineVersion.  # noqa: E501
         :rtype: ProtobufStruct
         """
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_predicate.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_predicate_operation.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_storage_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,35 +14,29 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1PredicateOperation(object):
+class V2beta1RunStorageState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    OPERATION_UNSPECIFIED = "OPERATION_UNSPECIFIED"
-    EQUALS = "EQUALS"
-    NOT_EQUALS = "NOT_EQUALS"
-    GREATER_THAN = "GREATER_THAN"
-    GREATER_THAN_EQUALS = "GREATER_THAN_EQUALS"
-    LESS_THAN = "LESS_THAN"
-    LESS_THAN_EQUALS = "LESS_THAN_EQUALS"
-    IN = "IN"
-    IS_SUBSTRING = "IS_SUBSTRING"
+    STORAGE_STATE_UNSPECIFIED = "STORAGE_STATE_UNSPECIFIED"
+    AVAILABLE = "AVAILABLE"
+    ARCHIVED = "ARCHIVED"
 
-    allowable_values = [OPERATION_UNSPECIFIED, EQUALS, NOT_EQUALS, GREATER_THAN, GREATER_THAN_EQUALS, LESS_THAN, LESS_THAN_EQUALS, IN, IS_SUBSTRING]  # noqa: E501
+    allowable_values = [STORAGE_STATE_UNSPECIFIED, AVAILABLE, ARCHIVED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -50,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1PredicateOperation - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RunStorageState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -90,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1PredicateOperation):
+        if not isinstance(other, V2beta1RunStorageState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1PredicateOperation):
+        if not isinstance(other, V2beta1RunStorageState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_recurring_run.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     """
     openapi_types = {
         'recurring_run_id': 'str',
         'display_name': 'str',
         'description': 'str',
         'pipeline_version_id': 'str',
         'pipeline_spec': 'ProtobufStruct',
+        'pipeline_version_reference': 'V2beta1PipelineVersionReference',
         'runtime_config': 'V2beta1RuntimeConfig',
         'service_account': 'str',
         'max_concurrency': 'str',
         'trigger': 'V2beta1Trigger',
         'mode': 'RecurringRunMode',
         'created_at': 'datetime',
         'updated_at': 'datetime',
@@ -54,39 +55,41 @@
 
     attribute_map = {
         'recurring_run_id': 'recurring_run_id',
         'display_name': 'display_name',
         'description': 'description',
         'pipeline_version_id': 'pipeline_version_id',
         'pipeline_spec': 'pipeline_spec',
+        'pipeline_version_reference': 'pipeline_version_reference',
         'runtime_config': 'runtime_config',
         'service_account': 'service_account',
         'max_concurrency': 'max_concurrency',
         'trigger': 'trigger',
         'mode': 'mode',
         'created_at': 'created_at',
         'updated_at': 'updated_at',
         'status': 'status',
         'error': 'error',
         'no_catchup': 'no_catchup',
         'namespace': 'namespace',
         'experiment_id': 'experiment_id'
     }
 
-    def __init__(self, recurring_run_id=None, display_name=None, description=None, pipeline_version_id=None, pipeline_spec=None, runtime_config=None, service_account=None, max_concurrency=None, trigger=None, mode=None, created_at=None, updated_at=None, status=None, error=None, no_catchup=None, namespace=None, experiment_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, recurring_run_id=None, display_name=None, description=None, pipeline_version_id=None, pipeline_spec=None, pipeline_version_reference=None, runtime_config=None, service_account=None, max_concurrency=None, trigger=None, mode=None, created_at=None, updated_at=None, status=None, error=None, no_catchup=None, namespace=None, experiment_id=None, local_vars_configuration=None):  # noqa: E501
         """V2beta1RecurringRun - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._recurring_run_id = None
         self._display_name = None
         self._description = None
         self._pipeline_version_id = None
         self._pipeline_spec = None
+        self._pipeline_version_reference = None
         self._runtime_config = None
         self._service_account = None
         self._max_concurrency = None
         self._trigger = None
         self._mode = None
         self._created_at = None
         self._updated_at = None
@@ -103,14 +106,16 @@
             self.display_name = display_name
         if description is not None:
             self.description = description
         if pipeline_version_id is not None:
             self.pipeline_version_id = pipeline_version_id
         if pipeline_spec is not None:
             self.pipeline_spec = pipeline_spec
+        if pipeline_version_reference is not None:
+            self.pipeline_version_reference = pipeline_version_reference
         if runtime_config is not None:
             self.runtime_config = runtime_config
         if service_account is not None:
             self.service_account = service_account
         if max_concurrency is not None:
             self.max_concurrency = max_concurrency
         if trigger is not None:
@@ -242,14 +247,35 @@
         :param pipeline_spec: The pipeline_spec of this V2beta1RecurringRun.  # noqa: E501
         :type pipeline_spec: ProtobufStruct
         """
 
         self._pipeline_spec = pipeline_spec
 
     @property
+    def pipeline_version_reference(self):
+        """Gets the pipeline_version_reference of this V2beta1RecurringRun.  # noqa: E501
+
+
+        :return: The pipeline_version_reference of this V2beta1RecurringRun.  # noqa: E501
+        :rtype: V2beta1PipelineVersionReference
+        """
+        return self._pipeline_version_reference
+
+    @pipeline_version_reference.setter
+    def pipeline_version_reference(self, pipeline_version_reference):
+        """Sets the pipeline_version_reference of this V2beta1RecurringRun.
+
+
+        :param pipeline_version_reference: The pipeline_version_reference of this V2beta1RecurringRun.  # noqa: E501
+        :type pipeline_version_reference: V2beta1PipelineVersionReference
+        """
+
+        self._pipeline_version_reference = pipeline_version_reference
+
+    @property
     def runtime_config(self):
         """Gets the runtime_config of this V2beta1RecurringRun.  # noqa: E501
 
 
         :return: The runtime_config of this V2beta1RecurringRun.  # noqa: E501
         :rtype: V2beta1RuntimeConfig
         """
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_recurring_run_status.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1RecurringRunStatus(object):
+class V2beta1RuntimeState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STATUS_UNSPECIFIED = "STATUS_UNSPECIFIED"
-    ENABLED = "ENABLED"
-    DISABLED = "DISABLED"
+    RUNTIME_STATE_UNSPECIFIED = "RUNTIME_STATE_UNSPECIFIED"
+    PENDING = "PENDING"
+    RUNNING = "RUNNING"
+    SUCCEEDED = "SUCCEEDED"
+    SKIPPED = "SKIPPED"
+    FAILED = "FAILED"
+    CANCELING = "CANCELING"
+    CANCELED = "CANCELED"
+    PAUSED = "PAUSED"
 
-    allowable_values = [STATUS_UNSPECIFIED, ENABLED, DISABLED]  # noqa: E501
+    allowable_values = [RUNTIME_STATE_UNSPECIFIED, PENDING, RUNNING, SUCCEEDED, SKIPPED, FAILED, CANCELING, CANCELED, PAUSED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +50,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1RecurringRunStatus - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RuntimeState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +90,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1RecurringRunStatus):
+        if not isinstance(other, V2beta1RuntimeState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1RecurringRunStatus):
+        if not isinstance(other, V2beta1RuntimeState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_run.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         'experiment_id': 'str',
         'run_id': 'str',
         'display_name': 'str',
         'storage_state': 'V2beta1RunStorageState',
         'description': 'str',
         'pipeline_version_id': 'str',
         'pipeline_spec': 'ProtobufStruct',
+        'pipeline_version_reference': 'V2beta1PipelineVersionReference',
         'runtime_config': 'V2beta1RuntimeConfig',
         'service_account': 'str',
         'created_at': 'datetime',
         'scheduled_at': 'datetime',
         'finished_at': 'datetime',
         'state': 'V2beta1RuntimeState',
         'error': 'GooglerpcStatus',
@@ -56,39 +57,41 @@
         'experiment_id': 'experiment_id',
         'run_id': 'run_id',
         'display_name': 'display_name',
         'storage_state': 'storage_state',
         'description': 'description',
         'pipeline_version_id': 'pipeline_version_id',
         'pipeline_spec': 'pipeline_spec',
+        'pipeline_version_reference': 'pipeline_version_reference',
         'runtime_config': 'runtime_config',
         'service_account': 'service_account',
         'created_at': 'created_at',
         'scheduled_at': 'scheduled_at',
         'finished_at': 'finished_at',
         'state': 'state',
         'error': 'error',
         'run_details': 'run_details',
         'recurring_run_id': 'recurring_run_id',
         'state_history': 'state_history'
     }
 
-    def __init__(self, experiment_id=None, run_id=None, display_name=None, storage_state=None, description=None, pipeline_version_id=None, pipeline_spec=None, runtime_config=None, service_account=None, created_at=None, scheduled_at=None, finished_at=None, state=None, error=None, run_details=None, recurring_run_id=None, state_history=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, experiment_id=None, run_id=None, display_name=None, storage_state=None, description=None, pipeline_version_id=None, pipeline_spec=None, pipeline_version_reference=None, runtime_config=None, service_account=None, created_at=None, scheduled_at=None, finished_at=None, state=None, error=None, run_details=None, recurring_run_id=None, state_history=None, local_vars_configuration=None):  # noqa: E501
         """V2beta1Run - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._experiment_id = None
         self._run_id = None
         self._display_name = None
         self._storage_state = None
         self._description = None
         self._pipeline_version_id = None
         self._pipeline_spec = None
+        self._pipeline_version_reference = None
         self._runtime_config = None
         self._service_account = None
         self._created_at = None
         self._scheduled_at = None
         self._finished_at = None
         self._state = None
         self._error = None
@@ -107,14 +110,16 @@
             self.storage_state = storage_state
         if description is not None:
             self.description = description
         if pipeline_version_id is not None:
             self.pipeline_version_id = pipeline_version_id
         if pipeline_spec is not None:
             self.pipeline_spec = pipeline_spec
+        if pipeline_version_reference is not None:
+            self.pipeline_version_reference = pipeline_version_reference
         if runtime_config is not None:
             self.runtime_config = runtime_config
         if service_account is not None:
             self.service_account = service_account
         if created_at is not None:
             self.created_at = created_at
         if scheduled_at is not None:
@@ -286,14 +291,35 @@
         :param pipeline_spec: The pipeline_spec of this V2beta1Run.  # noqa: E501
         :type pipeline_spec: ProtobufStruct
         """
 
         self._pipeline_spec = pipeline_spec
 
     @property
+    def pipeline_version_reference(self):
+        """Gets the pipeline_version_reference of this V2beta1Run.  # noqa: E501
+
+
+        :return: The pipeline_version_reference of this V2beta1Run.  # noqa: E501
+        :rtype: V2beta1PipelineVersionReference
+        """
+        return self._pipeline_version_reference
+
+    @pipeline_version_reference.setter
+    def pipeline_version_reference(self, pipeline_version_reference):
+        """Sets the pipeline_version_reference of this V2beta1Run.
+
+
+        :param pipeline_version_reference: The pipeline_version_reference of this V2beta1Run.  # noqa: E501
+        :type pipeline_version_reference: V2beta1PipelineVersionReference
+        """
+
+        self._pipeline_version_reference = pipeline_version_reference
+
+    @property
     def runtime_config(self):
         """Gets the runtime_config of this V2beta1Run.  # noqa: E501
 
 
         :return: The runtime_config of this V2beta1Run.  # noqa: E501
         :rtype: V2beta1RuntimeConfig
         """
```

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_run_details.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_details.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_runtime_config.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/models/v2beta1_trigger.py` & `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api/rest.py` & `kfp-server-api-2.0.0b1/kfp_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/kfp_server_api.egg-info/SOURCES.txt` & `kfp-server-api-2.0.0b1/kfp_server_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,18 @@
 kfp_server_api/api/pipeline_service_api.py
 kfp_server_api/api/pipeline_upload_service_api.py
 kfp_server_api/api/recurring_run_service_api.py
 kfp_server_api/api/report_service_api.py
 kfp_server_api/api/run_service_api.py
 kfp_server_api/api/visualization_service_api.py
 kfp_server_api/models/__init__.py
-kfp_server_api/models/api_parameter.py
-kfp_server_api/models/api_pipeline.py
-kfp_server_api/models/api_pipeline_version.py
-kfp_server_api/models/api_relationship.py
-kfp_server_api/models/api_resource_key.py
-kfp_server_api/models/api_resource_reference.py
-kfp_server_api/models/api_resource_type.py
-kfp_server_api/models/api_status.py
-kfp_server_api/models/api_url.py
 kfp_server_api/models/authorize_request_resources.py
 kfp_server_api/models/authorize_request_verb.py
 kfp_server_api/models/googlerpc_status.py
+kfp_server_api/models/pipeline_task_detail_child_task.py
 kfp_server_api/models/predicate_int_values.py
 kfp_server_api/models/predicate_long_values.py
 kfp_server_api/models/predicate_string_values.py
 kfp_server_api/models/protobuf_any.py
 kfp_server_api/models/protobuf_list_value.py
 kfp_server_api/models/protobuf_null_value.py
 kfp_server_api/models/protobuf_struct.py
@@ -56,14 +48,15 @@
 kfp_server_api/models/v2beta1_list_recurring_runs_response.py
 kfp_server_api/models/v2beta1_list_runs_response.py
 kfp_server_api/models/v2beta1_periodic_schedule.py
 kfp_server_api/models/v2beta1_pipeline.py
 kfp_server_api/models/v2beta1_pipeline_task_detail.py
 kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
 kfp_server_api/models/v2beta1_pipeline_version.py
+kfp_server_api/models/v2beta1_pipeline_version_reference.py
 kfp_server_api/models/v2beta1_predicate.py
 kfp_server_api/models/v2beta1_predicate_operation.py
 kfp_server_api/models/v2beta1_read_artifact_response.py
 kfp_server_api/models/v2beta1_recurring_run.py
 kfp_server_api/models/v2beta1_recurring_run_status.py
 kfp_server_api/models/v2beta1_run.py
 kfp_server_api/models/v2beta1_run_details.py
@@ -71,30 +64,22 @@
 kfp_server_api/models/v2beta1_runtime_config.py
 kfp_server_api/models/v2beta1_runtime_state.py
 kfp_server_api/models/v2beta1_runtime_status.py
 kfp_server_api/models/v2beta1_trigger.py
 kfp_server_api/models/v2beta1_url.py
 kfp_server_api/models/v2beta1_visualization.py
 kfp_server_api/models/v2beta1_visualization_type.py
-test/test_api_parameter.py
-test/test_api_pipeline.py
-test/test_api_pipeline_version.py
-test/test_api_relationship.py
-test/test_api_resource_key.py
-test/test_api_resource_reference.py
-test/test_api_resource_type.py
-test/test_api_status.py
-test/test_api_url.py
 test/test_auth_service_api.py
 test/test_authorize_request_resources.py
 test/test_authorize_request_verb.py
 test/test_experiment_service_api.py
 test/test_googlerpc_status.py
 test/test_healthz_service_api.py
 test/test_pipeline_service_api.py
+test/test_pipeline_task_detail_child_task.py
 test/test_pipeline_upload_service_api.py
 test/test_predicate_int_values.py
 test/test_predicate_long_values.py
 test/test_predicate_string_values.py
 test/test_protobuf_any.py
 test/test_protobuf_list_value.py
 test/test_protobuf_null_value.py
@@ -116,14 +101,15 @@
 test/test_v2beta1_list_recurring_runs_response.py
 test/test_v2beta1_list_runs_response.py
 test/test_v2beta1_periodic_schedule.py
 test/test_v2beta1_pipeline.py
 test/test_v2beta1_pipeline_task_detail.py
 test/test_v2beta1_pipeline_task_executor_detail.py
 test/test_v2beta1_pipeline_version.py
+test/test_v2beta1_pipeline_version_reference.py
 test/test_v2beta1_predicate.py
 test/test_v2beta1_predicate_operation.py
 test/test_v2beta1_read_artifact_response.py
 test/test_v2beta1_recurring_run.py
 test/test_v2beta1_recurring_run_status.py
 test/test_v2beta1_run.py
 test/test_v2beta1_run_details.py
```

### Comparing `kfp-server-api-2.0.0b0/setup.py` & `kfp-server-api-2.0.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-server-api"
-VERSION = "2.0.0-beta.0"
+VERSION = "2.0.0-beta.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_parameter.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_cron_schedule.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_parameter import ApiParameter  # noqa: E501
+from kfp_server_api.models.v2beta1_cron_schedule import V2beta1CronSchedule  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiParameter(unittest.TestCase):
-    """ApiParameter unit test stubs"""
+class TestV2beta1CronSchedule(unittest.TestCase):
+    """V2beta1CronSchedule unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiParameter
+        """Test V2beta1CronSchedule
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_parameter.ApiParameter()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_cron_schedule.V2beta1CronSchedule()  # noqa: E501
         if include_optional :
-            return ApiParameter(
-                name = '0', 
-                value = '0'
+            return V2beta1CronSchedule(
+                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                cron = '0'
             )
         else :
-            return ApiParameter(
+            return V2beta1CronSchedule(
         )
 
-    def testApiParameter(self):
-        """Test ApiParameter"""
+    def testV2beta1CronSchedule(self):
+        """Test V2beta1CronSchedule"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_pipeline.py` & `kfp-server-api-2.0.0b1/test/test_predicate_int_values.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,50 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_pipeline import ApiPipeline  # noqa: E501
+from kfp_server_api.models.predicate_int_values import PredicateIntValues  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiPipeline(unittest.TestCase):
-    """ApiPipeline unit test stubs"""
+class TestPredicateIntValues(unittest.TestCase):
+    """PredicateIntValues unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiPipeline
+        """Test PredicateIntValues
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_pipeline.ApiPipeline()  # noqa: E501
+        # model = kfp_server_api.models.predicate_int_values.PredicateIntValues()  # noqa: E501
         if include_optional :
-            return ApiPipeline(
-                id = '0', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                name = '0', 
-                description = '0', 
-                parameters = [
-                    kfp_server_api.models.api_parameter.apiParameter(
-                        name = '0', 
-                        value = '0', )
-                    ], 
-                error = '0'
+            return PredicateIntValues(
+                values = [
+                    56
+                    ]
             )
         else :
-            return ApiPipeline(
+            return PredicateIntValues(
         )
 
-    def testApiPipeline(self):
-        """Test ApiPipeline"""
+    def testPredicateIntValues(self):
+        """Test PredicateIntValues"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_pipeline_version.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,59 +12,53 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_pipeline_version import ApiPipelineVersion  # noqa: E501
+from kfp_server_api.models.v2beta1_pipeline import V2beta1Pipeline  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiPipelineVersion(unittest.TestCase):
-    """ApiPipelineVersion unit test stubs"""
+class TestV2beta1Pipeline(unittest.TestCase):
+    """V2beta1Pipeline unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiPipelineVersion
+        """Test V2beta1Pipeline
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_pipeline_version.ApiPipelineVersion()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_pipeline.V2beta1Pipeline()  # noqa: E501
         if include_optional :
-            return ApiPipelineVersion(
-                id = '0', 
-                name = '0', 
+            return V2beta1Pipeline(
+                pipeline_id = '0', 
+                display_name = '0', 
+                description = '0', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                parameters = [
-                    kfp_server_api.models.api_parameter.apiParameter(
-                        name = '0', 
-                        value = '0', )
-                    ], 
-                code_source_url = '0', 
-                package_url = kfp_server_api.models.api_url.apiUrl(
-                    pipeline_url = '0', ), 
-                resource_references = [
-                    kfp_server_api.models.api_resource_reference.apiResourceReference(
-                        key = kfp_server_api.models.api_resource_key.apiResourceKey(
-                            type = 'UNKNOWN_RESOURCE_TYPE', 
-                            id = '0', ), 
-                        name = '0', 
-                        relationship = 'UNKNOWN_RELATIONSHIP', )
-                    ]
+                namespace = '0', 
+                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                    code = 56, 
+                    message = '0', 
+                    details = [
+                        kfp_server_api.models.protobuf_any.protobufAny(
+                            type_url = '0', 
+                            value = 'YQ==', )
+                        ], )
             )
         else :
-            return ApiPipelineVersion(
+            return V2beta1Pipeline(
         )
 
-    def testApiPipelineVersion(self):
-        """Test ApiPipelineVersion"""
+    def testV2beta1Pipeline(self):
+        """Test V2beta1Pipeline"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_relationship.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_relationship import ApiRelationship  # noqa: E501
+from kfp_server_api.models.v2beta1_runtime_state import V2beta1RuntimeState  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiRelationship(unittest.TestCase):
-    """ApiRelationship unit test stubs"""
+class TestV2beta1RuntimeState(unittest.TestCase):
+    """V2beta1RuntimeState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiRelationship
+        """Test V2beta1RuntimeState
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_relationship.ApiRelationship()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_runtime_state.V2beta1RuntimeState()  # noqa: E501
         if include_optional :
-            return ApiRelationship(
+            return V2beta1RuntimeState(
             )
         else :
-            return ApiRelationship(
+            return V2beta1RuntimeState(
         )
 
-    def testApiRelationship(self):
-        """Test ApiRelationship"""
+    def testV2beta1RuntimeState(self):
+        """Test V2beta1RuntimeState"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_resource_key.py` & `kfp-server-api-2.0.0b1/test/test_protobuf_any.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_resource_key import ApiResourceKey  # noqa: E501
+from kfp_server_api.models.protobuf_any import ProtobufAny  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiResourceKey(unittest.TestCase):
-    """ApiResourceKey unit test stubs"""
+class TestProtobufAny(unittest.TestCase):
+    """ProtobufAny unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiResourceKey
+        """Test ProtobufAny
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_resource_key.ApiResourceKey()  # noqa: E501
+        # model = kfp_server_api.models.protobuf_any.ProtobufAny()  # noqa: E501
         if include_optional :
-            return ApiResourceKey(
-                type = 'UNKNOWN_RESOURCE_TYPE', 
-                id = '0'
+            return ProtobufAny(
+                type_url = '0', 
+                value = 'YQ=='
             )
         else :
-            return ApiResourceKey(
+            return ProtobufAny(
         )
 
-    def testApiResourceKey(self):
-        """Test ApiResourceKey"""
+    def testProtobufAny(self):
+        """Test ProtobufAny"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_resource_reference.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_trigger.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,45 +12,48 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_resource_reference import ApiResourceReference  # noqa: E501
+from kfp_server_api.models.v2beta1_trigger import V2beta1Trigger  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiResourceReference(unittest.TestCase):
-    """ApiResourceReference unit test stubs"""
+class TestV2beta1Trigger(unittest.TestCase):
+    """V2beta1Trigger unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiResourceReference
+        """Test V2beta1Trigger
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_resource_reference.ApiResourceReference()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_trigger.V2beta1Trigger()  # noqa: E501
         if include_optional :
-            return ApiResourceReference(
-                key = kfp_server_api.models.api_resource_key.apiResourceKey(
-                    type = 'UNKNOWN_RESOURCE_TYPE', 
-                    id = '0', ), 
-                name = '0', 
-                relationship = 'UNKNOWN_RELATIONSHIP'
+            return V2beta1Trigger(
+                cron_schedule = kfp_server_api.models.v2beta1_cron_schedule.v2beta1CronSchedule(
+                    start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    cron = '0', ), 
+                periodic_schedule = kfp_server_api.models.v2beta1_periodic_schedule.v2beta1PeriodicSchedule(
+                    start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    interval_second = '0', )
             )
         else :
-            return ApiResourceReference(
+            return V2beta1Trigger(
         )
 
-    def testApiResourceReference(self):
-        """Test ApiResourceReference"""
+    def testV2beta1Trigger(self):
+        """Test V2beta1Trigger"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_resource_type.py` & `kfp-server-api-2.0.0b1/test/test_authorize_request_resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_resource_type import ApiResourceType  # noqa: E501
+from kfp_server_api.models.authorize_request_resources import AuthorizeRequestResources  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiResourceType(unittest.TestCase):
-    """ApiResourceType unit test stubs"""
+class TestAuthorizeRequestResources(unittest.TestCase):
+    """AuthorizeRequestResources unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiResourceType
+        """Test AuthorizeRequestResources
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_resource_type.ApiResourceType()  # noqa: E501
+        # model = kfp_server_api.models.authorize_request_resources.AuthorizeRequestResources()  # noqa: E501
         if include_optional :
-            return ApiResourceType(
+            return AuthorizeRequestResources(
             )
         else :
-            return ApiResourceType(
+            return AuthorizeRequestResources(
         )
 
-    def testApiResourceType(self):
-        """Test ApiResourceType"""
+    def testAuthorizeRequestResources(self):
+        """Test AuthorizeRequestResources"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_status.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,47 +12,50 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_status import ApiStatus  # noqa: E501
+from kfp_server_api.models.v2beta1_runtime_status import V2beta1RuntimeStatus  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiStatus(unittest.TestCase):
-    """ApiStatus unit test stubs"""
+class TestV2beta1RuntimeStatus(unittest.TestCase):
+    """V2beta1RuntimeStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiStatus
+        """Test V2beta1RuntimeStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_status.ApiStatus()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_runtime_status.V2beta1RuntimeStatus()  # noqa: E501
         if include_optional :
-            return ApiStatus(
-                error = '0', 
-                code = 56, 
-                details = [
-                    kfp_server_api.models.protobuf_any.protobufAny(
-                        type_url = '0', 
-                        value = 'YQ==', )
-                    ]
+            return V2beta1RuntimeStatus(
+                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                state = 'RUNTIME_STATE_UNSPECIFIED', 
+                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                    code = 56, 
+                    message = '0', 
+                    details = [
+                        kfp_server_api.models.protobuf_any.protobufAny(
+                            type_url = '0', 
+                            value = 'YQ==', )
+                        ], )
             )
         else :
-            return ApiStatus(
+            return V2beta1RuntimeStatus(
         )
 
-    def testApiStatus(self):
-        """Test ApiStatus"""
+    def testV2beta1RuntimeStatus(self):
+        """Test V2beta1RuntimeStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_api_url.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.api_url import ApiUrl  # noqa: E501
+from kfp_server_api.models.v2beta1_url import V2beta1Url  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestApiUrl(unittest.TestCase):
-    """ApiUrl unit test stubs"""
+class TestV2beta1Url(unittest.TestCase):
+    """V2beta1Url unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ApiUrl
+        """Test V2beta1Url
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.api_url.ApiUrl()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_url.V2beta1Url()  # noqa: E501
         if include_optional :
-            return ApiUrl(
+            return V2beta1Url(
                 pipeline_url = '0'
             )
         else :
-            return ApiUrl(
+            return V2beta1Url(
         )
 
-    def testApiUrl(self):
-        """Test ApiUrl"""
+    def testV2beta1Url(self):
+        """Test V2beta1Url"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_auth_service_api.py` & `kfp-server-api-2.0.0b1/test/test_auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_authorize_request_resources.py` & `kfp-server-api-2.0.0b1/test/test_authorize_request_verb.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.authorize_request_resources import AuthorizeRequestResources  # noqa: E501
+from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestAuthorizeRequestResources(unittest.TestCase):
-    """AuthorizeRequestResources unit test stubs"""
+class TestAuthorizeRequestVerb(unittest.TestCase):
+    """AuthorizeRequestVerb unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AuthorizeRequestResources
+        """Test AuthorizeRequestVerb
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.authorize_request_resources.AuthorizeRequestResources()  # noqa: E501
+        # model = kfp_server_api.models.authorize_request_verb.AuthorizeRequestVerb()  # noqa: E501
         if include_optional :
-            return AuthorizeRequestResources(
+            return AuthorizeRequestVerb(
             )
         else :
-            return AuthorizeRequestResources(
+            return AuthorizeRequestVerb(
         )
 
-    def testAuthorizeRequestResources(self):
-        """Test AuthorizeRequestResources"""
+    def testAuthorizeRequestVerb(self):
+        """Test AuthorizeRequestVerb"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_authorize_request_verb.py` & `kfp-server-api-2.0.0b1/test/test_googlerpc_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,40 +12,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb  # noqa: E501
+from kfp_server_api.models.googlerpc_status import GooglerpcStatus  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestAuthorizeRequestVerb(unittest.TestCase):
-    """AuthorizeRequestVerb unit test stubs"""
+class TestGooglerpcStatus(unittest.TestCase):
+    """GooglerpcStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AuthorizeRequestVerb
+        """Test GooglerpcStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.authorize_request_verb.AuthorizeRequestVerb()  # noqa: E501
+        # model = kfp_server_api.models.googlerpc_status.GooglerpcStatus()  # noqa: E501
         if include_optional :
-            return AuthorizeRequestVerb(
+            return GooglerpcStatus(
+                code = 56, 
+                message = '0', 
+                details = [
+                    kfp_server_api.models.protobuf_any.protobufAny(
+                        type_url = '0', 
+                        value = 'YQ==', )
+                    ]
             )
         else :
-            return AuthorizeRequestVerb(
+            return GooglerpcStatus(
         )
 
-    def testAuthorizeRequestVerb(self):
-        """Test AuthorizeRequestVerb"""
+    def testGooglerpcStatus(self):
+        """Test GooglerpcStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_experiment_service_api.py` & `kfp-server-api-2.0.0b1/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_googlerpc_status.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,47 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.googlerpc_status import GooglerpcStatus  # noqa: E501
+from kfp_server_api.models.v2beta1_recurring_run_status import V2beta1RecurringRunStatus  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestGooglerpcStatus(unittest.TestCase):
-    """GooglerpcStatus unit test stubs"""
+class TestV2beta1RecurringRunStatus(unittest.TestCase):
+    """V2beta1RecurringRunStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GooglerpcStatus
+        """Test V2beta1RecurringRunStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.googlerpc_status.GooglerpcStatus()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_recurring_run_status.V2beta1RecurringRunStatus()  # noqa: E501
         if include_optional :
-            return GooglerpcStatus(
-                code = 56, 
-                message = '0', 
-                details = [
-                    kfp_server_api.models.protobuf_any.protobufAny(
-                        type_url = '0', 
-                        value = 'YQ==', )
-                    ]
+            return V2beta1RecurringRunStatus(
             )
         else :
-            return GooglerpcStatus(
+            return V2beta1RecurringRunStatus(
         )
 
-    def testGooglerpcStatus(self):
-        """Test GooglerpcStatus"""
+    def testV2beta1RecurringRunStatus(self):
+        """Test V2beta1RecurringRunStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_healthz_service_api.py` & `kfp-server-api-2.0.0b1/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_pipeline_service_api.py` & `kfp-server-api-2.0.0b1/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_pipeline_upload_service_api.py` & `kfp-server-api-2.0.0b1/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_predicate_int_values.py` & `kfp-server-api-2.0.0b1/test/test_predicate_long_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.predicate_int_values import PredicateIntValues  # noqa: E501
+from kfp_server_api.models.predicate_long_values import PredicateLongValues  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestPredicateIntValues(unittest.TestCase):
-    """PredicateIntValues unit test stubs"""
+class TestPredicateLongValues(unittest.TestCase):
+    """PredicateLongValues unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PredicateIntValues
+        """Test PredicateLongValues
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.predicate_int_values.PredicateIntValues()  # noqa: E501
+        # model = kfp_server_api.models.predicate_long_values.PredicateLongValues()  # noqa: E501
         if include_optional :
-            return PredicateIntValues(
+            return PredicateLongValues(
                 values = [
-                    56
+                    '0'
                     ]
             )
         else :
-            return PredicateIntValues(
+            return PredicateLongValues(
         )
 
-    def testPredicateIntValues(self):
-        """Test PredicateIntValues"""
+    def testPredicateLongValues(self):
+        """Test PredicateLongValues"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_predicate_long_values.py` & `kfp-server-api-2.0.0b1/test/test_predicate_string_values.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.predicate_long_values import PredicateLongValues  # noqa: E501
+from kfp_server_api.models.predicate_string_values import PredicateStringValues  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestPredicateLongValues(unittest.TestCase):
-    """PredicateLongValues unit test stubs"""
+class TestPredicateStringValues(unittest.TestCase):
+    """PredicateStringValues unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PredicateLongValues
+        """Test PredicateStringValues
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.predicate_long_values.PredicateLongValues()  # noqa: E501
+        # model = kfp_server_api.models.predicate_string_values.PredicateStringValues()  # noqa: E501
         if include_optional :
-            return PredicateLongValues(
+            return PredicateStringValues(
                 values = [
                     '0'
                     ]
             )
         else :
-            return PredicateLongValues(
+            return PredicateStringValues(
         )
 
-    def testPredicateLongValues(self):
-        """Test PredicateLongValues"""
+    def testPredicateStringValues(self):
+        """Test PredicateStringValues"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_predicate_string_values.py` & `kfp-server-api-2.0.0b1/test/test_protobuf_null_value.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,43 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.predicate_string_values import PredicateStringValues  # noqa: E501
+from kfp_server_api.models.protobuf_null_value import ProtobufNullValue  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestPredicateStringValues(unittest.TestCase):
-    """PredicateStringValues unit test stubs"""
+class TestProtobufNullValue(unittest.TestCase):
+    """ProtobufNullValue unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PredicateStringValues
+        """Test ProtobufNullValue
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.predicate_string_values.PredicateStringValues()  # noqa: E501
+        # model = kfp_server_api.models.protobuf_null_value.ProtobufNullValue()  # noqa: E501
         if include_optional :
-            return PredicateStringValues(
-                values = [
-                    '0'
-                    ]
+            return ProtobufNullValue(
             )
         else :
-            return PredicateStringValues(
+            return ProtobufNullValue(
         )
 
-    def testPredicateStringValues(self):
-        """Test PredicateStringValues"""
+    def testProtobufNullValue(self):
+        """Test ProtobufNullValue"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_protobuf_any.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,42 +12,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.protobuf_any import ProtobufAny  # noqa: E501
+from kfp_server_api.models.v2beta1_visualization import V2beta1Visualization  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestProtobufAny(unittest.TestCase):
-    """ProtobufAny unit test stubs"""
+class TestV2beta1Visualization(unittest.TestCase):
+    """V2beta1Visualization unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ProtobufAny
+        """Test V2beta1Visualization
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.protobuf_any.ProtobufAny()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_visualization.V2beta1Visualization()  # noqa: E501
         if include_optional :
-            return ProtobufAny(
-                type_url = '0', 
-                value = 'YQ=='
+            return V2beta1Visualization(
+                type = 'ROC_CURVE', 
+                source = '0', 
+                arguments = '0', 
+                html = '0', 
+                error = '0'
             )
         else :
-            return ProtobufAny(
+            return V2beta1Visualization(
         )
 
-    def testProtobufAny(self):
-        """Test ProtobufAny"""
+    def testV2beta1Visualization(self):
+        """Test V2beta1Visualization"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_protobuf_list_value.py` & `kfp-server-api-2.0.0b1/test/test_protobuf_list_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_protobuf_struct.py` & `kfp-server-api-2.0.0b1/test/test_protobuf_struct.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_protobuf_value.py` & `kfp-server-api-2.0.0b1/test/test_protobuf_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_recurring_run_mode.py` & `kfp-server-api-2.0.0b1/test/test_recurring_run_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_recurring_run_service_api.py` & `kfp-server-api-2.0.0b1/test/test_recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_report_service_api.py` & `kfp-server-api-2.0.0b1/test/test_report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_run_service_api.py` & `kfp-server-api-2.0.0b1/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_artifact_list.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_artifact_list.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_cron_schedule.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_run_storage_state.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,43 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_cron_schedule import V2beta1CronSchedule  # noqa: E501
+from kfp_server_api.models.v2beta1_run_storage_state import V2beta1RunStorageState  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1CronSchedule(unittest.TestCase):
-    """V2beta1CronSchedule unit test stubs"""
+class TestV2beta1RunStorageState(unittest.TestCase):
+    """V2beta1RunStorageState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1CronSchedule
+        """Test V2beta1RunStorageState
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_cron_schedule.V2beta1CronSchedule()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_run_storage_state.V2beta1RunStorageState()  # noqa: E501
         if include_optional :
-            return V2beta1CronSchedule(
-                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                cron = '0'
+            return V2beta1RunStorageState(
             )
         else :
-            return V2beta1CronSchedule(
+            return V2beta1RunStorageState(
         )
 
-    def testV2beta1CronSchedule(self):
-        """Test V2beta1CronSchedule"""
+    def testV2beta1RunStorageState(self):
+        """Test V2beta1RunStorageState"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_experiment.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_experiment_storage_state.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_filter.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_filter.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_get_healthz_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_list_experiments_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipeline_versions_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                         pipeline_id = '0', 
                         pipeline_version_id = '0', 
                         display_name = '0', 
                         description = '0', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         package_url = kfp_server_api.models.v2beta1_url.v2beta1Url(
                             pipeline_url = '0', ), 
+                        code_source_url = '0', 
                         pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
                             fields = {
                                 'key' : kfp_server_api.models.protobuf_value.protobufValue(
                                     null_value = 'NULL_VALUE', 
                                     number_value = 1.337, 
                                     string_value = '0', 
                                     bool_value = True,
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_list_pipelines_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_list_recurring_runs_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,17 @@
                                         values = [
                                             kfp_server_api.models.protobuf_value.protobufValue(
                                                 number_value = 1.337, 
                                                 string_value = '0', 
                                                 bool_value = True, )
                                             ], ), )
                                 }, ), 
+                        pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
+                            pipeline_id = '0', 
+                            pipeline_version_id = '0', ), 
                         runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                             parameters = {
                                 'key' : kfp_server_api.models.protobuf_value.protobufValue(
                                     number_value = 1.337, 
                                     string_value = '0', 
                                     bool_value = True, )
                                 },
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_list_runs_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_list_runs_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,17 @@
                                         values = [
                                             kfp_server_api.models.protobuf_value.protobufValue(
                                                 number_value = 1.337, 
                                                 string_value = '0', 
                                                 bool_value = True, )
                                             ], ), )
                                 }, ), 
+                        pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
+                            pipeline_id = '0', 
+                            pipeline_version_id = '0', ), 
                         runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                             parameters = {
                                 'key' : kfp_server_api.models.protobuf_value.protobufValue(
                                     number_value = 1.337, 
                                     string_value = '0', 
                                     bool_value = True, )
                                 }, 
@@ -111,14 +114,20 @@
                                     outputs = {
                                         'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList()
                                         }, 
                                     parent_task_id = '0', 
                                     state_history = [
                                         kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
                                             update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                                        ], 
+                                    pod_name = '0', 
+                                    child_tasks = [
+                                        kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                                            task_id = '0', 
+                                            pod_name = '0', )
                                         ], )
                                 ], ), 
                         recurring_run_id = '0', 
                         state_history = [
                             kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
                                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                             ], )
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_periodic_schedule.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_detail.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,20 @@
                             code = 56, 
                             message = '0', 
                             details = [
                                 kfp_server_api.models.protobuf_any.protobufAny(
                                     type_url = '0', 
                                     value = 'YQ==', )
                                 ], ), )
+                    ], 
+                pod_name = '0', 
+                child_tasks = [
+                    kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                        task_id = '0', 
+                        pod_name = '0', )
                     ]
             )
         else :
             return V2beta1PipelineTaskDetail(
         )
 
     def testV2beta1PipelineTaskDetail(self):
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_pipeline_version.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
                 pipeline_id = '0', 
                 pipeline_version_id = '0', 
                 display_name = '0', 
                 description = '0', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 package_url = kfp_server_api.models.v2beta1_url.v2beta1Url(
                     pipeline_url = '0', ), 
+                code_source_url = '0', 
                 pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
                     fields = {
                         'key' : kfp_server_api.models.protobuf_value.protobufValue(
                             null_value = 'NULL_VALUE', 
                             number_value = 1.337, 
                             string_value = '0', 
                             bool_value = True,
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_predicate.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_predicate_operation.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_predicate_operation.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_read_artifact_response.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_recurring_run.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
                                 values = [
                                     kfp_server_api.models.protobuf_value.protobufValue(
                                         number_value = 1.337, 
                                         string_value = '0', 
                                         bool_value = True, )
                                     ], ), )
                         }, ), 
+                pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
+                    pipeline_id = '0', 
+                    pipeline_version_id = '0', ), 
                 runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                     parameters = {
                         'key' : kfp_server_api.models.protobuf_value.protobufValue(
                             null_value = 'NULL_VALUE', 
                             number_value = 1.337, 
                             string_value = '0', 
                             bool_value = True,
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_recurring_run_status.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_visualization_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_recurring_run_status import V2beta1RecurringRunStatus  # noqa: E501
+from kfp_server_api.models.v2beta1_visualization_type import V2beta1VisualizationType  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1RecurringRunStatus(unittest.TestCase):
-    """V2beta1RecurringRunStatus unit test stubs"""
+class TestV2beta1VisualizationType(unittest.TestCase):
+    """V2beta1VisualizationType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1RecurringRunStatus
+        """Test V2beta1VisualizationType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_recurring_run_status.V2beta1RecurringRunStatus()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_visualization_type.V2beta1VisualizationType()  # noqa: E501
         if include_optional :
-            return V2beta1RecurringRunStatus(
+            return V2beta1VisualizationType(
             )
         else :
-            return V2beta1RecurringRunStatus(
+            return V2beta1VisualizationType(
         )
 
-    def testV2beta1RecurringRunStatus(self):
-        """Test V2beta1RecurringRunStatus"""
+    def testV2beta1VisualizationType(self):
+        """Test V2beta1VisualizationType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_run.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,17 @@
                                 values = [
                                     kfp_server_api.models.protobuf_value.protobufValue(
                                         number_value = 1.337, 
                                         string_value = '0', 
                                         bool_value = True, )
                                     ], ), )
                         }, ), 
+                pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
+                    pipeline_id = '0', 
+                    pipeline_version_id = '0', ), 
                 runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                     parameters = {
                         'key' : kfp_server_api.models.protobuf_value.protobufValue(
                             null_value = 'NULL_VALUE', 
                             number_value = 1.337, 
                             string_value = '0', 
                             bool_value = True, 
@@ -134,14 +137,20 @@
                             outputs = {
                                 'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList()
                                 }, 
                             parent_task_id = '0', 
                             state_history = [
                                 kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
                                     update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                                ], 
+                            pod_name = '0', 
+                            child_tasks = [
+                                kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                                    task_id = '0', 
+                                    pod_name = '0', )
                                 ], )
                         ], ), 
                 recurring_run_id = '0', 
                 state_history = [
                     kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
                         update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         state = 'RUNTIME_STATE_UNSPECIFIED',
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_run_details.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_run_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,14 +74,20 @@
                         outputs = {
                             'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList()
                             }, 
                         parent_task_id = '0', 
                         state_history = [
                             kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
                                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                            ], 
+                        pod_name = '0', 
+                        child_tasks = [
+                            kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                                task_id = '0', 
+                                pod_name = '0', )
                             ], )
                     ]
             )
         else :
             return V2beta1RunDetails(
         )
```

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_runtime_config.py` & `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b0/test/test_v2beta1_runtime_state.py` & `kfp-server-api-2.0.0b1/test/test_pipeline_task_detail_child_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_runtime_state import V2beta1RuntimeState  # noqa: E501
+from kfp_server_api.models.pipeline_task_detail_child_task import PipelineTaskDetailChildTask  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1RuntimeState(unittest.TestCase):
-    """V2beta1RuntimeState unit test stubs"""
+class TestPipelineTaskDetailChildTask(unittest.TestCase):
+    """PipelineTaskDetailChildTask unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1RuntimeState
+        """Test PipelineTaskDetailChildTask
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_runtime_state.V2beta1RuntimeState()  # noqa: E501
+        # model = kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask()  # noqa: E501
         if include_optional :
-            return V2beta1RuntimeState(
+            return PipelineTaskDetailChildTask(
+                task_id = '0', 
+                pod_name = '0'
             )
         else :
-            return V2beta1RuntimeState(
+            return PipelineTaskDetailChildTask(
         )
 
-    def testV2beta1RuntimeState(self):
-        """Test V2beta1RuntimeState"""
+    def testPipelineTaskDetailChildTask(self):
+        """Test PipelineTaskDetailChildTask"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b0/test/test_visualization_service_api.py` & `kfp-server-api-2.0.0b1/test/test_visualization_service_api.py`

 * *Files identical despite different names*

