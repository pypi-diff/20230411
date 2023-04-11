# Comparing `tmp/inductiva-0.0.5.tar.gz` & `tmp/inductiva-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.0.5.tar", last modified: Fri Mar 31 11:07:48 2023, max compression
+gzip compressed data, was "inductiva-0.0.6.tar", last modified: Tue Apr 11 15:58:03 2023, max compression
```

## Comparing `inductiva-0.0.5.tar` & `inductiva-0.0.6.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.229421 inductiva-0.0.5/
--rw-r--r--   0 lpcunha    (501) staff       (20)       43 2023-03-30 11:33:02.000000 inductiva-0.0.5/MANIFEST.in
--rw-r--r--   0 lpcunha    (501) staff       (20)      579 2023-03-31 11:07:48.229569 inductiva-0.0.5/PKG-INFO
--rw-r--r--   0 lpcunha    (501) staff       (20)      205 2023-03-30 08:38:52.000000 inductiva-0.0.5/README.md
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.207167 inductiva-0.0.5/inductiva/
--rw-r--r--   0 lpcunha    (501) staff       (20)      363 2023-03-30 09:55:59.000000 inductiva-0.0.5/inductiva/__init__.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.208639 inductiva-0.0.5/inductiva/api/
--rw-r--r--   0 lpcunha    (501) staff       (20)      122 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/api/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    12587 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/api/methods.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.210630 inductiva-0.0.5/inductiva/client/
--rw-r--r--   0 lpcunha    (501) staff       (20)      805 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    60856 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/api_client.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.211595 inductiva-0.0.5/inductiva/client/apis/
--rw-r--r--   0 lpcunha    (501) staff       (20)      214 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1421 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/path_to_api.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.213301 inductiva-0.0.5/inductiva/client/apis/paths/
--rw-r--r--   0 lpcunha    (501) staff       (20)      243 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      112 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/admin_user.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      137 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/admin_user_username_tasks.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      114 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/task_submit.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      126 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/task_task_id_input.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      124 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/task_task_id_kill.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      125 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/task_task_id_output.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      125 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/paths/task_task_id_status.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      400 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/tag_to_api.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.213829 inductiva-0.0.5/inductiva/client/apis/tags/
--rw-r--r--   0 lpcunha    (501) staff       (20)      329 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/tags/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      622 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/tags/admin_api.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      916 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/apis/tags/tasks_api.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    16615 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/configuration.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     4590 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/exceptions.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.215221 inductiva-0.0.5/inductiva/client/model/
--rw-r--r--   0 lpcunha    (501) staff       (20)      350 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     2759 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/body_upload_task_input.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     3636 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/http_validation_error.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     4386 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/new_user.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     4682 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/queue_status.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     3628 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/task_request.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     6465 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/task_status.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     7930 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/model/validation_error.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.215401 inductiva-0.0.5/inductiva/client/models/
--rw-r--r--   0 lpcunha    (501) staff       (20)      843 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/models/__init__.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.215568 inductiva-0.0.5/inductiva/client/paths/
--rw-r--r--   0 lpcunha    (501) staff       (20)      617 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/__init__.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.215982 inductiva-0.0.5/inductiva/client/paths/admin_user/
--rw-r--r--   0 lpcunha    (501) staff       (20)      311 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/admin_user/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    12303 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/admin_user/post.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.216362 inductiva-0.0.5/inductiva/client/paths/admin_user_username_tasks/
--rw-r--r--   0 lpcunha    (501) staff       (20)      341 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/admin_user_username_tasks/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    10351 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/admin_user_username_tasks/get.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.216707 inductiva-0.0.5/inductiva/client/paths/task_submit/
--rw-r--r--   0 lpcunha    (501) staff       (20)      313 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_submit/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    12455 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_submit/post.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.217170 inductiva-0.0.5/inductiva/client/paths/task_task_id_input/
--rw-r--r--   0 lpcunha    (501) staff       (20)      327 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_input/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    15178 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_input/post.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.217534 inductiva-0.0.5/inductiva/client/paths/task_task_id_kill/
--rw-r--r--   0 lpcunha    (501) staff       (20)      325 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_kill/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    10501 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_kill/post.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.217997 inductiva-0.0.5/inductiva/client/paths/task_task_id_output/
--rw-r--r--   0 lpcunha    (501) staff       (20)      329 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_output/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    10463 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_output/get.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.218526 inductiva-0.0.5/inductiva/client/paths/task_task_id_status/
--rw-r--r--   0 lpcunha    (501) staff       (20)      329 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_status/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    10400 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/paths/task_task_id_status/get.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    11962 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/rest.py
--rw-r--r--   0 lpcunha    (501) staff       (20)   103899 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/client/schemas.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.219271 inductiva-0.0.5/inductiva/core/
--rw-r--r--   0 lpcunha    (501) staff       (20)      120 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/__init__.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.219618 inductiva-0.0.5/inductiva/core/cupy/
--rw-r--r--   0 lpcunha    (501) staff       (20)       85 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/cupy/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      379 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/cupy/linalg.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      586 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/math.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.219945 inductiva-0.0.5/inductiva/core/slepc/
--rw-r--r--   0 lpcunha    (501) staff       (20)       64 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/slepc/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      491 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/slepc/linalg.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      333 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/core/test.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      102 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/exceptions.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.220603 inductiva-0.0.5/inductiva/fluids/
--rw-r--r--   0 lpcunha    (501) staff       (20)      411 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     2579 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/_output_post_processing.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1002 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/fluid_types.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.220900 inductiva-0.0.5/inductiva/fluids/post_processing/
--rw-r--r--   0 lpcunha    (501) staff       (20)        0 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/post_processing/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     5931 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/post_processing/splishsplash.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.221073 inductiva-0.0.5/inductiva/fluids/scenarios/
--rw-r--r--   0 lpcunha    (501) staff       (20)      110 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/__init__.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.221375 inductiva-0.0.5/inductiva/fluids/scenarios/dam_break/
--rw-r--r--   0 lpcunha    (501) staff       (20)       74 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/dam_break/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     3418 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/scenarios/dam_break/dam_break.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.222577 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/
--rw-r--r--   0 lpcunha    (501) staff       (20)       78 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     4031 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/dam_break_template.dualsphysics.xml.jinja
--rw-r--r--   0 lpcunha    (501) staff       (20)     8504 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/fluid_block.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1265 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
--rw-r--r--   0 lpcunha    (501) staff       (20)      700 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/unit_box.obj
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.223698 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/
--rw-r--r--   0 lpcunha    (501) staff       (20)      182 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     8179 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1914 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
--rw-r--r--   0 lpcunha    (501) staff       (20)     9161 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     6444 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     2507 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/fluids/shapes.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.225194 inductiva-0.0.5/inductiva/fluids/simulators/
--rw-r--r--   0 lpcunha    (501) staff       (20)      203 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      880 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/dualsphysics.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1136 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/openfoam.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      891 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/splishsplash.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      835 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/swash.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      702 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/fluids/simulators/xbeach.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.225756 inductiva-0.0.5/inductiva/simulation/
--rw-r--r--   0 lpcunha    (501) staff       (20)       76 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/simulation/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1258 2023-03-31 11:06:15.000000 inductiva-0.0.5/inductiva/simulation/simulator.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      142 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/types.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.229205 inductiva-0.0.5/inductiva/utils/
--rw-r--r--   0 lpcunha    (501) staff       (20)        0 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/utils/__init__.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     8337 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/utils/data.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1169 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/utils/files.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      783 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/utils/files_test.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1720 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/utils/flags.py
--rw-r--r--   0 lpcunha    (501) staff       (20)     1672 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/utils/meta.py
--rw-r--r--   0 lpcunha    (501) staff       (20)      509 2023-03-30 08:38:52.000000 inductiva-0.0.5/inductiva/utils/templates.py
--rw-r--r--   0 lpcunha    (501) staff       (20)    10104 2023-03-30 15:56:44.000000 inductiva-0.0.5/inductiva/utils/visualization.py
-drwxr-xr-x   0 lpcunha    (501) staff       (20)        0 2023-03-31 11:07:48.208207 inductiva-0.0.5/inductiva.egg-info/
--rw-r--r--   0 lpcunha    (501) staff       (20)      579 2023-03-31 11:07:48.000000 inductiva-0.0.5/inductiva.egg-info/PKG-INFO
--rw-r--r--   0 lpcunha    (501) staff       (20)     3936 2023-03-31 11:07:48.000000 inductiva-0.0.5/inductiva.egg-info/SOURCES.txt
--rw-r--r--   0 lpcunha    (501) staff       (20)        1 2023-03-31 11:07:48.000000 inductiva-0.0.5/inductiva.egg-info/dependency_links.txt
--rw-r--r--   0 lpcunha    (501) staff       (20)      164 2023-03-31 11:07:48.000000 inductiva-0.0.5/inductiva.egg-info/requires.txt
--rw-r--r--   0 lpcunha    (501) staff       (20)       10 2023-03-31 11:07:48.000000 inductiva-0.0.5/inductiva.egg-info/top_level.txt
--rw-r--r--   0 lpcunha    (501) staff       (20)       87 2023-03-31 11:06:15.000000 inductiva-0.0.5/pyproject.toml
--rw-r--r--   0 lpcunha    (501) staff       (20)      767 2023-03-31 11:07:48.230365 inductiva-0.0.5/setup.cfg
--rw-r--r--   0 lpcunha    (501) staff       (20)       56 2023-03-31 11:06:15.000000 inductiva-0.0.5/setup.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.137819 inductiva-0.0.6/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-03-29 15:57:40.000000 inductiva-0.0.6/MANIFEST.in
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      579 2023-04-11 15:58:03.137819 inductiva-0.0.6/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      205 2023-03-29 15:57:40.000000 inductiva-0.0.6/README.md
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      363 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/api/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/api/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13457 2023-04-10 16:30:57.000000 inductiva-0.0.6/inductiva/api/methods.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/client/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/api_client.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/path_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/admin_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/admin_user_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tag_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/tags/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/admin_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/tasks_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/configuration.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/model/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/body_upload_task_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/http_validation_error.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/new_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/queue_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/task_request.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/task_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/validation_error.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/models/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/models/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/admin_user/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/get.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/rest.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/schemas.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/cupy/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/cupy/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/cupy/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/math.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/slepc/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/slepc/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/slepc/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-10 14:10:43.000000 inductiva-0.0.6/inductiva/core/test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      411 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2579 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/_output_post_processing.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/fluid_types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/post_processing/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/post_processing/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5931 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/post_processing/splishsplash.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      110 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2341 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/dam_break.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6904 2023-04-10 16:28:58.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/unit_box.obj
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8165 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9161 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/shapes.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/fluids/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/dualsphysics.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1286 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/openfoam.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/splishsplash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/swash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-11 15:37:20.000000 inductiva-0.0.6/inductiva/fluids/simulators/xbeach.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1760 2023-04-11 14:04:20.000000 inductiva-0.0.6/inductiva/scenarios.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/simulation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/simulation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/simulation/simulator.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.137819 inductiva-0.0.6/inductiva/utils/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/utils/data.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      919 2023-04-11 14:04:20.000000 inductiva-0.0.6/inductiva/utils/files.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/files_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/flags.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/meta.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/utils/misc.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/utils/misc_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/templates.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10104 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/utils/visualization.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva.egg-info/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      579 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4014 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/requires.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/top_level.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-03 08:49:49.000000 inductiva-0.0.6/pyproject.toml
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-11 15:58:03.137819 inductiva-0.0.6/setup.cfg
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-03 08:49:49.000000 inductiva-0.0.6/setup.py
```

### Comparing `inductiva-0.0.5/PKG-INFO` & `inductiva-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `inductiva-0.0.5/inductiva/api/methods.py` & `inductiva-0.0.6/inductiva/api/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Methods that interact with the lower-level inductiva-web-api-client.
 
 The relevant function for usage outside of this file is invoke_api().
 Check the demos directory for examples on how it is used.
 """
+import asyncio
+import json
 import os
 import pathlib
 import signal
 import time
 from contextlib import contextmanager
-
 from typing import Any, Dict, Optional, Type
+from urllib.parse import urlparse
+
+import websockets
 from absl import logging
+
+import inductiva
 from inductiva.client import ApiClient, ApiException, Configuration
 from inductiva.client.apis.tags.tasks_api import TasksApi
-from inductiva.client.models import TaskRequest, TaskStatus, BodyUploadTaskInput
+from inductiva.client.models import (BodyUploadTaskInput, TaskRequest,
+                                     TaskStatus)
 from inductiva.exceptions import RemoteExecutionError
 from inductiva.types import Path
-
-import inductiva
 from inductiva.utils.data import (extract_output, get_validate_request_params,
                                   pack_input, unpack_output)
 from inductiva.utils.meta import get_method_name, get_type_annotations
 
 
 def submit_request(api_instance: TasksApi, request: TaskRequest) -> TaskStatus:
     """Submits a task request to the API.
@@ -93,15 +98,15 @@
         raise e
 
     logging.debug("Downloaded output to %s", api_response.body.name)
 
     return api_response.body.name
 
 
-def block_until_finish(api_instance: TasksApi, task_id: str) -> TaskRequest:
+def block_until_finish(api_instance: TasksApi, task_id: str) -> str:
     """Block until a task executing remotely finishes execution.
 
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
         task_id: ID of the task to wait for.
 
     Returns:
@@ -149,48 +154,33 @@
         task_id: ID of the task to wait for.
         desired_status: Task status to wait for.
         sleep_secs: Polling interval.
 
     Returns:
         Returns info related to the task, containing two fields,
     """
-    prev_queue_info = None
-
     prev_status = None
 
     while True:
         try:
             api_response = \
                 api_instance.get_task_status(
                     path_params={"task_id": task_id},
                 )
 
             status = api_response.body["status"]
-
-            logging.debug("Request status: %s", status)
+            logging.debug("Task status is %s", status)
         except ApiException as e:
             raise e
 
-        if status == "submitted":
-            queue_info = api_response.body["queue"]
-
-            if status != prev_status:
-                logging.info("Waiting for resources...")
+        if status == prev_status:
+            continue
 
-            if queue_info != prev_queue_info:
-                logging.info("\t> %d/%d executers busy.",
-                             queue_info["running_tasks"],
-                             queue_info["num_executers"])
-                logging.info("\t> %d requests ahead in the queue.",
-                             queue_info["tasks_ahead"])
-
-                prev_queue_info = queue_info
-        elif status == "started" and status != prev_status:
-            logging.info("An executer has picked up the request.")
-            logging.info("The requested task is being executed remotely...")
+        if status == "submitted":
+            logging.info("Waiting for resources...")
 
         prev_status = status
 
         # If status reaches the desired status, then stop polling
         if status in desired_status:
             break
 
@@ -228,32 +218,39 @@
         kill_task(api_instance, task_id)
         raise err
     finally:
         # Reset original SIGINT handler
         signal.signal(signal.SIGINT, original_sig)
 
 
-def invoke_api_from_fn_ptr(params,
-                           function_ptr,
-                           output_dir: Optional[Path] = None):
+def invoke_api_from_fn_ptr(
+    params,
+    function_ptr,
+    output_dir: Optional[Path] = None,
+    track_logs: bool = False,
+):
     """Perform a task remotely defined by a function pointer."""
     type_annotations = get_type_annotations(function_ptr)
     method_name = get_method_name(function_ptr)
-    return invoke_api(method_name,
-                      params,
-                      output_dir=output_dir,
-                      type_annotations=type_annotations,
-                      return_type=type_annotations["return"])
+    return invoke_api(
+        method_name,
+        params,
+        output_dir=output_dir,
+        type_annotations=type_annotations,
+        return_type=type_annotations["return"],
+        log_remote_execution=track_logs,
+    )
 
 
 def invoke_api(method_name: str,
                params,
                type_annotations: Dict[Any, Type],
                output_dir: Optional[Path] = None,
-               return_type: Type = pathlib.Path):
+               return_type: Type = pathlib.Path,
+               log_remote_execution: bool = False):
     """Perform a task remotely via Inductiva's Web API.
 
     Currently, the implementation handles the whole flow of the task execution,
     and blocks until the task finishes execution.
     The flow is summarized as follows:
         1. Transform request params into the params used to
         validate permission to execute the request.
@@ -317,46 +314,62 @@
                     original_params=params,
                     task_id=task_id,
                     type_annotations=type_annotations,
                 )
 
             logging.info("Request submitted.")
 
-            status = block_until_finish(
+            block_until_status_is(
                 api_instance=api_instance,
                 task_id=task_id,
+                desired_status={"started"},
             )
+            logging.info("An executer has picked up the request.")
+            logging.info("The requested task is being executed remotely...")
+
+            if log_remote_execution:
+                status = asyncio.run(follow_task(task_id))
+            else:
+                status = block_until_finish(
+                    api_instance=api_instance,
+                    task_id=task_id,
+                )
 
             if status == "success":
                 logging.info("Task executed successfuly.")
             else:
                 logging.info("Task failed.")
 
+        logging.info("Downloading output...")
         output_zip_path = download_output(
             api_instance=api_instance,
             task_id=task_id,
         )
+        logging.info("Output downloaded.")
 
     if output_dir is None:
         output_dir = os.path.join(inductiva.output_dir, task_id)
 
+    logging.info("Extracting output ZIP file to \"%s\"...", output_dir)
     result_list = extract_output(output_zip_path, output_dir)
+    logging.info("Output extracted.")
 
     if status == "failed":
         raise RemoteExecutionError(f"""Remote execution failed.
     Find more details in: \"{os.path.abspath(output_dir)}\".""")
 
     return unpack_output(result_list, output_dir, return_type)
 
 
 def run_simulation(
     api_method_name: str,
     input_dir: pathlib.Path,
     output_dir: pathlib.Path,
     params: Dict[str, Any],
+    log_remote_execution: bool = False,
 ) -> pathlib.Path:
 
     params = {
         "sim_dir": input_dir,
         **params,
     }
     type_annotations = {
@@ -365,13 +378,34 @@
 
     result = invoke_api(
         api_method_name,
         params,
         type_annotations,
         output_dir=output_dir,
         return_type=pathlib.Path,
+        log_remote_execution=log_remote_execution,
     )
 
     if not isinstance(result, pathlib.Path):
         raise RuntimeError(f"Expected result to be a Path, got {type(result)}")
 
     return result
+
+
+async def follow_task(task_id: str) -> str:
+    parsed_url = urlparse(inductiva.api_url)
+    url = f"ws://{parsed_url.hostname}:{parsed_url.port}/ \
+        task/{task_id}/logs/tail"
+
+    async with websockets.connect(url) as ws:
+        while True:
+            message = await ws.recv()
+            parsed_message = json.loads(message)
+
+            if parsed_message["type"] == "update":
+                status = parsed_message["content"]
+                logging.debug("Task status update: %s", status)
+
+                return status
+            else:
+                new_line = parsed_message["content"]
+                print(new_line, end="")
```

