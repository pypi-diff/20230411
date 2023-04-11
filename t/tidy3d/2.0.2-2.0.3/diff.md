# Comparing `tmp/tidy3d-2.0.2.tar.gz` & `tmp/tidy3d-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.0.2.tar", last modified: Sat Apr  1 13:12:21 2023, max compression
+gzip compressed data, was "tidy3d-2.0.3.tar", last modified: Tue Apr 11 13:11:50 2023, max compression
```

## Comparing `tidy3d-2.0.2.tar` & `tidy3d-2.0.3.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.376561 tidy3d-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-01 13:11:58.000000 tidy3d-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-01 13:11:58.000000 tidy3d-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-01 13:12:21.376561 tidy3d-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-01 13:11:58.000000 tidy3d-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-01 13:11:58.000000 tidy3d-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.344562 tidy3d-2.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-01 13:11:58.000000 tidy3d-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 13:12:21.376561 tidy3d-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-01 13:11:58.000000 tidy3d-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.344562 tidy3d-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.344562 tidy3d-2.0.2/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.348562 tidy3d-2.0.2/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    48855 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.352562 tidy3d-2.0.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.352562 tidy3d-2.0.2/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.352562 tidy3d-2.0.2/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_plugins/test_resonance_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.356562 tidy3d-2.0.2/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.356562 tidy3d-2.0.2/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.364562 tidy3d-2.0.2/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23162 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.364562 tidy3d-2.0.2/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    69858 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146855 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.364562 tidy3d-2.0.2/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   115366 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.364562 tidy3d-2.0.2/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.364562 tidy3d-2.0.2/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.368562 tidy3d-2.0.2/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.368562 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.368562 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.368562 tidy3d-2.0.2/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.372562 tidy3d-2.0.2/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.372562 tidy3d-2.0.2/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.372562 tidy3d-2.0.2/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.372562 tidy3d-2.0.2/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/plugins/smatrix/smatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.376561 tidy3d-2.0.2/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.376561 tidy3d-2.0.2/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-04-01 13:11:58.000000 tidy3d-2.0.2/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 13:12:21.360562 tidy3d-2.0.2/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-01 13:12:21.000000 tidy3d-2.0.2/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-11 13:11:30.000000 tidy3d-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 13:11:30.000000 tidy3d-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 13:11:50.249168 tidy3d-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-11 13:11:30.000000 tidy3d-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-11 13:11:30.000000 tidy3d-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:11:50.249168 tidy3d-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-11 13:11:30.000000 tidy3d-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49798 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_resonance_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23162 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69858 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146855 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115895 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/smatrix/smatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21550 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.0.2/LICENSE` & `tidy3d-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/PKG-INFO` & `tidy3d-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.0.2
+Version: 2.0.3
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,15 +118,15 @@
 pip install pipx
 pipx run tidy3d configure
 ```
 
 You can also specify your API key directly as an option to this command using the `api-key` argument, for example:
 
 ```
-tidy3d configure --api-key=XXX
+tidy3d configure --apikey=XXX
 ```
 
 #### Manually
 
 Alternatively, you can manually set up the config file where Tidy3D looks for the API key. The API key must be in a file called `.tidy3d/config` located in your home directory, containing the following
 
 ```
```

### Comparing `tidy3d-2.0.2/README.md` & `tidy3d-2.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 pip install pipx
 pipx run tidy3d configure
 ```
 
 You can also specify your API key directly as an option to this command using the `api-key` argument, for example:
 
 ```
-tidy3d configure --api-key=XXX
+tidy3d configure --apikey=XXX
 ```
 
 #### Manually
 
 Alternatively, you can manually set up the config file where Tidy3D looks for the API key. The API key must be in a file called `.tidy3d/config` located in your home directory, containing the following
 
 ```
```

### Comparing `tidy3d-2.0.2/setup.py` & `tidy3d-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.0.3/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/_test_local/_test_data_performance.py` & `tidy3d-2.0.3/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/_test_local/_test_fit_web.py` & `tidy3d-2.0.3/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.0.3/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/_test_local/_test_web.py` & `tidy3d-2.0.3/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_IO.py` & `tidy3d-2.0.3/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_apodization.py` & `tidy3d-2.0.3/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_base.py` & `tidy3d-2.0.3/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_boundaries.py` & `tidy3d-2.0.3/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_custom.py` & `tidy3d-2.0.3/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_field_projection.py` & `tidy3d-2.0.3/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_geometry.py` & `tidy3d-2.0.3/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_grid.py` & `tidy3d-2.0.3/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_grid_spec.py` & `tidy3d-2.0.3/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_medium.py` & `tidy3d-2.0.3/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_meshgenerate.py` & `tidy3d-2.0.3/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_mode.py` & `tidy3d-2.0.3/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_monitor.py` & `tidy3d-2.0.3/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_sidewall.py` & `tidy3d-2.0.3/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_simulation.py` & `tidy3d-2.0.3/tests/test_components/test_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1496,7 +1496,38 @@
     with pytest.raises(Exception):
         _ = td.Structure(
             geometry=td.PolySlab(vertices=[(0, 0), (1, 0), (1, 1)], slab_bounds=(-1, 1)),
             medium=box.medium,
         )
     with pytest.raises(Exception):
         _ = td.Structure(geometry=td.Sphere(radius=1), medium=box.medium)
