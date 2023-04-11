# Comparing `tmp/streamsets-5.2.0b2.tar.gz` & `tmp/streamsets-5.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamsets-5.2.0b2.tar", last modified: Fri Apr  7 15:33:13 2023, max compression
+gzip compressed data, was "dist/streamsets-5.2.0b3.tar", last modified: Tue Apr 11 05:01:01 2023, max compression
```

## Comparing `streamsets-5.2.0b2.tar` & `streamsets-5.2.0b3.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.852789 streamsets-5.2.0b2/
--rw-r--r--   0 marcusbachu   (502) staff       (20)     6081 2023-03-15 15:49:36.000000 streamsets-5.2.0b2/HISTORY.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      134 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/MANIFEST.in
--rw-r--r--   0 marcusbachu   (502) staff       (20)      508 2023-04-07 15:33:13.852932 streamsets-5.2.0b2/PKG-INFO
--rw-r--r--   0 marcusbachu   (502) staff       (20)     1078 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/README.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.279124 streamsets-5.2.0b2/docs/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.300884 streamsets-5.2.0b2/docs/_static/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   173553 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/TopologyMissingNodes.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    62347 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/TopologyMultipleJobsSingleSystem.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   253621 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/TopologyRestoredNodes.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    30199 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/dev_data_generator_to_trash.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    42218 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/dev_data_generator_to_two_trashes.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    42660 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/dev_data_generator_with_events.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   135357 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/dev_raw_data_source_help.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    77707 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/dev_raw_data_to_trash.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    37145 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/file_tail_to_two_trashes.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.200966 streamsets-5.2.0b2/docs/_static/images/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.328462 streamsets-5.2.0b2/docs/_static/images/build/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   278966 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/add_frag_to_pipeline.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   311595 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/fragment_canvas.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   203600 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/fragment_ui.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   459107 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/pipeline_canvas.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   270194 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/pipeline_check_in.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   179873 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/pipeline_ui.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   256830 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/pipelines_using_fragment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   135823 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/snowflake_required_parameters.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   279286 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/stages_unconnected.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   149312 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/build/update_pipeline_with_frag.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.330027 streamsets-5.2.0b2/docs/_static/images/learn/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    65839 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/learn/api_credentials.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.331252 streamsets-5.2.0b2/docs/_static/images/learn/examples/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    98048 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/learn/examples/find_sdc_id.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.200462 streamsets-5.2.0b2/docs/_static/images/manage/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.337813 streamsets-5.2.0b2/docs/_static/images/manage/permissions/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   102670 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/permissions/add_new_permissions.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   113899 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/permissions/change_owner.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   118722 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/permissions/delete_permissions.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   101679 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/permissions/share_button.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    94323 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/permissions/share_settings.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.360573 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   145182 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/activate_user.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   168504 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/add_new_group.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   143229 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/add_new_user.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   147039 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/deactivate_user.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   196081 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/delete_group.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   144752 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/delete_user.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   158367 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/groups_list.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   207126 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/invite_user_details.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   178507 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/new_group_details.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   300732 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/update_group_details.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   264831 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/update_user_details.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   132573 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/users_list.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.402837 streamsets-5.2.0b2/docs/_static/images/search/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    14767 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Mark_Favorite.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    24541 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Query_Builder.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    15113 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Remove.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    20541 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Save_Search.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    21075 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Saved_Searches.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    39808 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Search_Name_Wizard.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    15550 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/_static/images/search/SAQL_Update.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   231447 2023-03-15 15:49:36.000000 streamsets-5.2.0b2/docs/_static/images/search/Search_Advanced.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.202700 streamsets-5.2.0b2/docs/_static/images/set_up/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.202421 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.413092 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    69567 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_autoscaling_group.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    49564 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_ssh_access.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    42182 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_zone.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    85383 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_sdc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   229521 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_transformer.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    38223 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_review_and_launch.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.422788 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    34117 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/configure_install_type_docker.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    37276 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/configure_install_type_tarball.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    47539 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_as_a_list.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    88053 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_screen.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    31004 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_as_a_list.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   108673 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_screen.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   118611 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_share_deployment.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.432289 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    62522 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_autoscaling_group.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    53502 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_ssh_access.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    60330 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_engine.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    86365 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_define_deployment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    33461 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_review_and_launch.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    48959 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_share_deployment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    87773 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_transformer_define_deployment.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.449675 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   145516 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_engine.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   183842 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_autoscaling_group.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   124366 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_region.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   158544 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_ssh_access.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   144494 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_zone.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   224534 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_sdc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   200961 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_transformer.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    98287 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_review_and_launch.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.471842 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    44568 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_configure_engine.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    62314 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_sdc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    72965 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_transformer.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    36551 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_sdc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    30758 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_transformer.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    50647 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_share_deployment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   199180 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/get_install_script.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   154342 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/select_install_type.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.204387 streamsets-5.2.0b2/docs/_static/images/set_up/environments/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.489121 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    69803 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_access_keys.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    68635 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_subnets.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    66922 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_vpc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    69562 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_cross_account_role.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    43298 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_select_aws_region.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    54248 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_define_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    37328 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_review_and_activate_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    41372 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_share_environment.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.503228 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   159076 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_credentials.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   121562 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_region.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   192519 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_subnet.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   183338 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_vnet.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   163862 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_defaults_azure_vm_instances.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    52597 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_define_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    79593 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_review_and_activate_environment.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.513900 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)   121250 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_impersonation.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   127314 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_key.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    46951 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_gcp_project.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    54100 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_define_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    33543 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_review_and_activate.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   163961 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_select_gcp_vpc.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    87855 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_share_environment.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.515536 streamsets-5.2.0b2/docs/_static/images/set_up/environments/managing_environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    66265 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/managing_environments/managing_environments.png
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.519495 streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    53481 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_define_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    33914 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_review_and_activate.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    44651 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_share_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    36186 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/sample_fragment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    31721 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/sample_pipeline_using_fragment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)   146932 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/sdk_sample_pipeline1.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    30244 2023-03-06 15:56:22.000000 streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_deployment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    52894 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_deployment_details.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    25636 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_environment.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)    13605 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/docs/_static/streamsets-logo.png
--rw-r--r--   0 marcusbachu   (502) staff       (20)      128 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/advanced_search.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.520492 streamsets-5.2.0b2/docs/api/
--rw-r--r--   0 marcusbachu   (502) staff       (20)     8588 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/api/sch_api.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      201 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/api.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.534223 streamsets-5.2.0b2/docs/build/
--rw-r--r--   0 marcusbachu   (502) staff       (20)     7631 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/build/creating_pipelines.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)    12338 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/build/pipeline_fragments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      126 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/build.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     7092 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/conf.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)      659 2023-03-15 15:49:36.000000 streamsets-5.2.0b2/docs/index.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.570262 streamsets-5.2.0b2/docs/learn/
--rw-r--r--   0 marcusbachu   (502) staff       (20)     3198 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn/authentication.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.580949 streamsets-5.2.0b2/docs/learn/examples/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    17823 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn/examples/sdk_examples_job_pipeline.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     6679 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/learn/examples/sdk_examples_self_managed_deployment.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      635 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn/examples.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     1490 2023-04-07 15:32:34.000000 streamsets-5.2.0b2/docs/learn/installation.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      545 2023-03-15 15:49:36.000000 streamsets-5.2.0b2/docs/learn/known_issues.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     2150 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn/overview.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)       62 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn/release_notes.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      220 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/learn.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.583362 streamsets-5.2.0b2/docs/manage/
--rw-r--r--   0 marcusbachu   (502) staff       (20)       63 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage/legacy_kubernetes_integration.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.621067 streamsets-5.2.0b2/docs/manage/users_and_groups/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    17307 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage/users_and_groups/managing_users_and_groups.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)    10722 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage/users_and_groups/permissions.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     3960 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage/users_and_groups/roles.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     1007 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage/users_and_groups/users_and_groups.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      156 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/manage.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.635764 streamsets-5.2.0b2/docs/monitor/
--rw-r--r--   0 marcusbachu   (502) staff       (20)       19 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/monitor/reports.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)       31 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/monitor/subscriptions.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)       25 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/monitor/topologies.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      141 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/monitor.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.663215 streamsets-5.2.0b2/docs/run/
--rw-r--r--   0 marcusbachu   (502) staff       (20)     4256 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/run/job_templates.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)    19002 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/run/jobs_instances.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)       35 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/run/scheduled_tasks.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      129 2023-04-04 15:25:01.000000 streamsets-5.2.0b2/docs/run.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.677257 streamsets-5.2.0b2/docs/search/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    10854 2023-04-07 14:58:29.000000 streamsets-5.2.0b2/docs/search/saql_saved_search.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     4885 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/search/search_for_object.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      421 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/set_up.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.207403 streamsets-5.2.0b2/docs/usage/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.208161 streamsets-5.2.0b2/docs/usage/set_up/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.707766 streamsets-5.2.0b2/docs/usage/set_up/deployments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    13294 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/azure_vm_deployments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      583 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/deployments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)    12037 2023-04-07 15:23:13.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/ec2_deployments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     7124 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/gce_deployments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)    12721 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/self_managed_deployments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     3251 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/stage_libs_sdc.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     3252 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/docs/usage/set_up/deployments/stage_libs_st.rst
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.735355 streamsets-5.2.0b2/docs/usage/set_up/environments/
--rw-r--r--   0 marcusbachu   (502) staff       (20)    10507 2023-04-07 15:23:13.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/aws_environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     7339 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/azure_environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      496 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     9683 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/gcp_environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     5180 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/managing_environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)     2985 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/docs/usage/set_up/environments/self_managed_environments.rst
--rw-r--r--   0 marcusbachu   (502) staff       (20)      366 2023-04-07 15:33:13.855704 streamsets-5.2.0b2/setup.cfg
--rw-r--r--   0 marcusbachu   (502) staff       (20)      924 2023-04-07 15:32:34.000000 streamsets-5.2.0b2/setup.py
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.208871 streamsets-5.2.0b2/streamsets/
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.852073 streamsets-5.2.0b2/streamsets/sdk/
--rw-r--r--   0 marcusbachu   (502) staff       (20)      204 2023-04-07 15:32:34.000000 streamsets-5.2.0b2/streamsets/sdk/__init__.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    47020 2023-04-07 15:23:56.000000 streamsets-5.2.0b2/streamsets/sdk/aster_api.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)      177 2022-08-23 20:18:37.000000 streamsets-5.2.0b2/streamsets/sdk/constants.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)     3249 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/streamsets/sdk/exceptions.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    10737 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/streamsets/sdk/models.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)   188008 2023-04-07 15:23:56.000000 streamsets-5.2.0b2/streamsets/sdk/sch.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)   336919 2023-04-07 15:23:56.000000 streamsets-5.2.0b2/streamsets/sdk/sch_api.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)   448309 2023-04-07 15:23:56.000000 streamsets-5.2.0b2/streamsets/sdk/sch_models.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    43488 2023-03-06 15:56:23.000000 streamsets-5.2.0b2/streamsets/sdk/sdc.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    77513 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/streamsets/sdk/sdc_api.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)   117673 2023-04-07 15:22:58.000000 streamsets-5.2.0b2/streamsets/sdk/sdc_models.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    30503 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/streamsets/sdk/st.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    66802 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/streamsets/sdk/st_api.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    76903 2023-03-15 15:49:36.000000 streamsets-5.2.0b2/streamsets/sdk/st_models.py
--rw-r--r--   0 marcusbachu   (502) staff       (20)    36154 2023-04-05 20:26:10.000000 streamsets-5.2.0b2/streamsets/sdk/utils.py
-drwxr-xr-x   0 marcusbachu   (502) staff       (20)        0 2023-04-07 15:33:13.742014 streamsets-5.2.0b2/streamsets.egg-info/
--rw-r--r--   0 marcusbachu   (502) staff       (20)      508 2023-04-07 15:33:12.000000 streamsets-5.2.0b2/streamsets.egg-info/PKG-INFO
--rw-r--r--   0 marcusbachu   (502) staff       (20)    11126 2023-04-07 15:33:13.000000 streamsets-5.2.0b2/streamsets.egg-info/SOURCES.txt
--rw-r--r--   0 marcusbachu   (502) staff       (20)       74 2023-04-07 15:33:12.000000 streamsets-5.2.0b2/streamsets.egg-info/dependency_links.txt
--rw-r--r--   0 marcusbachu   (502) staff       (20)        1 2023-02-10 19:08:35.000000 streamsets-5.2.0b2/streamsets.egg-info/not-zip-safe
--rw-r--r--   0 marcusbachu   (502) staff       (20)       40 2023-04-07 15:33:12.000000 streamsets-5.2.0b2/streamsets.egg-info/requires.txt
--rw-r--r--   0 marcusbachu   (502) staff       (20)       11 2023-04-07 15:33:12.000000 streamsets-5.2.0b2/streamsets.egg-info/top_level.txt
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/
+-rw-r--r--   0 mitch      (502) staff       (20)     6081 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/HISTORY.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      134 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/MANIFEST.in
+-rw-r--r--   0 mitch      (502) staff       (20)      519 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/PKG-INFO
+-rw-r--r--   0 mitch      (502) staff       (20)     1078 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/README.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/
+-rw-r--r--   0 mitch      (502) staff       (20)   173553 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/TopologyMissingNodes.png
+-rw-r--r--   0 mitch      (502) staff       (20)    62347 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/TopologyMultipleJobsSingleSystem.png
+-rw-r--r--   0 mitch      (502) staff       (20)   253621 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/TopologyRestoredNodes.png
+-rw-r--r--   0 mitch      (502) staff       (20)    30199 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/dev_data_generator_to_trash.png
+-rw-r--r--   0 mitch      (502) staff       (20)    42218 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/dev_data_generator_to_two_trashes.png
+-rw-r--r--   0 mitch      (502) staff       (20)    42660 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/dev_data_generator_with_events.png
+-rw-r--r--   0 mitch      (502) staff       (20)   135357 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/dev_raw_data_source_help.png
+-rw-r--r--   0 mitch      (502) staff       (20)    77707 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/dev_raw_data_to_trash.png
+-rw-r--r--   0 mitch      (502) staff       (20)    37145 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/file_tail_to_two_trashes.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/build/
+-rw-r--r--   0 mitch      (502) staff       (20)   278966 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/add_frag_to_pipeline.png
+-rw-r--r--   0 mitch      (502) staff       (20)   311595 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/fragment_canvas.png
+-rw-r--r--   0 mitch      (502) staff       (20)   203600 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/fragment_ui.png
+-rw-r--r--   0 mitch      (502) staff       (20)   459107 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/pipeline_canvas.png
+-rw-r--r--   0 mitch      (502) staff       (20)   270194 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/pipeline_check_in.png
+-rw-r--r--   0 mitch      (502) staff       (20)   179873 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/pipeline_ui.png
+-rw-r--r--   0 mitch      (502) staff       (20)   256830 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/pipelines_using_fragment.png
+-rw-r--r--   0 mitch      (502) staff       (20)   135823 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/snowflake_required_parameters.png
+-rw-r--r--   0 mitch      (502) staff       (20)   279286 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/stages_unconnected.png
+-rw-r--r--   0 mitch      (502) staff       (20)   149312 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/build/update_pipeline_with_frag.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/learn/
+-rw-r--r--   0 mitch      (502) staff       (20)    65839 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/learn/api_credentials.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/learn/examples/
+-rw-r--r--   0 mitch      (502) staff       (20)    98048 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/learn/examples/find_sdc_id.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/manage/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/
+-rw-r--r--   0 mitch      (502) staff       (20)   102670 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/add_new_permissions.png
+-rw-r--r--   0 mitch      (502) staff       (20)   113899 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/change_owner.png
+-rw-r--r--   0 mitch      (502) staff       (20)   118722 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/delete_permissions.png
+-rw-r--r--   0 mitch      (502) staff       (20)   101679 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/share_button.png
+-rw-r--r--   0 mitch      (502) staff       (20)    94323 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/permissions/share_settings.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/
+-rw-r--r--   0 mitch      (502) staff       (20)   145182 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/activate_user.png
+-rw-r--r--   0 mitch      (502) staff       (20)   168504 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/add_new_group.png
+-rw-r--r--   0 mitch      (502) staff       (20)   143229 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/add_new_user.png
+-rw-r--r--   0 mitch      (502) staff       (20)   147039 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/deactivate_user.png
+-rw-r--r--   0 mitch      (502) staff       (20)   196081 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/delete_group.png
+-rw-r--r--   0 mitch      (502) staff       (20)   144752 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/delete_user.png
+-rw-r--r--   0 mitch      (502) staff       (20)   158367 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/groups_list.png
+-rw-r--r--   0 mitch      (502) staff       (20)   207126 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/invite_user_details.png
+-rw-r--r--   0 mitch      (502) staff       (20)   178507 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/new_group_details.png
+-rw-r--r--   0 mitch      (502) staff       (20)   300732 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/update_group_details.png
+-rw-r--r--   0 mitch      (502) staff       (20)   264831 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/update_user_details.png
+-rw-r--r--   0 mitch      (502) staff       (20)   132573 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/users_list.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/search/
+-rw-r--r--   0 mitch      (502) staff       (20)    14767 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Mark_Favorite.png
+-rw-r--r--   0 mitch      (502) staff       (20)    24541 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Query_Builder.png
+-rw-r--r--   0 mitch      (502) staff       (20)    15113 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Remove.png
+-rw-r--r--   0 mitch      (502) staff       (20)    20541 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Save_Search.png
+-rw-r--r--   0 mitch      (502) staff       (20)    21075 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Saved_Searches.png
+-rw-r--r--   0 mitch      (502) staff       (20)    39808 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Search_Name_Wizard.png
+-rw-r--r--   0 mitch      (502) staff       (20)    15550 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/_static/images/search/SAQL_Update.png
+-rw-r--r--   0 mitch      (502) staff       (20)   231447 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/search/Search_Advanced.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/
+-rw-r--r--   0 mitch      (502) staff       (20)    69567 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_autoscaling_group.png
+-rw-r--r--   0 mitch      (502) staff       (20)    49564 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_ssh_access.png
+-rw-r--r--   0 mitch      (502) staff       (20)    42182 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_zone.png
+-rw-r--r--   0 mitch      (502) staff       (20)    85383 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_sdc.png
+-rw-r--r--   0 mitch      (502) staff       (20)   229521 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_transformer.png
+-rw-r--r--   0 mitch      (502) staff       (20)    38223 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_review_and_launch.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/
+-rw-r--r--   0 mitch      (502) staff       (20)    34117 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/configure_install_type_docker.png
+-rw-r--r--   0 mitch      (502) staff       (20)    37276 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/configure_install_type_tarball.png
+-rw-r--r--   0 mitch      (502) staff       (20)    47539 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_as_a_list.png
+-rw-r--r--   0 mitch      (502) staff       (20)    88053 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_screen.png
+-rw-r--r--   0 mitch      (502) staff       (20)    31004 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_as_a_list.png
+-rw-r--r--   0 mitch      (502) staff       (20)   108673 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_screen.png
+-rw-r--r--   0 mitch      (502) staff       (20)   118611 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_share_deployment.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/
+-rw-r--r--   0 mitch      (502) staff       (20)    62522 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_autoscaling_group.png
+-rw-r--r--   0 mitch      (502) staff       (20)    53502 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_ssh_access.png
+-rw-r--r--   0 mitch      (502) staff       (20)    60330 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_engine.png
+-rw-r--r--   0 mitch      (502) staff       (20)    86365 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_define_deployment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    33461 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_review_and_launch.png
+-rw-r--r--   0 mitch      (502) staff       (20)    48959 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_share_deployment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    87773 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_transformer_define_deployment.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/
+-rw-r--r--   0 mitch      (502) staff       (20)   145516 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_engine.png
+-rw-r--r--   0 mitch      (502) staff       (20)   183842 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_autoscaling_group.png
+-rw-r--r--   0 mitch      (502) staff       (20)   124366 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_region.png
+-rw-r--r--   0 mitch      (502) staff       (20)   158544 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_ssh_access.png
+-rw-r--r--   0 mitch      (502) staff       (20)   144494 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_zone.png
+-rw-r--r--   0 mitch      (502) staff       (20)   224534 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_sdc.png
+-rw-r--r--   0 mitch      (502) staff       (20)   200961 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_transformer.png
+-rw-r--r--   0 mitch      (502) staff       (20)    98287 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_review_and_launch.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/
+-rw-r--r--   0 mitch      (502) staff       (20)    44568 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_configure_engine.png
+-rw-r--r--   0 mitch      (502) staff       (20)    62314 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_sdc.png
+-rw-r--r--   0 mitch      (502) staff       (20)    72965 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_transformer.png
+-rw-r--r--   0 mitch      (502) staff       (20)    36551 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_sdc.png
+-rw-r--r--   0 mitch      (502) staff       (20)    30758 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_transformer.png
+-rw-r--r--   0 mitch      (502) staff       (20)    50647 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_share_deployment.png
+-rw-r--r--   0 mitch      (502) staff       (20)   199180 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/get_install_script.png
+-rw-r--r--   0 mitch      (502) staff       (20)   154342 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/select_install_type.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/
+-rw-r--r--   0 mitch      (502) staff       (20)    69803 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_access_keys.png
+-rw-r--r--   0 mitch      (502) staff       (20)    68635 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_subnets.png
+-rw-r--r--   0 mitch      (502) staff       (20)    66922 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_vpc.png
+-rw-r--r--   0 mitch      (502) staff       (20)    69562 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_cross_account_role.png
+-rw-r--r--   0 mitch      (502) staff       (20)    43298 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_select_aws_region.png
+-rw-r--r--   0 mitch      (502) staff       (20)    54248 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_define_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    37328 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_review_and_activate_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    41372 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_share_environment.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/
+-rw-r--r--   0 mitch      (502) staff       (20)   159076 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_credentials.png
+-rw-r--r--   0 mitch      (502) staff       (20)   121562 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_region.png
+-rw-r--r--   0 mitch      (502) staff       (20)   192519 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_subnet.png
+-rw-r--r--   0 mitch      (502) staff       (20)   183338 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_vnet.png
+-rw-r--r--   0 mitch      (502) staff       (20)   163862 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_defaults_azure_vm_instances.png
+-rw-r--r--   0 mitch      (502) staff       (20)    52597 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_define_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    79593 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_review_and_activate_environment.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/
+-rw-r--r--   0 mitch      (502) staff       (20)   121250 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_impersonation.png
+-rw-r--r--   0 mitch      (502) staff       (20)   127314 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_key.png
+-rw-r--r--   0 mitch      (502) staff       (20)    46951 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_gcp_project.png
+-rw-r--r--   0 mitch      (502) staff       (20)    54100 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_define_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    33543 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_review_and_activate.png
+-rw-r--r--   0 mitch      (502) staff       (20)   163961 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_select_gcp_vpc.png
+-rw-r--r--   0 mitch      (502) staff       (20)    87855 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_share_environment.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/managing_environments/
+-rw-r--r--   0 mitch      (502) staff       (20)    66265 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/managing_environments/managing_environments.png
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/
+-rw-r--r--   0 mitch      (502) staff       (20)    53481 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_define_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    33914 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_review_and_activate.png
+-rw-r--r--   0 mitch      (502) staff       (20)    44651 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_share_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    36186 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/sample_fragment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    31721 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/sample_pipeline_using_fragment.png
+-rw-r--r--   0 mitch      (502) staff       (20)   146932 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/sdk_sample_pipeline1.png
+-rw-r--r--   0 mitch      (502) staff       (20)    30244 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_deployment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    52894 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_deployment_details.png
+-rw-r--r--   0 mitch      (502) staff       (20)    25636 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_environment.png
+-rw-r--r--   0 mitch      (502) staff       (20)    13605 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/docs/_static/streamsets-logo.png
+-rw-r--r--   0 mitch      (502) staff       (20)      128 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/advanced_search.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/api/
+-rw-r--r--   0 mitch      (502) staff       (20)     8588 2023-04-10 19:22:00.000000 streamsets-5.2.0b3/docs/api/sch_api.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      201 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/api.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/build/
+-rw-r--r--   0 mitch      (502) staff       (20)     7631 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/build/creating_pipelines.rst
+-rw-r--r--   0 mitch      (502) staff       (20)    12338 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/build/pipeline_fragments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      126 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/build.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     7092 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/conf.py
+-rw-r--r--   0 mitch      (502) staff       (20)      659 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/index.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/learn/
+-rw-r--r--   0 mitch      (502) staff       (20)     3198 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/authentication.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/learn/examples/
+-rw-r--r--   0 mitch      (502) staff       (20)    17823 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/examples/sdk_examples_job_pipeline.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     6679 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/examples/sdk_examples_self_managed_deployment.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      635 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/examples.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     1488 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/installation.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      545 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/known_issues.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     2150 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/overview.rst
+-rw-r--r--   0 mitch      (502) staff       (20)       62 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn/release_notes.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      220 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/learn.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/manage/
+-rw-r--r--   0 mitch      (502) staff       (20)       63 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/manage/legacy_kubernetes_integration.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/manage/users_and_groups/
+-rw-r--r--   0 mitch      (502) staff       (20)    17307 2023-04-10 19:22:00.000000 streamsets-5.2.0b3/docs/manage/users_and_groups/managing_users_and_groups.rst
+-rw-r--r--   0 mitch      (502) staff       (20)    10722 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/manage/users_and_groups/permissions.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     3960 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/manage/users_and_groups/roles.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     1007 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/manage/users_and_groups/users_and_groups.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      156 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/manage.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/monitor/
+-rw-r--r--   0 mitch      (502) staff       (20)       19 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/monitor/reports.rst
+-rw-r--r--   0 mitch      (502) staff       (20)       31 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/monitor/subscriptions.rst
+-rw-r--r--   0 mitch      (502) staff       (20)       25 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/monitor/topologies.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      141 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/monitor.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/run/
+-rw-r--r--   0 mitch      (502) staff       (20)     4256 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/run/job_templates.rst
+-rw-r--r--   0 mitch      (502) staff       (20)    19002 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/run/jobs_instances.rst
+-rw-r--r--   0 mitch      (502) staff       (20)       35 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/run/scheduled_tasks.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      129 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/run.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/search/
+-rw-r--r--   0 mitch      (502) staff       (20)    10854 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/search/saql_saved_search.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     4885 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/search/search_for_object.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      421 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/set_up.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/usage/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/usage/set_up/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/
+-rw-r--r--   0 mitch      (502) staff       (20)    13294 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/azure_vm_deployments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      583 2023-04-10 19:22:00.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/deployments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)    12037 2023-04-10 19:22:00.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/ec2_deployments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     7124 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/gce_deployments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)    12721 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/self_managed_deployments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     3251 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/stage_libs_sdc.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     3252 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/deployments/stage_libs_st.rst
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/
+-rw-r--r--   0 mitch      (502) staff       (20)    10507 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/aws_environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     7339 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/azure_environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      496 2023-04-10 19:22:00.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     9683 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/gcp_environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     5180 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/managing_environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)     2985 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/docs/usage/set_up/environments/self_managed_environments.rst
+-rw-r--r--   0 mitch      (502) staff       (20)      366 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/setup.cfg
+-rw-r--r--   0 mitch      (502) staff       (20)      924 2023-04-11 05:00:08.000000 streamsets-5.2.0b3/setup.py
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets/
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets/sdk/
+-rw-r--r--   0 mitch      (502) staff       (20)      204 2023-04-11 05:00:08.000000 streamsets-5.2.0b3/streamsets/sdk/__init__.py
+-rw-r--r--   0 mitch      (502) staff       (20)    46081 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/aster_api.py
+-rw-r--r--   0 mitch      (502) staff       (20)      177 2023-01-19 05:47:13.000000 streamsets-5.2.0b3/streamsets/sdk/constants.py
+-rw-r--r--   0 mitch      (502) staff       (20)     3249 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/exceptions.py
+-rw-r--r--   0 mitch      (502) staff       (20)    10737 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/models.py
+-rw-r--r--   0 mitch      (502) staff       (20)   189014 2023-04-07 16:05:20.000000 streamsets-5.2.0b3/streamsets/sdk/sch.py
+-rw-r--r--   0 mitch      (502) staff       (20)   337882 2023-04-11 05:00:08.000000 streamsets-5.2.0b3/streamsets/sdk/sch_api.py
+-rw-r--r--   0 mitch      (502) staff       (20)   449675 2023-04-11 04:58:40.000000 streamsets-5.2.0b3/streamsets/sdk/sch_models.py
+-rw-r--r--   0 mitch      (502) staff       (20)    43488 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/sdc.py
+-rw-r--r--   0 mitch      (502) staff       (20)    77513 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/sdc_api.py
+-rw-r--r--   0 mitch      (502) staff       (20)   117673 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/sdc_models.py
+-rw-r--r--   0 mitch      (502) staff       (20)    30503 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/st.py
+-rw-r--r--   0 mitch      (502) staff       (20)    66802 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/st_api.py
+-rw-r--r--   0 mitch      (502) staff       (20)    76903 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/st_models.py
+-rw-r--r--   0 mitch      (502) staff       (20)    36154 2023-04-06 17:31:39.000000 streamsets-5.2.0b3/streamsets/sdk/utils.py
+drwxr-xr-x   0 mitch      (502) staff       (20)        0 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/
+-rw-r--r--   0 mitch      (502) staff       (20)      519 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/PKG-INFO
+-rw-r--r--   0 mitch      (502) staff       (20)    11126 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/SOURCES.txt
+-rw-r--r--   0 mitch      (502) staff       (20)       74 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/dependency_links.txt
+-rw-r--r--   0 mitch      (502) staff       (20)        1 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/not-zip-safe
+-rw-r--r--   0 mitch      (502) staff       (20)       40 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/requires.txt
+-rw-r--r--   0 mitch      (502) staff       (20)       11 2023-04-11 05:01:01.000000 streamsets-5.2.0b3/streamsets.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `streamsets-5.2.0b2/HISTORY.rst` & `streamsets-5.2.0b3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/README.rst` & `streamsets-5.2.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/TopologyMissingNodes.png` & `streamsets-5.2.0b3/docs/_static/TopologyMissingNodes.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/TopologyMultipleJobsSingleSystem.png` & `streamsets-5.2.0b3/docs/_static/TopologyMultipleJobsSingleSystem.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/TopologyRestoredNodes.png` & `streamsets-5.2.0b3/docs/_static/TopologyRestoredNodes.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/dev_data_generator_to_trash.png` & `streamsets-5.2.0b3/docs/_static/dev_data_generator_to_trash.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/dev_data_generator_to_two_trashes.png` & `streamsets-5.2.0b3/docs/_static/dev_data_generator_to_two_trashes.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/dev_data_generator_with_events.png` & `streamsets-5.2.0b3/docs/_static/dev_data_generator_with_events.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/dev_raw_data_source_help.png` & `streamsets-5.2.0b3/docs/_static/dev_raw_data_source_help.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/dev_raw_data_to_trash.png` & `streamsets-5.2.0b3/docs/_static/dev_raw_data_to_trash.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/file_tail_to_two_trashes.png` & `streamsets-5.2.0b3/docs/_static/file_tail_to_two_trashes.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/add_frag_to_pipeline.png` & `streamsets-5.2.0b3/docs/_static/images/build/add_frag_to_pipeline.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/fragment_canvas.png` & `streamsets-5.2.0b3/docs/_static/images/build/fragment_canvas.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/fragment_ui.png` & `streamsets-5.2.0b3/docs/_static/images/build/fragment_ui.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/pipeline_canvas.png` & `streamsets-5.2.0b3/docs/_static/images/build/pipeline_canvas.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/pipeline_check_in.png` & `streamsets-5.2.0b3/docs/_static/images/build/pipeline_check_in.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/pipeline_ui.png` & `streamsets-5.2.0b3/docs/_static/images/build/pipeline_ui.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/pipelines_using_fragment.png` & `streamsets-5.2.0b3/docs/_static/images/build/pipelines_using_fragment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/snowflake_required_parameters.png` & `streamsets-5.2.0b3/docs/_static/images/build/snowflake_required_parameters.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/stages_unconnected.png` & `streamsets-5.2.0b3/docs/_static/images/build/stages_unconnected.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/build/update_pipeline_with_frag.png` & `streamsets-5.2.0b3/docs/_static/images/build/update_pipeline_with_frag.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/learn/api_credentials.png` & `streamsets-5.2.0b3/docs/_static/images/learn/api_credentials.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/learn/examples/find_sdc_id.png` & `streamsets-5.2.0b3/docs/_static/images/learn/examples/find_sdc_id.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/permissions/add_new_permissions.png` & `streamsets-5.2.0b3/docs/_static/images/manage/permissions/add_new_permissions.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/permissions/change_owner.png` & `streamsets-5.2.0b3/docs/_static/images/manage/permissions/change_owner.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/permissions/delete_permissions.png` & `streamsets-5.2.0b3/docs/_static/images/manage/permissions/delete_permissions.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/permissions/share_button.png` & `streamsets-5.2.0b3/docs/_static/images/manage/permissions/share_button.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/permissions/share_settings.png` & `streamsets-5.2.0b3/docs/_static/images/manage/permissions/share_settings.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/activate_user.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/activate_user.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/add_new_group.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/add_new_group.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/add_new_user.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/add_new_user.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/deactivate_user.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/deactivate_user.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/delete_group.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/delete_group.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/delete_user.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/delete_user.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/groups_list.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/groups_list.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/invite_user_details.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/invite_user_details.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/new_group_details.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/new_group_details.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/update_group_details.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/update_group_details.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/update_user_details.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/update_user_details.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/manage/users_and_groups/users_list.png` & `streamsets-5.2.0b3/docs/_static/images/manage/users_and_groups/users_list.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Mark_Favorite.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Mark_Favorite.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Query_Builder.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Query_Builder.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Remove.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Remove.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Save_Search.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Save_Search.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Saved_Searches.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Saved_Searches.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Search_Name_Wizard.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Search_Name_Wizard.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/SAQL_Update.png` & `streamsets-5.2.0b3/docs/_static/images/search/SAQL_Update.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/search/Search_Advanced.png` & `streamsets-5.2.0b3/docs/_static/images/search/Search_Advanced.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_autoscaling_group.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_autoscaling_group.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_ssh_access.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_ssh_access.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_zone.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_configure_azure_vm_zone.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_sdc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_sdc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_transformer.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_define_deployment_transformer.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_review_and_launch.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/azure_vm_deployments/creation_review_and_launch.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/configure_install_type_docker.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/configure_install_type_docker.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/configure_install_type_tarball.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/configure_install_type_tarball.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_as_a_list.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_as_a_list.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_screen.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_stage_lib_selection_screen.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_as_a_list.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_as_a_list.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_screen.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_configure_engine_transformer_stage_lib_selection_screen.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/common/creation_share_deployment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/common/creation_share_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_autoscaling_group.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_autoscaling_group.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_ssh_access.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_ec2_ssh_access.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_engine.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_configure_engine.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_define_deployment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_define_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_review_and_launch.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_review_and_launch.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_share_deployment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_share_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/ec2_deployments/creation_transformer_define_deployment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/ec2_deployments/creation_transformer_define_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_engine.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_engine.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_autoscaling_group.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_autoscaling_group.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_region.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_region.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_ssh_access.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_ssh_access.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_zone.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_configure_gce_zone.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_sdc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_sdc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_transformer.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_define_deployment_transformer.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/gce_deployments/creation_review_and_launch.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/gce_deployments/creation_review_and_launch.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_configure_engine.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_configure_engine.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_sdc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_sdc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_transformer.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_define_deployment_transformer.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_sdc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_sdc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_transformer.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_review_and_launch_transformer.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/creation_share_deployment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/creation_share_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/get_install_script.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/get_install_script.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/deployments/self_managed_deployments/select_install_type.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/deployments/self_managed_deployments/select_install_type.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_access_keys.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_access_keys.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_subnets.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_subnets.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_vpc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_aws_vpc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_cross_account_role.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_configure_cross_account_role.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_select_aws_region.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_configure_engine_select_aws_region.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_define_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_define_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_review_and_activate_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_review_and_activate_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/aws_environments/creation_share_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/aws_environments/creation_share_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_credentials.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_credentials.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_region.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_region.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_subnet.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_subnet.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_vnet.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_configure_azure_vnet.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_defaults_azure_vm_instances.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_configure_engine_defaults_azure_vm_instances.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_define_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_define_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/azure_environments/creation_review_and_activate_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/azure_environments/creation_review_and_activate_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_impersonation.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_impersonation.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_key.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_credentials_service_account_key.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_configure_gcp_project.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_configure_gcp_project.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_define_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_define_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_review_and_activate.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_review_and_activate.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_select_gcp_vpc.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_select_gcp_vpc.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/gcp_environments/creation_share_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/gcp_environments/creation_share_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/managing_environments/managing_environments.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/managing_environments/managing_environments.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_define_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_define_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_review_and_activate.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_review_and_activate.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/images/set_up/environments/self_managed_environments/creation_share_environment.png` & `streamsets-5.2.0b3/docs/_static/images/set_up/environments/self_managed_environments/creation_share_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sample_fragment.png` & `streamsets-5.2.0b3/docs/_static/sample_fragment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sample_pipeline_using_fragment.png` & `streamsets-5.2.0b3/docs/_static/sample_pipeline_using_fragment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sdk_sample_pipeline1.png` & `streamsets-5.2.0b3/docs/_static/sdk_sample_pipeline1.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_deployment.png` & `streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_deployment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_deployment_details.png` & `streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_deployment_details.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/sdk_sample_self_managed_environment.png` & `streamsets-5.2.0b3/docs/_static/sdk_sample_self_managed_environment.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/_static/streamsets-logo.png` & `streamsets-5.2.0b3/docs/_static/streamsets-logo.png`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/api/sch_api.rst` & `streamsets-5.2.0b3/docs/api/sch_api.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/build/creating_pipelines.rst` & `streamsets-5.2.0b3/docs/build/creating_pipelines.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/build/pipeline_fragments.rst` & `streamsets-5.2.0b3/docs/build/pipeline_fragments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/conf.py` & `streamsets-5.2.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/index.rst` & `streamsets-5.2.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/authentication.rst` & `streamsets-5.2.0b3/docs/learn/authentication.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/examples/sdk_examples_job_pipeline.rst` & `streamsets-5.2.0b3/docs/learn/examples/sdk_examples_job_pipeline.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/examples/sdk_examples_self_managed_deployment.rst` & `streamsets-5.2.0b3/docs/learn/examples/sdk_examples_self_managed_deployment.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/examples.rst` & `streamsets-5.2.0b3/docs/learn/examples.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/installation.rst` & `streamsets-5.2.0b3/docs/learn/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ============
 |
 
 Using pip
 ---------
 The pip3 package manager must be installed on the machine where the SDK will be installed and used.
 
