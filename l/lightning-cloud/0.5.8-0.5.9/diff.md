# Comparing `tmp/lightning_cloud-0.5.8.tar.gz` & `tmp/lightning_cloud-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightning_cloud-0.5.8.tar", last modified: Tue Sep 27 18:11:34 2022, max compression
+gzip compressed data, was "dist/lightning_cloud-0.5.9.tar", last modified: Fri Sep 30 15:29:06 2022, max compression
```

## Comparing `lightning_cloud-0.5.8.tar` & `lightning_cloud-0.5.9.tar`

### file list

```diff
@@ -1,213 +1,212 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.476990 lightning_cloud-0.5.8/
--rw-r--r--   0 runner    (1000) runner    (1000)    11360 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      853 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)      683 2022-09-27 18:11:34.476990 lightning_cloud-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       57 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.448990 lightning_cloud-0.5.8/lightning_cloud/
--rw-r--r--   0 runner    (1000) runner    (1000)       93 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/__version__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.449990 lightning_cloud-0.5.8/lightning_cloud/cli/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/cli/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      455 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/cli/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1310 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/env.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6981 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/login.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.450990 lightning_cloud-0.5.8/lightning_cloud/openapi/
--rw-r--r--   0 runner    (1000) runner    (1000)    17533 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.452990 lightning_cloud-0.5.8/lightning_cloud/openapi/api/
--rw-r--r--   0 runner    (1000) runner    (1000)      915 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19857 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/auth_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29714 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/cluster_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42949 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningapp_instance_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    64743 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningapp_v2_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29286 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningwork_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38024 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/models_store_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    80669 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/projects_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23277 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/secret_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17087 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/ssh_public_key_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5009 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api/user_service_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25996 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/api_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8309 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/configuration.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.475990 lightning_cloud-0.5.8/lightning_cloud/openapi/models/
--rw-r--r--   0 runner    (1000) runner    (1000)    14906 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15572 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/app_id_releases_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4361 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/appinstances_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3922 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/appsv2_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4227 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/clusters_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6451 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9426 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_lightningapp_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8273 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_lightningwork.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6302 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_user_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3227 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/get_cluster_health_response_health_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6522 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/id_get_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3648 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/id_release_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3217 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/instance_type_availability.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10037 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/model_version_archive_contains_information_about_a_specific_uploaded_model_version_its_versionfiles_and_metadata.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4662 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_appsv2_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5037 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_getapp_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4481 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_memberships_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11066 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_models_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3878 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_projectclustersbindings_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4237 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_secrets_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5018 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/projects_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5178 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/projects_project_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7120 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/protobuf_any.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4952 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/rpc_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3549 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/secrets_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4557 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/spec_lightningapp_instance_id_works_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3778 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/user_id_membershiprolebindings_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32161 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_aws_cluster_driver_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7535 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_azure_cluster_driver_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3021 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_azure_cluster_driver_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6791 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_build_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5358 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_driver.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5466 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_driver_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5118 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_log_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3239 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_performance_profile.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11299 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3221 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_state.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7253 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3129 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4508 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_compute_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6233 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_container_resources.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4339 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_cluster_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6607 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_cluster_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5162 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5221 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_ssh_public_key_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3003 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_cluster_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3081 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_instance_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3075 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_release_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3045 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_v2_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3039 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningwork_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3087 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_membership_role_binding_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2991 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_model_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3033 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_model_version_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3087 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_cluster_binding_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3063 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_membership_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3003 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_role_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2997 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_secret_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3033 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_ssh_public_key_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3184 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_dependency_cache_state.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4548 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_dependency_file_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3788 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_download_model_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4982 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6089 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3207 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_state.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3222 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_state_reason.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6791 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3098 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2955 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2967 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11490 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_eks_custer_driver_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4859 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_env_var.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3719 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_external_kubeconfig.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4065 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_flowserver.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22415 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_gallery_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23314 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_gallery_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3932 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_cluster_health_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6529 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_cluster_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3915 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_lightningapp_source_code_download_url_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15760 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_user_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10972 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_image_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6319 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_instance_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8973 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_instance_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12083 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_kubernetes_cluster_driver.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9845 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_kubernetes_cluster_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4329 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_app_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4447 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4411 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_basic_auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4825 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_o_auth_auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7055 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_artifact.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8807 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_event.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22128 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3511 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_state.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12233 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20523 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_release.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3225 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_restart_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7559 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_v2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4959 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_cost.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4508 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_drives.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13749 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_spec.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3405 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_state.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9286 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3495 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_status_reason.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4057 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_cluster_instance_types_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4742 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_clusters_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3972 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_gallery_components_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3829 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_gallery_lightningapps_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6204 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instance_artifacts_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4074 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instance_events_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6132 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instances_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5918 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapps_v2_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4060 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningwork_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4352 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_membership_role_binding_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3879 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_memberships_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3910 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_model_versions_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3699 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_models_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4020 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_project_cluster_bindings_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3949 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_project_memberships_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3663 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_roles_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3735 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_secrets_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5571 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_ssh_public_keys_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5027 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_login_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3569 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_login_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2955 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_logout_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2961 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_logout_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11044 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_membership.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6861 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_membership_role_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11049 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_metadata.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11184 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_model.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9107 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_model_version_archive.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4796 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_network_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3117 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_package_manager.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7710 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8830 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_project_cluster_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4678 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_python_dependency_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3145 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_queue_server_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11373 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_quotas.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3639 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_refresh_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3589 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_refresh_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6893 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_resources.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7665 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5140 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3163 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_action.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3059 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_effect.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3467 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_resource.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11185 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_search_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6364 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_search_users_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6313 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_secret.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_slurm_cluster_driver.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_slurm_cluster_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3047 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_source_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7135 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_ssh_public_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5795 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_update_cluster_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13111 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_update_user_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4442 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_upload_model_version_response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6800 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_user_requested_compute_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5357 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_user_requested_flow_compute_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4151 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_work.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3605 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/models/works_id_body.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14298 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/openapi/rest.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2559 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/rest_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.476990 lightning_cloud-0.5.8/lightning_cloud/source_code/
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6258 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/copytree.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/hashing.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3941 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/local.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3431 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/logs_socket_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5835 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/tar.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3207 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/source_code/uploader.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.476990 lightning_cloud-0.5.8/lightning_cloud/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    58046 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/utils/name_generator.py
--rw-r--r--   0 runner    (1000) runner    (1000)      406 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/lightning_cloud/utils/network.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 18:11:34.449990 lightning_cloud-0.5.8/lightning_cloud.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      683 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)    10979 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       71 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2022-09-27 18:11:34.000000 lightning_cloud-0.5.8/lightning_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       74 2022-09-27 18:11:34.477990 lightning_cloud-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1837 2022-09-27 18:11:03.000000 lightning_cloud-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.953113 lightning_cloud-0.5.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11360 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      853 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)      683 2022-09-30 15:29:06.953113 lightning_cloud-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       57 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.930113 lightning_cloud-0.5.9/lightning_cloud/
+-rw-r--r--   0 runner    (1000) runner    (1000)       93 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/__version__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.931113 lightning_cloud-0.5.9/lightning_cloud/cli/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/cli/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      455 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/cli/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1310 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/env.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6981 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/login.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.931113 lightning_cloud-0.5.9/lightning_cloud/openapi/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17265 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.933113 lightning_cloud-0.5.9/lightning_cloud/openapi/api/
+-rw-r--r--   0 runner    (1000) runner    (1000)      915 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19857 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/auth_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29714 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/cluster_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42949 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningapp_instance_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    64743 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningapp_v2_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29286 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningwork_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31635 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/models_store_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    80669 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/projects_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23277 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/secret_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17087 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/ssh_public_key_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5009 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api/user_service_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25996 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/api_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8309 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/configuration.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.952113 lightning_cloud-0.5.9/lightning_cloud/openapi/models/
+-rw-r--r--   0 runner    (1000) runner    (1000)    14638 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15572 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/app_id_releases_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4361 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/appinstances_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4630 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/appsv2_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4227 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/clusters_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6451 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9426 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_lightningapp_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8273 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_lightningwork.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6302 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_user_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3227 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/get_cluster_health_response_health_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6522 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/id_get_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3648 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/id_release_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3217 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/instance_type_availability.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5397 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_appsv2_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5037 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_getapp_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4481 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_memberships_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3878 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_projectclustersbindings_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4237 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_secrets_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5018 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/projects_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5178 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/projects_project_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7120 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/protobuf_any.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4952 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/rpc_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3549 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/secrets_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4557 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/spec_lightningapp_instance_id_works_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3778 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/user_id_membershiprolebindings_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32161 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_aws_cluster_driver_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7535 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_azure_cluster_driver_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3021 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_azure_cluster_driver_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6791 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_build_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5358 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_driver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5466 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_driver_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5118 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_log_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3239 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_performance_profile.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11299 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3221 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_state.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7253 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3129 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4508 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_compute_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6233 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_container_resources.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4339 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_cluster_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6607 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_cluster_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5162 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5221 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_ssh_public_key_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3003 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_cluster_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3081 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_instance_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3075 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_release_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3045 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_v2_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3039 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningwork_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3087 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_membership_role_binding_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2991 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_model_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3033 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_model_version_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3087 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_cluster_binding_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3063 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_membership_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3003 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_role_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2997 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_secret_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3033 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_ssh_public_key_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3184 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_dependency_cache_state.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4548 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_dependency_file_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5365 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_download_model_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4982 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6089 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3207 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_state.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3222 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_state_reason.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6791 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3098 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2955 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2967 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11490 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_eks_custer_driver_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4859 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_env_var.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3719 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_external_kubeconfig.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4065 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_flowserver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22415 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_gallery_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23314 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_gallery_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3932 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_cluster_health_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6529 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_cluster_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3915 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_lightningapp_source_code_download_url_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15760 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_user_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10972 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_image_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6319 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_instance_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8973 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_instance_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12083 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_kubernetes_cluster_driver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9845 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_kubernetes_cluster_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4329 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_app_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4447 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4411 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_basic_auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4825 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_o_auth_auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7055 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_artifact.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8807 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_event.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22869 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3511 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_state.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12233 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20523 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_release.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3225 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_restart_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8260 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_v2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4959 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_cost.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4508 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_drives.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13749 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_spec.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3405 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_state.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9286 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3495 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_status_reason.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4057 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_cluster_instance_types_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4742 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_clusters_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3972 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_gallery_components_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3829 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_gallery_lightningapps_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6204 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instance_artifacts_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4074 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instance_events_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6132 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instances_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5918 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapps_v2_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4060 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningwork_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4352 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_membership_role_binding_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3879 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_memberships_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3910 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_model_versions_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3699 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_models_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4020 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_project_cluster_bindings_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3949 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_project_memberships_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3663 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_roles_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3735 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_secrets_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5571 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_ssh_public_keys_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5027 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_login_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3569 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_login_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2955 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_logout_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2961 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_logout_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11044 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_membership.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6861 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_membership_role_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11049 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_metadata.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11184 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_model.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9160 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_model_version_archive.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4796 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_network_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3117 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_package_manager.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7710 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8830 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_project_cluster_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4678 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_python_dependency_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3145 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_queue_server_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11373 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_quotas.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3639 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_refresh_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3589 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_refresh_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6893 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_resources.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7665 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5140 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3163 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_action.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3059 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_effect.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3467 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_resource.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11185 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_search_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6364 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_search_users_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6313 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_secret.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_slurm_cluster_driver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2985 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_slurm_cluster_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3047 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_source_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7135 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_ssh_public_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5795 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_update_cluster_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13111 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_update_user_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6639 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_upload_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5192 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_upload_model_response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6800 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_user_requested_compute_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5357 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_user_requested_flow_compute_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4151 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_work.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3605 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/models/works_id_body.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14298 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/openapi/rest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2559 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/rest_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.953113 lightning_cloud-0.5.9/lightning_cloud/source_code/
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6258 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/copytree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/hashing.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3941 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/local.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3431 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/logs_socket_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5835 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/tar.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3207 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/source_code/uploader.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.953113 lightning_cloud-0.5.9/lightning_cloud/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    58046 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/utils/name_generator.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      406 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/lightning_cloud/utils/network.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-30 15:29:06.931113 lightning_cloud-0.5.9/lightning_cloud.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      683 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)    10825 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       71 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2022-09-30 15:29:06.000000 lightning_cloud-0.5.9/lightning_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       74 2022-09-30 15:29:06.954113 lightning_cloud-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1837 2022-09-30 15:28:39.000000 lightning_cloud-0.5.9/setup.py
```

### Comparing `lightning_cloud-0.5.8/LICENSE` & `lightning_cloud-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/MANIFEST.in` & `lightning_cloud-0.5.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/PKG-INFO` & `lightning_cloud-0.5.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning_cloud
-Version: 0.5.8
+Version: 0.5.9
 Summary: Lightning Cloud
 Home-page: https://lightning.ai
 Author: Grid.ai
 Author-email: grid-eng@grid.ai
 License: Apache Software License
 Description: Lightning AI Command Line Interface
 Platform: UNKNOWN
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/env.py` & `lightning_cloud-0.5.9/lightning_cloud/env.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/login.py` & `lightning_cloud-0.5.9/lightning_cloud/login.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/__init__.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,17 @@
 from lightning_cloud.openapi.models.externalv1_lightningapp_instance import Externalv1LightningappInstance
 from lightning_cloud.openapi.models.externalv1_lightningwork import Externalv1Lightningwork
 from lightning_cloud.openapi.models.externalv1_user_status import Externalv1UserStatus
 from lightning_cloud.openapi.models.get_cluster_health_response_health_status import GetClusterHealthResponseHealthStatus
 from lightning_cloud.openapi.models.id_get_body import IdGetBody
 from lightning_cloud.openapi.models.id_release_body import IdReleaseBody
 from lightning_cloud.openapi.models.instance_type_availability import InstanceTypeAvailability
