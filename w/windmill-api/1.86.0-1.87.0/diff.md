# Comparing `tmp/windmill_api-1.86.0.tar.gz` & `tmp/windmill_api-1.87.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.86.0.tar", max compression
+gzip compressed data, was "windmill_api-1.87.0.tar", max compression
```

## Comparing `windmill_api-1.86.0.tar` & `windmill_api-1.87.0.tar`

### file list

```diff
@@ -1,1241 +1,1241 @@
--rw-r--r--   0        0        0    11348 2023-04-08 20:03:14.828319 windmill_api-1.86.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-04-08 20:03:14.832320 windmill_api-1.86.0/README.md
--rw-r--r--   0        0        0      717 2023-04-08 20:03:14.828319 windmill_api-1.86.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-08 20:02:44.203774 windmill_api-1.86.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-04-08 20:02:44.679783 windmill_api-1.86.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.783784 windmill_api-1.86.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-04-08 20:02:54.755963 windmill_api-1.86.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-04-08 20:02:54.747963 windmill_api-1.86.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-04-08 20:02:54.779964 windmill_api-1.86.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-04-08 20:02:54.807964 windmill_api-1.86.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-04-08 20:02:54.819965 windmill_api-1.86.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3031 2023-04-08 20:02:54.847965 windmill_api-1.86.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-04-08 20:02:54.855965 windmill_api-1.86.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-04-08 20:02:54.903966 windmill_api-1.86.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-04-08 20:02:54.891966 windmill_api-1.86.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-04-08 20:02:54.983968 windmill_api-1.86.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-04-08 20:02:54.935967 windmill_api-1.86.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-04-08 20:02:54.963967 windmill_api-1.86.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.719783 windmill_api-1.86.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-08 20:02:55.003968 windmill_api-1.86.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-04-08 20:02:55.095970 windmill_api-1.86.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.835785 windmill_api-1.86.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-08 20:02:55.027968 windmill_api-1.86.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-04-08 20:02:55.055969 windmill_api-1.86.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-04-08 20:02:55.083969 windmill_api-1.86.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.835785 windmill_api-1.86.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-04-08 20:02:55.115970 windmill_api-1.86.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-04-08 20:02:55.119970 windmill_api-1.86.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.775784 windmill_api-1.86.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     1789 2023-04-08 20:02:55.147971 windmill_api-1.86.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-04-08 20:02:55.147971 windmill_api-1.86.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-04-08 20:02:55.175971 windmill_api-1.86.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-04-08 20:02:55.183971 windmill_api-1.86.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-04-08 20:02:55.215972 windmill_api-1.86.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     2667 2023-04-08 20:02:55.243972 windmill_api-1.86.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-04-08 20:02:55.259972 windmill_api-1.86.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-04-08 20:02:55.335974 windmill_api-1.86.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-04-08 20:02:55.291973 windmill_api-1.86.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-04-08 20:02:55.319974 windmill_api-1.86.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.827785 windmill_api-1.86.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-08 20:02:55.355974 windmill_api-1.86.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-04-08 20:02:55.359974 windmill_api-1.86.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-04-08 20:02:55.383975 windmill_api-1.86.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-04-08 20:02:55.399975 windmill_api-1.86.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-04-08 20:02:55.423975 windmill_api-1.86.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-04-08 20:02:55.443976 windmill_api-1.86.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-04-08 20:02:55.479976 windmill_api-1.86.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-04-08 20:02:55.471976 windmill_api-1.86.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-04-08 20:02:55.499977 windmill_api-1.86.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.831786 windmill_api-1.86.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-04-08 20:02:55.527977 windmill_api-1.86.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-04-08 20:02:55.579978 windmill_api-1.86.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-04-08 20:02:55.559978 windmill_api-1.86.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.819785 windmill_api-1.86.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-04-08 20:02:55.611979 windmill_api-1.86.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-04-08 20:02:55.607979 windmill_api-1.86.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-04-08 20:02:55.631979 windmill_api-1.86.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-04-08 20:02:55.651979 windmill_api-1.86.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-04-08 20:02:55.679980 windmill_api-1.86.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-04-08 20:02:55.707980 windmill_api-1.86.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-04-08 20:02:55.707980 windmill_api-1.86.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-04-08 20:02:55.735981 windmill_api-1.86.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.791785 windmill_api-1.86.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-04-08 20:02:55.743981 windmill_api-1.86.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-04-08 20:02:55.775982 windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-08 20:02:55.795982 windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-04-08 20:02:55.807982 windmill_api-1.86.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-04-08 20:02:55.835983 windmill_api-1.86.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-04-08 20:02:55.835983 windmill_api-1.86.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-04-08 20:02:55.875983 windmill_api-1.86.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:55.863983 windmill_api-1.86.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-04-08 20:02:55.915984 windmill_api-1.86.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-04-08 20:02:55.931984 windmill_api-1.86.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-04-08 20:02:55.963985 windmill_api-1.86.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-04-08 20:02:56.007986 windmill_api-1.86.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    12602 2023-04-08 20:02:56.099987 windmill_api-1.86.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    11829 2023-04-08 20:02:56.139988 windmill_api-1.86.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12367 2023-04-08 20:02:56.263990 windmill_api-1.86.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-04-08 20:02:56.171989 windmill_api-1.86.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-04-08 20:02:56.199989 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-04-08 20:02:56.243990 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-08 20:02:56.287991 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-04-08 20:02:56.319991 windmill_api-1.86.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-04-08 20:02:56.351992 windmill_api-1.86.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-04-08 20:02:56.371992 windmill_api-1.86.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-04-08 20:02:56.407993 windmill_api-1.86.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-04-08 20:02:56.407993 windmill_api-1.86.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-04-08 20:02:56.447993 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-04-08 20:02:56.451994 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-04-08 20:02:56.499994 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.747784 windmill_api-1.86.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-08 20:02:56.491994 windmill_api-1.86.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-04-08 20:02:56.519995 windmill_api-1.86.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-04-08 20:02:56.527995 windmill_api-1.86.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-04-08 20:02:56.543995 windmill_api-1.86.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-04-08 20:02:56.555995 windmill_api-1.86.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-04-08 20:02:56.567996 windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-04-08 20:02:56.591996 windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-04-08 20:02:56.615996 windmill_api-1.86.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.755784 windmill_api-1.86.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-08 20:02:56.623997 windmill_api-1.86.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-04-08 20:02:56.639997 windmill_api-1.86.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:56.651997 windmill_api-1.86.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-04-08 20:02:56.667997 windmill_api-1.86.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-04-08 20:02:56.707998 windmill_api-1.86.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-04-08 20:02:56.707998 windmill_api-1.86.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-04-08 20:02:56.747999 windmill_api-1.86.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-04-08 20:02:56.743999 windmill_api-1.86.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-04-08 20:02:56.771999 windmill_api-1.86.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-04-08 20:02:56.816000 windmill_api-1.86.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-04-08 20:02:56.812000 windmill_api-1.86.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-04-08 20:02:56.848001 windmill_api-1.86.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-04-08 20:02:56.848001 windmill_api-1.86.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-04-08 20:02:56.876001 windmill_api-1.86.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-04-08 20:02:56.880001 windmill_api-1.86.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.815785 windmill_api-1.86.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-08 20:02:56.908002 windmill_api-1.86.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:56.904002 windmill_api-1.86.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-04-08 20:02:56.944002 windmill_api-1.86.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-04-08 20:02:56.964003 windmill_api-1.86.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-04-08 20:02:57.000003 windmill_api-1.86.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-04-08 20:02:57.008003 windmill_api-1.86.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-04-08 20:02:57.048004 windmill_api-1.86.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-04-08 20:02:57.036004 windmill_api-1.86.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.763784 windmill_api-1.86.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-08 20:02:57.080005 windmill_api-1.86.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-04-08 20:02:57.072005 windmill_api-1.86.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-08 20:02:57.112005 windmill_api-1.86.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-04-08 20:02:57.108005 windmill_api-1.86.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-04-08 20:02:57.152006 windmill_api-1.86.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-04-08 20:02:57.148006 windmill_api-1.86.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-08 20:02:57.184007 windmill_api-1.86.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-04-08 20:02:57.200007 windmill_api-1.86.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-04-08 20:02:57.224007 windmill_api-1.86.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-04-08 20:02:57.228007 windmill_api-1.86.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-04-08 20:02:57.264008 windmill_api-1.86.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-04-08 20:02:57.288008 windmill_api-1.86.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3276 2023-04-08 20:02:57.304009 windmill_api-1.86.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-04-08 20:02:57.324009 windmill_api-1.86.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-04-08 20:02:57.352009 windmill_api-1.86.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-04-08 20:02:57.348009 windmill_api-1.86.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-04-08 20:02:57.476012 windmill_api-1.86.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-04-08 20:02:57.388010 windmill_api-1.86.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.412011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.440011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-04-08 20:02:57.468011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.691783 windmill_api-1.86.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-08 20:02:57.492012 windmill_api-1.86.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-04-08 20:02:57.504012 windmill_api-1.86.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.719783 windmill_api-1.86.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-08 20:02:57.516013 windmill_api-1.86.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-04-08 20:02:57.532013 windmill_api-1.86.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-04-08 20:02:57.544013 windmill_api-1.86.0/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-04-08 20:02:57.560013 windmill_api-1.86.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-04-08 20:02:57.568013 windmill_api-1.86.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-04-08 20:02:57.584014 windmill_api-1.86.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-04-08 20:02:57.596014 windmill_api-1.86.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-04-08 20:02:57.612014 windmill_api-1.86.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-04-08 20:02:57.616014 windmill_api-1.86.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-04-08 20:02:57.660015 windmill_api-1.86.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-04-08 20:02:57.644015 windmill_api-1.86.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-04-08 20:02:57.684015 windmill_api-1.86.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-04-08 20:02:57.692016 windmill_api-1.86.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-04-08 20:02:57.724016 windmill_api-1.86.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-04-08 20:02:57.720016 windmill_api-1.86.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-04-08 20:02:57.764017 windmill_api-1.86.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-04-08 20:02:57.760017 windmill_api-1.86.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-04-08 20:02:57.800017 windmill_api-1.86.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-04-08 20:02:57.816018 windmill_api-1.86.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-04-08 20:02:57.840018 windmill_api-1.86.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.844018 windmill_api-1.86.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-04-08 20:02:57.872019 windmill_api-1.86.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-04-08 20:02:57.864019 windmill_api-1.86.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-04-08 20:02:57.892019 windmill_api-1.86.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-04-08 20:02:57.900019 windmill_api-1.86.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-04-08 20:02:57.924020 windmill_api-1.86.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-04-08 20:02:57.944020 windmill_api-1.86.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.743784 windmill_api-1.86.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-08 20:02:57.960020 windmill_api-1.86.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.972020 windmill_api-1.86.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-04-08 20:02:58.044022 windmill_api-1.86.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-04-08 20:02:58.040022 windmill_api-1.86.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-04-08 20:02:58.080022 windmill_api-1.86.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-04-08 20:02:58.080022 windmill_api-1.86.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-04-08 20:02:58.116023 windmill_api-1.86.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.831786 windmill_api-1.86.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     3896 2023-04-08 20:02:58.140024 windmill_api-1.86.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-04-08 20:02:44.735784 windmill_api-1.86.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-08 20:02:58.144024 windmill_api-1.86.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-04-08 20:02:58.164024 windmill_api-1.86.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.168024 windmill_api-1.86.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-04-08 20:02:58.196025 windmill_api-1.86.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-04-08 20:02:58.192024 windmill_api-1.86.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-04-08 20:02:58.220025 windmill_api-1.86.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-04-08 20:02:58.228025 windmill_api-1.86.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-04-08 20:02:58.248026 windmill_api-1.86.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.256026 windmill_api-1.86.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.276026 windmill_api-1.86.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-04-08 20:02:58.304026 windmill_api-1.86.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-04-08 20:02:58.312027 windmill_api-1.86.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-04-08 20:02:58.336027 windmill_api-1.86.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-04-08 20:02:58.360027 windmill_api-1.86.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-04-08 20:02:58.396028 windmill_api-1.86.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-04-08 20:02:58.392028 windmill_api-1.86.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-04-08 20:02:58.428029 windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-04-08 20:02:58.448029 windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-04-08 20:02:58.452029 windmill_api-1.86.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-04-08 20:02:58.476029 windmill_api-1.86.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-04-08 20:03:14.824319 windmill_api-1.86.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-08 20:02:58.504030 windmill_api-1.86.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-04-08 20:02:58.528030 windmill_api-1.86.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-04-08 20:02:53.875948 windmill_api-1.86.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-04-08 20:02:58.552031 windmill_api-1.86.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-04-08 20:02:58.584031 windmill_api-1.86.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-04-08 20:02:58.596032 windmill_api-1.86.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-04-08 20:02:58.632032 windmill_api-1.86.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-04-08 20:02:53.795946 windmill_api-1.86.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-04-08 20:02:58.640032 windmill_api-1.86.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-04-08 20:02:58.680033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-04-08 20:02:53.263937 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-04-08 20:02:58.664033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-04-08 20:02:58.688033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     6879 2023-04-08 20:02:58.788035 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-04-08 20:02:58.708034 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-04-08 20:02:53.459940 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-04-08 20:02:53.915948 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-04-08 20:02:58.728034 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-04-08 20:02:58.772035 windmill_api-1.86.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-04-08 20:02:53.383939 windmill_api-1.86.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-04-08 20:02:53.291937 windmill_api-1.86.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-04-08 20:02:58.796035 windmill_api-1.86.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-04-08 20:02:58.828036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-08 20:02:58.852036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-08 20:02:53.355939 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-08 20:02:58.856036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-08 20:02:58.876037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-08 20:02:58.888037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-08 20:02:58.912037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-08 20:02:53.151935 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-08 20:02:58.916037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-08 20:02:58.944038 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-08 20:02:53.831947 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-08 20:02:58.940038 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-08 20:02:53.119934 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-04-08 20:02:58.976038 windmill_api-1.86.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-04-08 20:02:58.996039 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.056040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.036039 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.060040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.092040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.088040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.467940 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-08 20:02:59.116041 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.571942 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-08 20:02:59.152042 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-08 20:02:59.144041 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-08 20:02:54.127952 windmill_api-1.86.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-04-08 20:02:59.180042 windmill_api-1.86.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-04-08 20:02:59.184042 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.256043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.224043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.252043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.296044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.284044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.383939 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-08 20:02:59.312044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:54.007950 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-08 20:02:59.328045 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-08 20:02:59.356045 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-08 20:02:59.412046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-04-08 20:02:59.392046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-08 20:02:59.420046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-08 20:02:59.444047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-08 20:02:59.448047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-08 20:02:59.472047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-08 20:02:53.251937 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-08 20:02:59.476047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-08 20:02:59.504048 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-08 20:02:53.651944 windmill_api-1.86.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-04-08 20:02:59.516048 windmill_api-1.86.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-08 20:02:59.548048 windmill_api-1.86.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10376 2023-04-08 20:02:59.640050 windmill_api-1.86.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-04-08 20:02:59.568049 windmill_api-1.86.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-04-08 20:02:59.608049 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-04-08 20:02:59.692051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-04-08 20:02:59.668051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-04-08 20:02:59.720051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-04-08 20:02:53.847947 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-04-08 20:02:59.720051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-04-08 20:02:59.752052 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-04-08 20:02:53.451940 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-04-08 20:02:59.804053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-04-08 20:02:59.776053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-04-08 20:02:59.804053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-04-08 20:02:53.895948 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-04-08 20:02:59.828053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-04-08 20:02:59.844054 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-04-08 20:02:59.860054 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-04-08 20:02:53.407940 windmill_api-1.86.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-04-08 20:02:59.916055 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.936055 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.956056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.964056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.988056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.992056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.647944 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-08 20:03:00.020057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:54.127952 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-08 20:03:00.020057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-08 20:03:00.048057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-04-08 20:03:00.120059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-04-08 20:03:00.088058 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-04-08 20:03:00.116058 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-04-08 20:03:00.152059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-04-08 20:03:00.148059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-04-08 20:02:54.107952 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-04-08 20:03:00.172059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-04-08 20:02:53.287937 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-04-08 20:03:00.184060 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-04-08 20:03:00.200060 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-04-08 20:03:00.212060 windmill_api-1.86.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-04-08 20:03:00.236061 windmill_api-1.86.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-04-08 20:03:00.236061 windmill_api-1.86.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-04-08 20:03:00.264061 windmill_api-1.86.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-04-08 20:03:00.268061 windmill_api-1.86.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2035 2023-04-08 20:03:00.312062 windmill_api-1.86.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-08 20:03:00.316062 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:00.348063 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-08 20:03:00.332062 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-08 20:03:00.376063 windmill_api-1.86.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-08 20:03:00.372063 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-08 20:03:00.412064 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-08 20:03:00.480065 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-08 20:03:00.452064 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-08 20:03:00.480065 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-08 20:03:00.516066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-08 20:03:00.508066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.583943 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-08 20:03:00.536066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:54.099952 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-08 20:03:00.548066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-08 20:03:00.564067 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-08 20:03:00.628068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-08 20:03:00.600067 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-08 20:03:00.628068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-08 20:03:00.680069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-08 20:03:00.656068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-08 20:02:53.671944 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-08 20:03:00.688069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-08 20:02:53.779946 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:00.708069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-08 20:03:00.716069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2126 2023-04-08 20:03:00.744070 windmill_api-1.86.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-04-08 20:03:00.740069 windmill_api-1.86.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     2094 2023-04-08 20:03:00.772070 windmill_api-1.86.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-04-08 20:03:00.776070 windmill_api-1.86.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-04-08 20:03:00.832071 windmill_api-1.86.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-04-08 20:03:00.816071 windmill_api-1.86.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:00.836071 windmill_api-1.86.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     4616 2023-04-08 20:03:00.896072 windmill_api-1.86.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-04-08 20:02:53.647944 windmill_api-1.86.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-04-08 20:02:53.399939 windmill_api-1.86.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:00.864072 windmill_api-1.86.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-04-08 20:03:00.900072 windmill_api-1.86.0/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-04-08 20:03:00.928073 windmill_api-1.86.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-04-08 20:03:00.936073 windmill_api-1.86.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-08 20:03:00.952073 windmill_api-1.86.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-04-08 20:03:00.976074 windmill_api-1.86.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-04-08 20:03:00.992074 windmill_api-1.86.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-04-08 20:03:01.004074 windmill_api-1.86.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-04-08 20:03:01.016075 windmill_api-1.86.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-04-08 20:03:01.028075 windmill_api-1.86.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    10978 2023-04-08 20:03:01.184077 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-04-08 20:03:01.064075 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-04-08 20:03:01.108076 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-04-08 20:03:01.196078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-04-08 20:03:01.208078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-04-08 20:03:01.224078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-04-08 20:03:01.232078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-04-08 20:03:01.264079 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-04-08 20:02:53.995950 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-04-08 20:03:01.312080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-04-08 20:03:01.288079 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-04-08 20:03:01.320080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-04-08 20:02:53.947949 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-04-08 20:03:01.340080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-04-08 20:03:01.360081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-04-08 20:02:54.151953 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-04-08 20:03:01.372081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-04-08 20:02:54.111952 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-04-08 20:03:01.408081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-04-08 20:03:01.460082 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-04-08 20:03:01.476083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-04-08 20:03:01.492083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-04-08 20:03:01.508083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-04-08 20:03:01.560084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.211936 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-08 20:03:01.540084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.843947 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-04-08 20:03:01.572084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-04-08 20:03:01.588085 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-04-08 20:03:01.656086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-04-08 20:03:01.624085 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-04-08 20:03:01.652086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-04-08 20:03:01.684086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-04-08 20:03:01.684086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.291937 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-04-08 20:03:01.712087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.751946 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-04-08 20:03:01.716087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-04-08 20:03:01.736087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-04-08 20:03:01.752087 windmill_api-1.86.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     6853 2023-04-08 20:03:01.816089 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-04-08 20:03:01.772088 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-04-08 20:02:53.803947 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-04-08 20:02:54.063951 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-04-08 20:03:01.800088 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-04-08 20:03:01.860089 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-08 20:03:01.876090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-08 20:02:53.531942 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-08 20:03:01.888090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-08 20:03:01.936091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-08 20:03:01.916090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-08 20:03:01.956091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-08 20:03:01.960091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-08 20:03:01.996092 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-08 20:02:53.591943 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-08 20:03:01.984092 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-08 20:02:53.695945 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-04-08 20:03:02.008092 windmill_api-1.86.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-04-08 20:03:02.032092 windmill_api-1.86.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-04-08 20:03:02.036093 windmill_api-1.86.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-04-08 20:03:02.060093 windmill_api-1.86.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-04-08 20:03:02.056093 windmill_api-1.86.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-04-08 20:03:02.080093 windmill_api-1.86.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-04-08 20:03:02.100094 windmill_api-1.86.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-04-08 20:03:02.104094 windmill_api-1.86.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-04-08 20:03:02.132094 windmill_api-1.86.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-04-08 20:03:02.148095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-04-08 20:03:02.152095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-04-08 20:03:02.180095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-04-08 20:03:02.176095 windmill_api-1.86.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-04-08 20:03:02.200096 windmill_api-1.86.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4633 2023-04-08 20:03:02.240096 windmill_api-1.86.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-04-08 20:03:02.244096 windmill_api-1.86.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3416 2023-04-08 20:03:02.316098 windmill_api-1.86.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-04-08 20:03:02.264097 windmill_api-1.86.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-04-08 20:03:02.344098 windmill_api-1.86.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-04-08 20:03:02.352098 windmill_api-1.86.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-04-08 20:03:02.372099 windmill_api-1.86.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-04-08 20:03:02.384099 windmill_api-1.86.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-04-08 20:03:02.404099 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-04-08 20:02:53.303938 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-04-08 20:03:02.412099 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-04-08 20:02:53.307938 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-04-08 20:03:02.432100 windmill_api-1.86.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-04-08 20:03:02.440100 windmill_api-1.86.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3080 2023-04-08 20:03:02.472100 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.476100 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.504101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.243936 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.504101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-04-08 20:03:02.540101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.544102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.564102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.251937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.576102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-04-08 20:03:02.596103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.640103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.624103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:54.043951 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.680104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:54.167953 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-04-08 20:02:53.791946 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-04-08 20:03:02.692104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-04-08 20:03:02.708104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-04-08 20:02:53.315938 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-04-08 20:03:02.720105 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-04-08 20:02:54.131952 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-04-08 20:03:02.792106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-04-08 20:03:02.760105 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:02.788106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-08 20:03:02.816106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-08 20:03:02.824107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.459940 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-08 20:03:02.844107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.971949 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-08 20:03:02.852107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-08 20:03:02.876108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-04-08 20:03:02.888108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-04-08 20:03:02.912108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-08 20:03:02.972109 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-08 20:03:02.952109 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-08 20:03:03.004110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-08 20:03:03.000110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.068111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.591943 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-08 20:03:03.032110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.831947 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-08 20:03:03.064111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-08 20:03:03.092111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-04-08 20:03:03.148112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-04-08 20:03:03.132112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:03.160112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-08 20:03:03.180113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-08 20:03:03.192113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.239936 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-08 20:03:03.204113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-08 20:02:53.719945 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-08 20:03:03.220114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-08 20:03:03.232114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-04-08 20:03:03.260114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-04-08 20:03:03.268114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-08 20:03:03.368116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-08 20:03:03.308115 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-08 20:03:03.332116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-08 20:03:03.364116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.392117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-08 20:03:03.400117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.503941 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-08 20:03:03.456118 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-08 20:03:03.428117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:53.879948 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-04-08 20:03:03.460118 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-04-08 20:03:03.488119 windmill_api-1.86.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-04-08 20:03:03.480118 windmill_api-1.86.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-04-08 20:03:03.520119 windmill_api-1.86.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-04-08 20:03:03.564120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-04-08 20:03:03.560120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-04-08 20:03:03.588120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.596120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-04-08 20:03:03.620121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-04-08 20:03:03.624121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.507941 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-04-08 20:03:03.652121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-04-08 20:03:03.660122 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-04-08 20:03:03.728123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-04-08 20:03:03.696122 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-04-08 20:03:03.728123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-04-08 20:03:03.792124 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-04-08 20:03:03.760123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-04-08 20:03:03.828125 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-08 20:02:53.555942 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-04-08 20:03:03.824124 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-04-08 20:03:03.856125 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-04-08 20:03:03.848125 windmill_api-1.86.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-04-08 20:03:03.888126 windmill_api-1.86.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-04-08 20:03:03.936127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-04-08 20:03:03.912126 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-04-08 20:03:03.940127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-04-08 20:03:03.968127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-04-08 20:03:03.976127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-04-08 20:02:53.243936 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-04-08 20:03:04.052129 windmill_api-1.86.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-04-08 20:03:04.000128 windmill_api-1.86.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-04-08 20:03:04.028128 windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-04-08 20:02:53.515941 windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-04-08 20:03:04.056129 windmill_api-1.86.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-04-08 20:03:04.088129 windmill_api-1.86.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-04-08 20:02:53.979950 windmill_api-1.86.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-04-08 20:03:04.132130 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-04-08 20:03:04.112130 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-04-08 20:03:04.176131 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-04-08 20:02:53.339938 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-04-08 20:03:04.204131 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-04-08 20:03:04.216132 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-04-08 20:02:53.343938 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-04-08 20:03:04.240132 windmill_api-1.86.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-04-08 20:03:04.256132 windmill_api-1.86.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-04-08 20:03:04.316133 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-04-08 20:03:04.296133 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-04-08 20:03:04.328134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-08 20:03:04.348134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-08 20:03:04.356134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-08 20:02:53.351938 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-08 20:03:04.376134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-08 20:03:04.388135 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-08 20:03:04.404135 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-08 20:03:04.464136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-04-08 20:03:04.440136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-08 20:03:04.468136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-08 20:03:04.500137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-08 20:03:04.496137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-08 20:02:54.171953 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-08 20:03:04.524137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-08 20:02:53.611943 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-08 20:03:04.560138 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-08 20:03:04.552138 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-04-08 20:03:04.580138 windmill_api-1.86.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-04-08 20:03:04.580138 windmill_api-1.86.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-04-08 20:03:04.604138 windmill_api-1.86.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-04-08 20:03:04.664140 windmill_api-1.86.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-04-08 20:03:04.632139 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-04-08 20:02:53.811947 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-04-08 20:03:04.660140 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-04-08 20:03:04.744141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-04-08 20:03:04.704140 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-04-08 20:03:04.732141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-08 20:03:04.760141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-08 20:03:04.772142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-08 20:02:53.871948 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-08 20:03:04.788142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-08 20:03:04.800142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-08 20:03:04.816142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-04-08 20:02:53.175935 windmill_api-1.86.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-04-08 20:03:04.852143 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.719945 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-04-08 20:03:04.836143 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-04-08 20:03:04.884144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-04-08 20:02:53.471941 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-04-08 20:03:04.876144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-04-08 20:03:04.896144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-04-08 20:03:04.936144 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-04-08 20:02:54.019950 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-04-08 20:03:04.948145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-04-08 20:03:04.980145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-04-08 20:02:53.923949 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-04-08 20:03:04.976145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-04-08 20:03:04.996146 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-04-08 20:03:05.080147 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-04-08 20:02:53.499941 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-04-08 20:02:53.395939 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-04-08 20:03:05.020146 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    10876 2023-04-08 20:03:05.152148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-04-08 20:03:05.100148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-04-08 20:03:05.140148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-04-08 20:03:05.224150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-04-08 20:03:05.180149 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-04-08 20:03:05.208150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-04-08 20:02:53.763946 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-04-08 20:03:05.236150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-04-08 20:03:05.260150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-04-08 20:02:53.535942 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-04-08 20:03:05.380153 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-04-08 20:03:05.284151 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-08 20:03:05.312151 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-08 20:02:53.727945 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-08 20:03:05.340152 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-08 20:03:05.376152 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-04-08 20:02:53.111934 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-04-08 20:03:05.464154 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-04-08 20:02:54.147953 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-04-08 20:02:54.011950 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-04-08 20:03:05.428153 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-04-08 20:03:05.512155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-04-08 20:03:05.504155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-04-08 20:03:05.532155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-04-08 20:03:05.544155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-04-08 20:03:05.564156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-04-08 20:02:53.467940 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-04-08 20:03:05.576156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-04-08 20:02:54.023950 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-04-08 20:03:05.592156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-04-08 20:03:05.608157 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-04-08 20:03:05.676158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-04-08 20:03:05.648157 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-04-08 20:03:05.680158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-08 20:03:05.708158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-08 20:03:05.748159 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.143935 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-08 20:03:05.736159 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.751946 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-08 20:03:05.772160 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-08 20:03:05.780160 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5083 2023-04-08 20:03:05.896162 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-04-08 20:03:05.796160 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-04-08 20:03:05.816160 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-04-08 20:03:05.860161 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-04-08 20:03:05.940163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-04-08 20:03:05.936163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-04-08 20:03:05.964163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-08 20:03:05.976163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-08 20:03:05.992164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.499941 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-08 20:03:06.008164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.347938 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-08 20:03:06.024164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-08 20:03:06.036164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-04-08 20:03:06.104166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-04-08 20:03:06.076165 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-04-08 20:03:06.148166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-04-08 20:03:06.136166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-04-08 20:03:06.164167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-04-08 20:03:06.180167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:53.891948 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-04-08 20:03:06.192167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-04-08 20:03:06.208167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2010 2023-04-08 20:03:06.288169 windmill_api-1.86.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-04-08 20:03:06.228168 windmill_api-1.86.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-04-08 20:03:06.264168 windmill_api-1.86.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-04-08 20:02:53.363939 windmill_api-1.86.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-04-08 20:03:06.288169 windmill_api-1.86.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-04-08 20:03:06.332170 windmill_api-1.86.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-04-08 20:03:06.308169 windmill_api-1.86.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-04-08 20:03:06.332170 windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-04-08 20:03:06.360170 windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-04-08 20:03:06.364170 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-04-08 20:03:06.400171 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-04-08 20:03:06.380170 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-04-08 20:03:06.424171 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-04-08 20:03:06.488172 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-04-08 20:03:06.464172 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-04-08 20:03:06.492173 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-04-08 20:03:06.572174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-04-08 20:03:06.524173 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.555942 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-04-08 20:03:06.552174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.379939 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-04-08 20:03:06.584174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-04-08 20:03:06.600175 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-04-08 20:03:06.724177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-04-08 20:03:06.640175 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-04-08 20:03:06.668176 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-04-08 20:03:06.700176 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-04-08 20:03:06.732177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-04-08 20:02:53.563942 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-04-08 20:03:06.752177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-04-08 20:02:53.691944 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-04-08 20:03:06.760177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-04-08 20:03:06.784178 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-04-08 20:03:06.800178 windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-04-08 20:02:53.219936 windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1852 2023-04-08 20:03:06.816178 windmill_api-1.86.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-04-08 20:02:53.963949 windmill_api-1.86.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-04-08 20:03:06.836179 windmill_api-1.86.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-04-08 20:03:06.844179 windmill_api-1.86.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-04-08 20:03:06.888180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-04-08 20:03:06.868179 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-04-08 20:03:06.916180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-04-08 20:03:06.912180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-04-08 20:03:06.980181 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-04-08 20:03:06.964181 windmill_api-1.86.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-08 20:03:06.984182 windmill_api-1.86.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-04-08 20:03:07.016182 windmill_api-1.86.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-04-08 20:03:07.012182 windmill_api-1.86.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-04-08 20:03:07.072183 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:07.036182 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.056183 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     6775 2023-04-08 20:03:07.140184 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-08 20:03:07.092183 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.116184 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     6775 2023-04-08 20:03:07.268187 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-08 20:03:07.160185 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-08 20:02:54.027950 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.180185 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-04-08 20:03:07.212185 windmill_api-1.86.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-04-08 20:03:07.264186 windmill_api-1.86.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-04-08 20:03:07.296187 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-04-08 20:03:07.292187 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-04-08 20:03:07.324188 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-04-08 20:03:07.420189 windmill_api-1.86.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.344188 windmill_api-1.86.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-04-08 20:03:07.384189 windmill_api-1.86.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-04-08 20:02:53.275937 windmill_api-1.86.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-04-08 20:03:07.412189 windmill_api-1.86.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-04-08 20:03:07.448190 windmill_api-1.86.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.203936 windmill_api-1.86.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-04-08 20:03:07.460190 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-04-08 20:03:07.512191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-04-08 20:03:07.488191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-04-08 20:03:07.512191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-04-08 20:03:07.540192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-04-08 20:03:07.548192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-04-08 20:02:53.843947 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-04-08 20:03:07.564192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-04-08 20:03:07.584192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-08 20:03:07.588192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.187935 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-04-08 20:03:07.628193 windmill_api-1.86.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-04-08 20:03:07.608193 windmill_api-1.86.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-04-08 20:03:07.640193 windmill_api-1.86.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-04-08 20:02:53.819947 windmill_api-1.86.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     1820 2023-04-08 20:03:07.656194 windmill_api-1.86.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:53.707945 windmill_api-1.86.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-04-08 20:03:07.668194 windmill_api-1.86.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:53.607943 windmill_api-1.86.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-04-08 20:03:07.684194 windmill_api-1.86.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-04-08 20:03:07.696194 windmill_api-1.86.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-04-08 20:02:54.167953 windmill_api-1.86.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-04-08 20:03:07.716195 windmill_api-1.86.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-04-08 20:02:53.531942 windmill_api-1.86.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-04-08 20:03:07.804196 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.315938 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-04-08 20:03:07.780196 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-04-08 20:03:07.832197 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-04-08 20:02:53.875948 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-04-08 20:02:53.871948 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-04-08 20:03:07.828197 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11088 2023-04-08 20:03:07.956199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-04-08 20:03:07.852197 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-04-08 20:03:07.896198 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-04-08 20:03:07.980199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-04-08 20:03:07.980199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-04-08 20:03:08.008200 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-04-08 20:02:53.355939 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-04-08 20:03:08.008200 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-04-08 20:03:08.044201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-04-08 20:02:53.479941 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-04-08 20:03:08.092201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-04-08 20:03:08.068201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-04-08 20:03:08.092201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-04-08 20:02:53.743945 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-04-08 20:03:08.188203 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-04-08 20:03:08.188203 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-04-08 20:03:08.220204 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-04-08 20:02:53.203936 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.483941 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-04-08 20:03:08.236204 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-04-08 20:03:08.300205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-04-08 20:03:08.276205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-04-08 20:03:08.304205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-04-08 20:03:08.332206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-04-08 20:03:08.336206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-04-08 20:02:54.035951 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-04-08 20:03:08.360206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-04-08 20:02:53.559942 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-04-08 20:03:08.364206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-04-08 20:03:08.388207 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-04-08 20:03:08.444208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-04-08 20:03:08.428207 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-04-08 20:03:08.456208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-04-08 20:03:08.476208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-04-08 20:03:08.484208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-04-08 20:02:53.775946 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-04-08 20:03:08.504209 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-04-08 20:02:53.863947 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-04-08 20:03:08.516209 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-04-08 20:03:08.576210 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-04-08 20:03:08.540209 windmill_api-1.86.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     5077 2023-04-08 20:03:08.656211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-08 20:03:08.592210 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     1255 2023-04-08 20:03:08.616211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_schema.py
--rw-r--r--   0        0        0     3297 2023-04-08 20:03:08.656211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value.py
--rw-r--r--   0        0        0     7151 2023-04-08 20:03:08.736213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
--rw-r--r--   0        0        0     3318 2023-04-08 20:03:08.696212 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
--rw-r--r--   0        0        0     1985 2023-04-08 20:03:08.724213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2289 2023-04-08 20:03:08.756213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2187 2023-04-08 20:03:08.768214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.123934 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2054 2023-04-08 20:03:08.780214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.403939 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1978 2023-04-08 20:03:08.796214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2029 2023-04-08 20:03:08.808214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7049 2023-04-08 20:03:08.876216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
--rw-r--r--   0        0        0     3284 2023-04-08 20:03:08.844215 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
--rw-r--r--   0        0        0     1975 2023-04-08 20:03:08.872215 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-08 20:03:08.904216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-08 20:03:08.904216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:53.939949 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-08 20:03:08.988217 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:54.051951 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-08 20:03:08.976217 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-08 20:03:09.008218 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2074 2023-04-08 20:03:09.016218 windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-08 20:03:09.028218 windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-04-08 20:03:09.056219 windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-04-08 20:03:09.044219 windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-04-08 20:03:09.076219 windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-04-08 20:03:09.092219 windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-04-08 20:03:09.108220 windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-04-08 20:03:09.124220 windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-04-08 20:03:09.140220 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-04-08 20:03:09.164221 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-04-08 20:02:53.691944 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     1922 2023-04-08 20:03:09.176221 windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-04-08 20:02:53.327938 windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-04-08 20:03:09.192221 windmill_api-1.86.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    11982 2023-04-08 20:03:09.368224 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-04-08 20:03:09.212221 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-04-08 20:03:09.256222 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-04-08 20:03:09.336224 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-04-08 20:03:09.420225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-08 20:03:09.400225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-08 20:02:53.967949 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-08 20:03:09.428225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-08 20:03:09.452226 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-04-08 20:02:53.323938 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-04-08 20:03:09.512227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-04-08 20:03:09.476226 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-04-08 20:03:09.504227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-04-08 20:02:53.327938 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-04-08 20:03:09.532227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-04-08 20:03:09.544227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-04-08 20:03:09.564228 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-04-08 20:03:09.588228 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-04-08 20:03:09.644229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-04-08 20:03:09.624229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-04-08 20:03:09.652229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-08 20:03:09.676230 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-08 20:03:09.680230 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.687945 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-08 20:03:09.708231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.911949 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-08 20:03:09.760231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-08 20:03:09.736231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-04-08 20:03:09.876233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-04-08 20:03:09.796232 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-04-08 20:03:09.824233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-08 20:03:09.856233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-08 20:03:09.888234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-08 20:03:09.904234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-08 20:02:53.527942 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-08 20:03:09.916234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-08 20:03:09.932235 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-04-08 20:03:09.980235 windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-08 20:03:09.952235 windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-04-08 20:03:09.984235 windmill_api-1.86.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-04-08 20:03:10.036236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-04-08 20:03:10.004236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-04-08 20:03:10.020236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     6768 2023-04-08 20:03:10.104238 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-08 20:03:10.056237 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-04-08 20:02:53.279937 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-04-08 20:03:10.080237 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-04-08 20:03:10.168239 windmill_api-1.86.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-04-08 20:03:10.132238 windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-04-08 20:03:10.160239 windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-04-08 20:03:10.196239 windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-04-08 20:02:53.583943 windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4035 2023-04-08 20:03:10.228240 windmill_api-1.86.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-04-08 20:03:10.292241 windmill_api-1.86.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-04-08 20:03:10.288241 windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-08 20:03:10.308241 windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-04-08 20:03:10.328242 windmill_api-1.86.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-04-08 20:03:10.340242 windmill_api-1.86.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-04-08 20:03:10.360242 windmill_api-1.86.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-04-08 20:03:10.372243 windmill_api-1.86.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-04-08 20:03:10.404243 windmill_api-1.86.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-04-08 20:03:10.392243 windmill_api-1.86.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-04-08 20:03:10.456244 windmill_api-1.86.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:10.424243 windmill_api-1.86.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-04-08 20:03:10.484244 windmill_api-1.86.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:10.476244 windmill_api-1.86.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-04-08 20:03:10.544246 windmill_api-1.86.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-04-08 20:03:10.508245 windmill_api-1.86.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-04-08 20:03:10.536245 windmill_api-1.86.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-04-08 20:03:10.576246 windmill_api-1.86.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-04-08 20:03:10.604247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-04-08 20:02:54.071951 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-04-08 20:03:10.600247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-04-08 20:03:10.624247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-04-08 20:03:10.628247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-04-08 20:03:10.660248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-04-08 20:02:53.179935 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-08 20:03:10.652248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-04-08 20:03:10.688248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-04-08 20:02:53.983950 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-04-08 20:03:10.684248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-04-08 20:02:54.103952 windmill_api-1.86.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-04-08 20:03:10.724249 windmill_api-1.86.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-04-08 20:03:10.708248 windmill_api-1.86.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     2108 2023-04-08 20:03:10.744249 windmill_api-1.86.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-04-08 20:03:10.828251 windmill_api-1.86.0/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-04-08 20:03:10.772250 windmill_api-1.86.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-04-08 20:03:10.808250 windmill_api-1.86.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-04-08 20:03:10.832251 windmill_api-1.86.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-04-08 20:03:10.868251 windmill_api-1.86.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-04-08 20:03:10.956253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-04-08 20:03:10.904252 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-04-08 20:03:10.932253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-04-08 20:03:10.968253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-04-08 20:03:10.984253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-04-08 20:02:53.703945 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-04-08 20:03:10.996254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-04-08 20:02:54.003950 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-04-08 20:03:11.012254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-04-08 20:03:11.024254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-04-08 20:03:11.092255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-04-08 20:03:11.064255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-04-08 20:03:11.092255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-04-08 20:03:11.124256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-04-08 20:03:11.120256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-04-08 20:03:11.148256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-04-08 20:03:11.152256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-04-08 20:03:11.176257 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-08 20:03:11.192257 windmill_api-1.86.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-04-08 20:03:11.196257 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-04-08 20:03:11.236258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-04-08 20:03:11.276258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-04-08 20:03:11.272258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-04-08 20:03:11.376260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-04-08 20:03:11.372260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-04-08 20:03:11.400261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-04-08 20:02:53.743945 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-04-08 20:03:11.404260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-04-08 20:02:53.359938 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-04-08 20:03:11.432261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-04-08 20:03:11.436261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-04-08 20:03:11.512262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-04-08 20:03:11.472262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-04-08 20:03:11.500262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-04-08 20:03:11.532263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-04-08 20:03:11.540263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:54.011950 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-04-08 20:03:11.560263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.159935 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-04-08 20:03:11.568263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-04-08 20:03:11.588264 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-04-08 20:03:11.596264 windmill_api-1.86.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-04-08 20:03:11.624264 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-04-08 20:03:11.624264 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.795946 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-04-08 20:03:11.652265 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-04-08 20:02:53.427940 windmill_api-1.86.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-04-08 20:03:11.664265 windmill_api-1.86.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-04-08 20:03:11.688265 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-04-08 20:03:11.692266 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-04-08 20:02:53.403939 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-04-08 20:03:11.792267 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-04-08 20:03:11.744266 windmill_api-1.86.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-04-08 20:02:53.527942 windmill_api-1.86.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-04-08 20:03:11.768267 windmill_api-1.86.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-04-08 20:03:11.788267 windmill_api-1.86.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2147 2023-04-08 20:03:11.824268 windmill_api-1.86.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-04-08 20:03:11.812268 windmill_api-1.86.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-04-08 20:02:53.339938 windmill_api-1.86.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-04-08 20:03:11.840268 windmill_api-1.86.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-04-08 20:03:11.860268 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-04-08 20:03:11.900269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-04-08 20:02:54.015950 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-04-08 20:03:11.888269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-04-08 20:03:11.912269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-04-08 20:03:11.928270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-04-08 20:03:11.948270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-04-08 20:02:53.391939 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-04-08 20:03:11.952270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-04-08 20:03:12.052272 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-04-08 20:02:53.111934 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-04-08 20:03:11.976271 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-04-08 20:02:53.947949 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11448 2023-04-08 20:03:12.200274 windmill_api-1.86.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-04-08 20:03:12.072272 windmill_api-1.86.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-04-08 20:03:12.112273 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-04-08 20:03:12.196274 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-04-08 20:03:12.220275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-04-08 20:03:12.228275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-04-08 20:02:53.523942 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-04-08 20:03:12.244275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-04-08 20:03:12.264275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-04-08 20:03:12.324277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-04-08 20:03:12.288276 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-04-08 20:03:12.316276 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-04-08 20:02:53.595943 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-04-08 20:03:12.344277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-04-08 20:03:12.356277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-04-08 20:02:53.535942 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-04-08 20:03:12.380277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-04-08 20:02:53.107934 windmill_api-1.86.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.999950 windmill_api-1.86.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-04-08 20:03:12.476279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-04-08 20:03:12.460279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-04-08 20:03:12.500280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-04-08 20:03:12.504279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-04-08 20:03:12.572281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-04-08 20:03:12.532280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.651944 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-04-08 20:03:12.556280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-08 20:02:53.667944 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-04-08 20:03:12.592281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-04-08 20:03:12.596281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-04-08 20:03:12.668282 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-04-08 20:03:12.708283 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-04-08 20:03:12.696283 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-04-08 20:03:12.728284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-04-08 20:03:12.736284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-08 20:02:53.599943 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-04-08 20:03:12.756284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-08 20:02:53.219936 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-04-08 20:03:12.764284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-04-08 20:03:12.784284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-08 20:03:12.804285 windmill_api-1.86.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-04-08 20:03:12.816285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-04-08 20:03:12.832285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-04-08 20:02:53.187935 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-04-08 20:03:12.844285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-04-08 20:02:53.311938 windmill_api-1.86.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-04-08 20:02:53.927949 windmill_api-1.86.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-04-08 20:03:12.860286 windmill_api-1.86.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-04-08 20:03:12.868286 windmill_api-1.86.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-04-08 20:02:54.099952 windmill_api-1.86.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-04-08 20:03:12.888286 windmill_api-1.86.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-04-08 20:03:12.968288 windmill_api-1.86.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-04-08 20:03:12.936287 windmill_api-1.86.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-04-08 20:03:12.952287 windmill_api-1.86.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-04-08 20:03:12.988288 windmill_api-1.86.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-04-08 20:03:12.988288 windmill_api-1.86.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-08 20:03:13.008288 windmill_api-1.86.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-04-08 20:03:13.028288 windmill_api-1.86.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-04-08 20:03:13.036289 windmill_api-1.86.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-04-08 20:03:13.060289 windmill_api-1.86.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-04-08 20:03:13.052289 windmill_api-1.86.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-04-08 20:03:13.084289 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-04-08 20:03:13.080289 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-04-08 20:03:13.120290 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-04-08 20:03:13.164291 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-04-08 20:03:13.160291 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-04-08 20:03:13.260293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-08 20:03:13.196292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-08 20:03:13.224292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:53.887948 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-08 20:03:13.252292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-08 20:02:53.607943 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-08 20:03:13.280293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-08 20:03:13.288293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-04-08 20:03:13.360294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-04-08 20:03:13.328294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-04-08 20:03:13.356294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-04-08 20:03:13.388295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-04-08 20:03:13.388295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-04-08 20:03:13.484296 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-04-08 20:02:53.999950 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-04-08 20:03:13.416295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-04-08 20:03:13.444296 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-04-08 20:03:13.464296 windmill_api-1.86.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-04-08 20:03:13.484296 windmill_api-1.86.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2422 2023-04-08 20:03:13.516297 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-04-08 20:03:13.504297 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-04-08 20:03:13.524297 windmill_api-1.86.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-04-08 20:03:13.540297 windmill_api-1.86.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0     4086 2023-04-08 20:03:13.584298 windmill_api-1.86.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-04-08 20:03:13.560298 windmill_api-1.86.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-04-08 20:03:13.580298 windmill_api-1.86.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     6220 2023-04-08 20:03:13.660299 windmill_api-1.86.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-04-08 20:03:13.600299 windmill_api-1.86.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-04-08 20:03:13.620299 windmill_api-1.86.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-04-08 20:02:53.571942 windmill_api-1.86.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-04-08 20:03:13.644299 windmill_api-1.86.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-04-08 20:03:13.664300 windmill_api-1.86.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-04-08 20:03:13.680300 windmill_api-1.86.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-04-08 20:03:13.696300 windmill_api-1.86.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-04-08 20:03:13.704300 windmill_api-1.86.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-04-08 20:03:13.728301 windmill_api-1.86.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-04-08 20:03:13.736301 windmill_api-1.86.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-04-08 20:02:53.127935 windmill_api-1.86.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-04-08 20:03:13.768301 windmill_api-1.86.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-04-08 20:03:13.776301 windmill_api-1.86.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-04-08 20:03:13.800302 windmill_api-1.86.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-04-08 20:03:13.820302 windmill_api-1.86.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-08 20:03:13.904304 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-08 20:02:53.507941 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:13.844303 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-08 20:03:13.864303 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-08 20:03:13.904304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-08 20:03:13.924304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-08 20:03:13.944304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-08 20:03:14.084307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-08 20:03:13.984305 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-08 20:03:14.012306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-08 20:03:14.044306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-08 20:03:14.072306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-08 20:03:14.100307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-08 20:02:53.763946 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-08 20:03:14.112307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-08 20:03:14.128307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-08 20:03:14.188309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-08 20:03:14.164308 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-08 20:03:14.192309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-08 20:03:14.220309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-08 20:03:14.220309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-08 20:02:53.579943 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-08 20:03:14.248309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-08 20:02:53.167935 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-08 20:03:14.248309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-08 20:03:14.276310 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-04-08 20:03:14.280310 windmill_api-1.86.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-04-08 20:03:14.300310 windmill_api-1.86.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     2036 2023-04-08 20:03:14.312311 windmill_api-1.86.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-04-08 20:03:14.328311 windmill_api-1.86.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-04-08 20:03:14.336311 windmill_api-1.86.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-04-08 20:03:14.356311 windmill_api-1.86.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-08 20:03:14.356311 windmill_api-1.86.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-04-08 20:03:14.452313 windmill_api-1.86.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-04-08 20:03:14.392312 windmill_api-1.86.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-04-08 20:03:14.412312 windmill_api-1.86.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     3799 2023-04-08 20:03:14.556315 windmill_api-1.86.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-04-08 20:03:14.476313 windmill_api-1.86.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-04-08 20:03:14.504314 windmill_api-1.86.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-04-08 20:03:14.532314 windmill_api-1.86.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     3950 2023-04-08 20:03:14.588315 windmill_api-1.86.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-04-08 20:03:14.580315 windmill_api-1.86.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     3939 2023-04-08 20:03:14.636316 windmill_api-1.86.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-04-08 20:03:14.612316 windmill_api-1.86.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-04-08 20:03:14.648316 windmill_api-1.86.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-04-08 20:03:14.668317 windmill_api-1.86.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-04-08 20:03:14.676317 windmill_api-1.86.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-04-08 20:02:44.203774 windmill_api-1.86.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-04-08 20:03:14.684317 windmill_api-1.86.0/windmill_api/types.py
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 windmill_api-1.86.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.86.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-04-11 19:13:28.384709 windmill_api-1.87.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-04-11 19:13:28.388709 windmill_api-1.87.0/README.md
+-rw-r--r--   0        0        0      717 2023-04-11 19:13:28.384709 windmill_api-1.87.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-11 19:12:48.844307 windmill_api-1.87.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 19:12:49.536314 windmill_api-1.87.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.688316 windmill_api-1.87.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-04-11 19:13:01.724438 windmill_api-1.87.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-04-11 19:13:01.732438 windmill_api-1.87.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-04-11 19:13:01.780439 windmill_api-1.87.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-04-11 19:13:01.780439 windmill_api-1.87.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-04-11 19:13:01.836439 windmill_api-1.87.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3031 2023-04-11 19:13:01.832439 windmill_api-1.87.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-04-11 19:13:01.896440 windmill_api-1.87.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-04-11 19:13:01.888440 windmill_api-1.87.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-04-11 19:13:01.936440 windmill_api-1.87.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-04-11 19:13:02.024441 windmill_api-1.87.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-04-11 19:13:01.984440 windmill_api-1.87.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-04-11 19:13:02.024441 windmill_api-1.87.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.588315 windmill_api-1.87.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-04-11 19:13:02.076441 windmill_api-1.87.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-04-11 19:13:02.164442 windmill_api-1.87.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.756316 windmill_api-1.87.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-11 19:13:02.108442 windmill_api-1.87.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-04-11 19:13:02.144442 windmill_api-1.87.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-04-11 19:13:02.180442 windmill_api-1.87.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.756316 windmill_api-1.87.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-04-11 19:13:02.204443 windmill_api-1.87.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-04-11 19:13:02.216443 windmill_api-1.87.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.680316 windmill_api-1.87.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     1789 2023-04-11 19:13:02.244443 windmill_api-1.87.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-04-11 19:13:02.252443 windmill_api-1.87.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-04-11 19:13:02.280444 windmill_api-1.87.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-04-11 19:13:02.304444 windmill_api-1.87.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-04-11 19:13:02.328444 windmill_api-1.87.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     2667 2023-04-11 19:13:02.360444 windmill_api-1.87.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-04-11 19:13:02.380445 windmill_api-1.87.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-04-11 19:13:02.480445 windmill_api-1.87.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-04-11 19:13:02.424445 windmill_api-1.87.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-04-11 19:13:02.464445 windmill_api-1.87.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.744316 windmill_api-1.87.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-11 19:13:02.504446 windmill_api-1.87.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-04-11 19:13:02.516446 windmill_api-1.87.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-04-11 19:13:02.544446 windmill_api-1.87.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-04-11 19:13:02.568446 windmill_api-1.87.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-04-11 19:13:02.596447 windmill_api-1.87.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-04-11 19:13:02.628447 windmill_api-1.87.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-04-11 19:13:02.668448 windmill_api-1.87.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-04-11 19:13:02.664447 windmill_api-1.87.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-04-11 19:13:02.704448 windmill_api-1.87.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.752316 windmill_api-1.87.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-04-11 19:13:02.720448 windmill_api-1.87.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-04-11 19:13:02.788449 windmill_api-1.87.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-04-11 19:13:02.764449 windmill_api-1.87.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.736316 windmill_api-1.87.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-04-11 19:13:02.824449 windmill_api-1.87.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-04-11 19:13:02.824449 windmill_api-1.87.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-04-11 19:13:02.860449 windmill_api-1.87.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-04-11 19:13:02.872449 windmill_api-1.87.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-04-11 19:13:02.920450 windmill_api-1.87.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-04-11 19:13:02.944450 windmill_api-1.87.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-04-11 19:13:02.960451 windmill_api-1.87.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-04-11 19:13:02.984451 windmill_api-1.87.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.696316 windmill_api-1.87.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-11 19:13:03.004451 windmill_api-1.87.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-04-11 19:13:03.036451 windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-11 19:13:03.072452 windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-04-11 19:13:03.084452 windmill_api-1.87.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-04-11 19:13:03.128452 windmill_api-1.87.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-04-11 19:13:03.120452 windmill_api-1.87.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-04-11 19:13:03.176453 windmill_api-1.87.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:03.164452 windmill_api-1.87.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-04-11 19:13:03.220453 windmill_api-1.87.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-04-11 19:13:03.272454 windmill_api-1.87.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-04-11 19:13:03.316454 windmill_api-1.87.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-04-11 19:13:03.344454 windmill_api-1.87.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    12602 2023-04-11 19:13:03.492456 windmill_api-1.87.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    11829 2023-04-11 19:13:03.520456 windmill_api-1.87.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12367 2023-04-11 19:13:03.680458 windmill_api-1.87.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-04-11 19:13:03.560457 windmill_api-1.87.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-04-11 19:13:03.596457 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-04-11 19:13:03.652458 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-11 19:13:03.728458 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-04-11 19:13:03.780459 windmill_api-1.87.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-04-11 19:13:03.780459 windmill_api-1.87.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-04-11 19:13:03.856459 windmill_api-1.87.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-04-11 19:13:03.848460 windmill_api-1.87.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-04-11 19:13:03.904460 windmill_api-1.87.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-04-11 19:13:03.912460 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-04-11 19:13:03.964461 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-04-11 19:13:03.972461 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.632315 windmill_api-1.87.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-11 19:13:04.016461 windmill_api-1.87.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-04-11 19:13:04.008461 windmill_api-1.87.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-04-11 19:13:04.044461 windmill_api-1.87.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-04-11 19:13:04.052461 windmill_api-1.87.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-04-11 19:13:04.080462 windmill_api-1.87.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-04-11 19:13:04.088462 windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-04-11 19:13:04.132462 windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-04-11 19:13:04.128462 windmill_api-1.87.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.636315 windmill_api-1.87.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-11 19:13:04.180463 windmill_api-1.87.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-04-11 19:13:04.168463 windmill_api-1.87.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:04.204463 windmill_api-1.87.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-04-11 19:13:04.216463 windmill_api-1.87.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-04-11 19:13:04.276464 windmill_api-1.87.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-04-11 19:13:04.268464 windmill_api-1.87.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-04-11 19:13:04.324464 windmill_api-1.87.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-04-11 19:13:04.324464 windmill_api-1.87.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-04-11 19:13:04.360465 windmill_api-1.87.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-04-11 19:13:04.420465 windmill_api-1.87.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-04-11 19:13:04.420465 windmill_api-1.87.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-04-11 19:13:04.472466 windmill_api-1.87.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-04-11 19:13:04.460466 windmill_api-1.87.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-04-11 19:13:04.504466 windmill_api-1.87.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-04-11 19:13:04.512466 windmill_api-1.87.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.728316 windmill_api-1.87.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-11 19:13:04.548467 windmill_api-1.87.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:04.548467 windmill_api-1.87.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-04-11 19:13:04.596467 windmill_api-1.87.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-04-11 19:13:04.612467 windmill_api-1.87.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-04-11 19:13:04.688468 windmill_api-1.87.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-04-11 19:13:04.672468 windmill_api-1.87.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-04-11 19:13:04.712468 windmill_api-1.87.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-04-11 19:13:04.728469 windmill_api-1.87.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.660315 windmill_api-1.87.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-04-11 19:13:04.768469 windmill_api-1.87.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-04-11 19:13:04.764469 windmill_api-1.87.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-11 19:13:04.812469 windmill_api-1.87.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-04-11 19:13:04.804469 windmill_api-1.87.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-04-11 19:13:04.860470 windmill_api-1.87.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-04-11 19:13:04.860470 windmill_api-1.87.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-11 19:13:04.912470 windmill_api-1.87.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-04-11 19:13:04.928470 windmill_api-1.87.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-04-11 19:13:04.960471 windmill_api-1.87.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-04-11 19:13:04.968471 windmill_api-1.87.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-04-11 19:13:05.016471 windmill_api-1.87.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-04-11 19:13:05.020471 windmill_api-1.87.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3276 2023-04-11 19:13:05.088472 windmill_api-1.87.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-04-11 19:13:05.068472 windmill_api-1.87.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-04-11 19:13:05.124472 windmill_api-1.87.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-04-11 19:13:05.124472 windmill_api-1.87.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-04-11 19:13:05.316474 windmill_api-1.87.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-04-11 19:13:05.180473 windmill_api-1.87.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.216473 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.252474 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-04-11 19:13:05.292474 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.552314 windmill_api-1.87.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-11 19:13:05.332475 windmill_api-1.87.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-04-11 19:13:05.352475 windmill_api-1.87.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.592315 windmill_api-1.87.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-11 19:13:05.372475 windmill_api-1.87.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-04-11 19:13:05.384475 windmill_api-1.87.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-04-11 19:13:05.412475 windmill_api-1.87.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-04-11 19:13:05.424476 windmill_api-1.87.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-04-11 19:13:05.448476 windmill_api-1.87.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-04-11 19:13:05.460476 windmill_api-1.87.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-04-11 19:13:05.488476 windmill_api-1.87.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-04-11 19:13:05.496476 windmill_api-1.87.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-04-11 19:13:05.520476 windmill_api-1.87.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-04-11 19:13:05.548477 windmill_api-1.87.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-04-11 19:13:05.556477 windmill_api-1.87.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-04-11 19:13:05.588477 windmill_api-1.87.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-04-11 19:13:05.620478 windmill_api-1.87.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-04-11 19:13:05.640478 windmill_api-1.87.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-04-11 19:13:05.656478 windmill_api-1.87.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-04-11 19:13:05.688478 windmill_api-1.87.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-04-11 19:13:05.708478 windmill_api-1.87.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-04-11 19:13:05.744479 windmill_api-1.87.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-04-11 19:13:05.784479 windmill_api-1.87.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-04-11 19:13:05.792479 windmill_api-1.87.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.820479 windmill_api-1.87.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-04-11 19:13:05.828480 windmill_api-1.87.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-04-11 19:13:05.856480 windmill_api-1.87.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-04-11 19:13:05.864480 windmill_api-1.87.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-04-11 19:13:05.900480 windmill_api-1.87.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-04-11 19:13:05.916480 windmill_api-1.87.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-04-11 19:13:05.956481 windmill_api-1.87.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.624315 windmill_api-1.87.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-11 19:13:05.976481 windmill_api-1.87.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.996481 windmill_api-1.87.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-04-11 19:13:06.028482 windmill_api-1.87.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-04-11 19:13:06.080482 windmill_api-1.87.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-04-11 19:13:06.084482 windmill_api-1.87.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-04-11 19:13:06.136483 windmill_api-1.87.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-04-11 19:13:06.132483 windmill_api-1.87.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.752316 windmill_api-1.87.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     3896 2023-04-11 19:13:06.204483 windmill_api-1.87.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:12:49.612315 windmill_api-1.87.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-04-11 19:13:06.176483 windmill_api-1.87.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-04-11 19:13:06.212484 windmill_api-1.87.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.240484 windmill_api-1.87.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-04-11 19:13:06.252484 windmill_api-1.87.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-04-11 19:13:06.272484 windmill_api-1.87.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-04-11 19:13:06.292484 windmill_api-1.87.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-04-11 19:13:06.312485 windmill_api-1.87.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-04-11 19:13:06.332485 windmill_api-1.87.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.344485 windmill_api-1.87.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.368485 windmill_api-1.87.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-04-11 19:13:06.392485 windmill_api-1.87.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-04-11 19:13:06.440486 windmill_api-1.87.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-04-11 19:13:06.424486 windmill_api-1.87.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-04-11 19:13:06.464486 windmill_api-1.87.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-04-11 19:13:06.492486 windmill_api-1.87.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-04-11 19:13:06.520487 windmill_api-1.87.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-04-11 19:13:06.544487 windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-04-11 19:13:06.588487 windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-04-11 19:13:06.580487 windmill_api-1.87.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-04-11 19:13:06.620488 windmill_api-1.87.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-04-11 19:13:28.376709 windmill_api-1.87.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-04-11 19:13:06.652488 windmill_api-1.87.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-04-11 19:13:06.688488 windmill_api-1.87.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-04-11 19:13:06.724489 windmill_api-1.87.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-04-11 19:13:06.772489 windmill_api-1.87.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-04-11 19:13:06.776489 windmill_api-1.87.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-04-11 19:13:06.840490 windmill_api-1.87.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-04-11 19:13:00.512426 windmill_api-1.87.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-04-11 19:13:06.804489 windmill_api-1.87.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-04-11 19:13:06.884490 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-04-11 19:13:06.880490 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-04-11 19:13:06.908491 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     6879 2023-04-11 19:13:06.992491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-04-11 19:13:06.952491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-04-11 19:13:00.080421 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-04-11 19:13:00.664427 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-04-11 19:13:06.984491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-04-11 19:13:07.056492 windmill_api-1.87.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-04-11 19:12:59.984420 windmill_api-1.87.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-04-11 19:12:59.864419 windmill_api-1.87.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-04-11 19:13:07.024492 windmill_api-1.87.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-04-11 19:13:07.072492 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-11 19:13:07.144493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-11 19:12:59.944420 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-11 19:13:07.104493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-11 19:13:07.136493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-11 19:13:07.172493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-11 19:13:07.196493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-11 19:12:59.692417 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-11 19:13:07.200493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-11 19:13:07.248494 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-11 19:13:00.556426 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-11 19:13:07.232494 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-11 19:12:59.648417 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-04-11 19:13:07.276494 windmill_api-1.87.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-04-11 19:13:07.296495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-11 19:13:07.392495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-11 19:13:07.348495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-11 19:13:07.384495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-11 19:13:07.444496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-11 19:13:07.428496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.096421 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-11 19:13:07.460496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.228423 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-11 19:13:07.488496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-11 19:13:07.504497 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-11 19:13:00.932430 windmill_api-1.87.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-04-11 19:13:07.540497 windmill_api-1.87.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-04-11 19:13:07.556497 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-11 19:13:07.652498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-11 19:13:07.604498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-11 19:13:07.640498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-11 19:13:07.684498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-11 19:13:07.692499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:12:59.984420 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-11 19:13:07.720499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.780428 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-11 19:13:07.744499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-11 19:13:07.756499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-11 19:13:07.844500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-04-11 19:13:07.824500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-11 19:13:07.860500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-11 19:13:07.892500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-11 19:13:07.896501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-11 19:13:00.420425 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-11 19:13:07.956501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-11 19:12:59.816419 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-11 19:13:07.932501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-11 19:13:07.972501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-11 19:13:00.328424 windmill_api-1.87.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-04-11 19:13:07.996502 windmill_api-1.87.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-11 19:13:08.000502 windmill_api-1.87.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10376 2023-04-11 19:13:08.180503 windmill_api-1.87.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-04-11 19:13:08.024502 windmill_api-1.87.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-04-11 19:13:08.084503 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-04-11 19:13:08.192504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-04-11 19:13:08.216504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-04-11 19:13:08.232504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-04-11 19:13:08.256504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-04-11 19:13:08.276504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-04-11 19:13:00.072421 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-04-11 19:13:08.368505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-04-11 19:13:08.324505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-04-11 19:13:08.360505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-04-11 19:13:00.644427 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-04-11 19:13:08.396506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-04-11 19:13:08.420506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-04-11 19:13:00.084421 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-04-11 19:13:08.444506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-04-11 19:13:00.016420 windmill_api-1.87.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-04-11 19:13:00.128422 windmill_api-1.87.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-04-11 19:13:08.512507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-04-11 19:13:08.544507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-04-11 19:13:08.564507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-11 19:13:08.580508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-11 19:13:08.608508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-11 19:13:08.620508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.320424 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-11 19:13:08.648508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.936430 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-11 19:13:08.656508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-11 19:13:08.688509 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-04-11 19:13:08.788510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-04-11 19:13:08.744509 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-04-11 19:13:08.780510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-04-11 19:13:08.832510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-04-11 19:13:08.824510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-04-11 19:13:00.904430 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-04-11 19:13:08.860510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-04-11 19:12:59.860419 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-04-11 19:13:08.872511 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-04-11 19:13:08.896511 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-04-11 19:13:08.908511 windmill_api-1.87.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-04-11 19:13:08.948511 windmill_api-1.87.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-04-11 19:13:08.944511 windmill_api-1.87.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-04-11 19:13:09.012512 windmill_api-1.87.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-04-11 19:13:08.992512 windmill_api-1.87.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2035 2023-04-11 19:13:09.036512 windmill_api-1.87.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-11 19:13:09.076513 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:09.072512 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-11 19:13:09.104513 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-11 19:13:09.144513 windmill_api-1.87.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-11 19:13:09.132513 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-11 19:13:09.188514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-11 19:13:09.260514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-11 19:13:09.248514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-11 19:13:09.308515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-11 19:13:09.304515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-11 19:13:09.344515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-11 19:13:09.348515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.896429 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-11 19:13:09.388516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-11 19:13:09.396516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-11 19:13:09.524517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-11 19:13:09.452516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-11 19:13:09.492517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-11 19:13:09.540517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-11 19:13:09.560517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-11 19:13:00.348424 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-11 19:13:09.584518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-11 19:13:00.488425 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:09.600518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-11 19:13:09.624518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2126 2023-04-11 19:13:09.652518 windmill_api-1.87.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-04-11 19:13:09.660519 windmill_api-1.87.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     2094 2023-04-11 19:13:09.696519 windmill_api-1.87.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-04-11 19:13:09.704519 windmill_api-1.87.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-04-11 19:13:09.744519 windmill_api-1.87.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-04-11 19:13:09.756519 windmill_api-1.87.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:09.768519 windmill_api-1.87.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     4616 2023-04-11 19:13:09.872521 windmill_api-1.87.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-04-11 19:13:00.320424 windmill_api-1.87.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-04-11 19:13:00.004420 windmill_api-1.87.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:09.800520 windmill_api-1.87.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-04-11 19:13:09.848520 windmill_api-1.87.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-04-11 19:13:09.892521 windmill_api-1.87.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-04-11 19:13:09.920521 windmill_api-1.87.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-04-11 19:13:09.932521 windmill_api-1.87.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-04-11 19:13:09.976522 windmill_api-1.87.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-04-11 19:13:10.012522 windmill_api-1.87.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-04-11 19:13:10.020522 windmill_api-1.87.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-04-11 19:13:10.048522 windmill_api-1.87.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-04-11 19:13:10.052523 windmill_api-1.87.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    10978 2023-04-11 19:13:10.224524 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-04-11 19:13:10.080523 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-04-11 19:13:10.140523 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-04-11 19:13:10.256525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-04-11 19:13:10.260525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-04-11 19:13:10.296525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-04-11 19:13:10.296525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-04-11 19:13:10.392526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-04-11 19:13:00.764428 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-04-11 19:13:10.412526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-04-11 19:13:10.428526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-04-11 19:13:10.460527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-04-11 19:13:00.704428 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-04-11 19:13:10.468527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-04-11 19:13:10.540527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-04-11 19:13:00.968430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-04-11 19:13:10.512527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-04-11 19:13:00.912430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-04-11 19:13:00.948430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-04-11 19:13:10.576528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-04-11 19:13:10.648528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-04-11 19:13:10.628528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-04-11 19:13:10.668529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-04-11 19:13:10.692529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-04-11 19:13:10.732529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:12:59.764418 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-11 19:13:10.744530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:13:00.576426 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-04-11 19:13:10.772530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-04-11 19:13:10.780530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-04-11 19:13:10.908531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-04-11 19:13:10.832530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-04-11 19:13:10.872531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-04-11 19:13:10.912531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-04-11 19:13:10.948531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:12:59.868419 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-04-11 19:13:10.952532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:13:00.456425 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-04-11 19:13:10.992532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-04-11 19:13:11.012532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-04-11 19:13:11.032533 windmill_api-1.87.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     6853 2023-04-11 19:13:11.116533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-04-11 19:13:11.068533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-04-11 19:13:00.520426 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-04-11 19:13:00.852429 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-04-11 19:13:11.100533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-04-11 19:13:11.152534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-11 19:13:11.196534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-11 19:13:00.176422 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-11 19:13:11.188534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-11 19:13:11.228534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-11 19:13:11.232535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-11 19:13:11.276535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-11 19:13:11.268535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-11 19:13:11.320535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-11 19:13:00.252423 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-11 19:13:11.312535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-11 19:13:00.384424 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-04-11 19:13:11.348536 windmill_api-1.87.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-04-11 19:13:11.368536 windmill_api-1.87.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-04-11 19:13:11.408536 windmill_api-1.87.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-04-11 19:13:11.408536 windmill_api-1.87.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-04-11 19:13:11.436537 windmill_api-1.87.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-04-11 19:13:11.440537 windmill_api-1.87.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-04-11 19:13:11.512537 windmill_api-1.87.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-04-11 19:13:11.476537 windmill_api-1.87.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-04-11 19:13:11.516537 windmill_api-1.87.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-04-11 19:13:11.576538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-04-11 19:13:11.544538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-04-11 19:13:11.588538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-04-11 19:13:11.612538 windmill_api-1.87.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-04-11 19:13:11.616538 windmill_api-1.87.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4633 2023-04-11 19:13:11.696539 windmill_api-1.87.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-04-11 19:13:11.644539 windmill_api-1.87.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3416 2023-04-11 19:13:11.708539 windmill_api-1.87.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-04-11 19:13:11.724539 windmill_api-1.87.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-04-11 19:13:11.828540 windmill_api-1.87.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-04-11 19:13:11.776540 windmill_api-1.87.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-04-11 19:13:11.812540 windmill_api-1.87.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-04-11 19:13:11.852541 windmill_api-1.87.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-04-11 19:13:11.864541 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-04-11 19:12:59.880419 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-04-11 19:13:11.900541 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-04-11 19:12:59.884419 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-04-11 19:13:11.936542 windmill_api-1.87.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-04-11 19:13:11.944542 windmill_api-1.87.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3080 2023-04-11 19:13:11.992542 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.036543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.032543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.076543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-04-11 19:13:00.584426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-04-11 19:13:12.088543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.128543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.128543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:12:59.816419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.164544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-04-11 19:13:12.176544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.216544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.216544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:13:00.828429 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.252545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:13:00.992431 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-04-11 19:13:00.508426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-04-11 19:13:12.288545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-04-11 19:13:12.288545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-11 19:12:59.892419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-04-11 19:13:12.324545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-11 19:13:00.944430 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-04-11 19:13:12.396546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-04-11 19:13:12.376546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:12.412546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-11 19:13:12.472547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-11 19:13:12.452547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.080421 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-11 19:13:12.488547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.736428 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-11 19:13:12.508547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-11 19:13:12.552548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-04-11 19:13:12.560548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-04-11 19:13:12.600548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-11 19:13:12.676549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-11 19:13:12.652549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-11 19:13:12.692549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-11 19:13:12.724550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-11 19:13:12.728550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.248423 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-11 19:13:12.760550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.560426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-11 19:13:12.768550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-11 19:13:12.804551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-04-11 19:13:12.872551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-04-11 19:13:12.860551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:12.900551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-11 19:13:12.916552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-11 19:13:12.980552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-11 19:13:12.952552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-11 19:13:13.032553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-11 19:13:13.020553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-04-11 19:13:13.072553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-04-11 19:13:13.080553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-11 19:13:13.204554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-11 19:13:13.132554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-11 19:13:13.172554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-11 19:13:13.216555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-11 19:13:13.244555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.952430 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-11 19:13:13.252555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.140422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-11 19:13:13.284555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-11 19:13:13.292555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-04-11 19:13:13.324556 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-04-11 19:13:13.336556 windmill_api-1.87.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-04-11 19:13:13.356556 windmill_api-1.87.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-04-11 19:13:13.392557 windmill_api-1.87.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-04-11 19:13:13.512558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-04-11 19:13:13.440557 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-04-11 19:13:13.480557 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-04-11 19:13:13.552558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-04-11 19:13:13.556558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-04-11 19:13:13.588558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:13:00.144422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-04-11 19:13:13.604559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-04-11 19:13:13.628559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-04-11 19:13:13.716560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-04-11 19:13:13.680559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-04-11 19:13:13.720560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-04-11 19:13:13.764560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-04-11 19:13:13.756560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-04-11 19:13:13.796561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-11 19:13:00.204422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-04-11 19:13:13.808561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-04-11 19:13:13.836561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-04-11 19:13:13.840561 windmill_api-1.87.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-04-11 19:13:13.892562 windmill_api-1.87.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-04-11 19:13:13.960562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-04-11 19:13:13.928562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-04-11 19:13:13.964562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-04-11 19:13:00.088421 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-04-11 19:13:14.032563 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-04-11 19:13:14.016563 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-04-11 19:13:14.176564 windmill_api-1.87.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-04-11 19:13:14.064563 windmill_api-1.87.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-04-11 19:13:14.104564 windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-04-11 19:13:00.156422 windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-04-11 19:13:14.140564 windmill_api-1.87.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-04-11 19:13:14.188564 windmill_api-1.87.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-04-11 19:13:00.748428 windmill_api-1.87.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-04-11 19:13:14.288565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-04-11 19:13:14.224565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-04-11 19:13:14.264565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-04-11 19:12:59.924419 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-04-11 19:13:14.304566 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-04-11 19:13:14.336566 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-04-11 19:12:59.928420 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-04-11 19:13:14.348566 windmill_api-1.87.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-04-11 19:13:14.388567 windmill_api-1.87.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-04-11 19:13:14.452567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-04-11 19:13:14.440567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-11 19:13:14.476567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-11 19:13:14.496568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-11 19:13:14.516568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-11 19:12:59.940420 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-11 19:13:14.568568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-11 19:13:00.128422 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-11 19:13:14.600569 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-11 19:13:14.604569 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-11 19:13:14.712570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-04-11 19:13:14.656569 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-11 19:13:14.696570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-11 19:13:14.740570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-11 19:13:14.760570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-11 19:13:00.996430 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-11 19:13:14.784571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-11 19:13:00.280423 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-11 19:13:14.800571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-11 19:13:14.824571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-04-11 19:13:14.840571 windmill_api-1.87.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-04-11 19:13:14.852571 windmill_api-1.87.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-04-11 19:13:14.872572 windmill_api-1.87.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-04-11 19:13:14.920572 windmill_api-1.87.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-04-11 19:13:14.908572 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-04-11 19:13:00.528426 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-04-11 19:13:14.944572 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-04-11 19:13:15.072574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-04-11 19:13:14.996573 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-11 19:13:15.036573 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-11 19:13:15.116574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-11 19:13:15.112574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-11 19:13:00.612427 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-11 19:13:15.148574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-11 19:13:15.156574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-11 19:13:15.188575 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-04-11 19:12:59.720418 windmill_api-1.87.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-04-11 19:13:15.232575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-04-11 19:13:15.216575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-04-11 19:13:15.288576 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-04-11 19:13:00.100421 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-04-11 19:13:15.264575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-04-11 19:13:15.292576 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-04-11 19:13:15.360576 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-04-11 19:13:00.800428 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-04-11 19:13:15.320576 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-04-11 19:13:15.384577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-04-11 19:13:00.672427 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-04-11 19:13:15.396577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-04-11 19:13:15.408577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-04-11 19:13:15.468577 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-04-11 19:13:00.000420 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-04-11 19:13:15.444577 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    10876 2023-04-11 19:13:15.704580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-04-11 19:13:15.492578 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-04-11 19:13:15.616579 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-04-11 19:13:15.740580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-04-11 19:13:15.736580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-04-11 19:13:15.784581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-04-11 19:13:00.472425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-04-11 19:13:15.780581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-04-11 19:13:15.824581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-04-11 19:13:00.180422 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-04-11 19:13:15.956582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-04-11 19:13:15.864581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-11 19:13:15.904582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-11 19:13:00.424425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-11 19:13:15.948582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-11 19:13:16.000583 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-11 19:12:59.636417 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-04-11 19:13:16.000583 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-04-11 19:13:00.960430 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-04-11 19:13:00.784428 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-04-11 19:13:16.056584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-04-11 19:13:16.160585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-04-11 19:13:16.108584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-04-11 19:13:16.148584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-04-11 19:13:16.192585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-04-11 19:13:16.204585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-04-11 19:13:00.092421 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-04-11 19:13:16.276586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-04-11 19:13:00.804428 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-04-11 19:13:16.244585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-04-11 19:13:16.280586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-04-11 19:13:16.388587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-04-11 19:13:16.336586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-11 19:13:16.372587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-11 19:13:16.416587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-11 19:13:16.428587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:12:59.676417 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-11 19:13:16.456588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.456425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-11 19:13:16.476588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-11 19:13:16.496588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5083 2023-04-11 19:13:16.568589 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-04-11 19:13:16.524588 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-04-11 19:13:16.548588 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-04-11 19:13:16.604589 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-04-11 19:13:16.680590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-04-11 19:13:16.656590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-11 19:13:16.692590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-11 19:13:16.724590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-11 19:13:16.792591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-11 19:13:16.828591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:12:59.936420 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-11 19:13:16.832591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-11 19:13:16.868592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-04-11 19:13:16.940592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-04-11 19:13:16.924592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-04-11 19:13:16.964593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-04-11 19:13:16.984593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-04-11 19:13:17.008593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-04-11 19:13:17.024593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.636427 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-04-11 19:13:17.048594 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-04-11 19:13:17.060594 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2010 2023-04-11 19:13:17.096594 windmill_api-1.87.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-04-11 19:13:17.088594 windmill_api-1.87.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-04-11 19:13:17.136594 windmill_api-1.87.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-04-11 19:12:59.956420 windmill_api-1.87.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-04-11 19:13:17.128594 windmill_api-1.87.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-04-11 19:13:17.192595 windmill_api-1.87.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-04-11 19:13:17.160595 windmill_api-1.87.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-04-11 19:13:17.192595 windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-04-11 19:13:17.228595 windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-04-11 19:13:17.236595 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-04-11 19:13:17.280596 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-04-11 19:13:17.320596 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-04-11 19:13:17.384597 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-04-11 19:13:17.432597 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-04-11 19:13:17.452598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-04-11 19:13:17.472598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-04-11 19:13:17.488598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-04-11 19:13:17.512598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:13:00.204422 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-04-11 19:13:17.528598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:12:59.980420 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-04-11 19:13:17.552599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-04-11 19:13:17.568599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-04-11 19:13:17.664600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-04-11 19:13:17.620599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-04-11 19:13:17.660600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-04-11 19:13:17.704600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-04-11 19:13:17.700600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-04-11 19:13:00.212422 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-04-11 19:13:17.740601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-04-11 19:13:17.752601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-04-11 19:13:17.828601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-04-11 19:13:17.804601 windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-04-11 19:12:59.776418 windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1852 2023-04-11 19:13:17.844602 windmill_api-1.87.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-04-11 19:13:00.728428 windmill_api-1.87.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-04-11 19:13:17.876602 windmill_api-1.87.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-04-11 19:13:17.884602 windmill_api-1.87.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-04-11 19:13:17.944603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-04-11 19:13:17.908602 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-04-11 19:13:18.016603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-04-11 19:12:59.824419 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-04-11 19:13:17.984603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-04-11 19:13:18.008603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-04-11 19:13:18.076604 windmill_api-1.87.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.044604 windmill_api-1.87.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-04-11 19:13:18.100604 windmill_api-1.87.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-04-11 19:13:18.116604 windmill_api-1.87.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-04-11 19:13:18.180605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:18.140605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.164605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     6775 2023-04-11 19:13:18.272606 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-11 19:13:18.204605 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.232606 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     6775 2023-04-11 19:13:18.332607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-11 19:13:18.340607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-11 19:13:00.804428 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.360607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-04-11 19:13:18.376607 windmill_api-1.87.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-04-11 19:13:18.432608 windmill_api-1.87.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-04-11 19:13:18.420607 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-04-11 19:13:18.452608 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-04-11 19:13:18.472608 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-04-11 19:13:18.592609 windmill_api-1.87.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.500608 windmill_api-1.87.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-04-11 19:13:18.548609 windmill_api-1.87.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-04-11 19:12:59.848419 windmill_api-1.87.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-04-11 19:13:18.584609 windmill_api-1.87.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-04-11 19:13:18.636610 windmill_api-1.87.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:12:59.760418 windmill_api-1.87.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-04-11 19:13:18.644610 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-04-11 19:13:18.724611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-04-11 19:13:18.680610 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-04-11 19:13:18.716611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-04-11 19:13:18.760611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-04-11 19:13:18.780611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-04-11 19:13:00.572426 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-04-11 19:13:18.804611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-04-11 19:13:18.880612 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-11 19:13:18.840612 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:12:59.736418 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-04-11 19:13:18.900612 windmill_api-1.87.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-04-11 19:13:18.908612 windmill_api-1.87.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-04-11 19:13:18.940613 windmill_api-1.87.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-04-11 19:13:00.540426 windmill_api-1.87.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     1820 2023-04-11 19:13:18.956613 windmill_api-1.87.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.396424 windmill_api-1.87.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-04-11 19:13:18.980613 windmill_api-1.87.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.276423 windmill_api-1.87.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-04-11 19:13:18.992613 windmill_api-1.87.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-04-11 19:13:19.020614 windmill_api-1.87.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:13:00.988430 windmill_api-1.87.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-04-11 19:13:19.032614 windmill_api-1.87.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-04-11 19:13:00.176422 windmill_api-1.87.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-04-11 19:13:19.128615 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:12:59.896419 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-04-11 19:13:19.068614 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-04-11 19:13:19.136615 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-04-11 19:13:00.608427 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-04-11 19:13:19.160615 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11088 2023-04-11 19:13:19.316617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-04-11 19:13:19.188615 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-04-11 19:13:19.248616 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-04-11 19:13:19.412618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-04-11 19:13:19.352617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-04-11 19:13:19.392617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-04-11 19:12:59.944420 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-04-11 19:13:19.432618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-04-11 19:13:19.460618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-04-11 19:13:00.108421 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-04-11 19:13:19.556619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-04-11 19:13:19.492618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-04-11 19:13:19.532619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-04-11 19:13:00.448425 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-04-11 19:13:19.564619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-04-11 19:13:19.604620 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-04-11 19:13:00.956430 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-04-11 19:13:19.604620 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-04-11 19:12:59.756418 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:13:00.112422 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-04-11 19:13:19.708621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-04-11 19:13:19.712621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-04-11 19:13:19.764621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-04-11 19:13:19.744621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-04-11 19:13:19.784621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-04-11 19:13:19.804622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-04-11 19:13:00.816429 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-04-11 19:13:19.820622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-04-11 19:13:00.212422 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-04-11 19:13:19.840622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-04-11 19:13:19.856622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-04-11 19:13:19.956623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-04-11 19:13:19.908623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-04-11 19:13:19.992623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-04-11 19:13:20.000624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-04-11 19:13:20.028624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-04-11 19:13:00.480425 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-04-11 19:13:20.036624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-04-11 19:13:00.596426 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-04-11 19:13:20.072624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-04-11 19:13:20.072624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-04-11 19:13:20.108625 windmill_api-1.87.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     5077 2023-04-11 19:13:20.196626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-11 19:13:20.136625 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     1255 2023-04-11 19:13:20.164625 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_schema.py
+-rw-r--r--   0        0        0     3297 2023-04-11 19:13:20.228626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value.py
+-rw-r--r--   0        0        0     7151 2023-04-11 19:13:20.308627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
+-rw-r--r--   0        0        0     3318 2023-04-11 19:13:20.280626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1985 2023-04-11 19:13:20.316627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2289 2023-04-11 19:13:20.364627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2187 2023-04-11 19:13:20.356627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:12:59.652417 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2054 2023-04-11 19:13:20.392628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:13:00.012421 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1978 2023-04-11 19:13:20.408628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2029 2023-04-11 19:13:20.428628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7049 2023-04-11 19:13:20.508629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
+-rw-r--r--   0        0        0     3284 2023-04-11 19:13:20.476628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-11 19:13:20.512629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-11 19:13:20.548629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-11 19:13:20.592630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.696427 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-11 19:13:20.584629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.836429 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-11 19:13:20.664630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-11 19:13:20.628630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2074 2023-04-11 19:13:20.664630 windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-11 19:13:20.688630 windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-04-11 19:13:20.724631 windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-04-11 19:13:20.716631 windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-04-11 19:13:20.760631 windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-04-11 19:13:20.784632 windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-04-11 19:13:20.812632 windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-04-11 19:13:20.836632 windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-04-11 19:13:20.856632 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-04-11 19:13:20.888633 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     1922 2023-04-11 19:13:20.896633 windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-04-11 19:12:59.908419 windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-04-11 19:13:20.936633 windmill_api-1.87.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    11982 2023-04-11 19:13:21.104635 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-04-11 19:13:20.964633 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-04-11 19:13:21.024634 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-04-11 19:13:21.196636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-04-11 19:13:21.188636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-11 19:13:21.224636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-11 19:13:00.728428 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-11 19:13:21.232636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-11 19:13:21.276636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-11 19:12:59.904420 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-04-11 19:13:21.340637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-04-11 19:13:21.304637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-04-11 19:13:21.340637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-04-11 19:12:59.908419 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-04-11 19:13:21.384638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-04-11 19:13:21.388638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-04-11 19:13:21.424638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-04-11 19:13:00.420425 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-04-11 19:13:21.448638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-04-11 19:13:21.532639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-04-11 19:13:21.500639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-11 19:13:21.540639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-11 19:13:21.572640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-11 19:13:21.576640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-11 19:13:21.608640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.660427 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-11 19:13:21.612640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-11 19:13:21.700641 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-04-11 19:13:21.792642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-04-11 19:13:21.748641 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-11 19:13:21.788642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-11 19:13:21.828642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-11 19:13:21.836642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-11 19:13:21.868642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-11 19:13:00.168422 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-11 19:13:21.872643 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-11 19:13:21.904643 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-04-11 19:13:21.960643 windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-11 19:13:21.928643 windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-04-11 19:13:21.976644 windmill_api-1.87.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-04-11 19:13:22.052644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-04-11 19:13:22.004644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-04-11 19:13:22.032644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     6768 2023-04-11 19:13:22.148645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-11 19:13:22.080645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-04-11 19:12:59.848419 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-04-11 19:13:22.108645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-04-11 19:13:22.164646 windmill_api-1.87.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-04-11 19:13:22.188646 windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-04-11 19:13:22.264647 windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-04-11 19:13:22.240646 windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4035 2023-04-11 19:13:22.360648 windmill_api-1.87.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-04-11 19:13:22.296647 windmill_api-1.87.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-04-11 19:13:22.372648 windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-11 19:13:22.388648 windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-04-11 19:13:22.416648 windmill_api-1.87.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-04-11 19:13:22.424648 windmill_api-1.87.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-04-11 19:13:22.456648 windmill_api-1.87.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-04-11 19:13:22.464649 windmill_api-1.87.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-04-11 19:13:22.516649 windmill_api-1.87.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-04-11 19:13:22.488649 windmill_api-1.87.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-04-11 19:13:22.580650 windmill_api-1.87.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:22.536649 windmill_api-1.87.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-04-11 19:13:22.620650 windmill_api-1.87.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:22.604650 windmill_api-1.87.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-04-11 19:13:22.644650 windmill_api-1.87.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-04-11 19:13:22.664651 windmill_api-1.87.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-04-11 19:13:22.688651 windmill_api-1.87.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-04-11 19:13:22.720651 windmill_api-1.87.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-04-11 19:13:22.824652 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-04-11 19:13:00.860429 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-04-11 19:13:22.752652 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-04-11 19:13:22.844653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-04-11 19:13:22.860653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-04-11 19:13:22.896653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-04-11 19:12:59.724418 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-11 19:13:22.892653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-04-11 19:13:22.940653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-04-11 19:13:00.748428 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-04-11 19:13:22.928653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-11 19:13:00.904430 windmill_api-1.87.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-04-11 19:13:22.984654 windmill_api-1.87.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-04-11 19:13:22.968654 windmill_api-1.87.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     2108 2023-04-11 19:13:23.016654 windmill_api-1.87.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-04-11 19:13:23.032654 windmill_api-1.87.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-04-11 19:13:23.052655 windmill_api-1.87.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-04-11 19:13:23.084655 windmill_api-1.87.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-04-11 19:13:23.084655 windmill_api-1.87.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-04-11 19:13:23.136655 windmill_api-1.87.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-04-11 19:13:23.192656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-04-11 19:13:23.188656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-04-11 19:13:23.228656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-04-11 19:13:23.236657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-04-11 19:13:23.268657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-04-11 19:13:00.392424 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-04-11 19:13:23.272657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-04-11 19:13:00.776428 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-04-11 19:13:23.304657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-04-11 19:13:23.380658 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-04-11 19:13:23.412658 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-04-11 19:13:23.440658 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-04-11 19:13:23.452659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-04-11 19:13:23.484659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-04-11 19:13:23.540660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-11 19:13:00.088421 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-04-11 19:13:23.524659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-11 19:13:00.952430 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-04-11 19:13:23.564660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-04-11 19:13:23.576660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-11 19:13:23.624660 windmill_api-1.87.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-04-11 19:13:23.604660 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-04-11 19:13:23.656661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-04-11 19:13:23.728661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-04-11 19:13:23.708661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-04-11 19:13:23.748662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-04-11 19:13:23.776662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-04-11 19:13:23.788662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-04-11 19:13:00.444425 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-04-11 19:13:23.812662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-11 19:12:59.952420 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-04-11 19:13:23.824662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-04-11 19:13:23.852663 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-04-11 19:13:23.932664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-04-11 19:13:23.976664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-04-11 19:13:23.968664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-04-11 19:13:24.012664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-04-11 19:13:24.016664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:13:00.784428 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-04-11 19:13:24.052665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:12:59.696417 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-04-11 19:13:24.060665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-04-11 19:13:24.100665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-04-11 19:13:24.100665 windmill_api-1.87.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-04-11 19:13:24.148666 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-04-11 19:13:24.140666 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.512426 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-04-11 19:13:24.240667 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-04-11 19:13:00.044421 windmill_api-1.87.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-04-11 19:13:24.200666 windmill_api-1.87.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-04-11 19:13:24.264667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-04-11 19:13:24.280667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:13:00.008421 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-04-11 19:13:24.304667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-04-11 19:13:00.100421 windmill_api-1.87.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-04-11 19:13:24.344668 windmill_api-1.87.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-04-11 19:13:00.168422 windmill_api-1.87.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-04-11 19:13:24.344668 windmill_api-1.87.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-04-11 19:13:24.368668 windmill_api-1.87.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2147 2023-04-11 19:13:24.388668 windmill_api-1.87.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-04-11 19:13:24.396668 windmill_api-1.87.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-04-11 19:12:59.928420 windmill_api-1.87.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-04-11 19:13:24.428669 windmill_api-1.87.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-04-11 19:13:24.448669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-04-11 19:13:24.512669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-04-11 19:13:00.792428 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-04-11 19:13:24.488669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-04-11 19:13:24.524670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-04-11 19:13:24.556670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-04-11 19:13:24.572670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-04-11 19:12:59.996420 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-04-11 19:13:24.592670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-04-11 19:13:24.620670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-04-11 19:13:24.628671 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-04-11 19:13:00.704428 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11448 2023-04-11 19:13:24.892673 windmill_api-1.87.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-04-11 19:13:24.660671 windmill_api-1.87.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-04-11 19:13:24.724671 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-04-11 19:13:24.832673 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-04-11 19:13:24.932674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-04-11 19:13:24.932674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-04-11 19:13:00.164422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-04-11 19:13:24.968674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-04-11 19:13:24.980674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-04-11 19:13:25.076675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-04-11 19:13:25.012674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-04-11 19:13:25.052675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-04-11 19:13:00.256423 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-04-11 19:13:25.088675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-04-11 19:13:25.124676 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-04-11 19:13:00.180422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-04-11 19:13:25.136676 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-04-11 19:12:59.632417 windmill_api-1.87.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:13:00.772428 windmill_api-1.87.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-04-11 19:13:25.184676 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-04-11 19:13:25.320678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-04-11 19:13:25.236677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-04-11 19:13:25.272677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-04-11 19:13:25.316677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-04-11 19:13:25.356678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:13:00.324424 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-04-11 19:13:25.356678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-11 19:13:00.348424 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-04-11 19:13:25.396678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-04-11 19:13:25.460679 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-04-11 19:13:25.504680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-04-11 19:13:25.512679 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-04-11 19:13:25.544680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-04-11 19:13:25.556680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-04-11 19:13:25.584680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-11 19:13:00.264423 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-04-11 19:13:25.592680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-11 19:12:59.776418 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-04-11 19:13:25.628681 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-04-11 19:13:25.632681 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-11 19:13:25.684681 windmill_api-1.87.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-04-11 19:13:25.676681 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-04-11 19:13:25.712682 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-04-11 19:12:59.732418 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-04-11 19:13:25.720682 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-04-11 19:13:00.956430 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-04-11 19:12:59.888419 windmill_api-1.87.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-04-11 19:13:00.680427 windmill_api-1.87.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-04-11 19:13:25.748682 windmill_api-1.87.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-04-11 19:13:25.752682 windmill_api-1.87.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-04-11 19:13:00.896429 windmill_api-1.87.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-04-11 19:13:25.784682 windmill_api-1.87.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-04-11 19:13:25.784682 windmill_api-1.87.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-04-11 19:13:25.848683 windmill_api-1.87.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-04-11 19:13:25.812682 windmill_api-1.87.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-04-11 19:13:25.864683 windmill_api-1.87.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-04-11 19:13:25.876683 windmill_api-1.87.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-11 19:13:25.892683 windmill_api-1.87.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-04-11 19:13:25.928684 windmill_api-1.87.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-04-11 19:13:25.932684 windmill_api-1.87.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-04-11 19:13:25.972684 windmill_api-1.87.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-04-11 19:13:25.960684 windmill_api-1.87.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-04-11 19:13:26.000685 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-04-11 19:13:26.000685 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-04-11 19:13:26.140686 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-04-11 19:13:26.224687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-04-11 19:13:26.192686 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-11 19:13:26.232687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-11 19:13:26.264687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-11 19:13:26.276687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.628427 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-11 19:13:26.304688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:13:00.272423 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-11 19:13:26.316688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-11 19:13:26.344688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-04-11 19:13:26.424689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-04-11 19:13:26.400689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-04-11 19:13:26.436689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-04-11 19:13:26.464689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-04-11 19:13:26.468689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:12:59.824419 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-04-11 19:13:26.500690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:13:00.776428 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-04-11 19:13:26.508690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-04-11 19:13:26.540690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-04-11 19:13:26.532690 windmill_api-1.87.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-04-11 19:13:26.560690 windmill_api-1.87.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2422 2023-04-11 19:13:26.584690 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-04-11 19:13:26.588690 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-04-11 19:13:26.612691 windmill_api-1.87.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-04-11 19:13:26.612691 windmill_api-1.87.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0     4086 2023-04-11 19:13:26.776692 windmill_api-1.87.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-04-11 19:13:26.640691 windmill_api-1.87.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-04-11 19:13:26.668691 windmill_api-1.87.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     6220 2023-04-11 19:13:26.892694 windmill_api-1.87.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-04-11 19:13:26.812693 windmill_api-1.87.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-04-11 19:13:26.836693 windmill_api-1.87.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-04-11 19:13:00.224423 windmill_api-1.87.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-04-11 19:13:26.868693 windmill_api-1.87.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-04-11 19:13:26.900694 windmill_api-1.87.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-04-11 19:13:26.924694 windmill_api-1.87.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-04-11 19:13:26.948694 windmill_api-1.87.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-04-11 19:13:26.956694 windmill_api-1.87.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-04-11 19:13:26.992694 windmill_api-1.87.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.432425 windmill_api-1.87.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-04-11 19:13:26.996695 windmill_api-1.87.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-04-11 19:12:59.660417 windmill_api-1.87.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-04-11 19:13:27.048695 windmill_api-1.87.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-04-11 19:13:27.052695 windmill_api-1.87.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-04-11 19:13:27.092696 windmill_api-1.87.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-04-11 19:13:27.112696 windmill_api-1.87.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-11 19:13:27.156696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-11 19:13:00.144422 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:27.148696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-11 19:13:27.176696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-11 19:13:27.212697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-11 19:13:27.204697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-11 19:13:27.260697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-11 19:13:27.320698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-11 19:13:27.316698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-11 19:13:27.352698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-11 19:13:27.364698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-11 19:13:27.388699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.960430 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-11 19:13:27.400699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-11 19:13:00.468425 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-11 19:13:27.428699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-11 19:13:27.508700 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-11 19:13:27.632701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-11 19:13:27.564700 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-11 19:13:27.604701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-11 19:13:27.648701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-11 19:13:27.672701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-11 19:13:27.684702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-11 19:12:59.704417 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-11 19:13:27.708702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-11 19:13:27.720702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-04-11 19:13:27.752702 windmill_api-1.87.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-04-11 19:13:27.756702 windmill_api-1.87.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     2036 2023-04-11 19:13:27.800703 windmill_api-1.87.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-04-11 19:13:27.796703 windmill_api-1.87.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-04-11 19:13:27.828703 windmill_api-1.87.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-04-11 19:13:27.840703 windmill_api-1.87.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-11 19:13:27.856703 windmill_api-1.87.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-04-11 19:13:27.892704 windmill_api-1.87.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-04-11 19:13:27.904704 windmill_api-1.87.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-04-11 19:13:27.924704 windmill_api-1.87.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     3799 2023-04-11 19:13:27.996705 windmill_api-1.87.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-04-11 19:13:27.968705 windmill_api-1.87.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-04-11 19:13:28.008705 windmill_api-1.87.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-04-11 19:13:28.032705 windmill_api-1.87.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     3950 2023-04-11 19:13:28.092706 windmill_api-1.87.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-04-11 19:13:28.068705 windmill_api-1.87.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     3939 2023-04-11 19:13:28.140706 windmill_api-1.87.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-04-11 19:13:28.124706 windmill_api-1.87.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-04-11 19:13:28.176707 windmill_api-1.87.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-04-11 19:13:28.184707 windmill_api-1.87.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-04-11 19:13:28.216707 windmill_api-1.87.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-04-11 19:12:48.844307 windmill_api-1.87.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-04-11 19:13:28.204707 windmill_api-1.87.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 windmill_api-1.87.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.87.0/PKG-INFO
```

### Comparing `windmill_api-1.86.0/LICENSE` & `windmill_api-1.87.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/README.md` & `windmill_api-1.87.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/pyproject.toml` & `windmill_api-1.87.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.86.0"
+version = "1.87.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.86.0/windmill_api/api/app/create_app.py` & `windmill_api-1.87.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.87.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.87.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.87.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.87.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.87.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.87.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.87.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.87.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.87.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.87.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/app/update_app.py` & `windmill_api-1.87.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.87.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.87.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.87.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.87.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.87.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/favorite/star.py` & `windmill_api-1.87.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.87.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.87.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.87.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.87.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.87.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.87.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.87.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.87.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.87.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.87.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.87.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.87.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.87.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.87.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.87.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/create_group.py` & `windmill_api-1.87.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.87.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/get_group.py` & `windmill_api-1.87.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.87.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.87.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.87.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/group/update_group.py` & `windmill_api-1.87.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.87.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.87.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.87.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.87.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.87.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.87.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_job.py` & `windmill_api-1.87.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.87.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.87.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.87.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.87.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.87.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.87.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.87.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.87.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.87.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.87.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.87.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.87.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.87.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.87.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.87.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.87.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.87.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.87.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.87.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.87.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.87.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.87.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.87.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.87.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.87.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.87.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/create_script.py` & `windmill_api-1.87.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.87.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.87.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.87.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.87.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.87.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.87.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.87.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.87.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.87.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.87.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.87.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.87.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/create_token.py` & `windmill_api-1.87.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.87.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/create_user.py` & `windmill_api-1.87.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.87.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.87.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.87.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.87.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.87.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.87.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.87.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.87.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.87.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.87.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.87.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.87.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.87.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/list_users.py` & `windmill_api-1.87.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.87.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.87.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/login.py` & `windmill_api-1.87.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.87.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/logout.py` & `windmill_api-1.87.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/set_password.py` & `windmill_api-1.87.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/update_user.py` & `windmill_api-1.87.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/whoami.py` & `windmill_api-1.87.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/user/whois.py` & `windmill_api-1.87.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.87.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.87.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.87.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.87.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.87.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.87.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.87.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.87.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.87.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.87.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.87.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.87.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.87.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.87.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.87.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.87.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.87.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.87.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.87.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.87.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/client.py` & `windmill_api-1.87.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.87.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.87.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.87.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.87.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.87.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.87.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/audit_log.py` & `windmill_api-1.87.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.87.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.87.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all.py` & `windmill_api-1.87.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one.py` & `windmill_api-1.87.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.87.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.87.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job.py` & `windmill_api-1.87.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.87.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.87.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.87.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.87.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_schema.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_resource.py` & `windmill_api-1.87.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.87.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.87.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_variable.py` & `windmill_api-1.87.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_workspace.py` & `windmill_api-1.87.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.87.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.87.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.87.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.87.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_resource.py` & `windmill_api-1.87.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.87.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.87.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.87.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.87.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_variable.py` & `windmill_api-1.87.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.87.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.87.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.87.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.87.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.87.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.87.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.87.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow.py` & `windmill_api-1.87.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.87.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module.py` & `windmill_api-1.87.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_schema.py` & `windmill_api-1.87.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status.py` & `windmill_api-1.87.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value.py` & `windmill_api-1.87.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/folder.py` & `windmill_api-1.87.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.87.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.87.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/global_user_info.py` & `windmill_api-1.87.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.87.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.87.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/group.py` & `windmill_api-1.87.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/identity.py` & `windmill_api-1.87.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.87.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.87.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.87.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.87.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/job.py` & `windmill_api-1.87.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_schema.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.87.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.87.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_app.py` & `windmill_api-1.87.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_resource.py` & `windmill_api-1.87.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_variable.py` & `windmill_api-1.87.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/login.py` & `windmill_api-1.87.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/login_json_body.py` & `windmill_api-1.87.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.87.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/new_schedule.py` & `windmill_api-1.87.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.87.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/new_token.py` & `windmill_api-1.87.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.87.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/new_user.py` & `windmill_api-1.87.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow.py` & `windmill_api-1.87.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_flow.py` & `windmill_api-1.87.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_script.py` & `windmill_api-1.87.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/policy.py` & `windmill_api-1.87.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/preview.py` & `windmill_api-1.87.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/preview_args.py` & `windmill_api-1.87.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.87.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job.py` & `windmill_api-1.87.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/raw_script.py` & `windmill_api-1.87.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.87.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.87.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.87.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.87.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/resource.py` & `windmill_api-1.87.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/resource_type.py` & `windmill_api-1.87.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.87.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.87.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/retry.py` & `windmill_api-1.87.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.87.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/schedule.py` & `windmill_api-1.87.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/schedule_args.py` & `windmill_api-1.87.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/script.py` & `windmill_api-1.87.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/script_args.py` & `windmill_api-1.87.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.87.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/script_schema.py` & `windmill_api-1.87.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.87.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.87.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/slack_token.py` & `windmill_api-1.87.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.87.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/star_json_body.py` & `windmill_api-1.87.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/static_transform.py` & `windmill_api-1.87.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/token_response.py` & `windmill_api-1.87.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/truncated_token.py` & `windmill_api-1.87.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.87.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.87.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_user_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.87.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/usage.py` & `windmill_api-1.87.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/user.py` & `windmill_api-1.87.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/user_usage.py` & `windmill_api-1.87.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.87.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.87.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.87.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.87.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.87.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.87.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/worker_ping.py` & `windmill_api-1.87.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/workspace.py` & `windmill_api-1.87.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/models/workspace_invite.py` & `windmill_api-1.87.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/windmill_api/types.py` & `windmill_api-1.87.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.86.0/setup.py` & `windmill_api-1.87.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.86.0',
+    'version': '1.87.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.86.0/PKG-INFO` & `windmill_api-1.87.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.86.0
+Version: 1.87.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