-To install the 5.2.0b2 release of the library, use your Python 3 installation's instance of `pip`_:
+To install the 5.1.0 release of the library, use your Python 3 installation's instance of `pip`_:
 
 .. code-block:: console
 
     $ pip3 install streamsets~=5.0
 
 .. _pip: https://pip.pypa.io
```

### Comparing `streamsets-5.2.0b2/docs/learn/known_issues.rst` & `streamsets-5.2.0b3/docs/learn/known_issues.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/learn/overview.rst` & `streamsets-5.2.0b3/docs/learn/overview.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/manage/users_and_groups/managing_users_and_groups.rst` & `streamsets-5.2.0b3/docs/manage/users_and_groups/managing_users_and_groups.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/manage/users_and_groups/permissions.rst` & `streamsets-5.2.0b3/docs/manage/users_and_groups/permissions.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/manage/users_and_groups/roles.rst` & `streamsets-5.2.0b3/docs/manage/users_and_groups/roles.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/manage/users_and_groups/users_and_groups.rst` & `streamsets-5.2.0b3/docs/manage/users_and_groups/users_and_groups.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/run/job_templates.rst` & `streamsets-5.2.0b3/docs/run/job_templates.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/run/jobs_instances.rst` & `streamsets-5.2.0b3/docs/run/jobs_instances.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/search/saql_saved_search.rst` & `streamsets-5.2.0b3/docs/search/saql_saved_search.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/search/search_for_object.rst` & `streamsets-5.2.0b3/docs/search/search_for_object.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/azure_vm_deployments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/azure_vm_deployments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/deployments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/deployments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/ec2_deployments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/ec2_deployments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/gce_deployments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/gce_deployments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/self_managed_deployments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/self_managed_deployments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/stage_libs_sdc.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/stage_libs_sdc.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/deployments/stage_libs_st.rst` & `streamsets-5.2.0b3/docs/usage/set_up/deployments/stage_libs_st.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/environments/aws_environments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/environments/aws_environments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/environments/azure_environments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/environments/azure_environments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/environments/gcp_environments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/environments/gcp_environments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/environments/managing_environments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/environments/managing_environments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/docs/usage/set_up/environments/self_managed_environments.rst` & `streamsets-5.2.0b3/docs/usage/set_up/environments/self_managed_environments.rst`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/setup.py` & `streamsets-5.2.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'inflection',
     'PyYAML',
     'requests'
 ]
 
 setup(
     name='streamsets',
-    version='5.2.0b2',
+    version='5.2.0b3',
     description='A Python SDK for StreamSets',
     author='StreamSets Inc.',
     packages=['streamsets.sdk'],
     include_package_data=True,
     install_requires=requirements,
     dependency_links=['https://github.com/streamsets/dpath-python/tarball/master#egg=dpath-1.4.2'],
     python_requires='>=3',
```