-from lightning_cloud.openapi.models.model_version_archive_contains_information_about_a_specific_uploaded_model_version_its_versionfiles_and_metadata import ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata
 from lightning_cloud.openapi.models.project_id_appsv2_body import ProjectIdAppsv2Body
 from lightning_cloud.openapi.models.project_id_getapp_body import ProjectIdGetappBody
 from lightning_cloud.openapi.models.project_id_memberships_body import ProjectIdMembershipsBody
-from lightning_cloud.openapi.models.project_id_models_body import ProjectIdModelsBody
 from lightning_cloud.openapi.models.project_id_projectclustersbindings_body import ProjectIdProjectclustersbindingsBody
 from lightning_cloud.openapi.models.project_id_secrets_body import ProjectIdSecretsBody
 from lightning_cloud.openapi.models.projects_id_body import ProjectsIdBody
 from lightning_cloud.openapi.models.projects_project_id_body import ProjectsProjectIdBody
 from lightning_cloud.openapi.models.protobuf_any import ProtobufAny
 from lightning_cloud.openapi.models.rpc_status import RpcStatus
 from lightning_cloud.openapi.models.secrets_id_body import SecretsIdBody
@@ -184,15 +182,16 @@
 from lightning_cloud.openapi.models.v1_search_users_response import V1SearchUsersResponse
 from lightning_cloud.openapi.models.v1_secret import V1Secret
 from lightning_cloud.openapi.models.v1_slurm_cluster_driver import V1SlurmClusterDriver
 from lightning_cloud.openapi.models.v1_slurm_cluster_status import V1SlurmClusterStatus
 from lightning_cloud.openapi.models.v1_source_type import V1SourceType
 from lightning_cloud.openapi.models.v1_update_cluster_response import V1UpdateClusterResponse
 from lightning_cloud.openapi.models.v1_update_user_request import V1UpdateUserRequest
-from lightning_cloud.openapi.models.v1_upload_model_version_response import V1UploadModelVersionResponse
+from lightning_cloud.openapi.models.v1_upload_model_request import V1UploadModelRequest
+from lightning_cloud.openapi.models.v1_upload_model_response import V1UploadModelResponse
 from lightning_cloud.openapi.models.v1_user_requested_compute_config import V1UserRequestedComputeConfig
 from lightning_cloud.openapi.models.v1_user_requested_flow_compute_config import V1UserRequestedFlowComputeConfig
 from lightning_cloud.openapi.models.v1_work import V1Work
 from lightning_cloud.openapi.models.works_id_body import WorksIdBody
 from lightning_cloud.openapi.models.v1_image_spec import V1ImageSpec as Gridv1ImageSpec
 from lightning_cloud.openapi.models.clusters_id_body import ClustersIdBody as Body
 from lightning_cloud.openapi.models.projects_id_body import ProjectsIdBody as Body1
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/__init__.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/auth_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/auth_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/cluster_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/cluster_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningapp_instance_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningapp_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningapp_v2_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningapp_v2_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/lightningwork_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/lightningwork_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/models_store_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/models_store_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,127 +38,14 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     """
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def models_store_create_model(self, body: 'ProjectIdModelsBody',
-                                  project_id: 'str',
-                                  **kwargs) -> 'V1Model':  # noqa: E501
-        """CreateModel is used to create a new model  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_create_model(body, project_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param ProjectIdModelsBody body: (required)
-        :param str project_id: (required)
-        :return: V1Model
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.models_store_create_model_with_http_info(
-                body, project_id, **kwargs)  # noqa: E501
-        else:
-            (data) = self.models_store_create_model_with_http_info(
-                body, project_id, **kwargs)  # noqa: E501
-            return data
-
-    def models_store_create_model_with_http_info(
-            self, body: 'ProjectIdModelsBody', project_id: 'str',
-            **kwargs) -> 'V1Model':  # noqa: E501
-        """CreateModel is used to create a new model  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_create_model_with_http_info(body, project_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param ProjectIdModelsBody body: (required)
-        :param str project_id: (required)
-        :return: V1Model
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['body', 'project_id']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError("Got an unexpected keyword argument '%s'"
-                                " to method models_store_create_model" % key)
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or params['body'] is None):
-            raise ValueError(
-                "Missing the required parameter `body` when calling `models_store_create_model`"
-            )  # noqa: E501
-        # verify the required parameter 'project_id' is set
-        if ('project_id' not in params or params['project_id'] is None):
-            raise ValueError(
-                "Missing the required parameter `project_id` when calling `models_store_create_model`"
-            )  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'project_id' in params:
-            path_params['projectId'] = params['project_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params[
-            'Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-                ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = []  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/projects/{projectId}/models',
-            'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='V1Model',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def models_store_delete_model(
             self, project_id: 'str', model_id: 'str',
             **kwargs) -> 'V1DeleteModelResponse':  # noqa: E501
         """DeleteModel is used to delete the model and all uploaded archives  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -378,51 +265,49 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def models_store_download_model(
-            self, name: 'str',
-            **kwargs) -> 'V1DownloadModelResponse':  # noqa: E501
-        """DownloadModel is a public facing API used by the Python library to get a presigned URL to download the model  # noqa: E501
+            self, **kwargs) -> 'V1DownloadModelResponse':  # noqa: E501
+        """DownloadModel is a public facing API used by the Python library to get a presigned URL to download the model. Name is a required query parameter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_download_model(name, async_req=True)
+        >>> thread = api.models_store_download_model(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: (required)
+        :param str name:
         :param str version:
         :return: V1DownloadModelResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.models_store_download_model_with_http_info(
-                name, **kwargs)  # noqa: E501
+                **kwargs)  # noqa: E501
         else:
             (data) = self.models_store_download_model_with_http_info(
-                name, **kwargs)  # noqa: E501
+                **kwargs)  # noqa: E501
             return data
 
     def models_store_download_model_with_http_info(
-            self, name: 'str',
-            **kwargs) -> 'V1DownloadModelResponse':  # noqa: E501
-        """DownloadModel is a public facing API used by the Python library to get a presigned URL to download the model  # noqa: E501
+            self, **kwargs) -> 'V1DownloadModelResponse':  # noqa: E501
+        """DownloadModel is a public facing API used by the Python library to get a presigned URL to download the model. Name is a required query parameter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_download_model_with_http_info(name, async_req=True)
+        >>> thread = api.models_store_download_model_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: (required)
+        :param str name:
         :param str version:
         :return: V1DownloadModelResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['name', 'version']  # noqa: E501
