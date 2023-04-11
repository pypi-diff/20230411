# Comparing `tmp/rhoas_sdks-1.0.2.tar.gz` & `tmp/rhoas_sdks-1.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhoas_sdks-1.0.2.tar", max compression
+gzip compressed data, was "rhoas_sdks-1.0.2b2.tar", max compression
```

## Comparing `rhoas_sdks-1.0.2.tar` & `rhoas_sdks-1.0.2b2.tar`

### file list

```diff
@@ -1,373 +1,373 @@
--rw-r--r--   0        0        0      119 2023-04-11 14:03:33.816823 rhoas_sdks-1.0.2/auth/constants.py
--rw-r--r--   0        0        0      739 2023-04-11 14:03:33.816823 rhoas_sdks-1.0.2/auth/rhoas_auth.py
--rw-r--r--   0        0        0    13014 2023-04-11 14:03:33.816823 rhoas_sdks-1.0.2/docs/README.md
--rw-r--r--   0        0        0     1100 2023-04-11 14:06:44.859678 rhoas_sdks-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      856 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/__init__.py
--rw-r--r--   0        0        0      238 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/__init__.py
--rw-r--r--   0        0        0    46289 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_clusters_api.py
--rw-r--r--   0        0        0    20339 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_namespaces_api.py
--rw-r--r--   0        0        0     5593 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_service_api.py
--rw-r--r--   0        0        0    22768 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_types_api.py
--rw-r--r--   0        0        0    30236 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connectors_api.py
--rw-r--r--   0        0        0    39197 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api_client.py
--rw-r--r--   0        0        0      864 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/apis/__init__.py
--rw-r--r--   0        0        0    16938 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/configuration.py
--rw-r--r--   0        0        0     5108 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/exceptions.py
--rw-r--r--   0        0        0      358 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/__init__.py
--rw-r--r--   0        0        0    11633 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter.py
--rw-r--r--   0        0        0    12084 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter_list.py
--rw-r--r--   0        0        0    11602 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/channel.py
--rw-r--r--   0        0        0    18979 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector.py
--rw-r--r--   0        0        0    16118 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster.py
--rw-r--r--   0        0        0    14477 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list.py
--rw-r--r--   0        0        0    11742 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list_all_of.py
--rw-r--r--   0        0        0    14971 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_meta.py
--rw-r--r--   0        0        0    14209 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request.py
--rw-r--r--   0        0        0    12035 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request_meta.py
--rw-r--r--   0        0        0    12114 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_state.py
--rw-r--r--   0        0        0    11818 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status.py
--rw-r--r--   0        0        0    11964 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status_status.py
--rw-r--r--   0        0        0    13260 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_configuration.py
--rw-r--r--   0        0        0    12174 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_desired_state.py
--rw-r--r--   0        0        0    14370 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list.py
--rw-r--r--   0        0        0    11671 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list_all_of.py
--rw-r--r--   0        0        0    16328 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta.py
--rw-r--r--   0        0        0    11532 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta_all_of.py
--rw-r--r--   0        0        0    17393 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace.py
--rw-r--r--   0        0        0    13045 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_all_of.py
--rw-r--r--   0        0        0    14648 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_eval_request.py
--rw-r--r--   0        0        0    14507 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list.py
--rw-r--r--   0        0        0    11762 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list_all_of.py
--rw-r--r--   0        0        0    16268 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta.py
--rw-r--r--   0        0        0    12030 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta_all_of.py
--rw-r--r--   0        0        0    14651 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_patch_request.py
--rw-r--r--   0        0        0    12759 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_quota.py
--rw-r--r--   0        0        0    15370 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request.py
--rw-r--r--   0        0        0    12040 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_all_of.py
--rw-r--r--   0        0        0    12452 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_meta.py
--rw-r--r--   0        0        0    12198 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_state.py
--rw-r--r--   0        0        0    12562 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_status.py
--rw-r--r--   0        0        0    12148 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant.py
--rw-r--r--   0        0        0    12045 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant_kind.py
--rw-r--r--   0        0        0    16918 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request.py
--rw-r--r--   0        0        0    13469 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request_meta.py
--rw-r--r--   0        0        0    11267 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_resource_annotations.py
--rw-r--r--   0        0        0    12699 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_state.py
--rw-r--r--   0        0        0    11747 2023-04-11 14:03:33.820823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status.py
--rw-r--r--   0        0        0    11893 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status_status.py
--rw-r--r--   0        0        0    17665 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type.py
--rw-r--r--   0        0        0    15009 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_all_of.py
--rw-r--r--   0        0        0    11895 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count.py
--rw-r--r--   0        0        0    11799 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count_list.py
--rw-r--r--   0        0        0    14432 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list.py
--rw-r--r--   0        0        0    11712 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list_all_of.py
--rw-r--r--   0        0        0    11961 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/cpu_quota.py
--rw-r--r--   0        0        0    12452 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/error.py
--rw-r--r--   0        0        0    13789 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/kafka_connection_settings.py
--rw-r--r--   0        0        0    12053 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/list.py
--rw-r--r--   0        0        0    11982 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/memory_quota.py
--rw-r--r--   0        0        0    11904 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_meta.py
--rw-r--r--   0        0        0    11809 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_reference.py
--rw-r--r--   0        0        0    13816 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/schema_registry_connection_settings.py
--rw-r--r--   0        0        0    11846 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_account.py
--rw-r--r--   0        0        0    11692 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_connection_settings.py
--rw-r--r--   0        0        0    14441 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata.py
--rw-r--r--   0        0        0    11750 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata_all_of.py
--rw-r--r--   0        0        0    82645 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model_utils.py
--rw-r--r--   0        0        0     5510 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/models/__init__.py
--rw-r--r--   0        0        0    14345 2023-04-11 14:03:33.824823 rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/rest.py
--rw-r--r--   0        0        0      842 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/__init__.py
--rw-r--r--   0        0        0      225 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/__init__.py
--rw-r--r--   0        0        0    27080 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/acls_api.py
--rw-r--r--   0        0        0    10474 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/errors_api.py
--rw-r--r--   0        0        0    26325 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/groups_api.py
--rw-r--r--   0        0        0    14337 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/records_api.py
--rw-r--r--   0        0        0    28894 2023-04-11 14:03:33.828824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/topics_api.py
--rw-r--r--   0        0        0    39114 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api_client.py
--rw-r--r--   0        0        0      739 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/apis/__init__.py
--rw-r--r--   0        0        0    16782 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/configuration.py
--rw-r--r--   0        0        0     5094 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/exceptions.py
--rw-r--r--   0        0        0      358 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/__init__.py
--rw-r--r--   0        0        0    16700 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding.py
--rw-r--r--   0        0        0    14245 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_all_of.py
--rw-r--r--   0        0        0    14868 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page.py
--rw-r--r--   0        0        0    11728 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page_all_of.py
--rw-r--r--   0        0        0    12427 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_order_key.py
--rw-r--r--   0        0        0    12535 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation.py
--rw-r--r--   0        0        0    12607 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation_filter.py
--rw-r--r--   0        0        0    11983 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type.py
--rw-r--r--   0        0        0    12313 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type_filter.py
--rw-r--r--   0        0        0    11956 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type.py
--rw-r--r--   0        0        0    12028 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type_filter.py
--rw-r--r--   0        0        0    12166 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type.py
--rw-r--r--   0        0        0    12238 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type_filter.py
--rw-r--r--   0        0        0    12195 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/config_entry.py
--rw-r--r--   0        0        0    13848 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer.py
--rw-r--r--   0        0        0    15979 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group.py
--rw-r--r--   0        0        0    13063 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_all_of.py
--rw-r--r--   0        0        0    12181 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_description_order_key.py
--rw-r--r--   0        0        0    15781 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list.py
--rw-r--r--   0        0        0    11746 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list_all_of.py
--rw-r--r--   0        0        0    12032 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_metrics.py
--rw-r--r--   0        0        0    11606 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_order_key.py
--rw-r--r--   0        0        0    13012 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_parameters.py
--rw-r--r--   0        0        0    15137 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result.py
--rw-r--r--   0        0        0    11936 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_all_of.py
--rw-r--r--   0        0        0    11902 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_item.py
--rw-r--r--   0        0        0    12415 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_state.py
--rw-r--r--   0        0        0    15745 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error.py
--rw-r--r--   0        0        0    12598 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_all_of.py
--rw-r--r--   0        0        0    14760 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list.py
--rw-r--r--   0        0        0    11946 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list_all_of.py
--rw-r--r--   0        0        0    12315 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list.py
--rw-r--r--   0        0        0    15413 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated.py
--rw-r--r--   0        0        0    12133 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated_all_of.py
--rw-r--r--   0        0        0    12140 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/new_topic_input.py
--rw-r--r--   0        0        0    11406 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/node.py
--rw-r--r--   0        0        0    12107 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/object_reference.py
--rw-r--r--   0        0        0    12139 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/offset_type.py
--rw-r--r--   0        0        0    13002 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition.py
--rw-r--r--   0        0        0    13571 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition_leader.py
--rw-r--r--   0        0        0    16556 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record.py
--rw-r--r--   0        0        0    13502 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_all_of.py
--rw-r--r--   0        0        0    12409 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_included_property.py
--rw-r--r--   0        0        0    14743 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list.py
--rw-r--r--   0        0        0    12498 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list_all_of.py
--rw-r--r--   0        0        0    11932 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/sort_direction.py
--rw-r--r--   0        0        0    15627 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic.py
--rw-r--r--   0        0        0    12544 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_all_of.py
--rw-r--r--   0        0        0    12208 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_order_key.py
--rw-r--r--   0        0        0    12387 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_settings.py
--rw-r--r--   0        0        0    15667 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list.py
--rw-r--r--   0        0        0    11668 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list_all_of.py
--rw-r--r--   0        0        0    11728 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_to_reset_offset.py
--rw-r--r--   0        0        0    82631 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model_utils.py
--rw-r--r--   0        0        0     4561 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/models/__init__.py
--rw-r--r--   0        0        0    14331 2023-04-11 14:03:33.832824 rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/rest.py
--rw-r--r--   0        0        0      821 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/__init__.py
--rw-r--r--   0        0        0      224 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/__init__.py
--rw-r--r--   0        0        0    74161 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/default_api.py
--rw-r--r--   0        0        0    27109 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/enterprise_dataplane_clusters_api.py
--rw-r--r--   0        0        0    10387 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/errors_api.py
--rw-r--r--   0        0        0    30984 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/security_api.py
--rw-r--r--   0        0        0    39120 2023-04-11 14:03:33.836824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api_client.py
--rw-r--r--   0        0        0      715 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/apis/__init__.py
--rw-r--r--   0        0        0    16928 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/configuration.py
--rw-r--r--   0        0        0     5105 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/exceptions.py
--rw-r--r--   0        0        0      354 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/__init__.py
--rw-r--r--   0        0        0    12840 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider.py
--rw-r--r--   0        0        0    14431 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list.py
--rw-r--r--   0        0        0    11703 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list_all_of.py
--rw-r--r--   0        0        0    13304 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region.py
--rw-r--r--   0        0        0    14415 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list.py
--rw-r--r--   0        0        0    11697 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list_all_of.py
--rw-r--r--   0        0        0    17547 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster.py
--rw-r--r--   0        0        0    14650 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_addon_parameters.py
--rw-r--r--   0        0        0    15225 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of.py
--rw-r--r--   0        0        0    13911 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of_capacity_information.py
--rw-r--r--   0        0        0    11901 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_fleetshard_parameters.py
--rw-r--r--   0        0        0    14463 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list.py
--rw-r--r--   0        0        0    11715 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_all_of.py
--rw-r--r--   0        0        0    18189 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_registration_response.py
--rw-r--r--   0        0        0    14587 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_osd_cluster_payload.py
--rw-r--r--   0        0        0    12986 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error.py
--rw-r--r--   0        0        0    14287 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list.py
--rw-r--r--   0        0        0    11664 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list_all_of.py
--rw-r--r--   0        0        0    11637 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameter.py
--rw-r--r--   0        0        0    12215 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameters_array.py
--rw-r--r--   0        0        0    11923 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/instant_query.py
--rw-r--r--   0        0        0    13499 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_promote_request.py
--rw-r--r--   0        0        0    25271 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request.py
--rw-r--r--   0        0        0    22920 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_all_of.py
--rw-r--r--   0        0        0    14423 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list.py
--rw-r--r--   0        0        0    11700 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list_all_of.py
--rw-r--r--   0        0        0    14946 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_payload.py
--rw-r--r--   0        0        0    12125 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_update_request.py
--rw-r--r--   0        0        0    12042 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/list.py
--rw-r--r--   0        0        0    14257 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list.py
--rw-r--r--   0        0        0    12019 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list_all_of.py
--rw-r--r--   0        0        0    14241 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list.py
--rw-r--r--   0        0        0    12013 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list_all_of.py
--rw-r--r--   0        0        0    11852 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/object_reference.py
--rw-r--r--   0        0        0    11834 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/range_query.py
--rw-r--r--   0        0        0    12233 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/region_capacity_list_item.py
--rw-r--r--   0        0        0    15548 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account.py
--rw-r--r--   0        0        0    12995 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_all_of.py
--rw-r--r--   0        0        0    13948 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list.py
--rw-r--r--   0        0        0    11896 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_all_of.py
--rw-r--r--   0        0        0    15787 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item.py
--rw-r--r--   0        0        0    13192 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item_all_of.py
--rw-r--r--   0        0        0    11867 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_request.py
--rw-r--r--   0        0        0    15032 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider.py
--rw-r--r--   0        0        0    12324 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider_all_of.py
--rw-r--r--   0        0        0    13258 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_billing_model.py
--rw-r--r--   0        0        0    13608 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type.py
--rw-r--r--   0        0        0    20642 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type_sizes_inner.py
--rw-r--r--   0        0        0    14021 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list.py
--rw-r--r--   0        0        0    11742 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list_all_of.py
--rw-r--r--   0        0        0    18452 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size.py
--rw-r--r--   0        0        0    11508 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size_bytes_value_item.py
--rw-r--r--   0        0        0    11687 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/values.py
--rw-r--r--   0        0        0    14500 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata.py
--rw-r--r--   0        0        0    11963 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata_all_of.py
--rw-r--r--   0        0        0    82638 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model_utils.py
--rw-r--r--   0        0        0     5039 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/models/__init__.py
--rw-r--r--   0        0        0    14338 2023-04-11 14:03:33.840824 rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/rest.py
--rw-r--r--   0        0        0     2084 2023-04-11 14:03:33.844825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/__init__.py
--rw-r--r--   0        0        0      229 2023-04-11 14:03:33.844825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/__init__.py
--rw-r--r--   0        0        0   116696 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/admin_api.py
--rw-r--r--   0        0        0    47524 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifact_rules_api.py
--rw-r--r--   0        0        0    88869 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifacts_api.py
--rw-r--r--   0        0        0    23764 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/groups_api.py
--rw-r--r--   0        0        0    53464 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/metadata_api.py
--rw-r--r--   0        0        0    17954 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/search_api.py
--rw-r--r--   0        0        0    11617 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/system_api.py
--rw-r--r--   0        0        0     6836 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/users_api.py
--rw-r--r--   0        0        0    45766 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/versions_api.py
--rw-r--r--   0        0        0    40377 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api_client.py
--rw-r--r--   0        0        0     1046 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/apis/__init__.py
--rw-r--r--   0        0        0    17456 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/configuration.py
--rw-r--r--   0        0        0     6312 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/exceptions.py
--rw-r--r--   0        0        0      361 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/__init__.py
--rw-r--r--   0        0        0    13532 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_content.py
--rw-r--r--   0        0        0    16767 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_meta_data.py
--rw-r--r--   0        0        0    12672 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_owner.py
--rw-r--r--   0        0        0    13413 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_reference.py
--rw-r--r--   0        0        0    13610 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_search_results.py
--rw-r--r--   0        0        0    13816 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_state.py
--rw-r--r--   0        0        0    12676 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_type_info.py
--rw-r--r--   0        0        0    13598 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/configuration_property.py
--rw-r--r--   0        0        0    13326 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/create_group_meta_data.py
--rw-r--r--   0        0        0    12957 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/download_ref.py
--rw-r--r--   0        0        0    13493 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/editable_meta_data.py
--rw-r--r--   0        0        0    13676 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/error.py
--rw-r--r--   0        0        0    14548 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_meta_data.py
--rw-r--r--   0        0        0    13529 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_search_results.py
--rw-r--r--   0        0        0    13371 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/if_exists.py
--rw-r--r--   0        0        0    15923 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/limits.py
--rw-r--r--   0        0        0    12914 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_configuration.py
--rw-r--r--   0        0        0    13773 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_level.py
--rw-r--r--   0        0        0    15316 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration.py
--rw-r--r--   0        0        0    12750 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration_all_of.py
--rw-r--r--   0        0        0    12423 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/properties.py
--rw-r--r--   0        0        0    13466 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_mapping.py
--rw-r--r--   0        0        0    13281 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_type.py
--rw-r--r--   0        0        0    13067 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule.py
--rw-r--r--   0        0        0    13233 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_type.py
--rw-r--r--   0        0        0    12910 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_cause.py
--rw-r--r--   0        0        0    16461 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error.py
--rw-r--r--   0        0        0    13085 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error_all_of.py
--rw-r--r--   0        0        0    15207 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_artifact.py
--rw-r--r--   0        0        0    14104 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_group.py
--rw-r--r--   0        0        0    15782 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_version.py
--rw-r--r--   0        0        0    13179 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_by.py
--rw-r--r--   0        0        0    13152 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_order.py
--rw-r--r--   0        0        0    13276 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/system_info.py
--rw-r--r--   0        0        0    12762 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_configuration_property.py
--rw-r--r--   0        0        0    12885 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_role.py
--rw-r--r--   0        0        0    12934 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_state.py
--rw-r--r--   0        0        0    13472 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/user_info.py
--rw-r--r--   0        0        0    15795 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_meta_data.py
--rw-r--r--   0        0        0    13587 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_search_results.py
--rw-r--r--   0        0        0    83852 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model_utils.py
--rw-r--r--   0        0        0     3483 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/models/__init__.py
--rw-r--r--   0        0        0    15552 2023-04-11 14:03:33.848825 rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/rest.py
--rw-r--r--   0        0        0     1078 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/__init__.py
--rw-r--r--   0        0        0      234 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/__init__.py
--rw-r--r--   0        0        0     5947 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/default_api.py
--rw-r--r--   0        0        0    11488 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/errors_api.py
--rw-r--r--   0        0        0    23774 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/registries_api.py
--rw-r--r--   0        0        0    39320 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api_client.py
--rw-r--r--   0        0        0      659 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/apis/__init__.py
--rw-r--r--   0        0        0    17118 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/configuration.py
--rw-r--r--   0        0        0     5274 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/exceptions.py
--rw-r--r--   0        0        0      365 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/__init__.py
--rw-r--r--   0        0        0    12257 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/abstract_list.py
--rw-r--r--   0        0        0    11829 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/empty.py
--rw-r--r--   0        0        0    14633 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error.py
--rw-r--r--   0        0        0    12100 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_all_of.py
--rw-r--r--   0        0        0    14552 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list.py
--rw-r--r--   0        0        0    11866 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list_all_of.py
--rw-r--r--   0        0        0    14582 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list.py
--rw-r--r--   0        0        0    11922 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list_all_of.py
--rw-r--r--   0        0        0    12043 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/object_reference.py
--rw-r--r--   0        0        0    17009 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry.py
--rw-r--r--   0        0        0    12507 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_create.py
--rw-r--r--   0        0        0    13176 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_instance_type_value.py
--rw-r--r--   0        0        0    14597 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list.py
--rw-r--r--   0        0        0    11896 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list_all_of.py
--rw-r--r--   0        0        0    14374 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_status_value.py
--rw-r--r--   0        0        0    14892 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/root_type_for_registry.py
--rw-r--r--   0        0        0    12041 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/service_status.py
--rw-r--r--   0        0        0    82818 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model_utils.py
--rw-r--r--   0        0        0     1721 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/models/__init__.py
--rw-r--r--   0        0        0    14518 2023-04-11 14:03:33.852825 rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/rest.py
--rw-r--r--   0        0        0      921 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/__init__.py
--rw-r--r--   0        0        0      238 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/__init__.py
--rw-r--r--   0        0        0    11813 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/acs_tenants_api.py
--rw-r--r--   0        0        0    11471 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/default_api.py
--rw-r--r--   0        0        0    34067 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/service_accounts_api.py
--rw-r--r--   0        0        0    39199 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api_client.py
--rw-r--r--   0        0        0      688 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/apis/__init__.py
--rw-r--r--   0        0        0    17479 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/configuration.py
--rw-r--r--   0        0        0     5117 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/exceptions.py
--rw-r--r--   0        0        0      365 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/__init__.py
--rw-r--r--   0        0        0    12294 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_request_data.py
--rw-r--r--   0        0        0    12101 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_response_data.py
--rw-r--r--   0        0        0    11652 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_factors.py
--rw-r--r--   0        0        0    11870 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_policy.py
--rw-r--r--   0        0        0    11557 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/error.py
--rw-r--r--   0        0        0    11473 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/otp.py
--rw-r--r--   0        0        0    12719 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/red_hat_error_representation.py
--rw-r--r--   0        0        0    11979 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_create_request_data.py
--rw-r--r--   0        0        0    12824 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_data.py
--rw-r--r--   0        0        0    11919 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_request_data.py
--rw-r--r--   0        0        0    11976 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/validation_exception_data.py
--rw-r--r--   0        0        0    82661 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model_utils.py
--rw-r--r--   0        0        0     1411 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/models/__init__.py
--rw-r--r--   0        0        0    14361 2023-04-11 14:03:33.856825 rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/rest.py
--rw-r--r--   0        0        0      906 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/__init__.py
--rw-r--r--   0        0        0      231 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/__init__.py
--rw-r--r--   0        0        0    22654 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/bridges_api.py
--rw-r--r--   0        0        0    17973 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/cloud_providers_api.py
--rw-r--r--   0        0        0    11522 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/error_catalog_api.py
--rw-r--r--   0        0        0    30966 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/processors_api.py
--rw-r--r--   0        0        0    31097 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/sink_connectors_api.py
--rw-r--r--   0        0        0    31340 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/source_connectors_api.py
--rw-r--r--   0        0        0    39229 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api_client.py
--rw-r--r--   0        0        0      908 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/apis/__init__.py
--rw-r--r--   0        0        0    16974 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/configuration.py
--rw-r--r--   0        0        0     5134 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/exceptions.py
--rw-r--r--   0        0        0      361 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/__init__.py
--rw-r--r--   0        0        0    12252 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error.py
--rw-r--r--   0        0        0    12454 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_instance.py
--rw-r--r--   0        0        0    12014 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_type.py
--rw-r--r--   0        0        0    12543 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_list_response.py
--rw-r--r--   0        0        0    12474 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_request.py
--rw-r--r--   0        0        0    15062 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_response.py
--rw-r--r--   0        0        0    12614 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_list_response.py
--rw-r--r--   0        0        0    12897 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_response.py
--rw-r--r--   0        0        0    12594 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_list_response.py
--rw-r--r--   0        0        0    12243 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_response.py
--rw-r--r--   0        0        0    12627 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/connector_request.py
--rw-r--r--   0        0        0    12735 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error.py
--rw-r--r--   0        0        0    12476 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error_list_response.py
--rw-r--r--   0        0        0    11874 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/errors_list.py
--rw-r--r--   0        0        0    14500 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list.py
--rw-r--r--   0        0        0    11910 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_all_of.py
--rw-r--r--   0        0        0    11915 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_response.py
--rw-r--r--   0        0        0    12980 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/managed_resource_status.py
--rw-r--r--   0        0        0    12375 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/object_reference.py
--rw-r--r--   0        0        0    12634 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_list_response.py
--rw-r--r--   0        0        0    12183 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_response.py
--rw-r--r--   0        0        0    12573 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_list_response.py
--rw-r--r--   0        0        0    12220 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_request.py
--rw-r--r--   0        0        0    14580 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_response.py
--rw-r--r--   0        0        0    12614 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_list_response.py
--rw-r--r--   0        0        0    15396 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_response.py
--rw-r--r--   0        0        0    12634 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_list_response.py
--rw-r--r--   0        0        0    15063 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_response.py
--rw-r--r--   0        0        0    82674 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model_utils.py
--rw-r--r--   0        0        0     2755 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/models/__init__.py
--rw-r--r--   0        0        0    14374 2023-04-11 14:03:33.860826 rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/rest.py
--rw-r--r--   0        0        0    13626 1970-01-01 00:00:00.000000 rhoas_sdks-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-03-29 10:40:27.630118 rhoas_sdks-1.0.2b2/auth/constants.py
+-rw-r--r--   0        0        0      739 2023-03-29 10:40:27.630118 rhoas_sdks-1.0.2b2/auth/rhoas_auth.py
+-rw-r--r--   0        0        0    13055 2023-03-29 10:40:27.630118 rhoas_sdks-1.0.2b2/docs/README.md
+-rw-r--r--   0        0        0     1106 2023-03-29 10:43:42.539419 rhoas_sdks-1.0.2b2/pyproject.toml
+-rw-r--r--   0        0        0      856 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/__init__.py
+-rw-r--r--   0        0        0    46289 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_clusters_api.py
+-rw-r--r--   0        0        0    20339 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_namespaces_api.py
+-rw-r--r--   0        0        0     5593 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_service_api.py
+-rw-r--r--   0        0        0    22768 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_types_api.py
+-rw-r--r--   0        0        0    30236 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connectors_api.py
+-rw-r--r--   0        0        0    39197 2023-03-29 10:40:27.634118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api_client.py
+-rw-r--r--   0        0        0      864 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    16938 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/configuration.py
+-rw-r--r--   0        0        0     5108 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/exceptions.py
+-rw-r--r--   0        0        0      358 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/__init__.py
+-rw-r--r--   0        0        0    11633 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter.py
+-rw-r--r--   0        0        0    12084 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter_list.py
+-rw-r--r--   0        0        0    11602 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/channel.py
+-rw-r--r--   0        0        0    18979 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector.py
+-rw-r--r--   0        0        0    16118 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster.py
+-rw-r--r--   0        0        0    14477 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list.py
+-rw-r--r--   0        0        0    11742 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list_all_of.py
+-rw-r--r--   0        0        0    14971 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_meta.py
+-rw-r--r--   0        0        0    14209 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request.py
+-rw-r--r--   0        0        0    12035 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request_meta.py
+-rw-r--r--   0        0        0    12114 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_state.py
+-rw-r--r--   0        0        0    11818 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status.py
+-rw-r--r--   0        0        0    11964 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status_status.py
+-rw-r--r--   0        0        0    13260 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_configuration.py
+-rw-r--r--   0        0        0    12174 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_desired_state.py
+-rw-r--r--   0        0        0    14370 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list.py
+-rw-r--r--   0        0        0    11671 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list_all_of.py
+-rw-r--r--   0        0        0    16328 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta.py
+-rw-r--r--   0        0        0    11532 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta_all_of.py
+-rw-r--r--   0        0        0    17393 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace.py
+-rw-r--r--   0        0        0    13045 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_all_of.py
+-rw-r--r--   0        0        0    14648 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_eval_request.py
+-rw-r--r--   0        0        0    14507 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list.py
+-rw-r--r--   0        0        0    11762 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list_all_of.py
+-rw-r--r--   0        0        0    16268 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta.py
+-rw-r--r--   0        0        0    12030 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta_all_of.py
+-rw-r--r--   0        0        0    14651 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_patch_request.py
+-rw-r--r--   0        0        0    12759 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_quota.py
+-rw-r--r--   0        0        0    15370 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request.py
+-rw-r--r--   0        0        0    12040 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_all_of.py
+-rw-r--r--   0        0        0    12452 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_meta.py
+-rw-r--r--   0        0        0    12198 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_state.py
+-rw-r--r--   0        0        0    12562 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_status.py
+-rw-r--r--   0        0        0    12148 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant.py
+-rw-r--r--   0        0        0    12045 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant_kind.py
+-rw-r--r--   0        0        0    16918 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request.py
+-rw-r--r--   0        0        0    13469 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request_meta.py
+-rw-r--r--   0        0        0    11267 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_resource_annotations.py
+-rw-r--r--   0        0        0    12699 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_state.py
+-rw-r--r--   0        0        0    11747 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status.py
+-rw-r--r--   0        0        0    11893 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status_status.py
+-rw-r--r--   0        0        0    17665 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type.py
+-rw-r--r--   0        0        0    15009 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_all_of.py
+-rw-r--r--   0        0        0    11895 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count.py
+-rw-r--r--   0        0        0    11799 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count_list.py
+-rw-r--r--   0        0        0    14432 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list.py
+-rw-r--r--   0        0        0    11712 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list_all_of.py
+-rw-r--r--   0        0        0    11961 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/cpu_quota.py
+-rw-r--r--   0        0        0    12452 2023-03-29 10:40:27.638118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/error.py
+-rw-r--r--   0        0        0    13789 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/kafka_connection_settings.py
+-rw-r--r--   0        0        0    12491 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/list.py
+-rw-r--r--   0        0        0    11982 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/memory_quota.py
+-rw-r--r--   0        0        0    11904 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_meta.py
+-rw-r--r--   0        0        0    11809 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_reference.py
+-rw-r--r--   0        0        0    13816 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/schema_registry_connection_settings.py
+-rw-r--r--   0        0        0    11846 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_account.py
+-rw-r--r--   0        0        0    11692 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_connection_settings.py
+-rw-r--r--   0        0        0    14576 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata.py
+-rw-r--r--   0        0        0    11690 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata_all_of.py
+-rw-r--r--   0        0        0    82645 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model_utils.py
+-rw-r--r--   0        0        0     5510 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14345 2023-03-29 10:40:27.642118 rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/rest.py
+-rw-r--r--   0        0        0      842 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/__init__.py
+-rw-r--r--   0        0        0      225 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/__init__.py
+-rw-r--r--   0        0        0    27080 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/acls_api.py
+-rw-r--r--   0        0        0    10474 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/errors_api.py
+-rw-r--r--   0        0        0    26325 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/groups_api.py
+-rw-r--r--   0        0        0    14337 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/records_api.py
+-rw-r--r--   0        0        0    28894 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/topics_api.py
+-rw-r--r--   0        0        0    39114 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api_client.py
+-rw-r--r--   0        0        0      739 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    16782 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/configuration.py
+-rw-r--r--   0        0        0     5094 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/exceptions.py
+-rw-r--r--   0        0        0      358 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/__init__.py
+-rw-r--r--   0        0        0    16700 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding.py
+-rw-r--r--   0        0        0    14245 2023-03-29 10:40:27.646118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_all_of.py
+-rw-r--r--   0        0        0    14868 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page.py
+-rw-r--r--   0        0        0    11728 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page_all_of.py
+-rw-r--r--   0        0        0    12427 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_order_key.py
+-rw-r--r--   0        0        0    12535 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation.py
+-rw-r--r--   0        0        0    12607 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation_filter.py
+-rw-r--r--   0        0        0    11983 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type.py
+-rw-r--r--   0        0        0    12313 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type_filter.py
+-rw-r--r--   0        0        0    11956 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type.py
+-rw-r--r--   0        0        0    12028 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type_filter.py
+-rw-r--r--   0        0        0    12166 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type.py
+-rw-r--r--   0        0        0    12238 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type_filter.py
+-rw-r--r--   0        0        0    12195 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/config_entry.py
+-rw-r--r--   0        0        0    13848 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer.py
+-rw-r--r--   0        0        0    15979 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group.py
+-rw-r--r--   0        0        0    13063 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_all_of.py
+-rw-r--r--   0        0        0    12181 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_description_order_key.py
+-rw-r--r--   0        0        0    15781 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list.py
+-rw-r--r--   0        0        0    11746 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list_all_of.py
+-rw-r--r--   0        0        0    12032 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_metrics.py
+-rw-r--r--   0        0        0    11606 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_order_key.py
+-rw-r--r--   0        0        0    13012 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_parameters.py
+-rw-r--r--   0        0        0    15137 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result.py
+-rw-r--r--   0        0        0    11936 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_all_of.py
+-rw-r--r--   0        0        0    11902 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_item.py
+-rw-r--r--   0        0        0    12415 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_state.py
+-rw-r--r--   0        0        0    15745 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error.py
+-rw-r--r--   0        0        0    12598 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_all_of.py
+-rw-r--r--   0        0        0    14760 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list.py
+-rw-r--r--   0        0        0    11946 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list_all_of.py
+-rw-r--r--   0        0        0    12315 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list.py
+-rw-r--r--   0        0        0    15413 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated.py
+-rw-r--r--   0        0        0    12133 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated_all_of.py
+-rw-r--r--   0        0        0    12140 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/new_topic_input.py
+-rw-r--r--   0        0        0    11406 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/node.py
+-rw-r--r--   0        0        0    12107 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/object_reference.py
+-rw-r--r--   0        0        0    12139 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/offset_type.py
+-rw-r--r--   0        0        0    13002 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition.py
+-rw-r--r--   0        0        0    13571 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition_leader.py
+-rw-r--r--   0        0        0    16556 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record.py
+-rw-r--r--   0        0        0    13502 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_all_of.py
+-rw-r--r--   0        0        0    12409 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_included_property.py
+-rw-r--r--   0        0        0    14743 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list.py
+-rw-r--r--   0        0        0    12498 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list_all_of.py
+-rw-r--r--   0        0        0    11932 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/sort_direction.py
+-rw-r--r--   0        0        0    15627 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic.py
+-rw-r--r--   0        0        0    12544 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_all_of.py
+-rw-r--r--   0        0        0    12208 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_order_key.py
+-rw-r--r--   0        0        0    12387 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_settings.py
+-rw-r--r--   0        0        0    15667 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list.py
+-rw-r--r--   0        0        0    11668 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list_all_of.py
+-rw-r--r--   0        0        0    11728 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_to_reset_offset.py
+-rw-r--r--   0        0        0    82631 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model_utils.py
+-rw-r--r--   0        0        0     4561 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14331 2023-03-29 10:40:27.650118 rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/rest.py
+-rw-r--r--   0        0        0      821 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      224 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/__init__.py
+-rw-r--r--   0        0        0    74161 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/default_api.py
+-rw-r--r--   0        0        0    27032 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/enterprise_dataplane_clusters_api.py
+-rw-r--r--   0        0        0    10387 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/errors_api.py
+-rw-r--r--   0        0        0    30984 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/security_api.py
+-rw-r--r--   0        0        0    39120 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api_client.py
+-rw-r--r--   0        0        0      715 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    16928 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/configuration.py
+-rw-r--r--   0        0        0     5105 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/exceptions.py
+-rw-r--r--   0        0        0      354 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/__init__.py
+-rw-r--r--   0        0        0    12840 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider.py
+-rw-r--r--   0        0        0    14431 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list.py
+-rw-r--r--   0        0        0    11703 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list_all_of.py
+-rw-r--r--   0        0        0    13304 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region.py
+-rw-r--r--   0        0        0    14415 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list.py
+-rw-r--r--   0        0        0    11697 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list_all_of.py
+-rw-r--r--   0        0        0    17599 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster.py
+-rw-r--r--   0        0        0    12522 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of.py
+-rw-r--r--   0        0        0    13911 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of_capacity_information.py
+-rw-r--r--   0        0        0    14463 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list.py
+-rw-r--r--   0        0        0    11715 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_all_of.py
+-rw-r--r--   0        0        0    16450 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_item.py
+-rw-r--r--   0        0        0    14022 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_item_all_of.py
+-rw-r--r--   0        0        0    17031 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_with_addon_parameters.py
+-rw-r--r--   0        0        0    11792 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_with_addon_parameters_all_of.py
+-rw-r--r--   0        0        0    14587 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_osd_cluster_payload.py
+-rw-r--r--   0        0        0    12986 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error.py
+-rw-r--r--   0        0        0    14287 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list.py
+-rw-r--r--   0        0        0    11664 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list_all_of.py
+-rw-r--r--   0        0        0    11637 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameter.py
+-rw-r--r--   0        0        0    11923 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/instant_query.py
+-rw-r--r--   0        0        0    13499 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_promote_request.py
+-rw-r--r--   0        0        0    25271 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request.py
+-rw-r--r--   0        0        0    22920 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_all_of.py
+-rw-r--r--   0        0        0    14423 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list.py
+-rw-r--r--   0        0        0    11700 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list_all_of.py
+-rw-r--r--   0        0        0    14946 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_payload.py
+-rw-r--r--   0        0        0    12125 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_update_request.py
+-rw-r--r--   0        0        0    12042 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/list.py
+-rw-r--r--   0        0        0    14257 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list.py
+-rw-r--r--   0        0        0    12019 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list_all_of.py
+-rw-r--r--   0        0        0    14241 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list.py
+-rw-r--r--   0        0        0    12013 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list_all_of.py
+-rw-r--r--   0        0        0    11852 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/object_reference.py
+-rw-r--r--   0        0        0    11834 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/range_query.py
+-rw-r--r--   0        0        0    12233 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/region_capacity_list_item.py
+-rw-r--r--   0        0        0    15548 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account.py
+-rw-r--r--   0        0        0    12995 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_all_of.py
+-rw-r--r--   0        0        0    13948 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list.py
+-rw-r--r--   0        0        0    11896 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_all_of.py
+-rw-r--r--   0        0        0    15787 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item.py
+-rw-r--r--   0        0        0    13192 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item_all_of.py
+-rw-r--r--   0        0        0    11867 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_request.py
+-rw-r--r--   0        0        0    15032 2023-03-29 10:40:27.658118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider.py
+-rw-r--r--   0        0        0    12324 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider_all_of.py
+-rw-r--r--   0        0        0    13258 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_billing_model.py
+-rw-r--r--   0        0        0    13608 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type.py
+-rw-r--r--   0        0        0    20642 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type_sizes_inner.py
+-rw-r--r--   0        0        0    14021 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list.py
+-rw-r--r--   0        0        0    11742 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list_all_of.py
+-rw-r--r--   0        0        0    18452 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size.py
+-rw-r--r--   0        0        0    11508 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size_bytes_value_item.py
+-rw-r--r--   0        0        0    11687 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/values.py
+-rw-r--r--   0        0        0    14635 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata.py
+-rw-r--r--   0        0        0    11907 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata_all_of.py
+-rw-r--r--   0        0        0    82638 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model_utils.py
+-rw-r--r--   0        0        0     5048 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14338 2023-03-29 10:40:27.662118 rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/rest.py
+-rw-r--r--   0        0        0     2084 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/__init__.py
+-rw-r--r--   0        0        0      229 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/__init__.py
+-rw-r--r--   0        0        0   116696 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/admin_api.py
+-rw-r--r--   0        0        0    47524 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifact_rules_api.py
+-rw-r--r--   0        0        0    88699 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifacts_api.py
+-rw-r--r--   0        0        0    23764 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/groups_api.py
+-rw-r--r--   0        0        0    53083 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/metadata_api.py
+-rw-r--r--   0        0        0    17954 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/search_api.py
+-rw-r--r--   0        0        0    11617 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/system_api.py
+-rw-r--r--   0        0        0     6836 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/users_api.py
+-rw-r--r--   0        0        0    45777 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/versions_api.py
+-rw-r--r--   0        0        0    40377 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api_client.py
+-rw-r--r--   0        0        0     1046 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    17456 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/configuration.py
+-rw-r--r--   0        0        0     6312 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/exceptions.py
+-rw-r--r--   0        0        0      361 2023-03-29 10:40:27.666118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/__init__.py
+-rw-r--r--   0        0        0    16767 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_meta_data.py
+-rw-r--r--   0        0        0    12672 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_owner.py
+-rw-r--r--   0        0        0    13413 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_reference.py
+-rw-r--r--   0        0        0    13610 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_search_results.py
+-rw-r--r--   0        0        0    13816 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_state.py
+-rw-r--r--   0        0        0    12676 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_type_info.py
+-rw-r--r--   0        0        0    13598 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/configuration_property.py
+-rw-r--r--   0        0        0    13547 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/content_create_request.py
+-rw-r--r--   0        0        0    13326 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/create_group_meta_data.py
+-rw-r--r--   0        0        0    12957 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/download_ref.py
+-rw-r--r--   0        0        0    13493 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/editable_meta_data.py
+-rw-r--r--   0        0        0    13676 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/error.py
+-rw-r--r--   0        0        0    14548 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_meta_data.py
+-rw-r--r--   0        0        0    13529 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_search_results.py
+-rw-r--r--   0        0        0    13371 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/if_exists.py
+-rw-r--r--   0        0        0    15923 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/limits.py
+-rw-r--r--   0        0        0    12914 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_configuration.py
+-rw-r--r--   0        0        0    13773 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_level.py
+-rw-r--r--   0        0        0    15316 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration.py
+-rw-r--r--   0        0        0    12750 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration_all_of.py
+-rw-r--r--   0        0        0    12423 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/properties.py
+-rw-r--r--   0        0        0    13466 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_mapping.py
+-rw-r--r--   0        0        0    13281 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_type.py
+-rw-r--r--   0        0        0    13067 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule.py
+-rw-r--r--   0        0        0    13233 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_type.py
+-rw-r--r--   0        0        0    12910 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_cause.py
+-rw-r--r--   0        0        0    16461 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error.py
+-rw-r--r--   0        0        0    13085 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error_all_of.py
+-rw-r--r--   0        0        0    15207 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_artifact.py
+-rw-r--r--   0        0        0    14104 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_group.py
+-rw-r--r--   0        0        0    15782 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_version.py
+-rw-r--r--   0        0        0    13179 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_by.py
+-rw-r--r--   0        0        0    13152 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_order.py
+-rw-r--r--   0        0        0    13276 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/system_info.py
+-rw-r--r--   0        0        0    12762 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_configuration_property.py
+-rw-r--r--   0        0        0    12885 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_role.py
+-rw-r--r--   0        0        0    12934 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_state.py
+-rw-r--r--   0        0        0    13472 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/user_info.py
+-rw-r--r--   0        0        0    15795 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_meta_data.py
+-rw-r--r--   0        0        0    13587 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_search_results.py
+-rw-r--r--   0        0        0    83852 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model_utils.py
+-rw-r--r--   0        0        0     3494 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/models/__init__.py
+-rw-r--r--   0        0        0    15552 2023-03-29 10:40:27.670118 rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/rest.py
+-rw-r--r--   0        0        0     1078 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      234 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/__init__.py
+-rw-r--r--   0        0        0     5947 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/default_api.py
+-rw-r--r--   0        0        0    11488 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/errors_api.py
+-rw-r--r--   0        0        0    23774 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/registries_api.py
+-rw-r--r--   0        0        0    39320 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api_client.py
+-rw-r--r--   0        0        0      659 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    17118 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/configuration.py
+-rw-r--r--   0        0        0     5274 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/exceptions.py
+-rw-r--r--   0        0        0      365 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/__init__.py
+-rw-r--r--   0        0        0    12257 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/abstract_list.py
+-rw-r--r--   0        0        0    11829 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/empty.py
+-rw-r--r--   0        0        0    14633 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error.py
+-rw-r--r--   0        0        0    12100 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_all_of.py
+-rw-r--r--   0        0        0    14552 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list.py
+-rw-r--r--   0        0        0    11866 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list_all_of.py
+-rw-r--r--   0        0        0    14582 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list.py
+-rw-r--r--   0        0        0    11922 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list_all_of.py
+-rw-r--r--   0        0        0    12043 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/object_reference.py
+-rw-r--r--   0        0        0    17009 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry.py
+-rw-r--r--   0        0        0    12507 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_create.py
+-rw-r--r--   0        0        0    13176 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_instance_type_value.py
+-rw-r--r--   0        0        0    14597 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list.py
+-rw-r--r--   0        0        0    11896 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list_all_of.py
+-rw-r--r--   0        0        0    14374 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_status_value.py
+-rw-r--r--   0        0        0    14892 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/root_type_for_registry.py
+-rw-r--r--   0        0        0    12041 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/service_status.py
+-rw-r--r--   0        0        0    82818 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model_utils.py
+-rw-r--r--   0        0        0     1721 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14518 2023-03-29 10:40:27.674118 rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/rest.py
+-rw-r--r--   0        0        0      921 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/__init__.py
+-rw-r--r--   0        0        0    11813 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/acs_tenants_api.py
+-rw-r--r--   0        0        0    11471 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/default_api.py
+-rw-r--r--   0        0        0    34067 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/service_accounts_api.py
+-rw-r--r--   0        0        0    39199 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api_client.py
+-rw-r--r--   0        0        0      688 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    17479 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/configuration.py
+-rw-r--r--   0        0        0     5117 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/exceptions.py
+-rw-r--r--   0        0        0      365 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/__init__.py
+-rw-r--r--   0        0        0    12294 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_request_data.py
+-rw-r--r--   0        0        0    12101 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_response_data.py
+-rw-r--r--   0        0        0    11652 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_factors.py
+-rw-r--r--   0        0        0    11870 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_policy.py
+-rw-r--r--   0        0        0    11557 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/error.py
+-rw-r--r--   0        0        0    11473 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/otp.py
+-rw-r--r--   0        0        0    12719 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/red_hat_error_representation.py
+-rw-r--r--   0        0        0    11979 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_create_request_data.py
+-rw-r--r--   0        0        0    12824 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_data.py
+-rw-r--r--   0        0        0    11919 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_request_data.py
+-rw-r--r--   0        0        0    11976 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/validation_exception_data.py
+-rw-r--r--   0        0        0    82661 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model_utils.py
+-rw-r--r--   0        0        0     1411 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14361 2023-03-29 10:40:27.678118 rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/rest.py
+-rw-r--r--   0        0        0      906 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      231 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/__init__.py
+-rw-r--r--   0        0        0    22654 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/bridges_api.py
+-rw-r--r--   0        0        0    17973 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/cloud_providers_api.py
+-rw-r--r--   0        0        0    11522 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/error_catalog_api.py
+-rw-r--r--   0        0        0    30966 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/processors_api.py
+-rw-r--r--   0        0        0    31097 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/sink_connectors_api.py
+-rw-r--r--   0        0        0    31340 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/source_connectors_api.py
+-rw-r--r--   0        0        0    39229 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api_client.py
+-rw-r--r--   0        0        0      908 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    16974 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/configuration.py
+-rw-r--r--   0        0        0     5134 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/exceptions.py
+-rw-r--r--   0        0        0      361 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/__init__.py
+-rw-r--r--   0        0        0    12252 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error.py
+-rw-r--r--   0        0        0    12454 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_instance.py
+-rw-r--r--   0        0        0    12014 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_type.py
+-rw-r--r--   0        0        0    12543 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_list_response.py
+-rw-r--r--   0        0        0    12474 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_request.py
+-rw-r--r--   0        0        0    15062 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_response.py
+-rw-r--r--   0        0        0    12614 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_list_response.py
+-rw-r--r--   0        0        0    12897 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_response.py
+-rw-r--r--   0        0        0    12594 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_list_response.py
+-rw-r--r--   0        0        0    12243 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_response.py
+-rw-r--r--   0        0        0    12627 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/connector_request.py
+-rw-r--r--   0        0        0    12735 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error.py
+-rw-r--r--   0        0        0    12476 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error_list_response.py
+-rw-r--r--   0        0        0    11874 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/errors_list.py
+-rw-r--r--   0        0        0    14500 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list.py
+-rw-r--r--   0        0        0    11910 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_all_of.py
+-rw-r--r--   0        0        0    11915 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_response.py
+-rw-r--r--   0        0        0    12980 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/managed_resource_status.py
+-rw-r--r--   0        0        0    12375 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/object_reference.py
+-rw-r--r--   0        0        0    12634 2023-03-29 10:40:27.682118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_list_response.py
+-rw-r--r--   0        0        0    12183 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_response.py
+-rw-r--r--   0        0        0    12573 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_list_response.py
+-rw-r--r--   0        0        0    12220 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_request.py
+-rw-r--r--   0        0        0    14580 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_response.py
+-rw-r--r--   0        0        0    12614 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_list_response.py
+-rw-r--r--   0        0        0    15396 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_response.py
+-rw-r--r--   0        0        0    12634 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_list_response.py
+-rw-r--r--   0        0        0    15063 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_response.py
+-rw-r--r--   0        0        0    82674 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model_utils.py
+-rw-r--r--   0        0        0     2755 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/models/__init__.py
+-rw-r--r--   0        0        0    14374 2023-03-29 10:40:27.686118 rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/rest.py
+-rw-r--r--   0        0        0    13669 1970-01-01 00:00:00.000000 rhoas_sdks-1.0.2b2/PKG-INFO
```

### Comparing `rhoas_sdks-1.0.2/auth/rhoas_auth.py` & `rhoas_sdks-1.0.2b2/auth/rhoas_auth.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/docs/README.md` & `rhoas_sdks-1.0.2b2/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # RHOAS Core SDKs
 
 > If you are moving a project from the old RHOAS SDKs to core read this [moving](./MOVING.md) doc to get started.
 
 | Supported Langauge  | SDK |
 | ----------- | ----------- |