### Comparing `streamsets-5.2.0b2/streamsets/sdk/aster_api.py` & `streamsets-5.2.0b3/streamsets/sdk/aster_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,34 +170,14 @@
         if sort_unsorted is not None:
             params.update({'sort.unsorted': sort_unsorted})
         response = self._get(app='security',
                              endpoint='v{}/org-users'.format(self._api_version),
                              params=params)
         return Command(self, response)
 
-    def get_metering_event(self, order_by=None, order=None, page=None, size=None, search=None, with_wrapper=False):
-        """Get raw metering data from the metering app.
-
-        Args:
-            order_by (:obj:`str`, optional): Default: ``None``.
-            order (:obj:`str`, optional): Default: ``None``.
-            page (:obj:`int`, optional): Default: ``None``.
-            size (:obj:`int`, optional): Default: ``None``.
-            search (:obj:`str`, optional): Default: ``None``.
-            with_wrapper (:obj:`bool`, optional): Default: ``False``
-
-        Returns:
-            An instance of :py:class:`streamsets.sdk.aster_api.Command`
-        """
-        params = get_params(parameters=locals(), exclusions='self')
-        response = self._get(app='metering',
-                             endpoint='v{}/event'.format(self._api_version),
-                             params=params)
-        return Command(self, response)
-
     def get_org_user(self, user_id):
         """Get the org-user for the given user ID.
 
         Args:
             user_id (:obj:`str`): User ID
 
         Returns:
```

### Comparing `streamsets-5.2.0b2/streamsets/sdk/exceptions.py` & `streamsets-5.2.0b3/streamsets/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/models.py` & `streamsets-5.2.0b3/streamsets/sdk/models.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sch.py` & `streamsets-5.2.0b3/streamsets/sdk/sch.py`

 * *Files 0% similar despite different names*

```diff
@@ -3215,15 +3215,15 @@
         scala_binary_version = deployment._data['scalaBinaryVersion']
 
         if engine_type == 'DC':
             # The engine_id is used only when engineBuild is not None.
             # Otherwise, it is set to None, not affecting the following query
             if maybe_engine_build:
                 engine_build = maybe_engine_build
-                engine_id = '{}:{}::{}'.format(engine_type, engine_version, engine_build)
+                engine_id = f'{engine_type}:{engine_version}::{engine_build}'
                 logger.info('The deployment has version %s and build %s', engine_version, engine_build)
             else:
                 engine_id = None
 
             engine_version_config = self.engine_configurations.get(
                 engine_type=engine_type,
                 engine_version=engine_version,
@@ -3231,15 +3231,15 @@
                 disabled=False,
             )
         elif engine_type == 'TF':
             # The engine_id is used only when engineBuild is not None.
             # Otherwise, it is set to None, not affecting the following query
             if maybe_engine_build:
                 engine_build = maybe_engine_build
-                engine_id = '{}:{}:{}:{}'.format(engine_type, engine_version, scala_binary_version, engine_build)
+                engine_id = f'{engine_type}:{engine_version}:{scala_binary_version}:{engine_build}'
                 logger.info('The deployment has version %s and build %s', engine_version, engine_build)
             else:
                 engine_id = None
 
             engine_version_config = self.engine_configurations.get(
                 engine_type=engine_type,
                 engine_version=engine_version,
@@ -3371,14 +3371,42 @@
                         [deployment.deployment_name for deployment in enabled_deployments])
             self.stop_deployment(*enabled_deployments)
 
         deployment_ids = [deployment.deployment_id for deployment in deployments]
         logger.info('Deleting deployments %s ...', [deployment.deployment_name for deployment in deployments])
         self.api_client.delete_deployments(deployment_ids)
 
+    def lock_deployment(self, deployment):
+        """Lock deployment.
+
+        Args:
+            deployment: An instance of :py:class:`streamsets.sdk.sch_models.Deployment`.
+        """
+        logger.info('Locking deployment %s ...', deployment.deployment_id)
+        lock_deployment_command = self.api_client.lock_deployment(deployment.deployment_id)
+
+        # Update :py:class:`streamsets.sdk.sch_models.Deployment` with updated data.
+        deployment.refresh()
+
+        return lock_deployment_command
+
+    def unlock_deployment(self, deployment):
+        """Unlock deployment.
+
+        Args:
+            deployment: An instance of :py:class:`streamsets.sdk.sch_models.Deployment`.
+        """
+        logger.info('Unlocking deployment %s ...', deployment.deployment_id)
+        unlock_deployment_command = self.api_client.unlock_deployment(deployment.deployment_id)
+
+        # Update :py:class:`streamsets.sdk.sch_models.Deployment` with updated data.
+        deployment.refresh()
+
+        return unlock_deployment_command
+
     def get_self_managed_deployment_install_script(self, deployment, install_mechanism='DEFAULT'):
         """Get install script for a Self Managed deployment.
 
         Args:
             deployment (:py:class:`streamsets.sdk.sch_models.Deployment`): deployment object.
             install_mechanism (:obj:`str`, optional): Possible values for install are "DEFAULT", "BACKGROUND" and
                                                       "FOREGROUND". Default: ``DEFAULT``