### Comparing `inductiva-0.0.5/inductiva/client/__init__.py` & `inductiva-0.0.6/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/api_client.py` & `inductiva-0.0.6/inductiva/client/api_client.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/apis/path_to_api.py` & `inductiva-0.0.6/inductiva/client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/apis/tags/admin_api.py` & `inductiva-0.0.6/inductiva/client/apis/tags/admin_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.0.6/inductiva/client/apis/tags/tasks_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/configuration.py` & `inductiva-0.0.6/inductiva/client/configuration.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/exceptions.py` & `inductiva-0.0.6/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.0.6/inductiva/client/model/body_upload_task_input.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/http_validation_error.py` & `inductiva-0.0.6/inductiva/client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/new_user.py` & `inductiva-0.0.6/inductiva/client/model/new_user.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/queue_status.py` & `inductiva-0.0.6/inductiva/client/model/queue_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/task_request.py` & `inductiva-0.0.6/inductiva/client/model/task_request.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/task_status.py` & `inductiva-0.0.6/inductiva/client/model/task_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/model/validation_error.py` & `inductiva-0.0.6/inductiva/client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/models/__init__.py` & `inductiva-0.0.6/inductiva/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/__init__.py` & `inductiva-0.0.6/inductiva/client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/admin_user/post.py` & `inductiva-0.0.6/inductiva/client/paths/admin_user/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/admin_user_username_tasks/get.py` & `inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/task_submit/post.py` & `inductiva-0.0.6/inductiva/client/paths/task_submit/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/task_task_id_input/post.py` & `inductiva-0.0.6/inductiva/client/paths/task_task_id_input/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/task_task_id_kill/post.py` & `inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/task_task_id_output/get.py` & `inductiva-0.0.6/inductiva/client/paths/task_task_id_output/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/paths/task_task_id_status/get.py` & `inductiva-0.0.6/inductiva/client/paths/task_task_id_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/rest.py` & `inductiva-0.0.6/inductiva/client/rest.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/client/schemas.py` & `inductiva-0.0.6/inductiva/client/schemas.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/core/math.py` & `inductiva-0.0.6/inductiva/core/math.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/_output_post_processing.py` & `inductiva-0.0.6/inductiva/fluids/_output_post_processing.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/fluid_types.py` & `inductiva-0.0.6/inductiva/fluids/fluid_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/post_processing/splishsplash.py` & `inductiva-0.0.6/inductiva/fluids/post_processing/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/dam_break/dam_break.py` & `inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/dam_break.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Describes the physical scenarios and runs its simulation via API."""
 from typing import List, Literal, Optional
 from enum import Enum
 from dataclasses import dataclass
 