@@ -434,27 +319,22 @@
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError("Got an unexpected keyword argument '%s'"
                                 " to method models_store_download_model" % key)
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'name' is set
-        if ('name' not in params or params['name'] is None):
-            raise ValueError(
-                "Missing the required parameter `name` when calling `models_store_download_model`"
-            )  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'name' in params:
-            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
+        if 'name' in params:
+            query_params.append(('name', params['name']))  # noqa: E501
         if 'version' in params:
             query_params.append(('version', params['version']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -464,15 +344,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/models/{name}/url',
+            '/v1/models',
             'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
@@ -795,101 +675,78 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def models_store_upload_model_version(
-            self, body:
-        'ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata',
-            project_id: 'str', model_id: 'str',
-            **kwargs) -> 'V1UploadModelVersionResponse':  # noqa: E501
-        """UploadModelVersion used to upload a new model version. Once the new model archive version is created, a presigned URL is returned to the client for the upload  # noqa: E501
+    def models_store_upload_model(
+            self, body: 'V1UploadModelRequest',
+            **kwargs) -> 'V1UploadModelResponse':  # noqa: E501
+        """UploadModel used to upload a new model version. It will either create a new top level model entry or reuse existing if an existing model is found. If version is not supplied, it will overwrite 'latest' version entry.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_upload_model_version(body, project_id, model_id, async_req=True)
+        >>> thread = api.models_store_upload_model(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata body: (required)
-        :param str project_id: (required)
-        :param str model_id: (required)
-        :return: V1UploadModelVersionResponse
+        :param V1UploadModelRequest body: (required)
+        :return: V1UploadModelResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.models_store_upload_model_version_with_http_info(
-                body, project_id, model_id, **kwargs)  # noqa: E501
+            return self.models_store_upload_model_with_http_info(
+                body, **kwargs)  # noqa: E501
         else:
-            (data) = self.models_store_upload_model_version_with_http_info(
-                body, project_id, model_id, **kwargs)  # noqa: E501
+            (data) = self.models_store_upload_model_with_http_info(
+                body, **kwargs)  # noqa: E501
             return data
 
-    def models_store_upload_model_version_with_http_info(
-            self, body:
-        'ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata',
-            project_id: 'str', model_id: 'str',
-            **kwargs) -> 'V1UploadModelVersionResponse':  # noqa: E501
-        """UploadModelVersion used to upload a new model version. Once the new model archive version is created, a presigned URL is returned to the client for the upload  # noqa: E501
+    def models_store_upload_model_with_http_info(
+            self, body: 'V1UploadModelRequest',
+            **kwargs) -> 'V1UploadModelResponse':  # noqa: E501
+        """UploadModel used to upload a new model version. It will either create a new top level model entry or reuse existing if an existing model is found. If version is not supplied, it will overwrite 'latest' version entry.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_store_upload_model_version_with_http_info(body, project_id, model_id, async_req=True)
+        >>> thread = api.models_store_upload_model_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata body: (required)
-        :param str project_id: (required)
-        :param str model_id: (required)
-        :return: V1UploadModelVersionResponse
+        :param V1UploadModelRequest body: (required)
+        :return: V1UploadModelResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'project_id', 'model_id']  # noqa: E501
+        all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method models_store_upload_model_version" % key)
+                raise TypeError("Got an unexpected keyword argument '%s'"
+                                " to method models_store_upload_model" % key)
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or params['body'] is None):
             raise ValueError(
-                "Missing the required parameter `body` when calling `models_store_upload_model_version`"
-            )  # noqa: E501
-        # verify the required parameter 'project_id' is set
-        if ('project_id' not in params or params['project_id'] is None):
-            raise ValueError(
-                "Missing the required parameter `project_id` when calling `models_store_upload_model_version`"
-            )  # noqa: E501
-        # verify the required parameter 'model_id' is set
-        if ('model_id' not in params or params['model_id'] is None):
-            raise ValueError(
-                "Missing the required parameter `model_id` when calling `models_store_upload_model_version`"
+                "Missing the required parameter `body` when calling `models_store_upload_model`"
             )  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'project_id' in params:
-            path_params['projectId'] = params['project_id']  # noqa: E501
-        if 'model_id' in params:
-            path_params['modelId'] = params['model_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -906,22 +763,22 @@
             'Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
                 ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/projects/{projectId}/models/{modelId}/versions',
+            '/v1/models',
             'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1UploadModelVersionResponse',  # noqa: E501
+            response_type='V1UploadModelResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/projects_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/projects_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/secret_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/secret_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/ssh_public_key_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/ssh_public_key_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api/user_service_api.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api/user_service_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/api_client.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/configuration.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/__init__.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,17 @@
 from lightning_cloud.openapi.models.externalv1_lightningapp_instance import Externalv1LightningappInstance
 from lightning_cloud.openapi.models.externalv1_lightningwork import Externalv1Lightningwork
 from lightning_cloud.openapi.models.externalv1_user_status import Externalv1UserStatus
 from lightning_cloud.openapi.models.get_cluster_health_response_health_status import GetClusterHealthResponseHealthStatus
 from lightning_cloud.openapi.models.id_get_body import IdGetBody
 from lightning_cloud.openapi.models.id_release_body import IdReleaseBody
 from lightning_cloud.openapi.models.instance_type_availability import InstanceTypeAvailability
-from lightning_cloud.openapi.models.model_version_archive_contains_information_about_a_specific_uploaded_model_version_its_versionfiles_and_metadata import ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata
 from lightning_cloud.openapi.models.project_id_appsv2_body import ProjectIdAppsv2Body
 from lightning_cloud.openapi.models.project_id_getapp_body import ProjectIdGetappBody
 from lightning_cloud.openapi.models.project_id_memberships_body import ProjectIdMembershipsBody
-from lightning_cloud.openapi.models.project_id_models_body import ProjectIdModelsBody
 from lightning_cloud.openapi.models.project_id_projectclustersbindings_body import ProjectIdProjectclustersbindingsBody
 from lightning_cloud.openapi.models.project_id_secrets_body import ProjectIdSecretsBody
 from lightning_cloud.openapi.models.projects_id_body import ProjectsIdBody
 from lightning_cloud.openapi.models.projects_project_id_body import ProjectsProjectIdBody
 from lightning_cloud.openapi.models.protobuf_any import ProtobufAny
 from lightning_cloud.openapi.models.rpc_status import RpcStatus
 from lightning_cloud.openapi.models.secrets_id_body import SecretsIdBody
@@ -170,12 +168,13 @@
 from lightning_cloud.openapi.models.v1_search_users_response import V1SearchUsersResponse
 from lightning_cloud.openapi.models.v1_secret import V1Secret
 from lightning_cloud.openapi.models.v1_slurm_cluster_driver import V1SlurmClusterDriver
 from lightning_cloud.openapi.models.v1_slurm_cluster_status import V1SlurmClusterStatus
 from lightning_cloud.openapi.models.v1_source_type import V1SourceType
 from lightning_cloud.openapi.models.v1_update_cluster_response import V1UpdateClusterResponse
 from lightning_cloud.openapi.models.v1_update_user_request import V1UpdateUserRequest
-from lightning_cloud.openapi.models.v1_upload_model_version_response import V1UploadModelVersionResponse
+from lightning_cloud.openapi.models.v1_upload_model_request import V1UploadModelRequest
+from lightning_cloud.openapi.models.v1_upload_model_response import V1UploadModelResponse
 from lightning_cloud.openapi.models.v1_user_requested_compute_config import V1UserRequestedComputeConfig
 from lightning_cloud.openapi.models.v1_user_requested_flow_compute_config import V1UserRequestedFlowComputeConfig
 from lightning_cloud.openapi.models.v1_work import V1Work
 from lightning_cloud.openapi.models.works_id_body import WorksIdBody
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/app_id_releases_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/app_id_releases_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/appinstances_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/appinstances_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/appsv2_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/appsv2_id_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -36,24 +36,32 @@
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'can_download_source_code': 'bool'}
+    swagger_types = {'can_download_source_code': 'bool', 'private': 'bool'}
 
-    attribute_map = {'can_download_source_code': 'canDownloadSourceCode'}
-
-    def __init__(self, can_download_source_code: 'bool' = None):  # noqa: E501
+    attribute_map = {
+        'can_download_source_code': 'canDownloadSourceCode',
+        'private': 'private'
+    }
+
+    def __init__(self,
+                 can_download_source_code: 'bool' = None,
+                 private: 'bool' = None):  # noqa: E501
         """Appsv2IdBody - a model defined in Swagger"""  # noqa: E501
         self._can_download_source_code = None
+        self._private = None
         self.discriminator = None
         if can_download_source_code is not None:
             self.can_download_source_code = can_download_source_code
+        if private is not None:
+            self.private = private
 
     @property
     def can_download_source_code(self) -> 'bool':
         """Gets the can_download_source_code of this Appsv2IdBody.  # noqa: E501
 
 
         :return: The can_download_source_code of this Appsv2IdBody.  # noqa: E501
@@ -68,14 +76,35 @@
 
         :param can_download_source_code: The can_download_source_code of this Appsv2IdBody.  # noqa: E501
         :type: bool
         """
 
         self._can_download_source_code = can_download_source_code
 
+    @property
+    def private(self) -> 'bool':
+        """Gets the private of this Appsv2IdBody.  # noqa: E501
+
+
+        :return: The private of this Appsv2IdBody.  # noqa: E501
+        :rtype: bool
+        """
+        return self._private
+
+    @private.setter
+    def private(self, private: 'bool'):
+        """Sets the private of this Appsv2IdBody.
+
+
+        :param private: The private of this Appsv2IdBody.  # noqa: E501
+        :type: bool
+        """
+
+        self._private = private
+
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/clusters_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/clusters_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_cluster.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_cluster.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_lightningapp_instance.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_lightningapp_instance.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_lightningwork.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_lightningwork.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/externalv1_user_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/externalv1_user_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/get_cluster_health_response_health_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/get_cluster_health_response_health_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/id_get_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/id_get_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/id_release_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/id_release_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/instance_type_availability.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/instance_type_availability.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/model_version_archive_contains_information_about_a_specific_uploaded_model_version_its_versionfiles_and_metadata.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_model_version_archive.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,194 +24,247 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata(
-        object):
+class V1ModelVersionArchive(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'cluster_id': 'str',
         'created_at': 'datetime',
         'downloads': 'str',
         'metadata': 'dict(str, str)',
-        'private': 'bool',
+        'model_id': 'str',
+        'project_id': 'str',
         'updated_at': 'datetime',
         'version': 'str'
     }
 
     attribute_map = {
+        'cluster_id': 'clusterId',
         'created_at': 'createdAt',
         'downloads': 'downloads',
         'metadata': 'metadata',
-        'private': 'private',
+        'model_id': 'modelId',
+        'project_id': 'projectId',
         'updated_at': 'updatedAt',
         'version': 'version'
     }
 
     def __init__(self,
+                 cluster_id: 'str' = None,
                  created_at: 'datetime' = None,
                  downloads: 'str' = None,
                  metadata: 'dict(str, str)' = None,
-                 private: 'bool' = None,
+                 model_id: 'str' = None,
+                 project_id: 'str' = None,
                  updated_at: 'datetime' = None,
                  version: 'str' = None):  # noqa: E501
-        """ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata - a model defined in Swagger"""  # noqa: E501
+        """V1ModelVersionArchive - a model defined in Swagger"""  # noqa: E501
+        self._cluster_id = None
         self._created_at = None
         self._downloads = None
         self._metadata = None
-        self._private = None
+        self._model_id = None
+        self._project_id = None
         self._updated_at = None
         self._version = None
         self.discriminator = None
+        if cluster_id is not None:
+            self.cluster_id = cluster_id
         if created_at is not None:
             self.created_at = created_at
         if downloads is not None:
             self.downloads = downloads
         if metadata is not None:
             self.metadata = metadata
-        if private is not None:
-            self.private = private
+        if model_id is not None:
+            self.model_id = model_id
+        if project_id is not None:
+            self.project_id = project_id
         if updated_at is not None:
             self.updated_at = updated_at
         if version is not None:
             self.version = version
 
     @property
+    def cluster_id(self) -> 'str':
+        """Gets the cluster_id of this V1ModelVersionArchive.  # noqa: E501
+
+
+        :return: The cluster_id of this V1ModelVersionArchive.  # noqa: E501
+        :rtype: str
+        """
+        return self._cluster_id
+
+    @cluster_id.setter
+    def cluster_id(self, cluster_id: 'str'):
+        """Sets the cluster_id of this V1ModelVersionArchive.
+
+
+        :param cluster_id: The cluster_id of this V1ModelVersionArchive.  # noqa: E501
+        :type: str
+        """
+
+        self._cluster_id = cluster_id
+
+    @property
     def created_at(self) -> 'datetime':
-        """Gets the created_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        """Gets the created_at of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The created_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :return: The created_at of this V1ModelVersionArchive.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at: 'datetime'):
-        """Sets the created_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+        """Sets the created_at of this V1ModelVersionArchive.
 
 
-        :param created_at: The created_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :param created_at: The created_at of this V1ModelVersionArchive.  # noqa: E501
         :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def downloads(self) -> 'str':
-        """Gets the downloads of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        """Gets the downloads of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The downloads of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :return: The downloads of this V1ModelVersionArchive.  # noqa: E501
         :rtype: str
         """
         return self._downloads
 
     @downloads.setter
     def downloads(self, downloads: 'str'):
-        """Sets the downloads of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+        """Sets the downloads of this V1ModelVersionArchive.
 
 
-        :param downloads: The downloads of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :param downloads: The downloads of this V1ModelVersionArchive.  # noqa: E501
         :type: str
         """
 
         self._downloads = downloads
 
     @property
     def metadata(self) -> 'dict(str, str)':
-        """Gets the metadata of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        """Gets the metadata of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The metadata of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :return: The metadata of this V1ModelVersionArchive.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata: 'dict(str, str)'):
-        """Sets the metadata of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+        """Sets the metadata of this V1ModelVersionArchive.
 
 
-        :param metadata: The metadata of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :param metadata: The metadata of this V1ModelVersionArchive.  # noqa: E501
         :type: dict(str, str)
         """
 
         self._metadata = metadata
 
     @property
-    def private(self) -> 'bool':
-        """Gets the private of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+    def model_id(self) -> 'str':
+        """Gets the model_id of this V1ModelVersionArchive.  # noqa: E501
+
+
+        :return: The model_id of this V1ModelVersionArchive.  # noqa: E501
+        :rtype: str
+        """
+        return self._model_id
+
+    @model_id.setter
+    def model_id(self, model_id: 'str'):
+        """Sets the model_id of this V1ModelVersionArchive.
+
+
+        :param model_id: The model_id of this V1ModelVersionArchive.  # noqa: E501
+        :type: str
+        """
+
+        self._model_id = model_id
+
+    @property
+    def project_id(self) -> 'str':
+        """Gets the project_id of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The private of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
-        :rtype: bool
+        :return: The project_id of this V1ModelVersionArchive.  # noqa: E501
+        :rtype: str
         """
-        return self._private
+        return self._project_id
 
-    @private.setter
-    def private(self, private: 'bool'):
-        """Sets the private of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+    @project_id.setter
+    def project_id(self, project_id: 'str'):
+        """Sets the project_id of this V1ModelVersionArchive.
 
 
-        :param private: The private of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
-        :type: bool
+        :param project_id: The project_id of this V1ModelVersionArchive.  # noqa: E501
+        :type: str
         """
 
-        self._private = private
+        self._project_id = project_id
 
     @property
     def updated_at(self) -> 'datetime':
-        """Gets the updated_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        """Gets the updated_at of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The updated_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :return: The updated_at of this V1ModelVersionArchive.  # noqa: E501
         :rtype: datetime
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at: 'datetime'):
-        """Sets the updated_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+        """Sets the updated_at of this V1ModelVersionArchive.
 
 
-        :param updated_at: The updated_at of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :param updated_at: The updated_at of this V1ModelVersionArchive.  # noqa: E501
         :type: datetime
         """
 
         self._updated_at = updated_at
 
     @property
     def version(self) -> 'str':
-        """Gets the version of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        """Gets the version of this V1ModelVersionArchive.  # noqa: E501
 
 
-        :return: The version of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :return: The version of this V1ModelVersionArchive.  # noqa: E501
         :rtype: str
         """
         return self._version
 
     @version.setter
     def version(self, version: 'str'):
-        """Sets the version of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.
+        """Sets the version of this V1ModelVersionArchive.
 
 
-        :param version: The version of this ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata.  # noqa: E501
+        :param version: The version of this V1ModelVersionArchive.  # noqa: E501
         :type: str
         """
 
         self._version = version
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
@@ -229,42 +282,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(
-                ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata,
-                dict):
+        if issubclass(V1ModelVersionArchive, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(
-        self, other:
-        'ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata'
-    ) -> bool:
+    def __eq__(self, other: 'V1ModelVersionArchive') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(
-                other,
-                ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata
-        ):
+        if not isinstance(other, V1ModelVersionArchive):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(
-        self, other:
-        'ModelVersionArchiveContainsInformationAboutASpecificUploadedModelVersionItsVersionfilesAndMetadata'
-    ) -> bool:
+    def __ne__(self, other: 'V1ModelVersionArchive') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_appsv2_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_appsv2_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,32 +36,41 @@
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'can_download_source_code': 'bool', 'name': 'str'}
+    swagger_types = {
+        'can_download_source_code': 'bool',
+        'name': 'str',
+        'private': 'bool'
+    }
 
     attribute_map = {
         'can_download_source_code': 'canDownloadSourceCode',
-        'name': 'name'
+        'name': 'name',
+        'private': 'private'
     }
 
     def __init__(self,
                  can_download_source_code: 'bool' = None,
-                 name: 'str' = None):  # noqa: E501
+                 name: 'str' = None,
+                 private: 'bool' = None):  # noqa: E501
         """ProjectIdAppsv2Body - a model defined in Swagger"""  # noqa: E501
         self._can_download_source_code = None
         self._name = None