```

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sch_api.py` & `streamsets-5.2.0b3/streamsets/sdk/sch_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 DEFAULT_SCH_API_VERSION = 1  #:
 DEFAULT_SDP_API_VERSION = 2  #:
 DEFAULT_METERING_API_VERSION = 3  #:
 
 DEFAULT_ASTER_URL = 'https://cloud.login.streamsets.com/'
 # Any headers that DPM requires for all calls should be added to this dictionary.
 REQUIRED_HEADERS = {'X-Requested-By': 'sch',
-                    'X-SS-Sdk-Version': 'SDK 5.2.0',
+                    'X-SS-Sdk-Version': 'SDK 5.2.0b3',
                     'X-SS-REST-CALL': 'true',
                     'content-type': 'application/json'}
 
 
 class ApiClient(object):
     """
     API client to communicate with a ControlHub instance.
@@ -6264,14 +6264,40 @@
             An instance of :py:class:`streamsets.sdk.sch_api.Command`.
         """
         response = self._post(app='provisioning',
                               endpoint='/v{}/csp/deployments/disableDeployments'.format(self.api_version),
                               data=deployment_ids)
         return Command(self, response)
 
+    def lock_deployment(self, deployment_id):
+        """Lock the deployment for the given deployment ID.
+
+        Args:
+            deployment_id (:obj:`str`): Id of the deployment.
+
+        Returns:
+            An instance of :py:class:`streamsets.sdk.sch_api.Command`.
+        """
+        response = self._post(app='provisioning',
+                              endpoint='/v{}/csp/deployment/{}/lock'.format(self.api_version, deployment_id))
+        return Command(self, response)
+
+    def unlock_deployment(self, deployment_id):
+        """Unlock the deployment for the given deployment ID.
+
+        Args:
+            deployment_id (:obj:`str`): Id of the deployment.
+
+        Returns:
+            An instance of :py:class:`streamsets.sdk.sch_api.Command`.
+        """
+        response = self._post(app='provisioning',
+                              endpoint='/v{}/csp/deployment/{}/unlock'.format(self.api_version, deployment_id))
+        return Command(self, response)
+
     def wait_for_deployment_status(self, deployment_id, status, timeout_sec=900):
         """Block until a deployment reaches the desired status.
 
         Args:
             deployment_id (:obj:`str`): The deployment id.
             status (:obj:`str`): The desired status to wait for.
             timeout_sec (:obj:`int`, optional): Timeout to wait for ``deployment`` to reach ``status``, in seconds.
@@ -7488,15 +7514,15 @@
                 if status == 'RUNNING':
                     return True
 
         def success(time):
             logger.debug('Job reached desired state after %s s.', time)
 
         def failure(timeout):
-            raise TimeoutError('Timed out after {} seconds while waiting for pipeline job status.'.format(timeout))
+            raise TimeoutError('Timed out after {} seconds while waiting for status.'.format(timeout))
 
         # Actual execution of code starts here.
         for job in self.jobs:
             if job.executor_type != 'SNOWPARK':
                 logger.debug('Waiting for %s pipeline %s ...', job.number_of_instances,
                              'instances' if job.number_of_instances > 1 else 'instance')
                 wait_for_condition(all_pipeline_instances_running, [job], timeout=timeout_sec, success=success, failure=failure)
```

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sch_models.py` & `streamsets-5.2.0b3/streamsets/sdk/sch_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4271,15 +4271,15 @@
         """
         topology_node_json = {'nodeType': None, 'instanceName': None, 'library': None, 'stageName': None,
                               'stageVersion': None, 'jobId': None, 'pipelineId': None, 'pipelineCommitId': None,
                               'pipelineVersion': None, 'inputLanes': [], 'outputLanes': [], 'uiInfo': {}}
         try:
             system = next(system for system in ALL_TOPOLOGY_SYSTEMS if system['label'] == name)
         except StopIteration:
-            raise TopologyIssuesError('No system found with the name {}.'.format(name))
+            raise TopologyIssuesError(f'No system found with the name "{name}".')
         topology_nodes = (self._topology['topologyDefinition']['topologyNodes']
                           if 'topologyDefinition' in self._topology else {})
         x_pos = 100
         y_pos = 50
 
         for topology_node in topology_nodes:
             if topology_node['uiInfo']['xPos'] >= x_pos:
@@ -5806,16 +5806,16 @@
         """
         allow_snapshot_engine_versions = kwargs.get('allow_nightly_engine_builds') or kwargs.get('allow_nightly_builds')
         self._environment.update({'name': environment_name,
                                   'allowSnapshotEngineVersions': allow_snapshot_engine_versions})
         # if Kubernetes, make the agent attribute a dictionary to be extended later
         if self._environment['type'] == 'KUBERNETES':
             self._environment.update({'agent': {'extraJvmOpts': '',
-                                                'kubernetes_labels': '',
-                                                'kubernetes_namespace': ''}})
+                                                'kubernetesLabels': '',
+                                                'namespace': ''}})
         environment = Environment(self._environment, self._control_hub)
         if kwargs.get('environment_tags'):
             environment.tags = kwargs.get('environment_tags')
         return environment
 
 
 class Engine(BaseModel):