+
+
+@pytest.mark.parametrize("normal_axis", (0, 1, 2))
+def test_pml_boxes_2D(normal_axis):
+    """Ensure pml boxes have non-zero dimension for 2D sim."""
+
+    sim_size = [1, 1, 1]
+    sim_size[normal_axis] = 0
+    pml_on_kwargs = {dim: axis != normal_axis for axis, dim in enumerate("xyz")}
+
+    sim2d = td.Simulation(
+        size=sim_size,
+        run_time=1e-12,
+        grid_spec=td.GridSpec(wavelength=1.0),
+        sources=[
+            td.PointDipole(
+                center=(0, 0, 0),
+                polarization="Ex",
+                source_time=td.GaussianPulse(
+                    freq0=1e14,
+                    fwidth=1e12,
+                ),
+            )
+        ],
+        boundary_spec=td.BoundarySpec.pml(**pml_on_kwargs),
+    )
+
+    pml_boxes = sim2d._make_pml_boxes(normal_axis=normal_axis)
+
+    for pml_box in pml_boxes:
+        assert pml_box.size[normal_axis] > 0, "PML box has size of 0 in normal direction of 2D sim."
```

### Comparing `tidy3d-2.0.2/tests/test_components/test_source.py` & `tidy3d-2.0.3/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_components/test_types.py` & `tidy3d-2.0.3/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_data/test_data_arrays.py` & `tidy3d-2.0.3/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_data/test_monitor_data.py` & `tidy3d-2.0.3/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_data/test_sim_data.py` & `tidy3d-2.0.3/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_package/test_config.py` & `tidy3d-2.0.3/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_package/test_log.py` & `tidy3d-2.0.3/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_package/test_make_script.py` & `tidy3d-2.0.3/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_package/test_material_library.py` & `tidy3d-2.0.3/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_package/test_parametric_variants.py` & `tidy3d-2.0.3/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_adjoint.py` & `tidy3d-2.0.3/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.0.3/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.0.3/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.0.3/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_polyslab.py` & `tidy3d-2.0.3/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.0.3/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_auth.py` & `tidy3d-2.0.3/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_cli.py` & `tidy3d-2.0.3/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_material_fitter.py` & `tidy3d-2.0.3/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.0.3/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.0.3/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.0.3/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/test_web/test_webapi.py` & `tidy3d-2.0.3/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tests/utils.py` & `tidy3d-2.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/__init__.py` & `tidy3d-2.0.3/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/__main__.py` & `tidy3d-2.0.3/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/apodization.py` & `tidy3d-2.0.3/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/base.py` & `tidy3d-2.0.3/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/boundary.py` & `tidy3d-2.0.3/tidy3d/components/boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             and center frequency.
 
         Example
         -------
         >>> from tidy3d import GaussianPulse, PlaneWave, inf
         >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
         >>> pw_source = PlaneWave(
-        ...     size=(inf,inf,0), source_time=pulse, direction='+', angle_theta=1.5, angle_phi=0.3)
+        ...     size=(inf,inf,0), source_time=pulse, direction='+', angle_theta=0.2, angle_phi=0.3)
         >>> bloch = BlochBoundary.from_source(source=pw_source, domain_size=5, axis=0)
         """
 
         if not isinstance(source, BlochSourceType.__args__):
             raise SetupError(
                 "The `source` parameter must be `GaussianBeam`, `ModeSource`, `PlaneWave`, "
                 "or `TFSF` in order to define a Bloch boundary condition."
@@ -453,15 +453,15 @@
             Default: free space.
 
         Example
         -------
         >>> from tidy3d import GaussianPulse, PlaneWave, inf
         >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
         >>> pw_source = PlaneWave(
-        ...     size=(inf,inf,0), source_time=pulse, direction='+', angle_theta=1.5, angle_phi=0.3)
+        ...     size=(inf,inf,0), source_time=pulse, direction='+', angle_theta=0.2, angle_phi=0.3)
         >>> bloch = Boundary.bloch_from_source(source=pw_source, domain_size=5, axis=0)
         """
         plus = BlochBoundary.from_source(
             source=source, domain_size=domain_size, axis=axis, medium=medium
         )
         minus = BlochBoundary.from_source(
             source=source, domain_size=domain_size, axis=axis, medium=medium
```

### Comparing `tidy3d-2.0.2/tidy3d/components/data/data_array.py` & `tidy3d-2.0.3/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/data/dataset.py` & `tidy3d-2.0.3/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/data/monitor_data.py` & `tidy3d-2.0.3/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/data/sim_data.py` & `tidy3d-2.0.3/tidy3d/components/data/sim_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,50 @@
 
 
 class SimulationData(Tidy3dBaseModel):
     """Stores data from a collection of :class:`.Monitor` objects in a :class:`.Simulation`.
 
     Example
     -------
-    >>> from tidy3d import ModeSpec, GridSpec, ScalarFieldDataArray, FieldMonitor, FieldData
+    >>> import tidy3d as td
     >>> num_modes = 5
     >>> x = [-1,1]
     >>> y = [-2,0,2]
     >>> z = [-3,-1,1,3]
     >>> f = [2e14, 3e14]
     >>> t = [0, 1e-12, 2e-12]
     >>> mode_index = np.arange(num_modes)
     >>> direction = ["+", "-"]
     >>> coords = dict(x=x, y=y, z=z, f=f)
-    >>> scalar_field = ScalarFieldDataArray((1+1j) * np.random.random((2,3,4,2)), coords=coords)
-    >>> field_monitor = FieldMonitor(size=(2,4,6), freqs=[2e14, 3e14], name='field', fields=['Ex'])
+    >>> scalar_field = td.ScalarFieldDataArray((1+1j) * np.random.random((2,3,4,2)), coords=coords)
+    >>> field_monitor = td.FieldMonitor(
+    ...     size=(2,4,6),
+    ...     freqs=[2e14, 3e14],
+    ...     name='field',
+    ...     fields=['Ex'],
+    ... )
     >>> sim = Simulation(
     ...     size=(2, 4, 6),
-    ...     grid_spec=GridSpec(wavelength=1.0),
+    ...     grid_spec=td.GridSpec(wavelength=1.0),
     ...     monitors=[field_monitor],
     ...     run_time=2e-12,
+    ...     sources=[
+    ...         td.UniformCurrentSource(
+    ...             size=(0, 0, 0),
+    ...             center=(0, 0.5, 0),
+    ...             polarization="Hx",
+    ...             source_time=td.GaussianPulse(
+    ...                 freq0=2e14,
+    ...                 fwidth=4e13,
+    ...             ),
+    ...         )
+    ...     ],
     ... )
-    >>> field_data = FieldData(monitor=field_monitor, Ex=scalar_field)
-    >>> sim_data = SimulationData(simulation=sim, data=(field_data,))
+    >>> field_data = td.FieldData(monitor=field_monitor, Ex=scalar_field)
+    >>> sim_data = td.SimulationData(simulation=sim, data=(field_data,))
     """
 
     simulation: Simulation = pd.Field(
         ...,
         title="Simulation",
         description="Original :class:`.Simulation` associated with the data.",
     )
```

### Comparing `tidy3d-2.0.2/tidy3d/components/field_projection.py` & `tidy3d-2.0.3/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/geometry.py` & `tidy3d-2.0.3/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/grid/grid.py` & `tidy3d-2.0.3/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.0.3/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/grid/mesher.py` & `tidy3d-2.0.3/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/medium.py` & `tidy3d-2.0.3/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/mode.py` & `tidy3d-2.0.3/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/monitor.py` & `tidy3d-2.0.3/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/simulation.py` & `tidy3d-2.0.3/tidy3d/components/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 NUM_CELLS_WARN_EPSILON = 100_000_000
 # number of structures at which we warn about slow Simulation.epsilon()
 NUM_STRUCTURES_WARN_EPSILON = 10_000
 # for 2d materials. to find neighboring media, search a distance on either side
 # equal to this times the grid size
 DIST_NEIGHBOR_REL_2D_MED = 1e-5
 
+# height of the PML plotting boxes along any dimensions where sim.size[dim] == 0
+PML_HEIGHT_FOR_0_DIMS = 0.02
+
 
 class Simulation(Box):  # pylint:disable=too-many-public-methods
     """Contains all information about Tidy3d simulation.
 
     Example
     -------
     >>> from tidy3d import Sphere, Cylinder, PolySlab
@@ -990,20 +993,21 @@
                 # if the == test doesn't pass, that doesn't mean the materials are necessarily
                 # different, because it's possible that the sidewalls encounter different
                 # `Structure` objects but with an identical material profile, which is still
                 # a valid setup; in this case, compute the epsilon profile on the grid for each
                 # side wall - the profiles must be the same along the injection axis, so we take
                 # a single "stripe" of epsilon as the reference and subtract it from all other
                 # stripes, which should result in zero if all the epsilon profiles are the same
+                freq0 = source.source_time.freq0
                 _, plane_axs = source.pop_axis("xyz", axis=source.injection_axis)
-                ref_eps = self.epsilon(box=sidewall_surfaces[0], coord_key="centers", freq=None)
+                ref_eps = self.epsilon(box=sidewall_surfaces[0], coord_key="centers", freq=freq0)
                 kwargs = {plane_axs[0]: 0, plane_axs[1]: 0}
                 ref_eps = ref_eps.isel(**kwargs)
                 for surface in sidewall_surfaces:
-                    test_eps = self.epsilon(box=surface, coord_key="centers", freq=None) - ref_eps
+                    test_eps = self.epsilon(box=surface, coord_key="centers", freq=freq0) - ref_eps
                     if not np.allclose(test_eps.to_numpy(), 0):
                         raise SetupError(
                             f"All sidewalls of the TFSF source '{source.name}' must intersect "
                             "the same media along the injection axis "
                             f" '{'xyz'[source.injection_axis]}'."
                         )
 
@@ -1767,15 +1771,24 @@
     def _make_pml_box(self, pml_axis: Axis, pml_height: float, sign: int) -> Box:
         """Construct a :class:`.Box` representing an arborbing boundary to be plotted."""
         rmin, rmax = [list(bounds) for bounds in self.bounds_pml]
         if sign == -1:
             rmax[pml_axis] = rmin[pml_axis] + pml_height
         else:
             rmin[pml_axis] = rmax[pml_axis] - pml_height
-        return Box.from_bounds(rmin=rmin, rmax=rmax)
+        pml_box = Box.from_bounds(rmin=rmin, rmax=rmax)
+
+        # if any dimension of the sim has size 0, set the PML to a very small size along that dim
+        new_size = list(pml_box.size)
+        for dim_index, sim_size in enumerate(self.size):
+            if sim_size == 0.0:
+                new_size[dim_index] = PML_HEIGHT_FOR_0_DIMS
+        pml_box = pml_box.updated_copy(size=new_size)
+
+        return pml_box
 
     @equal_aspect
     @add_ax_if_none
     def plot_symmetries(
         self, x: float = None, y: float = None, z: float = None, ax: Ax = None
     ) -> Ax:
         """Plot each of simulation's symmetries on a plane defined by one nonzero x,y,z coordinate.
```

### Comparing `tidy3d-2.0.2/tidy3d/components/source.py` & `tidy3d-2.0.3/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/structure.py` & `tidy3d-2.0.3/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/types.py` & `tidy3d-2.0.3/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/validators.py` & `tidy3d-2.0.3/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/components/viz.py` & `tidy3d-2.0.3/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/config.py` & `tidy3d-2.0.3/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/constants.py` & `tidy3d-2.0.3/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/exceptions.py` & `tidy3d-2.0.3/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/log.py` & `tidy3d-2.0.3/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/material_library/material_library.py` & `tidy3d-2.0.3/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/material_library/material_reference.py` & `tidy3d-2.0.3/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.0.3/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.0.3/tidy3d/plugins/adjoint/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     Note
     ----
     This is an experimental feature and may not work on all systems or configurations.
     For more details, see ``https://realpython.com/async-io-python/``.
 
     Returns
     ------
-    Tuple[:class:`JaxSimulationData, ...]
+    Tuple[:class:`.JaxSimulationData`, ...]
         Contains the :class:`.JaxSimulationData` of each :class:`.JaxSimulation`.
     """
 
     simulations = {_task_name_orig(i, task_name_suffix): sim for i, sim in enumerate(simulations)}
 
     task_info = {task_name: jax_sim.to_simulation() for task_name, jax_sim in simulations.items()}
```

### Comparing `tidy3d-2.0.2/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.0.3/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.0.3/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.0.3/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.0.3/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/mode/solver.py` & `tidy3d-2.0.3/tidy3d/plugins/mode/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         Returns
         -------
         Tuple[Numpy, Numpy]
             The first array gives the E and H fields for all modes, the second one give sthe complex
             effective index.
         """
 
+        # freq += 0.0001j
         num_modes = mode_spec.num_modes
         bend_radius = mode_spec.bend_radius
         bend_axis = mode_spec.bend_axis
         angle_theta = mode_spec.angle_theta
         angle_phi = mode_spec.angle_phi
         omega = 2 * np.pi * freq
         k0 = omega / C_0
```

### Comparing `tidy3d-2.0.2/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.0.3/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.0.3/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.0.3/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.0.3/tidy3d/plugins/smatrix/smatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,19 @@
 
     @property
     def port_names(self) -> Tuple[List[str], List[str]]:
         """List of port names for inputs and outputs, respectively."""
 
         def get_port_names(matrix_elements: Tuple[str, int]) -> List[str]:
             """Get the port names from a list of (port name, mode index)."""
-            return [port_name for port_name, _ in matrix_elements]
+            port_names = []
+            for port_name, _ in matrix_elements:
+                if port_name not in port_names:
+                    port_names.append(port_name)
+            return port_names
 
         matrix_elements_in = self.matrix_indices_source(ports=self.ports, run_only=self.run_only)
         matrix_elements_out = self.matrix_indices_monitor(ports=self.ports)
 
         port_names_in = get_port_names(matrix_elements_in)
         port_names_out = get_port_names(matrix_elements_out)
```

### Comparing `tidy3d-2.0.2/tidy3d/updater.py` & `tidy3d-2.0.3/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/asynchronous.py` & `tidy3d-2.0.3/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/auth.py` & `tidy3d-2.0.3/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/cacert.pem` & `tidy3d-2.0.3/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/cli/app.py` & `tidy3d-2.0.3/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/cli/migrate.py` & `tidy3d-2.0.3/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/config.py` & `tidy3d-2.0.3/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/container.py` & `tidy3d-2.0.3/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/environment.py` & `tidy3d-2.0.3/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/http_management.py` & `tidy3d-2.0.3/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/httputils.py` & `tidy3d-2.0.3/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/material_fitter.py` & `tidy3d-2.0.3/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/material_libray.py` & `tidy3d-2.0.3/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/s3utils.py` & `tidy3d-2.0.3/tidy3d/web/s3utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,19 @@
     client = token.get_client()
     meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
 
     if not to_file:
         os.makedirs(resource_id, exist_ok=True)
         to_file = os.path.join(resource_id, os.path.basename(remote_filename))
 
+    # make the leading directories in the 'to_file', if specified.
+    base_dir, _ = os.path.split(to_file)
+    if base_dir and not os.path.exists(base_dir):
+        os.makedirs(base_dir, exist_ok=True)
+
     def _download(_callback: Callable) -> None:
         """Perform the download with a callback function.
 
         Parameters
         ----------
         _callback : Callable[[float], None]
             Callback function for download, accepts ``bytes_in_chunk``
```

### Comparing `tidy3d-2.0.2/tidy3d/web/simulation_task.py` & `tidy3d-2.0.3/tidy3d/web/simulation_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/task.py` & `tidy3d-2.0.3/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/types.py` & `tidy3d-2.0.3/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d/web/webapi.py` & `tidy3d-2.0.3/tidy3d/web/webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,16 @@
 
             while perc_done is not None and perc_done < 100 and get_status() == "running":
                 perc_done, field_decay = get_run_info(task_id)
                 new_description = f"solver progress (field decay = {field_decay:.2e})"
                 progress.update(pbar_pd, completed=perc_done, description=new_description)
                 time.sleep(RUN_REFRESH_TIME)
 
-            if perc_done is not None and perc_done < 100:
+            perc_done, field_decay = get_run_info(task_id)
+            if perc_done is not None and perc_done < 100 and field_decay > 0:
                 console.log("early shutoff detected, exiting.")
 
             progress.update(pbar_pd, completed=100, refresh=True)
 
     else:
 
         # non-verbose case, just keep checking until status is not running or perc_done >= 100
```

### Comparing `tidy3d-2.0.2/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.0.3/tidy3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.0.2
+Version: 2.0.3
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,15 +118,15 @@
 pip install pipx
 pipx run tidy3d configure
 ```
 
 You can also specify your API key directly as an option to this command using the `api-key` argument, for example:
 
 ```
-tidy3d configure --api-key=XXX
+tidy3d configure --apikey=XXX
 ```
 
 #### Manually
 
 Alternatively, you can manually set up the config file where Tidy3D looks for the API key. The API key must be in a file called `.tidy3d/config` located in your home directory, containing the following
 
 ```
```

### Comparing `tidy3d-2.0.2/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.0.3/tidy3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.2/tidy3d.egg-info/requires.txt` & `tidy3d-2.0.3/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