+from inductiva.simulation import Simulator
 from inductiva.fluids.scenarios.fluid_block import FluidBlock
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.fluid_types import WATER
 from inductiva.types import Path
 
-from inductiva.fluids._output_post_processing import SimulationOutput
-
 
 @dataclass
 class ParticleRadius(Enum):
     """Sets particle radius according to resolution."""
     HIGH = 0.008
     MEDIUM = 0.012
     LOW = 0.02
@@ -37,54 +36,40 @@
             pisition: A list containing fluid column position in a tank,
               in meters.
             """
 
         if dimensions is None:
             dimensions = [0.3, 1, 1]
 
-        FluidBlock.__init__(self,
-                            density=fluid.density,
-                            kinematic_viscosity=fluid.kinematic_viscosity,
-                            dimensions=dimensions,
-                            position=position)
-
-    #pylint: disable=arguments-renamed
-    def simulate(self,
-                 device: Literal["cpu", "gpu"] = "cpu",
-                 engine: Literal["SPlisHSPlasH",
-                                 "DualSPHysics"] = "SPlisHSPlasH",
-                 simulation_time: float = 1.,
-                 resolution: Literal["high", "medium", "low"] = "medium",
-                 output_dir: Optional[Path] = None):
-        """Runs SPH simulation of Dam Break scenario.
-
-        Use the FluidBlock class to run a simulation with less freedom of
-        choice of the parameters. Namely, the Dam Break scenario only allows
-        to change the following arguments.
+        super().__init__(density=fluid.density,
+                         kinematic_viscosity=fluid.kinematic_viscosity,
+                         dimensions=dimensions,
+                         position=position)
 