+        self._private = None
         self.discriminator = None
         if can_download_source_code is not None:
             self.can_download_source_code = can_download_source_code
         if name is not None:
             self.name = name
+        if private is not None:
+            self.private = private
 
     @property
     def can_download_source_code(self) -> 'bool':
         """Gets the can_download_source_code of this ProjectIdAppsv2Body.  # noqa: E501
 
 
         :return: The can_download_source_code of this ProjectIdAppsv2Body.  # noqa: E501
@@ -97,14 +106,35 @@
 
         :param name: The name of this ProjectIdAppsv2Body.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
+    @property
+    def private(self) -> 'bool':
+        """Gets the private of this ProjectIdAppsv2Body.  # noqa: E501
+
+
+        :return: The private of this ProjectIdAppsv2Body.  # noqa: E501
+        :rtype: bool
+        """
+        return self._private
+
+    @private.setter
+    def private(self, private: 'bool'):
+        """Sets the private of this ProjectIdAppsv2Body.
+
+
+        :param private: The private of this ProjectIdAppsv2Body.  # noqa: E501
+        :type: bool
+        """
+
+        self._private = private
+
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_getapp_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_getapp_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_memberships_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_memberships_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_models_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class ProjectIdModelsBody(object):
+class V1Model(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -46,54 +46,58 @@
         'description': 'str',
         'downloads': 'str',
         'id': 'str',
         'license': 'str',
         'metadata': 'dict(str, str)',
         'name': 'str',
         'private': 'bool',
+        'project_id': 'str',
         'tags': 'list[str]',
         'updated_at': 'datetime'
     }
 
     attribute_map = {
         'categories': 'categories',
         'created_at': 'createdAt',
         'description': 'description',
         'downloads': 'downloads',
         'id': 'id',
         'license': 'license',
         'metadata': 'metadata',
         'name': 'name',
         'private': 'private',
+        'project_id': 'projectId',
         'tags': 'tags',
         'updated_at': 'updatedAt'
     }
 
     def __init__(self,
                  categories: 'list[str]' = None,
                  created_at: 'datetime' = None,
                  description: 'str' = None,
                  downloads: 'str' = None,
                  id: 'str' = None,
                  license: 'str' = None,
                  metadata: 'dict(str, str)' = None,
                  name: 'str' = None,
                  private: 'bool' = None,
+                 project_id: 'str' = None,
                  tags: 'list[str]' = None,
                  updated_at: 'datetime' = None):  # noqa: E501
-        """ProjectIdModelsBody - a model defined in Swagger"""  # noqa: E501
+        """V1Model - a model defined in Swagger"""  # noqa: E501
         self._categories = None
         self._created_at = None
         self._description = None
         self._downloads = None
         self._id = None
         self._license = None
         self._metadata = None
         self._name = None
         self._private = None
+        self._project_id = None
         self._tags = None
         self._updated_at = None
         self.discriminator = None
         if categories is not None:
             self.categories = categories
         if created_at is not None:
             self.created_at = created_at
@@ -107,245 +111,268 @@
             self.license = license
         if metadata is not None:
             self.metadata = metadata
         if name is not None:
             self.name = name
         if private is not None:
             self.private = private
+        if project_id is not None:
+            self.project_id = project_id
         if tags is not None:
             self.tags = tags
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
     def categories(self) -> 'list[str]':
-        """Gets the categories of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the categories of this V1Model.  # noqa: E501
 
 
-        :return: The categories of this ProjectIdModelsBody.  # noqa: E501
+        :return: The categories of this V1Model.  # noqa: E501
         :rtype: list[str]
         """
         return self._categories
 
     @categories.setter
     def categories(self, categories: 'list[str]'):
-        """Sets the categories of this ProjectIdModelsBody.
+        """Sets the categories of this V1Model.
 
 
-        :param categories: The categories of this ProjectIdModelsBody.  # noqa: E501
+        :param categories: The categories of this V1Model.  # noqa: E501
         :type: list[str]
         """
 
         self._categories = categories
 
     @property
     def created_at(self) -> 'datetime':
-        """Gets the created_at of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the created_at of this V1Model.  # noqa: E501
 
 
-        :return: The created_at of this ProjectIdModelsBody.  # noqa: E501
+        :return: The created_at of this V1Model.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at: 'datetime'):
-        """Sets the created_at of this ProjectIdModelsBody.
+        """Sets the created_at of this V1Model.
 
 
-        :param created_at: The created_at of this ProjectIdModelsBody.  # noqa: E501
+        :param created_at: The created_at of this V1Model.  # noqa: E501
         :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def description(self) -> 'str':
-        """Gets the description of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the description of this V1Model.  # noqa: E501
 
 
-        :return: The description of this ProjectIdModelsBody.  # noqa: E501
+        :return: The description of this V1Model.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description: 'str'):
-        """Sets the description of this ProjectIdModelsBody.
+        """Sets the description of this V1Model.
 
 
-        :param description: The description of this ProjectIdModelsBody.  # noqa: E501
+        :param description: The description of this V1Model.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def downloads(self) -> 'str':
-        """Gets the downloads of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the downloads of this V1Model.  # noqa: E501
 
 
-        :return: The downloads of this ProjectIdModelsBody.  # noqa: E501
+        :return: The downloads of this V1Model.  # noqa: E501
         :rtype: str
         """
         return self._downloads
 
     @downloads.setter
     def downloads(self, downloads: 'str'):
-        """Sets the downloads of this ProjectIdModelsBody.
+        """Sets the downloads of this V1Model.
 
 
-        :param downloads: The downloads of this ProjectIdModelsBody.  # noqa: E501
+        :param downloads: The downloads of this V1Model.  # noqa: E501
         :type: str
         """
 
         self._downloads = downloads
 
     @property
     def id(self) -> 'str':
-        """Gets the id of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the id of this V1Model.  # noqa: E501
 
 
-        :return: The id of this ProjectIdModelsBody.  # noqa: E501
+        :return: The id of this V1Model.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id: 'str'):
-        """Sets the id of this ProjectIdModelsBody.
+        """Sets the id of this V1Model.
 
 
-        :param id: The id of this ProjectIdModelsBody.  # noqa: E501
+        :param id: The id of this V1Model.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
     def license(self) -> 'str':
-        """Gets the license of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the license of this V1Model.  # noqa: E501
 
 
-        :return: The license of this ProjectIdModelsBody.  # noqa: E501
+        :return: The license of this V1Model.  # noqa: E501
         :rtype: str
         """
         return self._license
 
     @license.setter
     def license(self, license: 'str'):
-        """Sets the license of this ProjectIdModelsBody.
+        """Sets the license of this V1Model.
 
 
-        :param license: The license of this ProjectIdModelsBody.  # noqa: E501
+        :param license: The license of this V1Model.  # noqa: E501
         :type: str
         """
 
         self._license = license
 
     @property
     def metadata(self) -> 'dict(str, str)':
-        """Gets the metadata of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the metadata of this V1Model.  # noqa: E501
 
 
-        :return: The metadata of this ProjectIdModelsBody.  # noqa: E501
+        :return: The metadata of this V1Model.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata: 'dict(str, str)'):
-        """Sets the metadata of this ProjectIdModelsBody.
+        """Sets the metadata of this V1Model.
 
 
-        :param metadata: The metadata of this ProjectIdModelsBody.  # noqa: E501
+        :param metadata: The metadata of this V1Model.  # noqa: E501
         :type: dict(str, str)
         """
 
         self._metadata = metadata
 
     @property
     def name(self) -> 'str':
-        """Gets the name of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the name of this V1Model.  # noqa: E501
 
 
-        :return: The name of this ProjectIdModelsBody.  # noqa: E501
+        :return: The name of this V1Model.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name: 'str'):
-        """Sets the name of this ProjectIdModelsBody.
+        """Sets the name of this V1Model.
 
 
-        :param name: The name of this ProjectIdModelsBody.  # noqa: E501
+        :param name: The name of this V1Model.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def private(self) -> 'bool':
-        """Gets the private of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the private of this V1Model.  # noqa: E501
 
 
-        :return: The private of this ProjectIdModelsBody.  # noqa: E501
+        :return: The private of this V1Model.  # noqa: E501
         :rtype: bool
         """
         return self._private
 
     @private.setter
     def private(self, private: 'bool'):
-        """Sets the private of this ProjectIdModelsBody.
+        """Sets the private of this V1Model.
 
 
-        :param private: The private of this ProjectIdModelsBody.  # noqa: E501
+        :param private: The private of this V1Model.  # noqa: E501
         :type: bool
         """
 
         self._private = private
 
     @property
+    def project_id(self) -> 'str':
+        """Gets the project_id of this V1Model.  # noqa: E501
+
+
+        :return: The project_id of this V1Model.  # noqa: E501
+        :rtype: str
+        """
+        return self._project_id
+
+    @project_id.setter
+    def project_id(self, project_id: 'str'):
+        """Sets the project_id of this V1Model.
+
+
+        :param project_id: The project_id of this V1Model.  # noqa: E501
+        :type: str
+        """
+
+        self._project_id = project_id
+
+    @property
     def tags(self) -> 'list[str]':
-        """Gets the tags of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the tags of this V1Model.  # noqa: E501
 
 
-        :return: The tags of this ProjectIdModelsBody.  # noqa: E501
+        :return: The tags of this V1Model.  # noqa: E501
         :rtype: list[str]
         """
         return self._tags
 
     @tags.setter
     def tags(self, tags: 'list[str]'):
-        """Sets the tags of this ProjectIdModelsBody.
+        """Sets the tags of this V1Model.
 
 
-        :param tags: The tags of this ProjectIdModelsBody.  # noqa: E501
+        :param tags: The tags of this V1Model.  # noqa: E501
         :type: list[str]
         """
 
         self._tags = tags
 
     @property
     def updated_at(self) -> 'datetime':
-        """Gets the updated_at of this ProjectIdModelsBody.  # noqa: E501
+        """Gets the updated_at of this V1Model.  # noqa: E501
 
 
-        :return: The updated_at of this ProjectIdModelsBody.  # noqa: E501
+        :return: The updated_at of this V1Model.  # noqa: E501
         :rtype: datetime
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at: 'datetime'):
-        """Sets the updated_at of this ProjectIdModelsBody.
+        """Sets the updated_at of this V1Model.
 
 
-        :param updated_at: The updated_at of this ProjectIdModelsBody.  # noqa: E501
+        :param updated_at: The updated_at of this V1Model.  # noqa: E501
         :type: datetime
         """
 
         self._updated_at = updated_at
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
@@ -363,31 +390,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(ProjectIdModelsBody, dict):
+        if issubclass(V1Model, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'ProjectIdModelsBody') -> bool:
+    def __eq__(self, other: 'V1Model') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectIdModelsBody):
+        if not isinstance(other, V1Model):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'ProjectIdModelsBody') -> bool:
+    def __ne__(self, other: 'V1Model') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_projectclustersbindings_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_projectclustersbindings_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/project_id_secrets_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/project_id_secrets_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/projects_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/projects_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/projects_project_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/projects_project_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/protobuf_any.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/rpc_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/secrets_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/secrets_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/spec_lightningapp_instance_id_works_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/spec_lightningapp_instance_id_works_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/user_id_membershiprolebindings_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/user_id_membershiprolebindings_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_aws_cluster_driver_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_aws_cluster_driver_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_azure_cluster_driver_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_azure_cluster_driver_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_azure_cluster_driver_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_azure_cluster_driver_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_build_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_build_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_driver.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_driver_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_driver_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_log_service.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_log_service.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_performance_profile.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_performance_profile.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_state.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_state.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_cluster_type.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_cluster_type.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_compute_config.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_compute_config.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_container_resources.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_container_resources.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_cluster_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_cluster_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_cluster_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_cluster_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_project_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_project_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_create_ssh_public_key_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_create_ssh_public_key_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_cluster_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_cluster_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_instance_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_instance_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_release_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_release_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningapp_v2_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningapp_v2_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_lightningwork_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_lightningwork_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_membership_role_binding_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_membership_role_binding_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_model_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_model_version_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_model_version_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_cluster_binding_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_cluster_binding_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_membership_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_membership_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_project_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_role_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_role_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_secret_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_secret_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_delete_ssh_public_key_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_delete_ssh_public_key_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_dependency_cache_state.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_dependency_cache_state.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_dependency_file_info.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_dependency_file_info.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_download_model_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_lightningapp_source_code_download_url_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,57 +24,57 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1DownloadModelResponse(object):
+class V1GetLightningappSourceCodeDownloadUrlResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'download_url': 'str'}
+    swagger_types = {'url': 'str'}
 
-    attribute_map = {'download_url': 'downloadUrl'}
+    attribute_map = {'url': 'url'}
 
-    def __init__(self, download_url: 'str' = None):  # noqa: E501
-        """V1DownloadModelResponse - a model defined in Swagger"""  # noqa: E501
-        self._download_url = None
+    def __init__(self, url: 'str' = None):  # noqa: E501
+        """V1GetLightningappSourceCodeDownloadUrlResponse - a model defined in Swagger"""  # noqa: E501
+        self._url = None
         self.discriminator = None
-        if download_url is not None:
-            self.download_url = download_url
+        if url is not None:
+            self.url = url
 
     @property
-    def download_url(self) -> 'str':
-        """Gets the download_url of this V1DownloadModelResponse.  # noqa: E501
+    def url(self) -> 'str':
+        """Gets the url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
 
 
-        :return: The download_url of this V1DownloadModelResponse.  # noqa: E501
+        :return: The url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
         :rtype: str
         """