@@ -8650,27 +8650,40 @@
             body (:obj:`str`, optional): Body of the email. Default: ``None``.
         """
         params = get_params(parameters=locals(), exclusions=('self', ))
         self._action.update({'eventType': 'EMAIL',
                              'config': params})
 
     def set_webhook_action(self, uri, method='GET', content_type=None, payload=None, auth_type=None, username=None,
-                           password=None, timeout=30000, headers=None):
+                           password=None, timeout=30000, headers=None, bearer_token=None, api_key_key=None,
+                           api_key_value=None, api_key_location=None, token_url=None, client_id=None,
+                           client_secret=None, scope=None, location=None, resources=None, audiences=None):
         """Set the Webhook action.
 
         Args:
             uri (:obj:`str`): URI for the Webhook.
             method (:obj:`str`, optional): HTTP method to use. Default: ``'GET'``.
             content_type (:obj:`str`, optional): Content Type of the request. Default:  ``None``.
             payload (:obj:`str`, optional): Payload of the request. Default:  ``None``.
             auth_type (:obj:`str`, optional): ``'basic'`` or ``None``. Default: ``None``.
-            username (:obj:`str`, optional): username for the authentication. Default: ``None``.
-            password (:obj:`str`, optional): password for the authentication. Default: ``None``.
-            timeout (:obj:`int`, optional): timeout for the Webhook action. Default: ``30000``.
+            username (:obj:`str`, optional): Username for the authentication. Default: ``None``.
+            password (:obj:`str`, optional): Password for the authentication. Default: ``None``.
+            timeout (:obj:`int`, optional): Timeout for the Webhook action. Default: ``30000``.
             headers (:obj:`dict`, optional): Headers to be sent to the Webhook call. Default: ``None``.