+    # pylint: disable=arguments-renamed
+    def simulate(
+        self,
+        simulator: Simulator,
+        output_dir: Optional[Path] = None,
+        device: Literal["cpu", "gpu"] = "cpu",
+        resolution: Literal["high", "medium", "low"] = "medium",
+        simulation_time: float = 1,
+    ):
+        """Simulates the scenario.
+        
         Args:
-            device: Sets the device for a simulation to be run.
-            engine: The software platform to be used for the simulation.
-              Available options are (the default is DualSPHysics):
-              - SPlisHSPlasH
-              - DualSPHysics
-            resolution: Sets the fluid resolution to simulate.
-              Available options are (the default is "medium"):
-                - "high"
-                - "medium"
-                - "low"
-            simulation_time: Simulation time in seconds.
-            output_dir: Directory in which the output files will be saved. If
-              not specified, the default directory used for API tasks
-              (based on an internal ID of the task) will be used.
+            simulator: Simulator to use.
+            output_dir: Directory to store the simulation output.
+            device: Device in which to run the simulation.
+            resolution: Resolution of the simulation.
+            simulation_time: Simulation time, in seconds.
         """
 
         particle_radius = ParticleRadius[resolution.upper()].value
 
-        sim_output_path = FluidBlock.simulate(self,
-                                              device=device,
-                                              engine=engine,
-                                              simulation_time=simulation_time,
-                                              particle_radius=particle_radius,
-                                              output_dir=output_dir)
-
-        return SimulationOutput(sim_output_path)
+        return super().simulate(
+            simulator,
+            output_dir=output_dir,
+            device=device,
+            particle_radius=particle_radius,
+            simulation_time=simulation_time,
+        )
```

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/dam_break_template.dualsphysics.xml.jinja` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

 * *Files 10% similar despite different names*

#### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/dam_break_template.dualsphysics.xml.jinja` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