-        return self._download_url
+        return self._url
 
-    @download_url.setter
-    def download_url(self, download_url: 'str'):
-        """Sets the download_url of this V1DownloadModelResponse.
+    @url.setter
+    def url(self, url: 'str'):
+        """Sets the url of this V1GetLightningappSourceCodeDownloadUrlResponse.
 
 
-        :param download_url: The download_url of this V1DownloadModelResponse.  # noqa: E501
+        :param url: The url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
         :type: str
         """
 
-        self._download_url = download_url
+        self._url = url
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -88,31 +88,36 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1DownloadModelResponse, dict):
+        if issubclass(V1GetLightningappSourceCodeDownloadUrlResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1DownloadModelResponse') -> bool:
+    def __eq__(
+            self,
+            other: 'V1GetLightningappSourceCodeDownloadUrlResponse') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1DownloadModelResponse):
+        if not isinstance(other,
+                          V1GetLightningappSourceCodeDownloadUrlResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1DownloadModelResponse') -> bool:
+    def __ne__(
+            self,
+            other: 'V1GetLightningappSourceCodeDownloadUrlResponse') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_state.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_state.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_state_reason.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_state_reason.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_drive_type_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_drive_type_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_eks_custer_driver_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_eks_custer_driver_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_env_var.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_env_var.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_external_kubeconfig.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_external_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_flowserver.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_flowserver.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_gallery_app.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_gallery_app.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_gallery_component.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_gallery_component.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_cluster_health_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_cluster_health_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_cluster_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_cluster_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_lightningapp_source_code_download_url_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningwork_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,57 +24,59 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1GetLightningappSourceCodeDownloadUrlResponse(object):
+class V1ListLightningworkResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'url': 'str'}
+    swagger_types = {'lightningworks': 'list[Externalv1Lightningwork]'}
 
-    attribute_map = {'url': 'url'}
+    attribute_map = {'lightningworks': 'lightningworks'}
 
-    def __init__(self, url: 'str' = None):  # noqa: E501
-        """V1GetLightningappSourceCodeDownloadUrlResponse - a model defined in Swagger"""  # noqa: E501
-        self._url = None
+    def __init__(self,
+                 lightningworks: 'list[Externalv1Lightningwork]' = None
+                 ):  # noqa: E501
+        """V1ListLightningworkResponse - a model defined in Swagger"""  # noqa: E501
+        self._lightningworks = None
         self.discriminator = None
-        if url is not None:
-            self.url = url
+        if lightningworks is not None:
+            self.lightningworks = lightningworks
 
     @property
-    def url(self) -> 'str':
-        """Gets the url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
+    def lightningworks(self) -> 'list[Externalv1Lightningwork]':
+        """Gets the lightningworks of this V1ListLightningworkResponse.  # noqa: E501
 
 
-        :return: The url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
-        :rtype: str
+        :return: The lightningworks of this V1ListLightningworkResponse.  # noqa: E501
+        :rtype: list[Externalv1Lightningwork]
         """
-        return self._url
+        return self._lightningworks
 
-    @url.setter
-    def url(self, url: 'str'):
-        """Sets the url of this V1GetLightningappSourceCodeDownloadUrlResponse.
+    @lightningworks.setter
+    def lightningworks(self, lightningworks: 'list[Externalv1Lightningwork]'):
+        """Sets the lightningworks of this V1ListLightningworkResponse.
 
 
-        :param url: The url of this V1GetLightningappSourceCodeDownloadUrlResponse.  # noqa: E501
-        :type: str
+        :param lightningworks: The lightningworks of this V1ListLightningworkResponse.  # noqa: E501
+        :type: list[Externalv1Lightningwork]
         """
 
-        self._url = url
+        self._lightningworks = lightningworks
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -88,36 +90,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1GetLightningappSourceCodeDownloadUrlResponse, dict):
+        if issubclass(V1ListLightningworkResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(
-            self,
-            other: 'V1GetLightningappSourceCodeDownloadUrlResponse') -> bool:
+    def __eq__(self, other: 'V1ListLightningworkResponse') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other,
-                          V1GetLightningappSourceCodeDownloadUrlResponse):
+        if not isinstance(other, V1ListLightningworkResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(
-            self,
-            other: 'V1GetLightningappSourceCodeDownloadUrlResponse') -> bool:
+    def __ne__(self, other: 'V1ListLightningworkResponse') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_get_user_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_get_user_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_image_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_image_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_instance_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_instance_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_instance_type.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_instance_type.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_kubernetes_cluster_driver.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_kubernetes_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_kubernetes_cluster_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_kubernetes_cluster_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_app_user.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_app_user.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_auth.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_auth.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_basic_auth.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_basic_auth.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightning_o_auth_auth.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightning_o_auth_auth.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_artifact.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_artifact.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_event.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_event.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         'dependency_cache_key': 'str',
         'desired_state': 'V1LightningappInstanceState',
         'enable_app_server': 'bool',
         'env': 'list[V1EnvVar]',
         'flow_servers': 'list[V1Flowserver]',
         'image_spec': 'V1ImageSpec',
         'pause_automation': 'bool',
+        'private': 'bool',
         'queue_server_type': 'V1QueueServerType',
         'redis_token': 'str',
         'release_id': 'str',
         'restart_policy': 'V1LightningappRestartPolicy',
         'source_code_url': 'str',
         'user_id': 'str',
         'user_requested_flow_compute_config':
@@ -75,14 +76,15 @@
         'dependency_cache_key': 'dependencyCacheKey',
         'desired_state': 'desiredState',
         'enable_app_server': 'enableAppServer',
         'env': 'env',
         'flow_servers': 'flowServers',
         'image_spec': 'imageSpec',
         'pause_automation': 'pauseAutomation',
+        'private': 'private',
         'queue_server_type': 'queueServerType',
         'redis_token': 'redisToken',
         'release_id': 'releaseId',
         'restart_policy': 'restartPolicy',
         'source_code_url': 'sourceCodeUrl',
         'user_id': 'userId',
         'user_requested_flow_compute_config': 'userRequestedFlowComputeConfig',
@@ -99,14 +101,15 @@
                  dependency_cache_key: 'str' = None,
                  desired_state: 'V1LightningappInstanceState' = None,
                  enable_app_server: 'bool' = None,
                  env: 'list[V1EnvVar]' = None,
                  flow_servers: 'list[V1Flowserver]' = None,
                  image_spec: 'V1ImageSpec' = None,
                  pause_automation: 'bool' = None,
+                 private: 'bool' = None,
                  queue_server_type: 'V1QueueServerType' = None,
                  redis_token: 'str' = None,
                  release_id: 'str' = None,
                  restart_policy: 'V1LightningappRestartPolicy' = None,
                  source_code_url: 'str' = None,
                  user_id: 'str' = None,
                  user_requested_flow_compute_config:
@@ -122,14 +125,15 @@
         self._dependency_cache_key = None
         self._desired_state = None
         self._enable_app_server = None
         self._env = None
         self._flow_servers = None
         self._image_spec = None
         self._pause_automation = None
+        self._private = None
         self._queue_server_type = None
         self._redis_token = None
         self._release_id = None
         self._restart_policy = None
         self._source_code_url = None
         self._user_id = None
         self._user_requested_flow_compute_config = None
@@ -157,14 +161,16 @@
             self.env = env
         if flow_servers is not None:
             self.flow_servers = flow_servers
         if image_spec is not None:
             self.image_spec = image_spec
         if pause_automation is not None:
             self.pause_automation = pause_automation
+        if private is not None:
+            self.private = private
         if queue_server_type is not None:
             self.queue_server_type = queue_server_type
         if redis_token is not None:
             self.redis_token = redis_token
         if release_id is not None:
             self.release_id = release_id
         if restart_policy is not None:
@@ -448,14 +454,35 @@
         :param pause_automation: The pause_automation of this V1LightningappInstanceSpec.  # noqa: E501
         :type: bool
         """
 
         self._pause_automation = pause_automation
 
     @property
+    def private(self) -> 'bool':
+        """Gets the private of this V1LightningappInstanceSpec.  # noqa: E501
+
+
+        :return: The private of this V1LightningappInstanceSpec.  # noqa: E501
+        :rtype: bool
+        """
+        return self._private
+
+    @private.setter
+    def private(self, private: 'bool'):
+        """Sets the private of this V1LightningappInstanceSpec.
+
+
+        :param private: The private of this V1LightningappInstanceSpec.  # noqa: E501
+        :type: bool
+        """
+
+        self._private = private
+
+    @property
     def queue_server_type(self) -> 'V1QueueServerType':
         """Gets the queue_server_type of this V1LightningappInstanceSpec.  # noqa: E501
 
 
         :return: The queue_server_type of this V1LightningappInstanceSpec.  # noqa: E501
         :rtype: V1QueueServerType
         """
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_state.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_state.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_instance_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_instance_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_release.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_release.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_restart_policy.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_restart_policy.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningapp_v2.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningapp_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,50 +41,56 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'can_download_source_code': 'bool',
         'created_at': 'datetime',
         'id': 'str',
         'name': 'str',
+        'private': 'bool',
         'project_id': 'str',
         'updated_at': 'datetime'
     }
 
     attribute_map = {
         'can_download_source_code': 'canDownloadSourceCode',
         'created_at': 'createdAt',
         'id': 'id',
         'name': 'name',
+        'private': 'private',
         'project_id': 'projectId',
         'updated_at': 'updatedAt'
     }
 
     def __init__(self,
                  can_download_source_code: 'bool' = None,
                  created_at: 'datetime' = None,
                  id: 'str' = None,
                  name: 'str' = None,
+                 private: 'bool' = None,
                  project_id: 'str' = None,
                  updated_at: 'datetime' = None):  # noqa: E501
         """V1LightningappV2 - a model defined in Swagger"""  # noqa: E501
         self._can_download_source_code = None
         self._created_at = None
         self._id = None
         self._name = None
+        self._private = None
         self._project_id = None
         self._updated_at = None
         self.discriminator = None
         if can_download_source_code is not None:
             self.can_download_source_code = can_download_source_code
         if created_at is not None:
             self.created_at = created_at
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
+        if private is not None:
+            self.private = private
         if project_id is not None:
             self.project_id = project_id
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
     def can_download_source_code(self) -> 'bool':
@@ -167,14 +173,35 @@
         :param name: The name of this V1LightningappV2.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