+            bearer_token (:obj:`str`, optional): Bearer token for the authentication. Default: ``None``.
+            token_url: (:obj:`str`, optional): Token URL for the authentication. Default: ``None``.
+            api_key_key (:obj:`str`, optional): API key name for the authentication. Default: ``None``.
+            api_key_value (:obj:`str`, optional): API key value for the authentication. Default: ``None``.
+            api_key_location (:obj:`str`, optional): Where to send the api key values. Default: ``None``.
+            audiences: (:obj:`list`, optional): Audiences for OAuth2 auth method. Default: ``None``.
+            resources: (:obj:`list`, optional): Resources for OAuth2 auth method.  Default: ``None``.
+            location: (:obj:`str`, optional): Location of OAuth2 credentials (body or header). Default: ``None``.
+            scope: (:obj:`str`, optional): Scope for OAuth2 auth method. Default: ``None``.
+            client_secret: (:obj:`str`, optional): Client secret for OAuth2 auth method. Default: ``None``.
+            client_id: (:obj:`str`, optional): Client id for OAuth2 auth method. Default: ``None``.
         """
         params = get_params(parameters=locals(), exclusions=('self', ))
         if auth_type is None:
             params['authType'] = "none"
         self._action.update({'eventType': 'WEBHOOKV1',
                              'config': params})
```

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sdc.py` & `streamsets-5.2.0b3/streamsets/sdk/sdc.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sdc_api.py` & `streamsets-5.2.0b3/streamsets/sdk/sdc_api.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/sdc_models.py` & `streamsets-5.2.0b3/streamsets/sdk/sdc_models.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/st.py` & `streamsets-5.2.0b3/streamsets/sdk/st.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/st_api.py` & `streamsets-5.2.0b3/streamsets/sdk/st_api.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/st_models.py` & `streamsets-5.2.0b3/streamsets/sdk/st_models.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets/sdk/utils.py` & `streamsets-5.2.0b3/streamsets/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `streamsets-5.2.0b2/streamsets.egg-info/SOURCES.txt` & `streamsets-5.2.0b3/streamsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