```diff
@@ -43,16 +43,17 @@
   </casedef>
   <execution>
     <parameters>
       <parameter key="Kernel" value="1" comment="Interaction Kernel 1:Cubic Spline, 2:Wendland (default=2)"/>
       <parameter key="ViscoTreatment" value="2" comment="Viscosity formulation 1:Artificial, 2:Laminar+SPS (default=1)"/>
       <parameter key="Visco" value="{{ fluid.kinematic_viscosity }}" comment="Viscosity value"/>
       <parameter key="DensityDT" value="2" comment="Density Diffusion Term 0:None, 1:Molteni, 2:Fourtakas, 3:Fourtakas(full) (default=0)"/>
-      <parameter key="DtIni" value="0" comment="Initial time step. Use 0 to defult use (default=h/speedsound)" units_comment="seconds"/>
+      <parameter key="DtIni" value="{{ time_step }}" comment="Initial time step. Use 0 to defult use (default=h/speedsound)" units_comment="seconds"/>
       <parameter key="DtMin" value="0" comment="Minimum time step. Use 0 to defult use (default=coefdtmin*h/speedsound)" units_comment="seconds"/>
+      <parameter key="DtFixed" value="{{ 0 | int if adaptive_time_step else time_step }}" comment="Fixed Dt value. Use 0 to disable (default=disabled)" units_comment="seconds"/>
       <parameter key="TimeMax" value="{{ simulation_time }}" comment="Time of simulation" units_comment="seconds"/>
       <parameter key="TimeOut" value="{{ output_time_step }}" comment="Time frequency in which the data is exported" units_comment="seconds"/>
       <simulationdomain comment="Defines domain of simulation (default=Uses minimum and maximum position of the generated particles)">
         <posmin x="default" y="default" z="default" comment="e.g.: x=0.5, y=default-1, z=default-10%"/>
         <posmax x="default" y="default" z="default + 50%"/>
       </simulationdomain>
     </parameters>
```

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/fluid_block.py` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 """Describes the physical scenarios and runs its simulation via API."""
-import tempfile
 import os
-import math
 from typing import List, Literal, Optional
 import shutil
-from pathlib import PurePosixPath
-
-from absl import logging
 
+from inductiva.types import Path
+from inductiva.scenarios import Scenario
+from inductiva.simulation import Simulator
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.simulators import SPlisHSPlasH
 from inductiva.fluids.simulators import DualSPHysics
-from inductiva.fluids.post_processing.splishsplash import convert_vtk_data_dir_to_netcdf
-from inductiva.types import Path
 from inductiva.utils.templates import replace_params_in_template
 
-# Global variables to define a scenario
 TANK_DIMENSIONS = [1, 1, 1]
-TIME_STEP = 0.001
 
 SPLISHSPLASH_TEMPLATE_FILENAME = "fluid_block_template.splishsplash.json.jinja"
-SPLISHSPLASH_INPUT_FILENAME = "fluid_block.json"
+SPLISHSPLASH_CONFIG_FILENAME = "fluid_block.json"
 UNIT_BOX_MESH_FILENAME = "unit_box.obj"
 
-SPLISHSPLASH_OUTPUT_TIM_STEP = 1. / 60.
-DUALSPH_OUTPUT_TIME_STEP = 0.01
+DUALSPHYSICS_TEMPLATE_FILENAME = "fluid_block_template.dualsphysics.xml.jinja"
+DUALSPHYSICS_CONFIG_FILENAME = "dam_break.xml"
 
-DUALSPHYSICS_TEMPLATE_FILENAME = "dam_break_template.dualsphysics.xml.jinja"
-DUALSPHYSICS_INPUT_FILENAME = "dam_break.xml"
 
-
-class FluidBlock:
+class FluidBlock(Scenario):
     """Physical scenario of a general fluid block simulation."""
 
     def __init__(self,
                  density: float,
                  kinematic_viscosity: float,
                  dimensions: List[float],
                  position: Optional[List[float]] = None,
@@ -57,160 +48,135 @@
                                kinematic_viscosity=kinematic_viscosity)
 
         if len(dimensions) != 3:
             raise ValueError("`fluid_dimensions` must have 3 values.")
         self.dimensions = dimensions
 
         if position is None:
-            self.position = [0.0, 0.0, 0.0]
+            self.position = [0, 0, 0]
         else:
             self.position = position
 
         if inital_velocity is None:
-            self.initial_velocity = [0.0, 0.0, 0.0]
+            self.initial_velocity = [0, 0, 0]
         else:
             self.initial_velocity = inital_velocity
 
     def simulate(
         self,
-        device: Literal["cpu", "gpu"] = "cpu",
-        engine: Literal["DualSPHysics", "SPlisHSPlasH"] = "SPlisHSPlasH",
-        simulation_time: float = 1.,
-        particle_radius: float = 0.015,
+        simulator: Simulator,
         output_dir: Optional[Path] = None,
+        device: Literal["cpu", "gpu"] = "cpu",
+        particle_radius: float = 0.02,
+        simulation_time: float = 1,
+        adaptive_time_step: bool = True,
+        particle_sorting: bool = True,
+        time_step: float = 0.001,
+        output_time_step: float = 0.02,
     ):
-        """Runs SPH simulation of the fluid block scenario.
-
+        """Simulates the scenario.
+        
         Args:
-            device: Sets the device for a simulation to be run.
-            engine: The software platform to be used for the simulation.
-            Available options are (the default is DualSPHysics):
-            - SPlisHSPlasH
-            - DualSPHysics
-            particle_radius: Radius of the discretization particles, in meters.
-            Used to control particle spacing. Smaller particle radius means a
-            finer discretization, hence more particles.
-            time_max: Maximum time of simulation, in seconds.
-            output_dir: Directory in which the output files will be saved. If
-                not specified, the default directory used for API tasks
-                (based on an internal ID of the task) will be used.
-            engine_parameters: Simulator specific parameters.
+            simulator: Simulator to use.
+            output_dir: Directory to store the simulation output.
+            device: Device in which to run the simulation.
+            particle_radius: Radius of the fluid particles, in meters.
+            simulation_time: Simulation time, in seconds.
+            adaptive_time_step: Whether to use adaptive time step.
+            particle_sorting: Whether to use particle sorting.
+            time_step: Time step, in seconds.
+            output_time_step: Time step between outputs, in seconds.
         """
+
+        # TODO: Avoid storing these as class attributes.
         self.particle_radius = particle_radius
         self.simulation_time = simulation_time
-        self.device: Literal["cpu", "gpu"] = device
-        self.output_dir = output_dir
-        self.fluid_block_dir = os.path.dirname(__file__)
-
-        # Create a temporary directory to store simulation input files
-        self.input_temp_dir = tempfile.TemporaryDirectory()  #pylint: disable=consider-using-with
-
-        if engine.lower() == "splishsplash":
-            sim_output_path = self._splishsplash_simulation()
-        elif engine.lower() == "dualsphysics":
-            sim_output_path = self._dualsphysics_simulation()
-        else:
-            raise ValueError("Entered `engine` does not exist or it \
-                             does not match with `engine_parameters` class")
-
-        # Delete temporary input directory
-        self.input_temp_dir.cleanup()
-
-        return sim_output_path
-
-    def _splishsplash_simulation(self):
-        """Runs SPlisHSPlasH simulation via API."""
-
-        input_dir = self.input_temp_dir.name
-
-        unit_box_file_path = os.path.join(self.fluid_block_dir,
-                                          UNIT_BOX_MESH_FILENAME)
-        shutil.copy(unit_box_file_path, input_dir)
-
-        fluid_margin = 2 * self.particle_radius
-
-        replace_params_in_template(
-            templates_dir=self.fluid_block_dir,
-            template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
-            params={
-                "simulation_time": self.simulation_time,
-                "time_step": TIME_STEP,
-                "particle_radius": self.particle_radius,
-                "data_export_rate": 1 / SPLISHSPLASH_OUTPUT_TIM_STEP,
-                "tank_filename": UNIT_BOX_MESH_FILENAME,
-                "tank_dimensions": TANK_DIMENSIONS,
-                "fluid_filename": UNIT_BOX_MESH_FILENAME,
-                "fluid": self.fluid,
-                "fluid_position": [fluid_margin] * 3,
-                "fluid_dimensions": [
-                    dimension - 2 * fluid_margin
-                    for dimension in self.dimensions
-                ],
-                "fluid_velocity": self.initial_velocity,
-            },
-            output_file_path=os.path.join(input_dir,
-                                          SPLISHSPLASH_INPUT_FILENAME),
-        )
-
-        logging.info("Estimated number of particles %d",
-                     self.estimate_num_particles())
-        logging.info("Estimated number of time steps %s",
-                     math.ceil(self.simulation_time / TIME_STEP))
-        logging.info(
-            "Number of output time steps %s",
-            math.ceil(self.simulation_time / SPLISHSPLASH_OUTPUT_TIM_STEP))
-
-        simulator = SPlisHSPlasH()
-        sim_output_path = simulator.run(
-            input_dir=input_dir,
-            device=self.device,
-            output_dir=self.output_dir,
-            sim_config_filename=SPLISHSPLASH_INPUT_FILENAME,
-        )
-
-        convert_vtk_data_dir_to_netcdf(
-            data_dir=os.path.join(sim_output_path, "vtk"),
-            output_time_step=SPLISHSPLASH_OUTPUT_TIM_STEP,
-            netcdf_data_dir=os.path.join(sim_output_path, "netcdf"))
-
-        return sim_output_path
-
-    def _dualsphysics_simulation(self):
-        """Runs simulation on DualSPHysics via API."""
-
-        replace_params_in_template(
-            templates_dir=self.fluid_block_dir,
-            template_filename=DUALSPHYSICS_TEMPLATE_FILENAME,
-            params={
-                "simulation_time": self.simulation_time,
-                "particle_radius": 2 * self.particle_radius,
-                "output_time_step": DUALSPH_OUTPUT_TIME_STEP,
-                "tank_dimensions": TANK_DIMENSIONS,
-                "fluid_dimensions": self.dimensions,
-                "fluid_position": self.position,
-                "fluid": self.fluid,
-            },
-            output_file_path=os.path.join(self.input_temp_dir.name,
-                                          DUALSPHYSICS_INPUT_FILENAME),
-        )
-
-        simulator = DualSPHysics()
-        return simulator.run(
-            input_dir=self.input_temp_dir.name,
-            sim_config_filename=PurePosixPath(DUALSPHYSICS_INPUT_FILENAME).stem,
-            device=self.device,
-            output_dir=self.output_dir,
+        self.adaptive_time_step = adaptive_time_step
+        self.particle_sorting = particle_sorting
+        self.time_step = time_step
+        self.output_time_step = output_time_step
+
+        output_path = super().simulate(
+            simulator,
+            output_dir=output_dir,
+            device=device,
         )
 
-    def estimate_num_particles(self):
-        """Estimate of the number of SPH particles contained in fluid blocks."""
-
-        # Calculate number of particles for a fluid block
-        n_particles_x = round(self.dimensions[0] /
-                              (2 * self.particle_radius)) - 1
-        n_particles_y = round(self.dimensions[1] /
-                              (2 * self.particle_radius)) - 1
-        n_particles_z = round(self.dimensions[2] /
-                              (2 * self.particle_radius)) - 1
-
-        # Add number of particles to the total sum
-        return n_particles_x * n_particles_y * n_particles_z
+        # TODO: Add any kind of post-processing here, e.g. convert files?
+        # convert_vtk_data_dir_to_netcdf(
+        #     data_dir=os.path.join(output_path, "vtk"),
+        #     output_time_step=SPLISHSPLASH_OUTPUT_TIM_STEP,
+        #     netcdf_data_dir=os.path.join(output_path, "netcdf"))
+
+        return output_path
+
+
+@FluidBlock.get_config_filename.register
+def _(cls, simulator: SPlisHSPlasH):  # pylint: disable=unused-argument
+    """Returns the configuration filename for SPlisHSPlasH."""
+    return SPLISHSPLASH_CONFIG_FILENAME
+
+
+@FluidBlock.gen_aux_files.register
+def _(self, simulator: SPlisHSPlasH, input_dir):  # pylint: disable=unused-argument
+    """Generates auxiliary files for SPlisHSPlasH."""
+    unit_box_file_path = os.path.join(os.path.dirname(__file__),
+                                      UNIT_BOX_MESH_FILENAME)
+    shutil.copy(unit_box_file_path, input_dir)
+
+
+@FluidBlock.gen_config.register
+def _(self, simulator: SPlisHSPlasH, input_dir: str):  # pylint: disable=unused-argument
+    """Generates the configuration file for SPlisHSPlasH."""
+
+    fluid_margin = 2 * self.particle_radius
+
+    replace_params_in_template(
+        templates_dir=os.path.dirname(__file__),
+        template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
+        params={
+            "simulation_time": self.simulation_time,
+            "time_step": self.time_step,
+            "particle_radius": self.particle_radius,
+            "data_export_rate": 1 / self.output_time_step,
+            "tank_filename": UNIT_BOX_MESH_FILENAME,
+            "tank_dimensions": TANK_DIMENSIONS,
+            "fluid_filename": UNIT_BOX_MESH_FILENAME,
+            "fluid": self.fluid,
+            "fluid_position": [fluid_margin] * 3,
+            "fluid_dimensions": [
+                dimension - 2 * fluid_margin for dimension in self.dimensions
+            ],
+            "fluid_velocity": self.initial_velocity,
+            "particle_sorting": self.particle_sorting,
+            "adaptive_time_step": self.adaptive_time_step,
+        },
+        output_file_path=os.path.join(input_dir, SPLISHSPLASH_CONFIG_FILENAME),
+    )
+
+
+@FluidBlock.get_config_filename.register
+def _(cls, simulator: DualSPHysics):  # pylint: disable=unused-argument
+    """Returns the configuration filename for DualSPHysics."""
+    return DUALSPHYSICS_CONFIG_FILENAME
+
+
+@FluidBlock.gen_config.register
+def _(self, simulator: DualSPHysics, input_dir: str):  # pylint: disable=unused-argument
+    """Generates the configuration file for DualSPHysics."""
+
+    replace_params_in_template(
+        templates_dir=os.path.dirname(__file__),
+        template_filename=DUALSPHYSICS_TEMPLATE_FILENAME,
+        params={
+            "simulation_time": self.simulation_time,
+            "time_step": self.time_step,
+            "particle_distance": 2 * self.particle_radius,
+            "output_time_step": self.output_time_step,
+            "tank_dimensions": TANK_DIMENSIONS,
+            "fluid_dimensions": self.dimensions,
+            "fluid_position": self.position,
+            "fluid": self.fluid,
+            "adaptive_time_step": self.adaptive_time_step,
+        },
+        output_file_path=os.path.join(input_dir, DUALSPHYSICS_CONFIG_FILENAME),
+    )
```

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,24 @@
     "Configuration": {
         "stopAt": {{ simulation_time }},
         "timeStepSize": {{ time_step }},
         "particleRadius": {{ particle_radius }},
         "simulationMethod": 4,
         "boundaryHandlingMethod": 0,
         "kernel": 1,
-        "cflMethod": 1,
+        "cflMethod": {{ adaptive_time_step | int }},
         "cflFactor": 0.5,
         "cflMinTimeStepSize": 0.0001,
         "cflMaxTimeStepSize": 0.005,
         "gravitation": [0, 0, -9.81],
         "gradKernel": 1,
         "enableVTKExport": true,
         "dataExportFPS": {{ data_export_rate }},
-        "particleAttributes": "velocity;density"
+        "particleAttributes": "velocity;density",
+        "enableZSort": {{ particle_sorting | tojson }}
     },
     "RigidBodies": [
         {
             "geometryFile": "{{ tank_filename }}",
             "translation": [0, 0, 0],
             "scale": {{ tank_dimensions }},
             "isDynamic": false
```

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_block/unit_box.obj` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/unit_box.obj`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 """Classes describing fluid tank scenarios."""
 
 from dataclasses import dataclass, field
+from enum import Enum
 import os
-import tempfile
 from typing import List, Literal, Optional
 
 from inductiva.types import Path
+from inductiva.scenarios import Scenario
+from inductiva.simulation import Simulator
 from inductiva.fluids.shapes import BaseShape
 from inductiva.fluids.shapes import Rectangle
 from inductiva.fluids.shapes import Circle
 from inductiva.fluids.shapes import Cube
 from inductiva.fluids.shapes import Cylinder
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.fluid_types import WATER
 from inductiva.fluids.simulators import SPlisHSPlasH
 from inductiva.fluids.post_processing.splishsplash import convert_vtk_data_dir_to_netcdf
 from inductiva.utils.templates import replace_params_in_template
 
-from inductiva.fluids._output_post_processing import SimulationOutput
-
 from . import mesh_file_utils
 
 SPLISHSPLASH_TEMPLATE_FILENAME = "fluid_tank_template.splishsplash.json.jinja"
-SPLISHSPLASH_INPUT_FILENAME = "fluid_tank.json"
+SPLISHSPLASH_CONFIG_FILENAME = "fluid_tank.json"
 TANK_MESH_FILENAME = "tank.obj"
 FLUID_MESH_FILENAME = "fluid.obj"
 
-SIMULATION_TIME = 5
-OUTPUT_TIME_STEP = 0.1
-TIME_STEP = 0.005
-PARTICLE_RADIUS = 0.02
-Z_SORT = False
+
+@dataclass
+class ParticleRadius(Enum):
+    """Sets particle radius according to resolution."""
+    HIGH = 0.005
+    MEDIUM = 0.01
+    LOW = 0.02
+
+
+@dataclass
+class TimeStep(Enum):
+    """Sets time step according to resolution."""
+    HIGH = 0.0025
+    MEDIUM = 0.005
+    LOW = 0.01
 
 
 # Tank inlets.
 @dataclass
 class BaseTankInlet:
     """Base tank inlet."""
     fluid_velocity: float = 1
@@ -102,15 +112,15 @@
         self.shape = Cylinder(
             radius=radius,
             height=height,
             position=[*top_base_position, -height],
         )
 
 
-class FluidTank:
+class FluidTank(Scenario):
     """Fluid tank."""
 
     def __init__(
         self,
         shape: BaseShape = Cylinder(radius=0.5, height=1),
         fluid: FluidType = WATER,
         fluid_level: float = 0,
@@ -131,120 +141,56 @@
         self.fluid = fluid
         self.fluid_level = fluid_level
         self.inlet = inlet
         self.outlet = outlet
 
     def simulate(
         self,
-        device: Literal["cpu", "gpu"] = "cpu",
-        engine: Literal["SPlisHSPlasH"] = "SPlisHSPlasH",
+        simulator: Simulator,
         output_dir: Optional[Path] = None,
+        device: Literal["cpu", "gpu"] = "cpu",
+        simulation_time: float = 5,
+        resolution: Literal["low", "medium", "high"] = "low",
+        output_time_step: float = 0.1,
+        particle_sorting: bool = False,
     ):
-        """Simulates the fluid tank.
-
+        """Simulates the scenario.
+        
         Args:
-            device: Device to run the simulation on.
-            engine: Simulation engine to use.
-            engine_params: Engine parameters.
-            output_dir: Directory to store simulation output.
-
-        Returns:
-            Simulation output.
+            simulator: Simulator to use.
+            output_dir: Directory to store the simulation output.
+            device: Device in which to run the simulation.
+            simulation_time: Simulation time, in seconds.
+            output_time_step: Time step between output files, in seconds.
+            resolution: Resolution of the simulation. Controls the particle
+                radius and time step.
+            particle_sorting: Whether to use particle sorting.
         """
 
-        # Create a temporary directory to store simulation input files
-        self.input_temp_dir = tempfile.TemporaryDirectory()  #pylint: disable=consider-using-with
-
-        if engine.lower() == "splishsplash":
-            sim_output_path = self._simulate_with_splishsplash(
-                device=device, output_dir=output_dir)
-        elif engine.lower() == "dualsphysics":
-            raise NotImplementedError(
-                "The engine 'DualSPHysics' is not supported yet "
-                "for fluid tank simulations.")
-        else:
-            raise ValueError(f"Invalid engine `{engine}`.")
-
-        # Delete temporary input directory
-        self.input_temp_dir.cleanup()
-
-        return SimulationOutput(sim_output_path)
-
-    def _simulate_with_splishsplash(self, device, output_dir):
-        """Simulates the fluid tank with SPlisHSPlasH."""
-
-        input_dir = self.input_temp_dir.name
-
-        self._create_splishsplash_aux_files(input_dir)
-        self._replace_params_in_splishsplash_template(input_dir)
-
-        simulator = SPlisHSPlasH()
-
-        output_path = simulator.run(
-            input_dir=input_dir,
-            sim_config_filename=SPLISHSPLASH_INPUT_FILENAME,
+        self.simulation_time = simulation_time
+        self.particle_radius = ParticleRadius[resolution.upper()].value
+        self.time_step = TimeStep[resolution.upper()].value
+        self.output_time_step = output_time_step
+        self.particle_sorting = particle_sorting
+
+        output_path = super().simulate(
+            simulator,
+            output_dir=output_dir,
             device=device,
-            output_dir=output_dir)
+        )
 
+        # TODO: Add any kind of post-processing here, e.g. convert files?
         convert_vtk_data_dir_to_netcdf(
             data_dir=os.path.join(output_path, "vtk"),
-            output_time_step=OUTPUT_TIME_STEP,
+            output_time_step=self.output_time_step,
             netcdf_data_dir=os.path.join(output_path, "netcdf"))
 
         return output_path
 
-    def _create_splishsplash_aux_files(self, input_dir):
-        """Creates auxiliary files for SPlisHSPlasH simulation."""
-
-        mesh_file_utils.create_tank_mesh_file(
-            shape=self.shape,
-            outlet=self.outlet,
-            path=os.path.join(input_dir, TANK_MESH_FILENAME),
-        )
-
-        mesh_file_utils.create_tank_fluid_mesh_file(
-            shape=self.shape,
-            fluid_level=self.fluid_level,
-            margin=2 * PARTICLE_RADIUS,
-            path=os.path.join(input_dir, FLUID_MESH_FILENAME),
-        )
-
-    def _replace_params_in_splishsplash_template(self, input_dir):
-        """Replaces parameters in SPlisHSPlasH template input file."""
-
-        bounding_box_min, bounding_box_max = self._get_bounding_box()
-        inlet_position = [
-            self.inlet.position[0],
-            self.inlet.position[1],
-            bounding_box_max[2],
-        ]
-
-        replace_params_in_template(
-            templates_dir=os.path.dirname(__file__),
-            template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
-            params={
-                "simulation_time": SIMULATION_TIME,
-                "time_step": TIME_STEP,
-                "particle_radius": PARTICLE_RADIUS,
-                "data_export_rate": 1 / OUTPUT_TIME_STEP,
-                "z_sort": Z_SORT,
-                "tank_filename": TANK_MESH_FILENAME,
-                "fluid_filename": FLUID_MESH_FILENAME,
-                "fluid": self.fluid,
-                "inlet_position": inlet_position,
-                "inlet_width": int(self.inlet.radius / PARTICLE_RADIUS),
-                "inlet_fluid_velocity": self.inlet.fluid_velocity,
-                "bounding_box_min": bounding_box_min,
-                "bounding_box_max": bounding_box_max,
-            },
-            output_file_path=os.path.join(input_dir,
-                                          SPLISHSPLASH_INPUT_FILENAME),
-        )
-
-    def _get_bounding_box(self):
+    def get_bounding_box(self):
         """Gets the bounding box of the tank.
 
         Returns:
             Tuple of two lists representing the minimum and maximum coordinates
             of the bounding box of the tank, respectively.
         """
 
@@ -252,7 +198,63 @@
 
         # Extend the bounding box to include the outlet.
         if self.outlet is not None:
             outlet_bounding_box_min, _ = self.outlet.shape.get_bounding_box()
             bounding_box_min[2] = outlet_bounding_box_min[2]
 
         return bounding_box_min, bounding_box_max
+
+
+@FluidTank.get_config_filename.register
+def _(cls, simulator: SPlisHSPlasH) -> str:  # pylint: disable=unused-argument
+    """Returns the config filename for SPlisHSPlasH."""
+    return SPLISHSPLASH_CONFIG_FILENAME
+
+
+@FluidTank.gen_aux_files.register
+def _(self, simulator: SPlisHSPlasH, input_dir):  # pylint: disable=unused-argument
+    """Generates auxiliary files for SPlisHSPlasH."""
+    mesh_file_utils.create_tank_mesh_file(
+        shape=self.shape,
+        outlet=self.outlet,
+        path=os.path.join(input_dir, TANK_MESH_FILENAME),
+    )
+
+    mesh_file_utils.create_tank_fluid_mesh_file(
+        shape=self.shape,
+        fluid_level=self.fluid_level,
+        margin=2 * self.particle_radius,
+        path=os.path.join(input_dir, FLUID_MESH_FILENAME),
+    )
+
+
+@FluidTank.gen_config.register
+def _(self, simulator: SPlisHSPlasH, input_dir: str):  # pylint: disable=unused-argument
+    """Generates the configuration file for SPlisHSPlasH."""
+
+    bounding_box_min, bounding_box_max = self.get_bounding_box()
+    inlet_position = [
+        self.inlet.position[0],
+        self.inlet.position[1],
+        bounding_box_max[2],
+    ]
+
+    replace_params_in_template(
+        templates_dir=os.path.dirname(__file__),
+        template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
+        params={
+            "simulation_time": self.simulation_time,
+            "time_step": self.time_step,
+            "particle_radius": self.particle_radius,
+            "data_export_rate": 1 / self.output_time_step,
+            "z_sort": self.particle_sorting,
+            "tank_filename": TANK_MESH_FILENAME,
+            "fluid_filename": FLUID_MESH_FILENAME,
+            "fluid": self.fluid,
+            "inlet_position": inlet_position,
+            "inlet_width": int(self.inlet.radius / self.particle_radius),
+            "inlet_fluid_velocity": self.inlet.fluid_velocity,
+            "bounding_box_min": bounding_box_min,
+            "bounding_box_max": bounding_box_max,
+        },
+        output_file_path=os.path.join(input_dir, SPLISHSPLASH_CONFIG_FILENAME),
+    )
```

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py` & `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/shapes.py` & `inductiva-0.0.6/inductiva/fluids/shapes.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/fluids/simulators/dualsphysics.py` & `inductiva-0.0.6/inductiva/fluids/simulators/xbeach.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """DualSPHysics module of the API."""
 import pathlib
-from typing import Literal, Optional
+from typing import Optional
 
 from inductiva import types
 from inductiva.simulation import Simulator
 
 
-class DualSPHysics(Simulator):
-    """Class to invoke a generic DualSPHysics simulation on the API."""
+class XBeach(Simulator):
+    """Class to invoke a generic XBeach simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
-        return "sph.dualsphysics.run_simulation"
+        return "sw.xbeach.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
-        sim_config_filename: str,
+        sim_config_filename: Optional[str] = "params.txt",
         output_dir: Optional[types.Path] = None,
-        device: Literal["gpu", "cpu"] = "cpu",
+        n_cores: int = 1,
+        track_logs: bool = False,
     ) -> pathlib.Path:
         """Run the simulation.
 
         Args:
-            device: Device in which to run the simulation.
+            n_cores: Number of MPI cores to use for the simulation.
+            other arguments: See the documentation of the base class.
         """
-        return super().run(input_dir,
-                           output_dir,
-                           device=device,
-                           input_filename=sim_config_filename)
+        return super().run(
+            input_dir,
+            input_filename=sim_config_filename,
+            n_cores=n_cores,
+            track_logs=track_logs,
+            output_dir=output_dir,
+        )
```

### Comparing `inductiva-0.0.5/inductiva/fluids/simulators/openfoam.py` & `inductiva-0.0.6/inductiva/fluids/simulators/openfoam.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 
 
 class OpenFOAM(Simulator):
     """Class to invoke a generic DualSPHysics simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
-        return "fvm.opemfoam.run_simulation"
+        return "fvm.openfoam.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
         output_dir: Optional[types.Path] = None,
         openfoam_solver: str = "isoFoam",
         n_cores=1,
+        track_logs: bool = False,
     ) -> pathlib.Path:
         """Run the simulation.
 
         Args:
             n_cores: Number of MPI cores to use for the simulation.
             openfoam_solver: specific solver to simulate with OpenFOAM.
                 OpenFOAM contains lots of solvers inside of it, which are used
                 to call the run simulation through terminal, e.g.,
                 [isoFoam, sonicFoam, ...]. The default solver is isoFoam.
+            other arguments: See the documentation of the base class.
         """
         return super().run(
             input_dir,
-            output_dir,
+            output_dir=output_dir,
+            track_logs=track_logs,
             openfoam_solver=openfoam_solver,
             n_cores=n_cores,
         )
```

### Comparing `inductiva-0.0.5/inductiva/fluids/simulators/splishsplash.py` & `inductiva-0.0.6/inductiva/fluids/simulators/dualsphysics.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 import pathlib
 from typing import Literal, Optional
 
 from inductiva import types
 from inductiva.simulation import Simulator
 
 
-class SPlisHSPlasH(Simulator):
-    """Class to invoke a generic SPlisHSPlasH simulation on the API."""
+class DualSPHysics(Simulator):
+    """Class to invoke a generic DualSPHysics simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
-        return "sph.splishsplash.run_simulation"
+        return "sph.dualsphysics.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
         sim_config_filename: str,
         output_dir: Optional[types.Path] = None,
         device: Literal["gpu", "cpu"] = "cpu",
+        track_logs: bool = False,
     ) -> pathlib.Path:
         """Run the simulation.
 
         Args:
             device: Device in which to run the simulation.
+            sim_config_filename: Name of the simulation configuration file.
+            other arguments: See the documentation of the base class.
         """
         return super().run(input_dir,
                            output_dir=output_dir,
+                           track_logs=track_logs,
                            device=device,
                            input_filename=sim_config_filename)
```

### Comparing `inductiva-0.0.5/inductiva/simulation/simulator.py` & `inductiva-0.0.6/inductiva/simulation/simulator.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,20 +15,34 @@
     @abstractmethod
     def api_method_name(self) -> str:
         pass
 
     def run(
         self,
         input_dir: types.Path,
-        *_args,  # unused in this method, but defined to allow for more
-        # non-default arguments in method override in subclasses.
+        *_args,
         output_dir: Optional[types.Path] = None,
+        track_logs: bool = False,
         **kwargs,
     ) -> pathlib.Path:
-        """Run the simulation."""
+        """Run the simulation.
+
+        Args:
+            input_dir: Path to the directory containing the input files.
+            _args: Unused in this method, but defined to allow for more
+                non-default arguments in method override in subclasses.
+            output_dir: Path to the directory where the output files will be
+                stored. If not provided, a timestamped directory will be
+                created with the same name as the input directory appended
+                with "-output".
+            track_logs: If True, the logs of the remote execution will be
+                streamed to the console.
+            **kwargs: Additional keyword arguments to be passed to the
+                simulation API method.
+        """
         input_dir = files.resolve_path(input_dir)
         if not input_dir.is_dir():
             raise ValueError(
                 f"The provided path (\"{input_dir}\") is not a directory.")
 
         if output_dir is None:
             output_dir = input_dir.with_name(f"{input_dir.name}-output")
@@ -37,8 +51,9 @@
             output_dir = files.resolve_path(output_dir)
 
         return api.run_simulation(
             self.api_method_name,
             input_dir,
             output_dir,
             params=kwargs,
+            log_remote_execution=track_logs,
         )
```

### Comparing `inductiva-0.0.5/inductiva/utils/data.py` & `inductiva-0.0.6/inductiva/utils/data.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/utils/files_test.py` & `inductiva-0.0.6/inductiva/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/utils/flags.py` & `inductiva-0.0.6/inductiva/utils/flags.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/utils/meta.py` & `inductiva-0.0.6/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva/utils/visualization.py` & `inductiva-0.0.6/inductiva/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.5/inductiva.egg-info/PKG-INFO` & `inductiva-0.0.6/inductiva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `inductiva-0.0.5/inductiva.egg-info/SOURCES.txt` & `inductiva-0.0.6/inductiva.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 inductiva/__init__.py
 inductiva/exceptions.py
+inductiva/scenarios.py
 inductiva/types.py
 inductiva.egg-info/PKG-INFO
 inductiva.egg-info/SOURCES.txt
 inductiva.egg-info/dependency_links.txt
 inductiva.egg-info/requires.txt
 inductiva.egg-info/top_level.txt
 inductiva/api/__init__.py
@@ -70,16 +71,16 @@
 inductiva/fluids/shapes.py
 inductiva/fluids/post_processing/__init__.py
 inductiva/fluids/post_processing/splishsplash.py
 inductiva/fluids/scenarios/__init__.py
 inductiva/fluids/scenarios/dam_break/__init__.py
 inductiva/fluids/scenarios/dam_break/dam_break.py
 inductiva/fluids/scenarios/fluid_block/__init__.py
-inductiva/fluids/scenarios/fluid_block/dam_break_template.dualsphysics.xml.jinja
 inductiva/fluids/scenarios/fluid_block/fluid_block.py
+inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
 inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
 inductiva/fluids/scenarios/fluid_block/unit_box.obj
 inductiva/fluids/scenarios/fluid_tank/__init__.py
 inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
 inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
 inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
 inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
@@ -93,9 +94,11 @@
 inductiva/simulation/simulator.py
 inductiva/utils/__init__.py
 inductiva/utils/data.py
 inductiva/utils/files.py
 inductiva/utils/files_test.py
 inductiva/utils/flags.py
 inductiva/utils/meta.py
+inductiva/utils/misc.py
+inductiva/utils/misc_test.py
 inductiva/utils/templates.py
 inductiva/utils/visualization.py
```

### Comparing `inductiva-0.0.5/setup.cfg` & `inductiva-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductiva
-version = 0.0.5
+version = 0.0.6
 description = Python client for the Inductiva API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Inductiva Research Labs
 author_email = contact@inductiva.ai
 url = https://github.com/inductiva/inductiva
 classifiers = 
@@ -29,14 +29,15 @@
 	xarray
 	gmsh
 	meshio
 	vtk
 	imageio
 	imageio-ffmpeg
 	ipython
+	websockets
 
 [options.package_data]
 * = *.obj, *.jinja
 
 [options.packages.find]
 exclude = 
 	tests
```