+    def private(self) -> 'bool':
+        """Gets the private of this V1LightningappV2.  # noqa: E501
+
+
+        :return: The private of this V1LightningappV2.  # noqa: E501
+        :rtype: bool
+        """
+        return self._private
+
+    @private.setter
+    def private(self, private: 'bool'):
+        """Sets the private of this V1LightningappV2.
+
+
+        :param private: The private of this V1LightningappV2.  # noqa: E501
+        :type: bool
+        """
+
+        self._private = private
+
+    @property
     def project_id(self) -> 'str':
         """Gets the project_id of this V1LightningappV2.  # noqa: E501
 
 
         :return: The project_id of this V1LightningappV2.  # noqa: E501
         :rtype: str
         """
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_cost.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_cost.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_drives.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_drives.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_spec.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_spec.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_state.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_state.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_lightningwork_status_reason.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_lightningwork_status_reason.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_cluster_instance_types_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_cluster_instance_types_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_clusters_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_clusters_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_gallery_components_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_gallery_components_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_gallery_lightningapps_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_gallery_lightningapps_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instance_artifacts_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instance_artifacts_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instance_events_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instance_events_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapp_instances_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapp_instances_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningapps_v2_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_lightningapps_v2_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_lightningwork_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_project_cluster_bindings_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,59 +24,59 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1ListLightningworkResponse(object):
+class V1ListProjectClusterBindingsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'lightningworks': 'list[Externalv1Lightningwork]'}
+    swagger_types = {'clusters': 'list[V1ProjectClusterBinding]'}
 
-    attribute_map = {'lightningworks': 'lightningworks'}
+    attribute_map = {'clusters': 'clusters'}
 
-    def __init__(self,
-                 lightningworks: 'list[Externalv1Lightningwork]' = None
-                 ):  # noqa: E501
-        """V1ListLightningworkResponse - a model defined in Swagger"""  # noqa: E501
-        self._lightningworks = None
+    def __init__(
+            self,
+            clusters: 'list[V1ProjectClusterBinding]' = None):  # noqa: E501
+        """V1ListProjectClusterBindingsResponse - a model defined in Swagger"""  # noqa: E501
+        self._clusters = None
         self.discriminator = None
-        if lightningworks is not None:
-            self.lightningworks = lightningworks
+        if clusters is not None:
+            self.clusters = clusters
 
     @property
-    def lightningworks(self) -> 'list[Externalv1Lightningwork]':
-        """Gets the lightningworks of this V1ListLightningworkResponse.  # noqa: E501
+    def clusters(self) -> 'list[V1ProjectClusterBinding]':
+        """Gets the clusters of this V1ListProjectClusterBindingsResponse.  # noqa: E501
 
 
-        :return: The lightningworks of this V1ListLightningworkResponse.  # noqa: E501
-        :rtype: list[Externalv1Lightningwork]
+        :return: The clusters of this V1ListProjectClusterBindingsResponse.  # noqa: E501
+        :rtype: list[V1ProjectClusterBinding]
         """
-        return self._lightningworks
+        return self._clusters
 
-    @lightningworks.setter
-    def lightningworks(self, lightningworks: 'list[Externalv1Lightningwork]'):
-        """Sets the lightningworks of this V1ListLightningworkResponse.
+    @clusters.setter
+    def clusters(self, clusters: 'list[V1ProjectClusterBinding]'):
+        """Sets the clusters of this V1ListProjectClusterBindingsResponse.
 
 
-        :param lightningworks: The lightningworks of this V1ListLightningworkResponse.  # noqa: E501
-        :type: list[Externalv1Lightningwork]
+        :param clusters: The clusters of this V1ListProjectClusterBindingsResponse.  # noqa: E501
+        :type: list[V1ProjectClusterBinding]
         """
 
-        self._lightningworks = lightningworks
+        self._clusters = clusters
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -90,31 +90,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1ListLightningworkResponse, dict):
+        if issubclass(V1ListProjectClusterBindingsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1ListLightningworkResponse') -> bool:
+    def __eq__(self, other: 'V1ListProjectClusterBindingsResponse') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1ListLightningworkResponse):
+        if not isinstance(other, V1ListProjectClusterBindingsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1ListLightningworkResponse') -> bool:
+    def __ne__(self, other: 'V1ListProjectClusterBindingsResponse') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_membership_role_binding_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_membership_role_binding_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_memberships_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_memberships_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_model_versions_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_model_versions_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_models_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_models_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_project_memberships_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_project_memberships_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_roles_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_roles_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_secrets_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_secrets_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_list_ssh_public_keys_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_list_ssh_public_keys_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_login_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_login_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_login_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_login_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_logout_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_logout_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_logout_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_logout_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_membership.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_membership.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_membership_role_binding.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_membership_role_binding.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_metadata.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_metadata.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_model.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_project.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,355 +24,220 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1Model(object):
+class V1Project(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'categories': 'list[str]',
         'created_at': 'datetime',
         'description': 'str',
-        'downloads': 'str',
         'id': 'str',
-        'license': 'str',
-        'metadata': 'dict(str, str)',
         'name': 'str',
         'private': 'bool',
-        'project_id': 'str',
-        'tags': 'list[str]',
+        'quotas': 'V1Quotas',
         'updated_at': 'datetime'
     }
 
     attribute_map = {
-        'categories': 'categories',
         'created_at': 'createdAt',
         'description': 'description',
-        'downloads': 'downloads',
         'id': 'id',
-        'license': 'license',
-        'metadata': 'metadata',
         'name': 'name',
         'private': 'private',
-        'project_id': 'projectId',
-        'tags': 'tags',
+        'quotas': 'quotas',
         'updated_at': 'updatedAt'
     }
 
     def __init__(self,
-                 categories: 'list[str]' = None,
                  created_at: 'datetime' = None,
                  description: 'str' = None,
-                 downloads: 'str' = None,
                  id: 'str' = None,
-                 license: 'str' = None,
-                 metadata: 'dict(str, str)' = None,
                  name: 'str' = None,
                  private: 'bool' = None,
-                 project_id: 'str' = None,
-                 tags: 'list[str]' = None,
+                 quotas: 'V1Quotas' = None,
                  updated_at: 'datetime' = None):  # noqa: E501
-        """V1Model - a model defined in Swagger"""  # noqa: E501
-        self._categories = None
+        """V1Project - a model defined in Swagger"""  # noqa: E501
         self._created_at = None
         self._description = None
-        self._downloads = None
         self._id = None
-        self._license = None
-        self._metadata = None
         self._name = None
         self._private = None
-        self._project_id = None
-        self._tags = None
+        self._quotas = None
         self._updated_at = None
         self.discriminator = None
-        if categories is not None:
-            self.categories = categories
         if created_at is not None:
             self.created_at = created_at
         if description is not None:
             self.description = description
-        if downloads is not None:
-            self.downloads = downloads
         if id is not None:
             self.id = id
-        if license is not None:
-            self.license = license
-        if metadata is not None:
-            self.metadata = metadata
         if name is not None:
             self.name = name
         if private is not None:
             self.private = private
-        if project_id is not None:
-            self.project_id = project_id
-        if tags is not None:
-            self.tags = tags
+        if quotas is not None:
+            self.quotas = quotas
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
-    def categories(self) -> 'list[str]':
-        """Gets the categories of this V1Model.  # noqa: E501
-
-
-        :return: The categories of this V1Model.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._categories
-
-    @categories.setter
-    def categories(self, categories: 'list[str]'):
-        """Sets the categories of this V1Model.
-
-
-        :param categories: The categories of this V1Model.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._categories = categories
-
-    @property
     def created_at(self) -> 'datetime':
-        """Gets the created_at of this V1Model.  # noqa: E501
+        """Gets the created_at of this V1Project.  # noqa: E501
 
 
-        :return: The created_at of this V1Model.  # noqa: E501
+        :return: The created_at of this V1Project.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at: 'datetime'):
-        """Sets the created_at of this V1Model.
+        """Sets the created_at of this V1Project.
 
 
-        :param created_at: The created_at of this V1Model.  # noqa: E501
+        :param created_at: The created_at of this V1Project.  # noqa: E501
         :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def description(self) -> 'str':
-        """Gets the description of this V1Model.  # noqa: E501
+        """Gets the description of this V1Project.  # noqa: E501
 
 
-        :return: The description of this V1Model.  # noqa: E501
+        :return: The description of this V1Project.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description: 'str'):
-        """Sets the description of this V1Model.
+        """Sets the description of this V1Project.
 
 
-        :param description: The description of this V1Model.  # noqa: E501
+        :param description: The description of this V1Project.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
-    def downloads(self) -> 'str':
-        """Gets the downloads of this V1Model.  # noqa: E501
-
-
-        :return: The downloads of this V1Model.  # noqa: E501
-        :rtype: str
-        """
-        return self._downloads
-
-    @downloads.setter
-    def downloads(self, downloads: 'str'):
-        """Sets the downloads of this V1Model.
-
-
-        :param downloads: The downloads of this V1Model.  # noqa: E501
-        :type: str
-        """
-
-        self._downloads = downloads
-
-    @property
     def id(self) -> 'str':
-        """Gets the id of this V1Model.  # noqa: E501
+        """Gets the id of this V1Project.  # noqa: E501
 
 
-        :return: The id of this V1Model.  # noqa: E501
+        :return: The id of this V1Project.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id: 'str'):
-        """Sets the id of this V1Model.
+        """Sets the id of this V1Project.
 
 
-        :param id: The id of this V1Model.  # noqa: E501
+        :param id: The id of this V1Project.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
-    def license(self) -> 'str':
-        """Gets the license of this V1Model.  # noqa: E501
-
-
-        :return: The license of this V1Model.  # noqa: E501
-        :rtype: str
-        """
-        return self._license
-
-    @license.setter
-    def license(self, license: 'str'):
-        """Sets the license of this V1Model.
-
-
-        :param license: The license of this V1Model.  # noqa: E501
-        :type: str
-        """
-
-        self._license = license
-
-    @property
-    def metadata(self) -> 'dict(str, str)':
-        """Gets the metadata of this V1Model.  # noqa: E501
-
-
-        :return: The metadata of this V1Model.  # noqa: E501
-        :rtype: dict(str, str)
-        """
-        return self._metadata
-
-    @metadata.setter
-    def metadata(self, metadata: 'dict(str, str)'):
-        """Sets the metadata of this V1Model.
-
-
-        :param metadata: The metadata of this V1Model.  # noqa: E501
-        :type: dict(str, str)
-        """
-
-        self._metadata = metadata
-
-    @property
     def name(self) -> 'str':
-        """Gets the name of this V1Model.  # noqa: E501
+        """Gets the name of this V1Project.  # noqa: E501
 
 
-        :return: The name of this V1Model.  # noqa: E501
+        :return: The name of this V1Project.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name: 'str'):
-        """Sets the name of this V1Model.
+        """Sets the name of this V1Project.
 
 
-        :param name: The name of this V1Model.  # noqa: E501
+        :param name: The name of this V1Project.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def private(self) -> 'bool':
-        """Gets the private of this V1Model.  # noqa: E501
+        """Gets the private of this V1Project.  # noqa: E501
 
 
-        :return: The private of this V1Model.  # noqa: E501
+        :return: The private of this V1Project.  # noqa: E501
         :rtype: bool
         """
         return self._private
 
     @private.setter
     def private(self, private: 'bool'):
-        """Sets the private of this V1Model.
+        """Sets the private of this V1Project.
 
 
-        :param private: The private of this V1Model.  # noqa: E501
+        :param private: The private of this V1Project.  # noqa: E501
         :type: bool
         """
 
         self._private = private
 
     @property
-    def project_id(self) -> 'str':
-        """Gets the project_id of this V1Model.  # noqa: E501
-
-
-        :return: The project_id of this V1Model.  # noqa: E501
-        :rtype: str
-        """
-        return self._project_id
-
-    @project_id.setter
-    def project_id(self, project_id: 'str'):
-        """Sets the project_id of this V1Model.
-
-
-        :param project_id: The project_id of this V1Model.  # noqa: E501
-        :type: str
-        """
-
-        self._project_id = project_id
-
-    @property
-    def tags(self) -> 'list[str]':
-        """Gets the tags of this V1Model.  # noqa: E501
+    def quotas(self) -> 'V1Quotas':
+        """Gets the quotas of this V1Project.  # noqa: E501
 
 
-        :return: The tags of this V1Model.  # noqa: E501
-        :rtype: list[str]
+        :return: The quotas of this V1Project.  # noqa: E501
+        :rtype: V1Quotas
         """
-        return self._tags
+        return self._quotas
 
-    @tags.setter
-    def tags(self, tags: 'list[str]'):
-        """Sets the tags of this V1Model.
+    @quotas.setter
+    def quotas(self, quotas: 'V1Quotas'):
+        """Sets the quotas of this V1Project.
 
 
-        :param tags: The tags of this V1Model.  # noqa: E501
-        :type: list[str]
+        :param quotas: The quotas of this V1Project.  # noqa: E501
+        :type: V1Quotas
         """
 