-| JavaScript  | [app-services-sdk-ts](/app-services-sdk-ts/) |
+| JavaScript/TypeScript  | [app-services-sdk-js](/app-services-sdk-js/) |
 | Python   | [app-services-sdk-python](/app-services-sdk-python/)    |
 | Java   | [app-services-sdk-java](/app-services-sdk-java/)        |
 |  Go   | [app-services-sdk-go](/app-services-sdk-go/)        |
 
 ## Structure
 
 RHOAS SDK's are delivered as set of individual packages.
@@ -18,17 +18,17 @@
 - **Instance SDKs** -  support direct interaction with services
 
 ## Purpose of this repository
 
 Repository contains source code for openapi based generator along with automation scripts that generate all
 underlying RHOAS SDKS. 
 
-# RHOAS SDK for Typescript
+# RHOAS SDK for Typescript and JavaScript
 
-Typescript packages and API clients for RHOAS services
+Typescript and JavaScript packages and API clients for RHOAS services
 
 ## Prequisites
 
 - [NodeJS 14.x lts](https://nodejs.org/en/about/releases/) or above
 
 ## Management SDK's
```

### Comparing `rhoas_sdks-1.0.2/pyproject.toml` & `rhoas_sdks-1.0.2b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhoas_sdks"
-version = "1.0.2"
+version = "1.0.2-beta2"
 description = "A package which includes RHOAS SDKs"
 authors = ["dimakis <dsaridak@redhat.com>"]
 license = "Apache License"
 readme = "docs/README.md"
 packages = [
     { include = "rhoas_connector_mgmt_sdk", from = "sdks/connector_mgmt_sdk/" },
     { include = "rhoas_kafka_instance_sdk", from = "sdks/kafka_instance_sdk/"},
```

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_clusters_api.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_clusters_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_namespaces_api.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_namespaces_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_service_api.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_service_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_types_api.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connector_types_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connectors_api.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api/connectors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/addon_parameter_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/channel.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/channel.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_request_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_state.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status_status.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_cluster_status_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_configuration.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_desired_state.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_desired_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_meta_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_eval_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_eval_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_meta_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_patch_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_patch_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_quota.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_quota.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_request_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_state.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_status.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant_kind.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_namespace_tenant_kind.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_request_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_resource_annotations.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_resource_annotations.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_state.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status_status.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_status_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_label_count_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/connector_type_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/cpu_quota.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/cpu_quota.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/kafka_connection_settings.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/kafka_connection_settings.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
-    Connector Management API
+    Kafka Management API
 
-    Connector Management API is a REST API to manage connectors.  # noqa: E501
+    Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_connector_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_kafka_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_connector_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
 
 class List(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/memory_quota.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/memory_quota.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_meta.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_meta.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_reference.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/object_reference.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/schema_registry_connection_settings.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/schema_registry_connection_settings.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_account.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_account.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_connection_settings.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/service_connection_settings.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'kind': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
-            'collections': ([ObjectReference],),  # noqa: E501
+            'collections': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -146,15 +146,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             kind (str): [optional]  # noqa: E501
             href (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,15 +253,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             kind (str): [optional]  # noqa: E501
             href (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/version_metadata_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,14 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_connector_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_connector_mgmt_sdk.model.object_reference import ObjectReference
-    globals()['ObjectReference'] = ObjectReference
-
 
 class VersionMetadataAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -67,32 +63,30 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'collections': ([ObjectReference],),  # noqa: E501
+            'collections': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -137,15 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -223,15 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/acls_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/acls_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/errors_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/errors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/groups_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/records_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/records_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/topics_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api/topics_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_list_page_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_order_key.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_binding_order_key.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation_filter.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_operation_filter.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type_filter.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_pattern_type_filter.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type_filter.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_permission_type_filter.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type_filter.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/acl_resource_type_filter.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/config_entry.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/config_entry.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_description_order_key.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_description_order_key.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_metrics.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_metrics.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_order_key.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_order_key.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_parameters.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_parameters.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_item.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_reset_offset_result_item.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_state.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/consumer_group_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/error_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/list_deprecated_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/new_topic_input.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/new_topic_input.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/node.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/node.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/object_reference.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/object_reference.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/offset_type.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/offset_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition_leader.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/partition_leader.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_included_property.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_included_property.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/record_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/sort_direction.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/sort_direction.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_order_key.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_order_key.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_settings.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topic_settings.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_to_reset_offset.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model/topics_to_reset_offset.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_instance_sdk/rhoas_kafka_instance_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/default_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/enterprise_dataplane_clusters_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/enterprise_dataplane_clusters_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -19,17 +19,16 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster import EnterpriseCluster
-from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_addon_parameters import EnterpriseClusterAddonParameters
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list import EnterpriseClusterList
-from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_registration_response import EnterpriseClusterRegistrationResponse
+from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_with_addon_parameters import EnterpriseClusterWithAddonParameters
 from rhoas_kafka_mgmt_sdk.model.enterprise_osd_cluster_payload import EnterpriseOsdClusterPayload
 from rhoas_kafka_mgmt_sdk.model.error import Error
 
 
 class EnterpriseDataplaneClustersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -94,22 +93,22 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_enterprise_cluster_addon_parameters_endpoint = _Endpoint(
+        self.get_enterprise_cluster_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': (EnterpriseClusterAddonParameters,),
+                'response_type': (EnterpriseCluster,),
                 'auth': [
                     'Bearer'
                 ],
-                'endpoint_path': '/api/kafkas_mgmt/v1/clusters/{id}/addon_parameters',
-                'operation_id': 'get_enterprise_cluster_addon_parameters',
+                'endpoint_path': '/api/kafkas_mgmt/v1/clusters/{id}',
+                'operation_id': 'get_enterprise_cluster_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
@@ -145,22 +144,22 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_enterprise_cluster_by_id_endpoint = _Endpoint(
+        self.get_enterprise_cluster_with_addon_parameters_endpoint = _Endpoint(
             settings={
-                'response_type': (EnterpriseCluster,),
+                'response_type': (EnterpriseClusterWithAddonParameters,),
                 'auth': [
                     'Bearer'
                 ],
-                'endpoint_path': '/api/kafkas_mgmt/v1/clusters/{id}',
-                'operation_id': 'get_enterprise_cluster_by_id',
+                'endpoint_path': '/api/kafkas_mgmt/v1/clusters/{id}/addon_parameters',
+                'operation_id': 'get_enterprise_cluster_with_addon_parameters',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
@@ -242,15 +241,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.register_enterprise_osd_cluster_endpoint = _Endpoint(
             settings={
-                'response_type': (EnterpriseClusterRegistrationResponse,),
+                'response_type': (EnterpriseClusterWithAddonParameters,),
                 'auth': [
                     'Bearer'
                 ],
                 'endpoint_path': '/api/kafkas_mgmt/v1/clusters',
                 'operation_id': 'register_enterprise_osd_cluster',
                 'http_method': 'POST',
                 'servers': None,
@@ -379,26 +378,26 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['_async'] = \
             _async
         kwargs['id'] = \
             id
         return self.delete_enterprise_cluster_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_enterprise_cluster_addon_parameters(
+    def get_enterprise_cluster_by_id(
         self,
         id,
         **kwargs
     ):
-        """get_enterprise_cluster_addon_parameters  # noqa: E501
+        """get_enterprise_cluster_by_id  # noqa: E501
 
-        Returns the addon parameters belonging to the enterprise dataplane cluster {id}  # noqa: E501
+        Returns enterprise data plane cluster by ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_enterprise_cluster_addon_parameters(id, async_req=True)
+        >>> thread = api.get_enterprise_cluster_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): ID of the enterprise data plane cluster
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -429,15 +428,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnterpriseClusterAddonParameters
+            EnterpriseCluster
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -460,28 +459,28 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_enterprise_cluster_addon_parameters_endpoint.call_with_http_info(**kwargs)
+        return self.get_enterprise_cluster_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_enterprise_cluster_by_id(
+    def get_enterprise_cluster_with_addon_parameters(
         self,
         id,
         **kwargs
     ):
-        """get_enterprise_cluster_by_id  # noqa: E501
+        """get_enterprise_cluster_with_addon_parameters  # noqa: E501
 
-        Returns enterprise data plane cluster by ID  # noqa: E501
+        Returns enterprise data plane cluster by ID along with its addon parameters  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_enterprise_cluster_by_id(id, async_req=True)
+        >>> thread = api.get_enterprise_cluster_with_addon_parameters(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): ID of the enterprise data plane cluster
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -512,15 +511,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnterpriseCluster
+            EnterpriseClusterWithAddonParameters
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -543,15 +542,15 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_enterprise_cluster_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.get_enterprise_cluster_with_addon_parameters_endpoint.call_with_http_info(**kwargs)
 
     def get_enterprise_osd_clusters(
         self,
         **kwargs
     ):
         """get_enterprise_osd_clusters  # noqa: E501
 
@@ -673,15 +672,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnterpriseClusterRegistrationResponse
+            EnterpriseClusterWithAddonParameters
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/errors_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/errors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/security_api.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api/security_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.16.0\n"\
+               "Version of the API: 1.15.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_provider_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/cloud_region_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -29,19 +29,19 @@
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of import EnterpriseClusterAllOf
     from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of_capacity_information import EnterpriseClusterAllOfCapacityInformation
-    from rhoas_kafka_mgmt_sdk.model.object_reference import ObjectReference
+    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_item import EnterpriseClusterListItem
     from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list import SupportedKafkaInstanceTypesList
     globals()['EnterpriseClusterAllOf'] = EnterpriseClusterAllOf
     globals()['EnterpriseClusterAllOfCapacityInformation'] = EnterpriseClusterAllOfCapacityInformation
-    globals()['ObjectReference'] = ObjectReference
+    globals()['EnterpriseClusterListItem'] = EnterpriseClusterListItem
     globals()['SupportedKafkaInstanceTypesList'] = SupportedKafkaInstanceTypesList
 
 
 class EnterpriseCluster(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -356,12 +356,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               EnterpriseClusterAllOf,
-              ObjectReference,
+              EnterpriseClusterListItem,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_addon_parameters.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,23 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_fleetshard_parameters import EnterpriseClusterFleetshardParameters
-    from rhoas_kafka_mgmt_sdk.model.fleetshard_parameters_array import FleetshardParametersArray
-    from rhoas_kafka_mgmt_sdk.model.object_reference import ObjectReference
-    globals()['EnterpriseClusterFleetshardParameters'] = EnterpriseClusterFleetshardParameters
-    globals()['FleetshardParametersArray'] = FleetshardParametersArray
-    globals()['ObjectReference'] = ObjectReference
+    from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list_all_of import SupportedKafkaInstanceTypesListAllOf
+    globals()['SupportedKafkaInstanceTypesListAllOf'] = SupportedKafkaInstanceTypesListAllOf
 
 
-class EnterpriseClusterAddonParameters(ModelComposed):
+class SupportedKafkaInstanceTypesList(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,44 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'kind': (str,),  # noqa: E501
-            'href': (str,),  # noqa: E501
-            'fleetshard_parameters': (FleetshardParametersArray,),  # noqa: E501
+            'instance_types': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'kind': 'kind',  # noqa: E501
-        'href': 'href',  # noqa: E501
-        'fleetshard_parameters': 'fleetshard_parameters',  # noqa: E501
+        'instance_types': 'instance_types',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterAddonParameters - a model defined in OpenAPI
+        """SupportedKafkaInstanceTypesList - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            kind (str):
-            href (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -148,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            instance_types ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,20 +206,17 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterAddonParameters - a model defined in OpenAPI
+        """SupportedKafkaInstanceTypesList - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            kind (str):
-            href (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -255,15 +239,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            instance_types ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -325,13 +309,12 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              EnterpriseClusterFleetshardParameters,
-              ObjectReference,
+              SupportedKafkaInstanceTypesListAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_item_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of_capacity_information import EnterpriseClusterAllOfCapacityInformation
-    from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list import SupportedKafkaInstanceTypesList
-    globals()['EnterpriseClusterAllOfCapacityInformation'] = EnterpriseClusterAllOfCapacityInformation
-    globals()['SupportedKafkaInstanceTypesList'] = SupportedKafkaInstanceTypesList
 
-
-class EnterpriseClusterAllOf(ModelNormal):
+class EnterpriseClusterListItemAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,66 +63,60 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'access_kafkas_via_private_network': (bool,),  # noqa: E501
             'multi_az': (bool,),  # noqa: E501
             'cluster_id': (str,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'cloud_provider': (str,),  # noqa: E501
             'region': (str,),  # noqa: E501
-            'supported_instance_types': (SupportedKafkaInstanceTypesList,),  # noqa: E501
-            'capacity_information': (EnterpriseClusterAllOfCapacityInformation,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'access_kafkas_via_private_network': 'access_kafkas_via_private_network',  # noqa: E501
         'multi_az': 'multi_az',  # noqa: E501
         'cluster_id': 'cluster_id',  # noqa: E501
         'status': 'status',  # noqa: E501
         'cloud_provider': 'cloud_provider',  # noqa: E501
         'region': 'region',  # noqa: E501
-        'supported_instance_types': 'supported_instance_types',  # noqa: E501
-        'capacity_information': 'capacity_information',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, access_kafkas_via_private_network, multi_az, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterAllOf - a model defined in OpenAPI
+        """EnterpriseClusterListItemAllOf - a model defined in OpenAPI
 
         Args:
             access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
             multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -161,16 +149,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
             status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
             cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
             region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
-            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
-            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -217,15 +203,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, access_kafkas_via_private_network, multi_az, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterAllOf - a model defined in OpenAPI
+        """EnterpriseClusterListItemAllOf - a model defined in OpenAPI
 
         Args:
             access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
             multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -258,16 +244,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
             status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
             cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
             region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
-            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
-            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of_capacity_information.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of_capacity_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_fleetshard_parameters.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_with_addon_parameters_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.fleetshard_parameters_array import FleetshardParametersArray
-    globals()['FleetshardParametersArray'] = FleetshardParametersArray
 
-
-class EnterpriseClusterFleetshardParameters(ModelNormal):
+class EnterpriseClusterWithAddonParametersAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,32 +63,30 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'fleetshard_parameters': (FleetshardParametersArray,),  # noqa: E501
+            'fleetshard_parameters': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,15 +98,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterFleetshardParameters - a model defined in OpenAPI
+        """EnterpriseClusterWithAddonParametersAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            fleetshard_parameters ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterFleetshardParameters - a model defined in OpenAPI
+        """EnterpriseClusterWithAddonParametersAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            fleetshard_parameters ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_registration_response.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_with_addon_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,27 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster import EnterpriseCluster
-    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of_capacity_information import EnterpriseClusterAllOfCapacityInformation
-    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_fleetshard_parameters import EnterpriseClusterFleetshardParameters
-    from rhoas_kafka_mgmt_sdk.model.fleetshard_parameters_array import FleetshardParametersArray
-    from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list import SupportedKafkaInstanceTypesList
-    globals()['EnterpriseCluster'] = EnterpriseCluster
-    globals()['EnterpriseClusterAllOfCapacityInformation'] = EnterpriseClusterAllOfCapacityInformation
-    globals()['EnterpriseClusterFleetshardParameters'] = EnterpriseClusterFleetshardParameters
-    globals()['FleetshardParametersArray'] = FleetshardParametersArray
-    globals()['SupportedKafkaInstanceTypesList'] = SupportedKafkaInstanceTypesList
+    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_item import EnterpriseClusterListItem
+    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_with_addon_parameters_all_of import EnterpriseClusterWithAddonParametersAllOf
+    globals()['EnterpriseClusterListItem'] = EnterpriseClusterListItem
+    globals()['EnterpriseClusterWithAddonParametersAllOf'] = EnterpriseClusterWithAddonParametersAllOf
 
 
-class EnterpriseClusterRegistrationResponse(ModelComposed):
+class EnterpriseClusterWithAddonParameters(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -101,17 +95,15 @@
             'href': (str,),  # noqa: E501
             'access_kafkas_via_private_network': (bool,),  # noqa: E501
             'multi_az': (bool,),  # noqa: E501
             'cluster_id': (str,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'cloud_provider': (str,),  # noqa: E501
             'region': (str,),  # noqa: E501
-            'supported_instance_types': (SupportedKafkaInstanceTypesList,),  # noqa: E501
-            'capacity_information': (EnterpriseClusterAllOfCapacityInformation,),  # noqa: E501
-            'fleetshard_parameters': (FleetshardParametersArray,),  # noqa: E501
+            'fleetshard_parameters': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -121,26 +113,24 @@
         'href': 'href',  # noqa: E501
         'access_kafkas_via_private_network': 'access_kafkas_via_private_network',  # noqa: E501
         'multi_az': 'multi_az',  # noqa: E501
         'cluster_id': 'cluster_id',  # noqa: E501
         'status': 'status',  # noqa: E501
         'cloud_provider': 'cloud_provider',  # noqa: E501
         'region': 'region',  # noqa: E501
-        'supported_instance_types': 'supported_instance_types',  # noqa: E501
-        'capacity_information': 'capacity_information',  # noqa: E501
         'fleetshard_parameters': 'fleetshard_parameters',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterRegistrationResponse - a model defined in OpenAPI
+        """EnterpriseClusterWithAddonParameters - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
             kind (str):
             href (str):
             access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
             multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
@@ -174,17 +164,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
             status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
             cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
             region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
-            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
-            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            fleetshard_parameters ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,15 +235,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EnterpriseClusterRegistrationResponse - a model defined in OpenAPI
+        """EnterpriseClusterWithAddonParameters - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
             kind (str):
             href (str):
             access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
             multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
@@ -289,17 +277,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
             status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
             cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
             region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
-            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
-            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
-            fleetshard_parameters (FleetshardParametersArray): [optional]  # noqa: E501
+            fleetshard_parameters ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -361,13 +347,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              EnterpriseCluster,
-              EnterpriseClusterFleetshardParameters,
+              EnterpriseClusterListItem,
+              EnterpriseClusterWithAddonParametersAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_osd_cluster_payload.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_osd_cluster_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/error_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameter.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/fleetshard_parameters_array.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_instance_type_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 """
-    Kafka Management API
+    Service Registry Management API
 
-    Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
+    Service Registry Management API is a REST API for managing Service Registry instances. Service Registry is a datastore for event schemas and API designs, which is based on the open source Apicurio Registry project.  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
-    Contact: rhosak-support@redhat.com
+    The version of the OpenAPI document: 1.0.0
+    Contact: rhosak-eval-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_kafka_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_service_registry_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_service_registry_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.fleetshard_parameter import FleetshardParameter
-    globals()['FleetshardParameter'] = FleetshardParameter
 
-
-class FleetshardParametersArray(ModelSimple):
+class RegistryInstanceTypeValue(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,14 +48,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('value',): {
+            'STANDARD': "standard",
+            'EVAL': "eval",
+        },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
@@ -71,17 +71,16 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'value': ([FleetshardParameter],),
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -98,23 +97,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """FleetshardParametersArray - a model defined in OpenAPI
+        """RegistryInstanceTypeValue - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] ([FleetshardParameter]): Enterprise Cluster fleetshard parameters array.  # noqa: E501
+            args[0] (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
 
         Keyword Args:
-            value ([FleetshardParameter]): Enterprise Cluster fleetshard parameters array.  # noqa: E501
+            value (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -192,23 +191,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """FleetshardParametersArray - a model defined in OpenAPI
+        """RegistryInstanceTypeValue - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] ([FleetshardParameter]): Enterprise Cluster fleetshard parameters array.  # noqa: E501
+            args[0] (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
 
         Keyword Args:
-            value ([FleetshardParameter]): Enterprise Cluster fleetshard parameters array.  # noqa: E501
+            value (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/instant_query.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/instant_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_promote_request.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_promote_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_payload.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_request_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_update_request.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/kafka_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/range_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rhoas_kafka_mgmt_sdk.model.values import Values
+    globals()['Values'] = Values
 
-class List(ModelNormal):
+
+class RangeQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,62 +67,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'kind': (str,),  # noqa: E501
-            'page': (int,),  # noqa: E501
-            'size': (int,),  # noqa: E501
-            'total': (int,),  # noqa: E501
+            'metric': ({str: (str,)},),  # noqa: E501
+            'values': ([Values],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'kind': 'kind',  # noqa: E501
-        'page': 'page',  # noqa: E501
-        'size': 'size',  # noqa: E501
-        'total': 'total',  # noqa: E501
+        'metric': 'metric',  # noqa: E501
+        'values': 'values',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """List - a model defined in OpenAPI
-
-        Args:
-            kind (str):
-            page (int):
-            size (int):
-            total (int):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """RangeQuery - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            metric ({str: (str,)}): [optional]  # noqa: E501
+            values ([Values]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,18 +172,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
-        self.page = page
-        self.size = size
-        self.total = total
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,22 +192,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """List - a model defined in OpenAPI
-
-        Args:
-            kind (str):
-            page (int):
-            size (int):
-            total (int):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """RangeQuery - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,14 +226,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            metric ({str: (str,)}): [optional]  # noqa: E501
+            values ([Values]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,18 +257,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
-        self.page = page
-        self.size = size
-        self.total = total
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_instant_query_list_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/metrics_range_query_list_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/object_reference.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/object_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/range_query.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/otp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 """
-    Kafka Management API
+    sso.redhat.com API documentation
 
-    Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
+    This is the API documentation for sso.redhat.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
-    Contact: rhosak-support@redhat.com
+    The version of the OpenAPI document: 5.0.19-SNAPSHOT
+    Contact: it-user-team-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_kafka_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_service_accounts_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_service_accounts_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.values import Values
-    globals()['Values'] = Values
 
-
-class RangeQuery(ModelNormal):
+class Otp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,54 +63,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'metric': ({str: (str,)},),  # noqa: E501
-            'values': ([Values],),  # noqa: E501
+            'required': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'metric': 'metric',  # noqa: E501
-        'values': 'values',  # noqa: E501
+        'required': 'required',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RangeQuery - a model defined in OpenAPI
+        """Otp - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metric ({str: (str,)}): [optional]  # noqa: E501
-            values ([Values]): [optional]  # noqa: E501
+            required (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RangeQuery - a model defined in OpenAPI
+        """Otp - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,16 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metric ({str: (str,)}): [optional]  # noqa: E501
-            values ([Values]): [optional]  # noqa: E501
+            required (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/region_capacity_list_item.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/region_capacity_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_list_item_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_request.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/service_account_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/sso_provider_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_billing_model.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_billing_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type_sizes_inner.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_type_sizes_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_all_of.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list_all_of import SupportedKafkaInstanceTypesListAllOf
-    globals()['SupportedKafkaInstanceTypesListAllOf'] = SupportedKafkaInstanceTypesListAllOf
+    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of_capacity_information import EnterpriseClusterAllOfCapacityInformation
+    from rhoas_kafka_mgmt_sdk.model.supported_kafka_instance_types_list import SupportedKafkaInstanceTypesList
+    globals()['EnterpriseClusterAllOfCapacityInformation'] = EnterpriseClusterAllOfCapacityInformation
+    globals()['SupportedKafkaInstanceTypesList'] = SupportedKafkaInstanceTypesList
 
 
-class SupportedKafkaInstanceTypesList(ModelComposed):
+class EnterpriseClusterAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,33 +86,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'instance_types': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'supported_instance_types': (SupportedKafkaInstanceTypesList,),  # noqa: E501
+            'capacity_information': (EnterpriseClusterAllOfCapacityInformation,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'instance_types': 'instance_types',  # noqa: E501
+        'supported_instance_types': 'supported_instance_types',  # noqa: E501
+        'capacity_information': 'capacity_information',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
+    _composed_schemas = {}
+
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SupportedKafkaInstanceTypesList - a model defined in OpenAPI
+        """EnterpriseClusterAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,19 +141,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            instance_types ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
+            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
+            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -167,54 +174,36 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
-
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
-        '_composed_instances',
-        '_var_name_to_model_instances',
-        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SupportedKafkaInstanceTypesList - a model defined in OpenAPI
+        """EnterpriseClusterAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,15 +228,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            instance_types ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
+            supported_instance_types (SupportedKafkaInstanceTypesList): [optional]  # noqa: E501
+            capacity_information (EnterpriseClusterAllOfCapacityInformation): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -269,52 +259,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
-
-    @cached_property
-    def _composed_schemas():
-        # we need this here to make our import statements work
-        # we must store _composed_schemas in here so the code is only run
-        # when we invoke this method. If we kept this at the class
-        # level we would get an error because the class level
-        # code would be run when this module is imported, and these composed
-        # classes don't exist yet because their module has not finished
-        # loading
-        lazy_import()
-        return {
-          'anyOf': [
-          ],
-          'allOf': [
-              SupportedKafkaInstanceTypesListAllOf,
-          ],
-          'oneOf': [
-          ],
-        }
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_instance_types_list_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size_bytes_value_item.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/supported_kafka_size_bytes_value_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/values.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -90,15 +90,15 @@
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'kind': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'server_version': (str,),  # noqa: E501
-            'collections': ([ObjectReference],),  # noqa: E501
+            'collections': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -149,15 +149,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             server_version (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,15 +257,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             server_version (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/version_metadata_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,18 +26,14 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_kafka_mgmt_sdk.model.object_reference import ObjectReference
-    globals()['ObjectReference'] = ObjectReference
-
 
 class VersionMetadataAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -67,33 +63,31 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'server_version': (str,),  # noqa: E501
-            'collections': ([ObjectReference],),  # noqa: E501
+            'collections': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -140,15 +134,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             server_version (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,15 +221,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             server_version (str): [optional]  # noqa: E501
-            collections ([ObjectReference]): [optional]  # noqa: E501
+            collections ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from rhoas_kafka_mgmt_sdk.model.cloud_provider import CloudProvider
 from rhoas_kafka_mgmt_sdk.model.cloud_provider_list import CloudProviderList
 from rhoas_kafka_mgmt_sdk.model.cloud_provider_list_all_of import CloudProviderListAllOf
 from rhoas_kafka_mgmt_sdk.model.cloud_region import CloudRegion
 from rhoas_kafka_mgmt_sdk.model.cloud_region_list import CloudRegionList
 from rhoas_kafka_mgmt_sdk.model.cloud_region_list_all_of import CloudRegionListAllOf
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster import EnterpriseCluster
-from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_addon_parameters import EnterpriseClusterAddonParameters
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of import EnterpriseClusterAllOf
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_all_of_capacity_information import EnterpriseClusterAllOfCapacityInformation
-from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_fleetshard_parameters import EnterpriseClusterFleetshardParameters
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list import EnterpriseClusterList
 from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_all_of import EnterpriseClusterListAllOf
-from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_registration_response import EnterpriseClusterRegistrationResponse
+from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_item import EnterpriseClusterListItem
+from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_item_all_of import EnterpriseClusterListItemAllOf
+from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_with_addon_parameters import EnterpriseClusterWithAddonParameters
+from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_with_addon_parameters_all_of import EnterpriseClusterWithAddonParametersAllOf
 from rhoas_kafka_mgmt_sdk.model.enterprise_osd_cluster_payload import EnterpriseOsdClusterPayload
 from rhoas_kafka_mgmt_sdk.model.error import Error
 from rhoas_kafka_mgmt_sdk.model.error_list import ErrorList
 from rhoas_kafka_mgmt_sdk.model.error_list_all_of import ErrorListAllOf
 from rhoas_kafka_mgmt_sdk.model.fleetshard_parameter import FleetshardParameter
-from rhoas_kafka_mgmt_sdk.model.fleetshard_parameters_array import FleetshardParametersArray
 from rhoas_kafka_mgmt_sdk.model.instant_query import InstantQuery
 from rhoas_kafka_mgmt_sdk.model.kafka_promote_request import KafkaPromoteRequest
 from rhoas_kafka_mgmt_sdk.model.kafka_request import KafkaRequest
 from rhoas_kafka_mgmt_sdk.model.kafka_request_all_of import KafkaRequestAllOf
 from rhoas_kafka_mgmt_sdk.model.kafka_request_list import KafkaRequestList
 from rhoas_kafka_mgmt_sdk.model.kafka_request_list_all_of import KafkaRequestListAllOf
 from rhoas_kafka_mgmt_sdk.model.kafka_request_payload import KafkaRequestPayload
```

### Comparing `rhoas_sdks-1.0.2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Kafka Management API
 
     Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 1.16.0
+    The version of the OpenAPI document: 1.15.0
     Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/admin_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifact_rules_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifact_rules_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifacts_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/artifacts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rhoas_registry_instance_sdk.model.artifact_content import ArtifactContent
 from rhoas_registry_instance_sdk.model.artifact_meta_data import ArtifactMetaData
 from rhoas_registry_instance_sdk.model.artifact_reference import ArtifactReference
 from rhoas_registry_instance_sdk.model.artifact_search_results import ArtifactSearchResults
+from rhoas_registry_instance_sdk.model.content_create_request import ContentCreateRequest
 from rhoas_registry_instance_sdk.model.error import Error
 from rhoas_registry_instance_sdk.model.if_exists import IfExists
 from rhoas_registry_instance_sdk.model.rule_violation_error import RuleViolationError
 from rhoas_registry_instance_sdk.model.sort_by import SortBy
 from rhoas_registry_instance_sdk.model.sort_order import SortOrder
 from rhoas_registry_instance_sdk.model.update_state import UpdateState
 
@@ -1383,15 +1383,15 @@
         self,
         group_id,
         artifact_id,
         **kwargs
     ):
         """Get latest artifact  # noqa: E501
 
-        Returns the latest version of the artifact in its raw form.  The `Content-Type` of the response depends on the artifact type.  In most cases, this is `application/json`, but  for some types it may be different (for example, `PROTOBUF`). If the latest version of the artifact is marked as `DISABLED`, the next available non-disabled version will be used.  This operation may fail for one of the following reasons:  * No artifact with this `artifactId` exists or all versions are `DISABLED` (HTTP error `404`) * A server error occurred (HTTP error `500`)   # noqa: E501
+        Returns the latest version of the artifact in its raw form.  The `Content-Type` of the response depends on the artifact type.  In most cases, this is `application/json`, but  for some types it may be different (for example, `PROTOBUF`).  This operation may fail for one of the following reasons:  * No artifact with this `artifactId` exists (HTTP error `404`) * A server error occurred (HTTP error `500`)   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_latest_artifact(group_id, artifact_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1905,15 +1905,15 @@
         group_id,
         artifact_id,
         update_state,
         **kwargs
     ):
         """Update artifact state  # noqa: E501
 
-        Updates the state of the artifact.  For example, you can use this to mark the latest version of an artifact as `DEPRECATED`. The operation changes the state of the latest version of the artifact, even if this version is `DISABLED`. If multiple versions exist, only the most recent is changed.  This operation can fail for the following reasons:  * No artifact with this `artifactId` exists (HTTP error `404`) * A server error occurred (HTTP error `500`)   # noqa: E501
+        Updates the state of the artifact.  For example, you can use this to mark the latest version of an artifact as `DEPRECATED`.  The operation changes the state of the latest  version of the artifact.  If multiple versions exist, only the most recent is changed.  This operation can fail for the following reasons:  * No artifact with this `artifactId` exists (HTTP error `404`) * A server error occurred (HTTP error `500`)   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_artifact_state(group_id, artifact_id, update_state, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/groups_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/metadata_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rhoas_registry_instance_sdk.model.artifact_content import ArtifactContent
 from rhoas_registry_instance_sdk.model.artifact_meta_data import ArtifactMetaData
 from rhoas_registry_instance_sdk.model.artifact_owner import ArtifactOwner
 from rhoas_registry_instance_sdk.model.editable_meta_data import EditableMetaData
 from rhoas_registry_instance_sdk.model.error import Error
 from rhoas_registry_instance_sdk.model.version_meta_data import VersionMetaData
 
 
@@ -330,18 +329,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/get.extended+json',
-                    'application/vnd.get.extended+json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
         self.update_artifact_meta_data_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [],
@@ -629,15 +625,15 @@
         self,
         group_id,
         artifact_id,
         **kwargs
     ):
         """Get artifact metadata  # noqa: E501
 
-        Gets the metadata for an artifact in the registry, based on the latest version. If the latest version of the artifact is marked as `DISABLED`, the next available non-disabled version will be used. The returned metadata includes both generated (read-only) and editable metadata (such as name and description).  This operation can fail for the following reasons:  * No artifact with this `artifactId` exists  or all versions are `DISABLED` (HTTP error `404`) * A server error occurred (HTTP error `500`)  # noqa: E501
+        Gets the metadata for an artifact in the registry.  The returned metadata includes both generated (read-only) and editable metadata (such as name and description).  This operation can fail for the following reasons:  * No artifact with this `artifactId` exists (HTTP error `404`) * A server error occurred (HTTP error `500`)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_artifact_meta_data(group_id, artifact_id, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/search_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/search_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/system_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/system_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/users_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/users_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/versions_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api/versions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rhoas_registry_instance_sdk.model.artifact_content import ArtifactContent
 from rhoas_registry_instance_sdk.model.artifact_reference import ArtifactReference
+from rhoas_registry_instance_sdk.model.content_create_request import ContentCreateRequest
 from rhoas_registry_instance_sdk.model.error import Error
 from rhoas_registry_instance_sdk.model.rule_violation_error import RuleViolationError
 from rhoas_registry_instance_sdk.model.update_state import UpdateState
 from rhoas_registry_instance_sdk.model.version_meta_data import VersionMetaData
 from rhoas_registry_instance_sdk.model.version_search_results import VersionSearchResults
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_content.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/content_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def lazy_import():
     from rhoas_registry_instance_sdk.model.artifact_reference import ArtifactReference
     globals()['ArtifactReference'] = ArtifactReference
 
 
-class ArtifactContent(ModelNormal):
+class ContentCreateRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -106,15 +106,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, content, references, *args, **kwargs):  # noqa: E501
-        """ArtifactContent - a model defined in OpenAPI
+        """ContentCreateRequest - a model defined in OpenAPI
 
         Args:
             content (str): Raw content of the artifact or a valid (and accessible) URL where the content can be found.
             references ([ArtifactReference]): Collection of references to other artifacts.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -197,15 +197,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, content, references, *args, **kwargs):  # noqa: E501
-        """ArtifactContent - a model defined in OpenAPI
+        """ContentCreateRequest - a model defined in OpenAPI
 
         Args:
             content (str): Raw content of the artifact or a valid (and accessible) URL where the content can be found.
             references ([ArtifactReference]): Collection of references to other artifacts.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_meta_data.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_meta_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_owner.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_owner.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_reference.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_reference.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_search_results.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_search_results.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_state.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_type_info.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/artifact_type_info.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/configuration_property.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/configuration_property.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/create_group_meta_data.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/create_group_meta_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/download_ref.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/download_ref.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/editable_meta_data.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/editable_meta_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_meta_data.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_meta_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_search_results.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/group_search_results.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/if_exists.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/if_exists.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/limits.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/limits.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_configuration.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_level.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/log_level.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/named_log_configuration_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/properties.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/properties.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_mapping.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_mapping.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_type.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/role_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_type.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_type.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_cause.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_cause.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/rule_violation_error_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_artifact.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_artifact.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_group.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_group.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_version.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/searched_version.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_by.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_by.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_order.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/system_info.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/system_info.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_configuration_property.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_configuration_property.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_role.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_role.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_state.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/update_state.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/user_info.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/user_info.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_meta_data.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_meta_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_search_results.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model/version_search_results.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from rhoas_registry_instance_sdk.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from rhoas_registry_instance_sdk.model.artifact_content import ArtifactContent
 from rhoas_registry_instance_sdk.model.artifact_meta_data import ArtifactMetaData
 from rhoas_registry_instance_sdk.model.artifact_owner import ArtifactOwner
 from rhoas_registry_instance_sdk.model.artifact_reference import ArtifactReference
 from rhoas_registry_instance_sdk.model.artifact_search_results import ArtifactSearchResults
 from rhoas_registry_instance_sdk.model.artifact_state import ArtifactState
 from rhoas_registry_instance_sdk.model.artifact_type_info import ArtifactTypeInfo
 from rhoas_registry_instance_sdk.model.configuration_property import ConfigurationProperty
+from rhoas_registry_instance_sdk.model.content_create_request import ContentCreateRequest
 from rhoas_registry_instance_sdk.model.create_group_meta_data import CreateGroupMetaData
 from rhoas_registry_instance_sdk.model.download_ref import DownloadRef
 from rhoas_registry_instance_sdk.model.editable_meta_data import EditableMetaData
 from rhoas_registry_instance_sdk.model.error import Error
 from rhoas_registry_instance_sdk.model.group_meta_data import GroupMetaData
 from rhoas_registry_instance_sdk.model.group_search_results import GroupSearchResults
 from rhoas_registry_instance_sdk.model.if_exists import IfExists
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/registry_instance_sdk/rhoas_registry_instance_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/default_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/default_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/errors_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/errors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/registries_api.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api/registries_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/abstract_list.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/abstract_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/empty.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/empty.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/error_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/object_reference.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/object_reference.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_create.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_create.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_instance_type_value.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
-    Service Registry Management API
+    Red Hat Openshift SmartEvents Fleet Manager V2
 
-    Service Registry Management API is a REST API for managing Service Registry instances. Service Registry is a datastore for event schemas and API designs, which is based on the open source Apicurio Registry project.  # noqa: E501
+    The API exposed by the fleet manager of the SmartEvents service.  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: rhosak-eval-support@redhat.com
+    The version of the OpenAPI document: 0.0.1
+    Contact: openbridge-dev@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_service_registry_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_smart_events_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_service_registry_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 
-class RegistryInstanceTypeValue(ModelSimple):
+class BridgeErrorType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,16 +49,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'STANDARD': "standard",
-            'EVAL': "eval",
+            'USER': "USER",
+            'PLATFORM': "PLATFORM",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -97,23 +97,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """RegistryInstanceTypeValue - a model defined in OpenAPI
+        """BridgeErrorType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
+            args[0] (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
+            value (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,23 +191,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """RegistryInstanceTypeValue - a model defined in OpenAPI
+        """BridgeErrorType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
+            args[0] (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Type of the Registry instance. This will determine functional and/or non-functional features provided by the instance.  \"standard\": Standard, full-featured Registry instance  \"eval\": Evaluation (Trial) instance, provided for a limited time ., must be one of ["standard", "eval", ]  # noqa: E501
+            value (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_status_value.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/registry_status_value.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/root_type_for_registry.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/root_type_for_registry.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/service_status.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model/service_status.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/registry_mgmt_sdk/rhoas_service_registry_mgmt_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/acs_tenants_api.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/acs_tenants_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/default_api.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/default_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/service_accounts_api.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api/service_accounts_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_request_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_request_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_response_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/acs_client_response_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_factors.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_factors.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_policy.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/authentication_policy.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/otp.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/errors_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
-    sso.redhat.com API documentation
+    Red Hat Openshift SmartEvents Fleet Manager V2
 
-    This is the API documentation for sso.redhat.com  # noqa: E501
+    The API exposed by the fleet manager of the SmartEvents service.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.19-SNAPSHOT
-    Contact: it-user-team-list@redhat.com
+    The version of the OpenAPI document: 0.0.1
+    Contact: openbridge-dev@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_service_accounts_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_smart_events_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_service_accounts_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rhoas_smart_events_mgmt_sdk.model.error import Error
+    globals()['Error'] = Error
 
-class Otp(ModelNormal):
+
+class ErrorsList(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'required': (bool,),  # noqa: E501
+            'kind': (str,),  # noqa: E501
+            'items': ([Error],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'required': 'required',  # noqa: E501
+        'kind': 'kind',  # noqa: E501
+        'items': 'items',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Otp - a model defined in OpenAPI
+    def _from_openapi_data(cls, kind, *args, **kwargs):  # noqa: E501
+        """ErrorsList - a model defined in OpenAPI
+
+        Args:
+            kind (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +142,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            required (bool): [optional]  # noqa: E501
+            items ([Error]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +174,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.kind = kind
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +195,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Otp - a model defined in OpenAPI
+    def __init__(self, kind, *args, **kwargs):  # noqa: E501
+        """ErrorsList - a model defined in OpenAPI
+
+        Args:
+            kind (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            required (bool): [optional]  # noqa: E501
+            items ([Error]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +262,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.kind = kind
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/red_hat_error_representation.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/red_hat_error_representation.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_create_request_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_create_request_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_request_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/service_account_request_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/validation_exception_data.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model/validation_exception_data.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/service_accounts_mgmt_sdk/rhoas_service_accounts_mgmt_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/bridges_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/bridges_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/cloud_providers_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/cloud_providers_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/error_catalog_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/error_catalog_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/processors_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/processors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/sink_connectors_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/sink_connectors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/source_connectors_api.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api/source_connectors_api.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api_client.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/apis/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/configuration.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/exceptions.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_instance.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_instance.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_error_type.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/managed_resource_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 
-class BridgeErrorType(ModelSimple):
+class ManagedResourceStatus(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,16 +49,25 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'USER': "USER",
-            'PLATFORM': "PLATFORM",
+            'ACCEPTED': "accepted",
+            'PREPARING': "preparing",
+            'PROVISIONING': "provisioning",
+            'READY': "ready",
+            'UPDATE_ACCEPTED': "update_accepted",
+            'UPDATE_PREPARING': "update_preparing",
+            'UPDATE_PROVISIONING': "update_provisioning",
+            'DEPROVISION': "deprovision",
+            'DELETING': "deleting",
+            'DELETED': "deleted",
+            'FAILED': "failed",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -97,23 +106,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """BridgeErrorType - a model defined in OpenAPI
+        """ManagedResourceStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
+            args[0] (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
+            value (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,23 +200,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """BridgeErrorType - a model defined in OpenAPI
+        """ManagedResourceStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
+            args[0] (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["USER", "PLATFORM", ]  # noqa: E501
+            value (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_list_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_request.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/bridge_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_list_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_provider_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_list_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/cloud_region_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/connector_request.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/connector_request.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/error_list_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/errors_list.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_smart_events_mgmt_sdk.model.error import Error
-    globals()['Error'] = Error
 
-
-class ErrorsList(ModelNormal):
+class ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,33 +63,31 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'kind': (str,),  # noqa: E501
-            'items': ([Error],),  # noqa: E501
+            'items': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -106,15 +100,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, kind, *args, **kwargs):  # noqa: E501
-        """ErrorsList - a model defined in OpenAPI
+        """ListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -142,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([Error]): [optional]  # noqa: E501
+            items ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,15 +190,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, kind, *args, **kwargs):  # noqa: E501
-        """ErrorsList - a model defined in OpenAPI
+        """ListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -232,15 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([Error]): [optional]  # noqa: E501
+            items ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_all_of.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_all_of.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 
-class ListResponse(ModelNormal):
+class ProcessorRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,14 +55,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -78,40 +81,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'kind': (str,),  # noqa: E501
-            'items': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'flows': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'kind': 'kind',  # noqa: E501
-        'items': 'items',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'flows': 'flows',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, kind, *args, **kwargs):  # noqa: E501
-        """ListResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, flows, *args, **kwargs):  # noqa: E501
+        """ProcessorRequest - a model defined in OpenAPI
 
         Args:
-            kind (str):
+            name (str): The name of the processor
+            flows ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Camel YAML DSL code, formatted as JSON, that defines the flows in the processor
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +171,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
+        self.name = name
+        self.flows = flows
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +193,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, kind, *args, **kwargs):  # noqa: E501
-        """ListResponse - a model defined in OpenAPI
+    def __init__(self, name, flows, *args, **kwargs):  # noqa: E501
+        """ProcessorRequest - a model defined in OpenAPI
 
         Args:
-            kind (str):
+            name (str): The name of the processor
+            flows ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Camel YAML DSL code, formatted as JSON, that defines the flows in the processor
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +231,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +260,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
+        self.name = name
+        self.flows = flows
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/managed_resource_status.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,102 +27,92 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 
-class ManagedResourceStatus(ModelSimple):
+class ProcessingErrorResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'ACCEPTED': "accepted",
-            'PREPARING': "preparing",
-            'PROVISIONING': "provisioning",
-            'READY': "ready",
-            'UPDATE_ACCEPTED': "update_accepted",
-            'UPDATE_PREPARING': "update_preparing",
-            'UPDATE_PROVISIONING': "update_provisioning",
-            'DEPROVISION': "deprovision",
-            'DELETING': "deleting",
-            'DELETED': "deleted",
-            'FAILED': "failed",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'recorded_at': (datetime,),  # noqa: E501
+            'headers': ({str: (str,)},),  # noqa: E501
+            'payload': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'recorded_at': 'recorded_at',  # noqa: E501
+        'headers': 'headers',  # noqa: E501
+        'payload': 'payload',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """ManagedResourceStatus - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
-
-        Args:
-            args[0] (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ProcessingErrorResponse - a model defined in OpenAPI
 
         Keyword Args:
-            value (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,35 +135,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            recorded_at (datetime): [optional]  # noqa: E501
+            headers ({str: (str,)}): [optional]  # noqa: E501
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -186,37 +168,39 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """ManagedResourceStatus - a model defined in OpenAPI
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Args:
-            args[0] (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ProcessingErrorResponse - a model defined in OpenAPI
 
         Keyword Args:
-            value (str):, must be one of ["accepted", "preparing", "provisioning", "ready", "update_accepted", "update_preparing", "update_provisioning", "deprovision", "deleting", "deleted", "failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -239,34 +223,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            recorded_at (datetime): [optional]  # noqa: E501
+            headers ({str: (str,)}): [optional]  # noqa: E501
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -282,19 +254,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/object_reference.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/object_reference.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_list_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processing_error_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rhoas_smart_events_mgmt_sdk.model.processor_response import ProcessorResponse
+    globals()['ProcessorResponse'] = ProcessorResponse
 
-class ProcessingErrorResponse(ModelNormal):
+
+class ProcessorListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,54 +67,66 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'recorded_at': (datetime,),  # noqa: E501
-            'headers': ({str: (str,)},),  # noqa: E501
-            'payload': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'kind': (str,),  # noqa: E501
+            'page': (int,),  # noqa: E501
+            'size': (int,),  # noqa: E501
+            'total': (int,),  # noqa: E501
+            'items': ([ProcessorResponse],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'recorded_at': 'recorded_at',  # noqa: E501
-        'headers': 'headers',  # noqa: E501
-        'payload': 'payload',  # noqa: E501
+        'kind': 'kind',  # noqa: E501
+        'page': 'page',  # noqa: E501
+        'size': 'size',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'items': 'items',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProcessingErrorResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, kind, page, size, total, *args, **kwargs):  # noqa: E501
+        """ProcessorListResponse - a model defined in OpenAPI
+
+        Args:
+            kind (str):
+            page (int):
+            size (int):
+            total (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +151,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            recorded_at (datetime): [optional]  # noqa: E501
-            headers ({str: (str,)}): [optional]  # noqa: E501
-            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            items ([ProcessorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,14 +183,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.kind = kind
+        self.page = page
+        self.size = size
+        self.total = total
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,16 +207,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProcessingErrorResponse - a model defined in OpenAPI
+    def __init__(self, kind, page, size, total, *args, **kwargs):  # noqa: E501
+        """ProcessorListResponse - a model defined in OpenAPI
+
+        Args:
+            kind (str):
+            page (int):
+            size (int):
+            total (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +247,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            recorded_at (datetime): [optional]  # noqa: E501
-            headers ({str: (str,)}): [optional]  # noqa: E501
-            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            items ([ProcessorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,14 +277,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.kind = kind
+        self.page = page
+        self.size = size
+        self.total = total
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_list_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rhoas_smart_events_mgmt_sdk.model.processor_response import ProcessorResponse
-    globals()['ProcessorResponse'] = ProcessorResponse
+    from rhoas_smart_events_mgmt_sdk.model.sink_connector_response import SinkConnectorResponse
+    globals()['SinkConnectorResponse'] = SinkConnectorResponse
 
 
-class ProcessorListResponse(ModelNormal):
+class SinkConnectorListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,15 +88,15 @@
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'page': (int,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'total': (int,),  # noqa: E501
-            'items': ([ProcessorResponse],),  # noqa: E501
+            'items': ([SinkConnectorResponse],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -112,15 +112,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """ProcessorListResponse - a model defined in OpenAPI
+        """SinkConnectorListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
             page (int):
             size (int):
             total (int):
 
@@ -151,15 +151,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([ProcessorResponse]): [optional]  # noqa: E501
+            items ([SinkConnectorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """ProcessorListResponse - a model defined in OpenAPI
+        """SinkConnectorListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
             page (int):
             size (int):
             total (int):
 
@@ -247,15 +247,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([ProcessorResponse]): [optional]  # noqa: E501
+            items ([SinkConnectorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_request.py` & `rhoas_sdks-1.0.2b2/sdks/connector_mgmt_sdk/rhoas_connector_mgmt_sdk/model/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
-    Red Hat Openshift SmartEvents Fleet Manager V2
+    Connector Management API
 
-    The API exposed by the fleet manager of the SmartEvents service.  # noqa: E501
+    Connector Management API is a REST API to manage connectors.  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.1
-    Contact: openbridge-dev@redhat.com
+    The version of the OpenAPI document: 0.1.0
+    Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_smart_events_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_connector_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_connector_mgmt_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rhoas_connector_mgmt_sdk.model.object_reference import ObjectReference
+    globals()['ObjectReference'] = ObjectReference
 
-class ProcessorRequest(ModelNormal):
+
+class List(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,67 +59,75 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'flows': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'kind': (str,),  # noqa: E501
+            'page': (int,),  # noqa: E501
+            'size': (int,),  # noqa: E501
+            'total': (int,),  # noqa: E501
+            'items': ([ObjectReference],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'flows': 'flows',  # noqa: E501
+        'kind': 'kind',  # noqa: E501
+        'page': 'page',  # noqa: E501
+        'size': 'size',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'items': 'items',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, flows, *args, **kwargs):  # noqa: E501
-        """ProcessorRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, kind, page, size, total, items, *args, **kwargs):  # noqa: E501
+        """List - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the processor
-            flows ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Camel YAML DSL code, formatted as JSON, that defines the flows in the processor
+            kind (str):
+            page (int):
+            size (int):
+            total (int):
+            items ([ObjectReference]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,16 +183,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.flows = flows
+        self.kind = kind
+        self.page = page
+        self.size = size
+        self.total = total
+        self.items = items
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,20 +208,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, flows, *args, **kwargs):  # noqa: E501
-        """ProcessorRequest - a model defined in OpenAPI
+    def __init__(self, kind, page, size, total, items, *args, **kwargs):  # noqa: E501
+        """List - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the processor
-            flows ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Camel YAML DSL code, formatted as JSON, that defines the flows in the processor
+            kind (str):
+            page (int):
+            size (int):
+            total (int):
+            items ([ObjectReference]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -260,16 +278,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.flows = flows
+        self.kind = kind
+        self.page = page
+        self.size = size
+        self.total = total
+        self.items = items
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/processor_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_list_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rhoas_smart_events_mgmt_sdk.model.sink_connector_response import SinkConnectorResponse
-    globals()['SinkConnectorResponse'] = SinkConnectorResponse
+    from rhoas_smart_events_mgmt_sdk.model.source_connector_response import SourceConnectorResponse
+    globals()['SourceConnectorResponse'] = SourceConnectorResponse
 
 
-class SinkConnectorListResponse(ModelNormal):
+class SourceConnectorListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,15 +88,15 @@
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'page': (int,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'total': (int,),  # noqa: E501
-            'items': ([SinkConnectorResponse],),  # noqa: E501
+            'items': ([SourceConnectorResponse],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -112,15 +112,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """SinkConnectorListResponse - a model defined in OpenAPI
+        """SourceConnectorListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
             page (int):
             size (int):
             total (int):
 
@@ -151,15 +151,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([SinkConnectorResponse]): [optional]  # noqa: E501
+            items ([SourceConnectorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """SinkConnectorListResponse - a model defined in OpenAPI
+        """SourceConnectorListResponse - a model defined in OpenAPI
 
         Args:
             kind (str):
             page (int):
             size (int):
             total (int):
 
@@ -247,15 +247,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([SinkConnectorResponse]): [optional]  # noqa: E501
+            items ([SourceConnectorResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/sink_connector_response.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_list_response.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rhoas_smart_events_mgmt_sdk.model.source_connector_response import SourceConnectorResponse
-    globals()['SourceConnectorResponse'] = SourceConnectorResponse
 
-
-class SourceConnectorListResponse(ModelNormal):
+class SourceConnectorResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,66 +63,83 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'kind': (str,),  # noqa: E501
-            'page': (int,),  # noqa: E501
-            'size': (int,),  # noqa: E501
-            'total': (int,),  # noqa: E501
-            'items': ([SourceConnectorResponse],),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'href': (str,),  # noqa: E501
+            'submitted_at': (datetime,),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'owner': (str,),  # noqa: E501
+            'connector_type_id': (str,),  # noqa: E501
+            'connector': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'published_at': (datetime,),  # noqa: E501
+            'modified_at': (datetime,),  # noqa: E501
+            'status_message': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
-        'page': 'page',  # noqa: E501
-        'size': 'size',  # noqa: E501
-        'total': 'total',  # noqa: E501
-        'items': 'items',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'href': 'href',  # noqa: E501
+        'submitted_at': 'submitted_at',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
+        'connector_type_id': 'connector_type_id',  # noqa: E501
+        'connector': 'connector',  # noqa: E501
+        'published_at': 'published_at',  # noqa: E501
+        'modified_at': 'modified_at',  # noqa: E501
+        'status_message': 'status_message',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """SourceConnectorListResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, kind, id, name, href, submitted_at, status, owner, connector_type_id, connector, *args, **kwargs):  # noqa: E501
+        """SourceConnectorResponse - a model defined in OpenAPI
 
         Args:
-            kind (str):
-            page (int):
-            size (int):
-            total (int):
+            kind (str): The kind (type) of this resource
+            id (str): The unique identifier of this resource
+            name (str): The name of this resource
+            href (str): The URL of this resource, without the protocol
+            submitted_at (datetime):
+            status (bool, date, datetime, dict, float, int, list, str, none_type):
+            owner (str): The user that owns this resource
+            connector_type_id (str): The connector type
+            connector ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Connector configuration payload
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,15 +164,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([SourceConnectorResponse]): [optional]  # noqa: E501
+            published_at (datetime): [optional]  # noqa: E501
+            modified_at (datetime): [optional]  # noqa: E501
+            status_message (str): A detailed status message in case there is a problem with the connector. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,17 +199,22 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.kind = kind
-        self.page = page
-        self.size = size
-        self.total = total
+        self.id = id
+        self.name = name
+        self.href = href
+        self.submitted_at = submitted_at
+        self.status = status
+        self.owner = owner
+        self.connector_type_id = connector_type_id
+        self.connector = connector
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -207,22 +227,27 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, kind, page, size, total, *args, **kwargs):  # noqa: E501
-        """SourceConnectorListResponse - a model defined in OpenAPI
+    def __init__(self, kind, id, name, href, submitted_at, status, owner, connector_type_id, connector, *args, **kwargs):  # noqa: E501
+        """SourceConnectorResponse - a model defined in OpenAPI
 
         Args:
-            kind (str):
-            page (int):
-            size (int):
-            total (int):
+            kind (str): The kind (type) of this resource
+            id (str): The unique identifier of this resource
+            name (str): The name of this resource
+            href (str): The URL of this resource, without the protocol
+            submitted_at (datetime):
+            status (bool, date, datetime, dict, float, int, list, str, none_type):
+            owner (str): The user that owns this resource
+            connector_type_id (str): The connector type
+            connector ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Connector configuration payload
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -247,15 +272,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            items ([SourceConnectorResponse]): [optional]  # noqa: E501
+            published_at (datetime): [optional]  # noqa: E501
+            modified_at (datetime): [optional]  # noqa: E501
+            status_message (str): A detailed status message in case there is a problem with the connector. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -278,17 +305,22 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.kind = kind
-        self.page = page
-        self.size = size
-        self.total = total
+        self.id = id
+        self.name = name
+        self.href = href
+        self.submitted_at = submitted_at
+        self.status = status
+        self.owner = owner
+        self.connector_type_id = connector_type_id
+        self.connector = connector
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model/source_connector_response.py` & `rhoas_sdks-1.0.2b2/sdks/kafka_mgmt_sdk/rhoas_kafka_mgmt_sdk/model/enterprise_cluster_list_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 """
-    Red Hat Openshift SmartEvents Fleet Manager V2
+    Kafka Management API
 
-    The API exposed by the fleet manager of the SmartEvents service.  # noqa: E501
+    Kafka Management API is a REST API to manage Kafka instances  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.1
-    Contact: openbridge-dev@redhat.com
+    The version of the OpenAPI document: 1.15.0
+    Contact: rhosak-support@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rhoas_smart_events_mgmt_sdk.model_utils import (  # noqa: F401
+from rhoas_kafka_mgmt_sdk.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rhoas_smart_events_mgmt_sdk.exceptions import ApiAttributeError
+from rhoas_kafka_mgmt_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rhoas_kafka_mgmt_sdk.model.enterprise_cluster_list_item_all_of import EnterpriseClusterListItemAllOf
+    from rhoas_kafka_mgmt_sdk.model.object_reference import ObjectReference
+    globals()['EnterpriseClusterListItemAllOf'] = EnterpriseClusterListItemAllOf
+    globals()['ObjectReference'] = ObjectReference
 
-class SourceConnectorResponse(ModelNormal):
+
+class EnterpriseClusterListItem(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,85 +69,73 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'kind': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
-            'submitted_at': (datetime,),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'owner': (str,),  # noqa: E501
-            'connector_type_id': (str,),  # noqa: E501
-            'connector': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'published_at': (datetime,),  # noqa: E501
-            'modified_at': (datetime,),  # noqa: E501
-            'status_message': (str,),  # noqa: E501
+            'access_kafkas_via_private_network': (bool,),  # noqa: E501
+            'multi_az': (bool,),  # noqa: E501
+            'cluster_id': (str,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'cloud_provider': (str,),  # noqa: E501
+            'region': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'kind': 'kind',  # noqa: E501
         'href': 'href',  # noqa: E501
-        'submitted_at': 'submitted_at',  # noqa: E501
+        'access_kafkas_via_private_network': 'access_kafkas_via_private_network',  # noqa: E501
+        'multi_az': 'multi_az',  # noqa: E501
+        'cluster_id': 'cluster_id',  # noqa: E501
         'status': 'status',  # noqa: E501
-        'owner': 'owner',  # noqa: E501
-        'connector_type_id': 'connector_type_id',  # noqa: E501
-        'connector': 'connector',  # noqa: E501
-        'published_at': 'published_at',  # noqa: E501
-        'modified_at': 'modified_at',  # noqa: E501
-        'status_message': 'status_message',  # noqa: E501
+        'cloud_provider': 'cloud_provider',  # noqa: E501
+        'region': 'region',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, kind, id, name, href, submitted_at, status, owner, connector_type_id, connector, *args, **kwargs):  # noqa: E501
-        """SourceConnectorResponse - a model defined in OpenAPI
-
-        Args:
-            kind (str): The kind (type) of this resource
-            id (str): The unique identifier of this resource
-            name (str): The name of this resource
-            href (str): The URL of this resource, without the protocol
-            submitted_at (datetime):
-            status (bool, date, datetime, dict, float, int, list, str, none_type):
-            owner (str): The user that owns this resource
-            connector_type_id (str): The connector type
-            connector ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Connector configuration payload
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """EnterpriseClusterListItem - a model defined in OpenAPI
 
         Keyword Args:
+            id (str):
+            kind (str):
+            href (str):
+            access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
+            multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -164,21 +158,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            published_at (datetime): [optional]  # noqa: E501
-            modified_at (datetime): [optional]  # noqa: E501
-            status_message (str): A detailed status message in case there is a problem with the connector. [optional]  # noqa: E501
+            cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
+            status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
+            cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
+            region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -198,58 +193,61 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
-        self.id = id
-        self.name = name
-        self.href = href
-        self.submitted_at = submitted_at
-        self.status = status
-        self.owner = owner
-        self.connector_type_id = connector_type_id
-        self.connector = connector
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, kind, id, name, href, submitted_at, status, owner, connector_type_id, connector, *args, **kwargs):  # noqa: E501
-        """SourceConnectorResponse - a model defined in OpenAPI
-
-        Args:
-            kind (str): The kind (type) of this resource
-            id (str): The unique identifier of this resource
-            name (str): The name of this resource
-            href (str): The URL of this resource, without the protocol
-            submitted_at (datetime):
-            status (bool, date, datetime, dict, float, int, list, str, none_type):
-            owner (str): The user that owns this resource
-            connector_type_id (str): The connector type
-            connector ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The Connector configuration payload
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """EnterpriseClusterListItem - a model defined in OpenAPI
 
         Keyword Args:
+            id (str):
+            kind (str):
+            href (str):
+            access_kafkas_via_private_network (bool): Indicates whether Kafkas created on this data plane cluster have to be accessed via private network
+            multi_az (bool): A flag indicating whether this cluster is available on multiple availability zones or not
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -272,17 +270,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            published_at (datetime): [optional]  # noqa: E501
-            modified_at (datetime): [optional]  # noqa: E501
-            status_message (str): A detailed status message in case there is a problem with the connector. [optional]  # noqa: E501
+            cluster_id (str): The OCM's cluster id of the registered Enterprise cluster.. [optional]  # noqa: E501
+            status (str): The status of Enterprise cluster registration. [optional]  # noqa: E501
+            cloud_provider (str): The cloud provider for this cluster. This valus will be used as the Kafka's cloud provider value when a Kafka is created on this cluster. [optional]  # noqa: E501
+            region (str): The region of this cluster. This valus will be used as the Kafka's region value when a Kafka is created on this cluster. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -304,27 +303,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.kind = kind
-        self.id = id
-        self.name = name
-        self.href = href
-        self.submitted_at = submitted_at
-        self.status = status
-        self.owner = owner
-        self.connector_type_id = connector_type_id
-        self.connector = connector
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              EnterpriseClusterListItemAllOf,
+              ObjectReference,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model_utils.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/models/__init__.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/rest.py` & `rhoas_sdks-1.0.2b2/sdks/smart_events_mgmt_sdk/rhoas_smart_events_mgmt_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `rhoas_sdks-1.0.2/PKG-INFO` & `rhoas_sdks-1.0.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhoas-sdks
-Version: 1.0.2
+Version: 1.0.2b2
 Summary: A package which includes RHOAS SDKs
 License: Apache License
 Author: dimakis
 Author-email: dsaridak@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 # RHOAS Core SDKs
 
 > If you are moving a project from the old RHOAS SDKs to core read this [moving](./MOVING.md) doc to get started.
 
 | Supported Langauge  | SDK |
 | ----------- | ----------- |
-| JavaScript  | [app-services-sdk-ts](/app-services-sdk-ts/) |
+| JavaScript/TypeScript  | [app-services-sdk-js](/app-services-sdk-js/) |
 | Python   | [app-services-sdk-python](/app-services-sdk-python/)    |
 | Java   | [app-services-sdk-java](/app-services-sdk-java/)        |
 |  Go   | [app-services-sdk-go](/app-services-sdk-go/)        |
 
 ## Structure
 
 RHOAS SDK's are delivered as set of individual packages.
@@ -36,17 +36,17 @@
 - **Instance SDKs** -  support direct interaction with services
 
 ## Purpose of this repository
 
 Repository contains source code for openapi based generator along with automation scripts that generate all
 underlying RHOAS SDKS. 
 
-# RHOAS SDK for Typescript
+# RHOAS SDK for Typescript and JavaScript
 
-Typescript packages and API clients for RHOAS services
+Typescript and JavaScript packages and API clients for RHOAS services
 
 ## Prequisites
 
 - [NodeJS 14.x lts](https://nodejs.org/en/about/releases/) or above
 
 ## Management SDK's
```