-        self._tags = tags
+        self._quotas = quotas
 
     @property
     def updated_at(self) -> 'datetime':
-        """Gets the updated_at of this V1Model.  # noqa: E501
+        """Gets the updated_at of this V1Project.  # noqa: E501
 
 
-        :return: The updated_at of this V1Model.  # noqa: E501
+        :return: The updated_at of this V1Project.  # noqa: E501
         :rtype: datetime
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at: 'datetime'):
-        """Sets the updated_at of this V1Model.
+        """Sets the updated_at of this V1Project.
 
 
-        :param updated_at: The updated_at of this V1Model.  # noqa: E501
+        :param updated_at: The updated_at of this V1Project.  # noqa: E501
         :type: datetime
         """
 
         self._updated_at = updated_at
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
@@ -390,31 +255,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1Model, dict):
+        if issubclass(V1Project, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1Model') -> bool:
+    def __eq__(self, other: 'V1Project') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1Model):
+        if not isinstance(other, V1Project):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1Model') -> bool:
+    def __ne__(self, other: 'V1Project') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_network_config.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_network_config.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_package_manager.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_package_manager.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_project.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_ssh_public_key.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,224 +24,197 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1Project(object):
+class V1SSHPublicKey(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'created_at': 'datetime',
-        'description': 'str',
         'id': 'str',
+        'last_used_at': 'datetime',
         'name': 'str',
-        'private': 'bool',
-        'quotas': 'V1Quotas',
-        'updated_at': 'datetime'
+        'public_key': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
         'created_at': 'createdAt',
-        'description': 'description',
         'id': 'id',
+        'last_used_at': 'lastUsedAt',
         'name': 'name',
-        'private': 'private',
-        'quotas': 'quotas',
-        'updated_at': 'updatedAt'
+        'public_key': 'publicKey',
+        'type': 'type'
     }
 
     def __init__(self,
                  created_at: 'datetime' = None,
-                 description: 'str' = None,
                  id: 'str' = None,
+                 last_used_at: 'datetime' = None,
                  name: 'str' = None,
-                 private: 'bool' = None,
-                 quotas: 'V1Quotas' = None,
-                 updated_at: 'datetime' = None):  # noqa: E501
-        """V1Project - a model defined in Swagger"""  # noqa: E501
+                 public_key: 'str' = None,
+                 type: 'str' = None):  # noqa: E501
+        """V1SSHPublicKey - a model defined in Swagger"""  # noqa: E501
         self._created_at = None
-        self._description = None
         self._id = None
+        self._last_used_at = None
         self._name = None
-        self._private = None
-        self._quotas = None
-        self._updated_at = None
+        self._public_key = None
+        self._type = None
         self.discriminator = None
         if created_at is not None:
             self.created_at = created_at
-        if description is not None:
-            self.description = description
         if id is not None:
             self.id = id
+        if last_used_at is not None:
+            self.last_used_at = last_used_at
         if name is not None:
             self.name = name
-        if private is not None:
-            self.private = private
-        if quotas is not None:
-            self.quotas = quotas
-        if updated_at is not None:
-            self.updated_at = updated_at
+        if public_key is not None:
+            self.public_key = public_key
+        if type is not None:
+            self.type = type
 
     @property
     def created_at(self) -> 'datetime':
-        """Gets the created_at of this V1Project.  # noqa: E501
+        """Gets the created_at of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The created_at of this V1Project.  # noqa: E501
+        :return: The created_at of this V1SSHPublicKey.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at: 'datetime'):
-        """Sets the created_at of this V1Project.
+        """Sets the created_at of this V1SSHPublicKey.
 
 
-        :param created_at: The created_at of this V1Project.  # noqa: E501
+        :param created_at: The created_at of this V1SSHPublicKey.  # noqa: E501
         :type: datetime
         """
 
         self._created_at = created_at
 
     @property
-    def description(self) -> 'str':
-        """Gets the description of this V1Project.  # noqa: E501
+    def id(self) -> 'str':
+        """Gets the id of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The description of this V1Project.  # noqa: E501
+        :return: The id of this V1SSHPublicKey.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._id
 
-    @description.setter
-    def description(self, description: 'str'):
-        """Sets the description of this V1Project.
+    @id.setter
+    def id(self, id: 'str'):
+        """Sets the id of this V1SSHPublicKey.
 
 
-        :param description: The description of this V1Project.  # noqa: E501
+        :param id: The id of this V1SSHPublicKey.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._id = id
 
     @property
-    def id(self) -> 'str':
-        """Gets the id of this V1Project.  # noqa: E501
+    def last_used_at(self) -> 'datetime':
+        """Gets the last_used_at of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The id of this V1Project.  # noqa: E501
-        :rtype: str
+        :return: The last_used_at of this V1SSHPublicKey.  # noqa: E501
+        :rtype: datetime
         """
-        return self._id
+        return self._last_used_at
 
-    @id.setter
-    def id(self, id: 'str'):
-        """Sets the id of this V1Project.
+    @last_used_at.setter
+    def last_used_at(self, last_used_at: 'datetime'):
+        """Sets the last_used_at of this V1SSHPublicKey.
 
 
-        :param id: The id of this V1Project.  # noqa: E501
-        :type: str
+        :param last_used_at: The last_used_at of this V1SSHPublicKey.  # noqa: E501
+        :type: datetime
         """
 
-        self._id = id
+        self._last_used_at = last_used_at
 
     @property
     def name(self) -> 'str':
-        """Gets the name of this V1Project.  # noqa: E501
+        """Gets the name of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The name of this V1Project.  # noqa: E501
+        :return: The name of this V1SSHPublicKey.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name: 'str'):
-        """Sets the name of this V1Project.
+        """Sets the name of this V1SSHPublicKey.
 
 
-        :param name: The name of this V1Project.  # noqa: E501
+        :param name: The name of this V1SSHPublicKey.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
-    def private(self) -> 'bool':
-        """Gets the private of this V1Project.  # noqa: E501
-
-
-        :return: The private of this V1Project.  # noqa: E501
-        :rtype: bool
-        """
-        return self._private
-
-    @private.setter
-    def private(self, private: 'bool'):
-        """Sets the private of this V1Project.
-
-
-        :param private: The private of this V1Project.  # noqa: E501
-        :type: bool
-        """
-
-        self._private = private
-
-    @property
-    def quotas(self) -> 'V1Quotas':
-        """Gets the quotas of this V1Project.  # noqa: E501
+    def public_key(self) -> 'str':
+        """Gets the public_key of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The quotas of this V1Project.  # noqa: E501
-        :rtype: V1Quotas
+        :return: The public_key of this V1SSHPublicKey.  # noqa: E501
+        :rtype: str
         """
-        return self._quotas
+        return self._public_key
 
-    @quotas.setter
-    def quotas(self, quotas: 'V1Quotas'):
-        """Sets the quotas of this V1Project.
+    @public_key.setter
+    def public_key(self, public_key: 'str'):
+        """Sets the public_key of this V1SSHPublicKey.
 
 
-        :param quotas: The quotas of this V1Project.  # noqa: E501
-        :type: V1Quotas
+        :param public_key: The public_key of this V1SSHPublicKey.  # noqa: E501
+        :type: str
         """
 
-        self._quotas = quotas
+        self._public_key = public_key
 
     @property
-    def updated_at(self) -> 'datetime':
-        """Gets the updated_at of this V1Project.  # noqa: E501
+    def type(self) -> 'str':
+        """Gets the type of this V1SSHPublicKey.  # noqa: E501
 
 
-        :return: The updated_at of this V1Project.  # noqa: E501
-        :rtype: datetime
+        :return: The type of this V1SSHPublicKey.  # noqa: E501
+        :rtype: str
         """
-        return self._updated_at
+        return self._type
 
-    @updated_at.setter
-    def updated_at(self, updated_at: 'datetime'):
-        """Sets the updated_at of this V1Project.
+    @type.setter
+    def type(self, type: 'str'):
+        """Sets the type of this V1SSHPublicKey.
 
 
-        :param updated_at: The updated_at of this V1Project.  # noqa: E501
-        :type: datetime
+        :param type: The type of this V1SSHPublicKey.  # noqa: E501
+        :type: str
         """
 
-        self._updated_at = updated_at
+        self._type = type
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -255,31 +228,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1Project, dict):
+        if issubclass(V1SSHPublicKey, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1Project') -> bool:
+    def __eq__(self, other: 'V1SSHPublicKey') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1Project):
+        if not isinstance(other, V1SSHPublicKey):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1Project') -> bool:
+    def __ne__(self, other: 'V1SSHPublicKey') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_project_cluster_binding.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_project_cluster_binding.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_python_dependency_info.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_python_dependency_info.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_queue_server_type.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_queue_server_type.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_quotas.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_quotas.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_refresh_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_refresh_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_refresh_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_refresh_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_resources.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_resources.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_role.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_role.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_action.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_action.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_effect.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_effect.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_rule_resource.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_rule_resource.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_search_user.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_search_user.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_search_users_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_search_users_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_secret.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_secret.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_slurm_cluster_driver.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_slurm_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_slurm_cluster_status.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_slurm_cluster_status.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_source_type.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_source_type.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_ssh_public_key.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_upload_model_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,197 +24,170 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1SSHPublicKey(object):
+class V1UploadModelRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'created_at': 'datetime',
-        'id': 'str',
-        'last_used_at': 'datetime',
+        'metadata': 'dict(str, str)',
         'name': 'str',
-        'public_key': 'str',
-        'type': 'str'
+        'private': 'bool',
+        'project_id': 'str',
+        'version': 'str'
     }
 
     attribute_map = {
-        'created_at': 'createdAt',
-        'id': 'id',
-        'last_used_at': 'lastUsedAt',
+        'metadata': 'metadata',
         'name': 'name',
-        'public_key': 'publicKey',
-        'type': 'type'
+        'private': 'private',
+        'project_id': 'projectId',
+        'version': 'version'
     }
 
     def __init__(self,
-                 created_at: 'datetime' = None,
-                 id: 'str' = None,
-                 last_used_at: 'datetime' = None,
+                 metadata: 'dict(str, str)' = None,
                  name: 'str' = None,
-                 public_key: 'str' = None,
-                 type: 'str' = None):  # noqa: E501
-        """V1SSHPublicKey - a model defined in Swagger"""  # noqa: E501
-        self._created_at = None
-        self._id = None
-        self._last_used_at = None
+                 private: 'bool' = None,
+                 project_id: 'str' = None,
+                 version: 'str' = None):  # noqa: E501
+        """V1UploadModelRequest - a model defined in Swagger"""  # noqa: E501
+        self._metadata = None
         self._name = None
-        self._public_key = None
-        self._type = None
+        self._private = None
+        self._project_id = None
+        self._version = None
         self.discriminator = None
-        if created_at is not None:
-            self.created_at = created_at
-        if id is not None:
-            self.id = id
-        if last_used_at is not None:
-            self.last_used_at = last_used_at
+        if metadata is not None:
+            self.metadata = metadata
         if name is not None:
             self.name = name
-        if public_key is not None:
-            self.public_key = public_key
-        if type is not None:
-            self.type = type
+        if private is not None:
+            self.private = private
+        if project_id is not None:
+            self.project_id = project_id
+        if version is not None:
+            self.version = version
 
     @property
-    def created_at(self) -> 'datetime':
-        """Gets the created_at of this V1SSHPublicKey.  # noqa: E501
+    def metadata(self) -> 'dict(str, str)':
+        """Gets the metadata of this V1UploadModelRequest.  # noqa: E501
 
 
-        :return: The created_at of this V1SSHPublicKey.  # noqa: E501
-        :rtype: datetime
+        :return: The metadata of this V1UploadModelRequest.  # noqa: E501
+        :rtype: dict(str, str)
         """
-        return self._created_at
+        return self._metadata
 
-    @created_at.setter
-    def created_at(self, created_at: 'datetime'):
-        """Sets the created_at of this V1SSHPublicKey.
+    @metadata.setter
+    def metadata(self, metadata: 'dict(str, str)'):
+        """Sets the metadata of this V1UploadModelRequest.
 
 
-        :param created_at: The created_at of this V1SSHPublicKey.  # noqa: E501
-        :type: datetime
+        :param metadata: The metadata of this V1UploadModelRequest.  # noqa: E501
+        :type: dict(str, str)
         """
 
-        self._created_at = created_at
+        self._metadata = metadata
 
     @property
-    def id(self) -> 'str':
-        """Gets the id of this V1SSHPublicKey.  # noqa: E501
+    def name(self) -> 'str':
+        """Gets the name of this V1UploadModelRequest.  # noqa: E501
 
 
-        :return: The id of this V1SSHPublicKey.  # noqa: E501
+        :return: The name of this V1UploadModelRequest.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._name
 
-    @id.setter
-    def id(self, id: 'str'):
-        """Sets the id of this V1SSHPublicKey.
+    @name.setter
+    def name(self, name: 'str'):
+        """Sets the name of this V1UploadModelRequest.
 
 
-        :param id: The id of this V1SSHPublicKey.  # noqa: E501
+        :param name: The name of this V1UploadModelRequest.  # noqa: E501
         :type: str
         """
 
-        self._id = id
-
-    @property
-    def last_used_at(self) -> 'datetime':
-        """Gets the last_used_at of this V1SSHPublicKey.  # noqa: E501
-
-
-        :return: The last_used_at of this V1SSHPublicKey.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._last_used_at
-
-    @last_used_at.setter
-    def last_used_at(self, last_used_at: 'datetime'):
-        """Sets the last_used_at of this V1SSHPublicKey.
-
-
-        :param last_used_at: The last_used_at of this V1SSHPublicKey.  # noqa: E501
-        :type: datetime
-        """
-
-        self._last_used_at = last_used_at
+        self._name = name
 
     @property
-    def name(self) -> 'str':
-        """Gets the name of this V1SSHPublicKey.  # noqa: E501
+    def private(self) -> 'bool':
+        """Gets the private of this V1UploadModelRequest.  # noqa: E501
 
 
-        :return: The name of this V1SSHPublicKey.  # noqa: E501
-        :rtype: str
+        :return: The private of this V1UploadModelRequest.  # noqa: E501
+        :rtype: bool
         """
-        return self._name
+        return self._private
 
-    @name.setter
-    def name(self, name: 'str'):
-        """Sets the name of this V1SSHPublicKey.
+    @private.setter
+    def private(self, private: 'bool'):
+        """Sets the private of this V1UploadModelRequest.
 
 
-        :param name: The name of this V1SSHPublicKey.  # noqa: E501
-        :type: str
+        :param private: The private of this V1UploadModelRequest.  # noqa: E501
+        :type: bool
         """
 
-        self._name = name
+        self._private = private
 
     @property
-    def public_key(self) -> 'str':
-        """Gets the public_key of this V1SSHPublicKey.  # noqa: E501
+    def project_id(self) -> 'str':
+        """Gets the project_id of this V1UploadModelRequest.  # noqa: E501
 
 
-        :return: The public_key of this V1SSHPublicKey.  # noqa: E501
+        :return: The project_id of this V1UploadModelRequest.  # noqa: E501
         :rtype: str
         """
-        return self._public_key
+        return self._project_id
 
-    @public_key.setter
-    def public_key(self, public_key: 'str'):
-        """Sets the public_key of this V1SSHPublicKey.
+    @project_id.setter
+    def project_id(self, project_id: 'str'):
+        """Sets the project_id of this V1UploadModelRequest.
 
 
-        :param public_key: The public_key of this V1SSHPublicKey.  # noqa: E501
+        :param project_id: The project_id of this V1UploadModelRequest.  # noqa: E501
         :type: str
         """
 
-        self._public_key = public_key
+        self._project_id = project_id
 
     @property
-    def type(self) -> 'str':
-        """Gets the type of this V1SSHPublicKey.  # noqa: E501
+    def version(self) -> 'str':
+        """Gets the version of this V1UploadModelRequest.  # noqa: E501
 
 
-        :return: The type of this V1SSHPublicKey.  # noqa: E501
+        :return: The version of this V1UploadModelRequest.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._version
 
-    @type.setter
-    def type(self, type: 'str'):
-        """Sets the type of this V1SSHPublicKey.
+    @version.setter
+    def version(self, version: 'str'):
+        """Sets the version of this V1UploadModelRequest.
 
 
-        :param type: The type of this V1SSHPublicKey.  # noqa: E501
+        :param version: The version of this V1UploadModelRequest.  # noqa: E501
         :type: str
         """
 
-        self._type = type
+        self._version = version
 
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -228,31 +201,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1SSHPublicKey, dict):
+        if issubclass(V1UploadModelRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1SSHPublicKey') -> bool:
+    def __eq__(self, other: 'V1UploadModelRequest') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1SSHPublicKey):
+        if not isinstance(other, V1UploadModelRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1SSHPublicKey') -> bool:
+    def __ne__(self, other: 'V1UploadModelRequest') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_update_cluster_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_update_cluster_response.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_update_user_request.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_update_user_request.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_upload_model_version_response.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_upload_model_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,84 +24,113 @@
 import six
 
 if TYPE_CHECKING:
     from datetime import datetime
     from lightning_cloud.openapi.models import *
 
 
-class V1UploadModelVersionResponse(object):
+class V1UploadModelResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {'id': 'str', 'upload_url': 'str'}
+    swagger_types = {'model_id': 'str', 'upload_url': 'str', 'version': 'str'}
 
-    attribute_map = {'id': 'id', 'upload_url': 'uploadUrl'}
+    attribute_map = {
+        'model_id': 'modelId',
+        'upload_url': 'uploadUrl',
+        'version': 'version'
+    }
 
     def __init__(self,
-                 id: 'str' = None,
-                 upload_url: 'str' = None):  # noqa: E501
-        """V1UploadModelVersionResponse - a model defined in Swagger"""  # noqa: E501
-        self._id = None
+                 model_id: 'str' = None,
+                 upload_url: 'str' = None,
+                 version: 'str' = None):  # noqa: E501
+        """V1UploadModelResponse - a model defined in Swagger"""  # noqa: E501
+        self._model_id = None
         self._upload_url = None
+        self._version = None
         self.discriminator = None
-        if id is not None:
-            self.id = id
+        if model_id is not None:
+            self.model_id = model_id
         if upload_url is not None:
             self.upload_url = upload_url
+        if version is not None:
+            self.version = version
 
     @property
-    def id(self) -> 'str':
-        """Gets the id of this V1UploadModelVersionResponse.  # noqa: E501
+    def model_id(self) -> 'str':
+        """Gets the model_id of this V1UploadModelResponse.  # noqa: E501
 
 
-        :return: The id of this V1UploadModelVersionResponse.  # noqa: E501
+        :return: The model_id of this V1UploadModelResponse.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._model_id
 
-    @id.setter
-    def id(self, id: 'str'):
-        """Sets the id of this V1UploadModelVersionResponse.
+    @model_id.setter
+    def model_id(self, model_id: 'str'):
+        """Sets the model_id of this V1UploadModelResponse.
 
 
-        :param id: The id of this V1UploadModelVersionResponse.  # noqa: E501
+        :param model_id: The model_id of this V1UploadModelResponse.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._model_id = model_id
 
     @property
     def upload_url(self) -> 'str':
-        """Gets the upload_url of this V1UploadModelVersionResponse.  # noqa: E501
+        """Gets the upload_url of this V1UploadModelResponse.  # noqa: E501
 
 
-        :return: The upload_url of this V1UploadModelVersionResponse.  # noqa: E501
+        :return: The upload_url of this V1UploadModelResponse.  # noqa: E501
         :rtype: str
         """
         return self._upload_url
 
     @upload_url.setter
     def upload_url(self, upload_url: 'str'):
-        """Sets the upload_url of this V1UploadModelVersionResponse.
+        """Sets the upload_url of this V1UploadModelResponse.
 
 
-        :param upload_url: The upload_url of this V1UploadModelVersionResponse.  # noqa: E501
+        :param upload_url: The upload_url of this V1UploadModelResponse.  # noqa: E501
         :type: str
         """
 
         self._upload_url = upload_url
 
+    @property
+    def version(self) -> 'str':
+        """Gets the version of this V1UploadModelResponse.  # noqa: E501
+
+
+        :return: The version of this V1UploadModelResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._version
+
+    @version.setter
+    def version(self, version: 'str'):
+        """Sets the version of this V1UploadModelResponse.
+
+
+        :param version: The version of this V1UploadModelResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._version = version
+
     def to_dict(self) -> dict:
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -114,31 +143,31 @@
                 result[attr] = dict(
                     map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()))
             else:
                 result[attr] = value
-        if issubclass(V1UploadModelVersionResponse, dict):
+        if issubclass(V1UploadModelResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
-    def __eq__(self, other: 'V1UploadModelVersionResponse') -> bool:
+    def __eq__(self, other: 'V1UploadModelResponse') -> bool:
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1UploadModelVersionResponse):
+        if not isinstance(other, V1UploadModelResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: 'V1UploadModelVersionResponse') -> bool:
+    def __ne__(self, other: 'V1UploadModelResponse') -> bool:
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_user_requested_compute_config.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_user_requested_compute_config.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_user_requested_flow_compute_config.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_user_requested_flow_compute_config.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/v1_work.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/v1_work.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/models/works_id_body.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/models/works_id_body.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/openapi/rest.py` & `lightning_cloud-0.5.9/lightning_cloud/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/rest_client.py` & `lightning_cloud-0.5.9/lightning_cloud/rest_client.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/copytree.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/hashing.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/local.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/logs_socket_api.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/tar.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/source_code/uploader.py` & `lightning_cloud-0.5.9/lightning_cloud/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud/utils/name_generator.py` & `lightning_cloud-0.5.9/lightning_cloud/utils/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning_cloud-0.5.8/lightning_cloud.egg-info/PKG-INFO` & `lightning_cloud-0.5.9/lightning_cloud.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-cloud
-Version: 0.5.8
+Version: 0.5.9
 Summary: Lightning Cloud
 Home-page: https://lightning.ai
 Author: Grid.ai
 Author-email: grid-eng@grid.ai
 License: Apache Software License
 Description: Lightning AI Command Line Interface
 Platform: UNKNOWN
```

### Comparing `lightning_cloud-0.5.8/lightning_cloud.egg-info/SOURCES.txt` & `lightning_cloud-0.5.9/lightning_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,17 @@
 lightning_cloud/openapi/models/externalv1_lightningapp_instance.py
 lightning_cloud/openapi/models/externalv1_lightningwork.py
 lightning_cloud/openapi/models/externalv1_user_status.py
 lightning_cloud/openapi/models/get_cluster_health_response_health_status.py
 lightning_cloud/openapi/models/id_get_body.py
 lightning_cloud/openapi/models/id_release_body.py
 lightning_cloud/openapi/models/instance_type_availability.py
-lightning_cloud/openapi/models/model_version_archive_contains_information_about_a_specific_uploaded_model_version_its_versionfiles_and_metadata.py
 lightning_cloud/openapi/models/project_id_appsv2_body.py
 lightning_cloud/openapi/models/project_id_getapp_body.py
 lightning_cloud/openapi/models/project_id_memberships_body.py
-lightning_cloud/openapi/models/project_id_models_body.py
 lightning_cloud/openapi/models/project_id_projectclustersbindings_body.py
 lightning_cloud/openapi/models/project_id_secrets_body.py
 lightning_cloud/openapi/models/projects_id_body.py
 lightning_cloud/openapi/models/projects_project_id_body.py
 lightning_cloud/openapi/models/protobuf_any.py
 lightning_cloud/openapi/models/rpc_status.py
 lightning_cloud/openapi/models/secrets_id_body.py
@@ -182,15 +180,16 @@
 lightning_cloud/openapi/models/v1_secret.py
 lightning_cloud/openapi/models/v1_slurm_cluster_driver.py
 lightning_cloud/openapi/models/v1_slurm_cluster_status.py
 lightning_cloud/openapi/models/v1_source_type.py
 lightning_cloud/openapi/models/v1_ssh_public_key.py
 lightning_cloud/openapi/models/v1_update_cluster_response.py
 lightning_cloud/openapi/models/v1_update_user_request.py
-lightning_cloud/openapi/models/v1_upload_model_version_response.py
+lightning_cloud/openapi/models/v1_upload_model_request.py
+lightning_cloud/openapi/models/v1_upload_model_response.py
 lightning_cloud/openapi/models/v1_user_requested_compute_config.py
 lightning_cloud/openapi/models/v1_user_requested_flow_compute_config.py
 lightning_cloud/openapi/models/v1_work.py
 lightning_cloud/openapi/models/works_id_body.py
 lightning_cloud/source_code/__init__.py
 lightning_cloud/source_code/copytree.py
 lightning_cloud/source_code/hashing.py
```

### Comparing `lightning_cloud-0.5.8/setup.py` & `lightning_cloud-0.5.9/setup.py`

 * *Files identical despite different names*

