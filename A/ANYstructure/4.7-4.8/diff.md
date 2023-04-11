# Comparing `tmp/ANYstructure-4.7.tar.gz` & `tmp/ANYstructure-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANYstructure-4.7.tar", last modified: Wed Feb 15 12:07:54 2023, max compression
+gzip compressed data, was "ANYstructure-4.8.tar", last modified: Tue Apr 11 06:56:12 2023, max compression
```

## Comparing `ANYstructure-4.7.tar` & `ANYstructure-4.8.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:54.889181 ANYstructure-4.7/
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:54.850184 ANYstructure-4.7/ANYstructure.egg-info/
--rw-rw-rw-   0        0        0     2062 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3480 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-15 12:07:54.000000 ANYstructure-4.7/ANYstructure.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1097 2023-02-15 10:00:39.000000 ANYstructure-4.7/LICENSE
--rw-rw-rw-   0        0        0     2974 2023-02-15 11:40:47.000000 ANYstructure-4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2062 2023-02-15 12:07:54.890181 ANYstructure-4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2268 2023-02-15 12:05:30.000000 ANYstructure-4.7/README.md
--rw-rw-rw-   0        0        0     1365 2023-02-15 10:00:39.000000 ANYstructure-4.7/README.rst
--rw-rw-rw-   0        0        0      141 2023-02-15 10:00:39.000000 ANYstructure-4.7/__init__.py
--rw-rw-rw-   0        0        0      660 2023-02-15 11:02:45.000000 ANYstructure-4.7/__main__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:54.869181 ANYstructure-4.7/any_files/
--rw-rw-rw-   0        0        0  1788080 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ANYstructure_documentation.pdf
--rw-rw-rw-   0        0        0     3182 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/SN_curve_parameters.py
--rw-rw-rw-   0        0        0        0 2023-02-15 11:00:07.000000 ANYstructure-4.7/any_files/__init__.py
--rw-rw-rw-   0        0        0      666 2023-02-15 11:24:06.000000 ANYstructure-4.7/any_files/__main__.py
--rw-rw-rw-   0        0        0    20024 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/bulb_anglebar_tbar_flatbar.csv
--rw-rw-rw-   0        0        0    18559 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/calc_loads.py
--rw-rw-rw-   0        0        0   198191 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/calc_structure.py
--rw-rw-rw-   0        0        0     6673 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/compartment_window.py
--rw-rw-rw-   0        0        0    79599 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/example_data.py
--rw-rw-rw-   0        0        0     3869 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/example_data_puls.py
--rw-rw-rw-   0        0        0    10718 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/excel_inteface.py
--rw-rw-rw-   0        0        0    17616 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/fatigue_window.py
--rw-rw-rw-   0        0        0    12739 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/grid_window.py
--rw-rw-rw-   0        0        0    32093 2023-02-15 11:40:06.000000 ANYstructure-4.7/any_files/helper.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:54.878181 ANYstructure-4.7/any_files/images/
--rw-rw-rw-   0        0        0    13325 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/ANYstructure_logo.jpg
--rw-rw-rw-   0        0        0    28711 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/Buckling_Strength_of_Shells.png
--rw-rw-rw-   0        0        0    23283 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/Panel_geometry_definitions.png
--rw-rw-rw-   0        0        0    17342 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/current_comps_NONE.png
--rw-rw-rw-   0        0        0    10668 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_T_L_FB.gif
--rw-rw-rw-   0        0        0    32263 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_fixation_parameters.gif
--rw-rw-rw-   0        0        0     3415 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_generate_report.gif
--rw-rw-rw-   0        0        0     2698 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_int_pressure_button.gif
--rw-rw-rw-   0        0        0     2565 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_int_pressure_button_search.gif
--rw-rw-rw-   0        0        0     2175 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_multi_opt.gif
--rw-rw-rw-   0        0        0     3219 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_optimize.gif
--rw-rw-rw-   0        0        0    10465 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_plate_and_stiffener.gif
--rw-rw-rw-   0        0        0     1495 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_stf_button.gif
--rw-rw-rw-   0        0        0     5442 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_stiffener.gif
--rw-rw-rw-   0        0        0     1949 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_stress_button.gif
--rw-rw-rw-   0        0        0     5258 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_title.gif
--rw-rw-rw-   0        0        0    15715 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/images/img_transverse_stress.gif
--rw-rw-rw-   0        0        0     8961 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/load_factor_window.py
--rw-rw-rw-   0        0        0    36341 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/load_window.py
--rw-rw-rw-   0        0        0   446490 2023-02-15 12:02:30.000000 ANYstructure-4.7/any_files/main_application.py
--rw-rw-rw-   0        0        0    16726 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/make_grid_numpy.py
--rw-rw-rw-   0        0        0     1031 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/make_queue.py
--rw-rw-rw-   0        0        0     1035 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/make_stack.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:54.889181 ANYstructure-4.7/any_files/ml_files/
--rw-rw-rw-   0        0        0      785 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_CSR-Tank_req_cl_UP_scaler.pickle
--rw-rw-rw-   0        0        0    85557 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_CSR-Tank_req_cl_predictor.pickle
--rw-rw-rw-   0        0        0      857 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_SP_scaler.pickle
--rw-rw-rw-   0        0        0    89722 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_predictor.pickle
--rw-rw-rw-   0        0        0    95680 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_SP.pickle
--rw-rw-rw-   0        0        0    91329 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_UP.pickle
--rw-rw-rw-   0        0        0    95832 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_SP.pickle
--rw-rw-rw-   0        0        0    90684 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_UP.pickle
--rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_SP.pickle
--rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_UP.pickle
--rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_SP.pickle
--rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_UP.pickle
--rw-rw-rw-   0        0        0    95984 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_SP.pickle
--rw-rw-rw-   0        0        0    90816 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_UP.pickle
--rw-rw-rw-   0        0        0    97562 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_SP.pickle
--rw-rw-rw-   0        0        0    92071 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_UP.pickle
--rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_SP.pickle
--rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_UP.pickle
--rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_SP.pickle
--rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_UP.pickle
--rw-rw-rw-   0        0        0      925 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/opt_problem.py
--rw-rw-rw-   0        0        0    86184 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/optimize.py
--rw-rw-rw-   0        0        0    48514 2023-02-15 11:40:06.000000 ANYstructure-4.7/any_files/optimize_cylinder.py
--rw-rw-rw-   0        0        0    98462 2023-02-15 11:40:06.000000 ANYstructure-4.7/any_files/optimize_geometry.py
--rw-rw-rw-   0        0        0    87164 2023-02-15 11:40:06.000000 ANYstructure-4.7/any_files/optimize_multiple_window.py
--rw-rw-rw-   0        0        0    66917 2023-02-15 11:40:06.000000 ANYstructure-4.7/any_files/optimize_window.py
--rw-rw-rw-   0        0        0    27723 2023-02-15 11:38:16.000000 ANYstructure-4.7/any_files/pl_stf_window.py
--rw-rw-rw-   0        0        0    48854 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/report_generator.py
--rw-rw-rw-   0        0        0     5615 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/sections.csv
--rw-rw-rw-   0        0        0     4126 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/sesam_interface.py
--rw-rw-rw-   0        0        0   495083 2023-02-15 10:00:39.000000 ANYstructure-4.7/any_files/ship_section_example.txt
--rw-rw-rw-   0        0        0    13750 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/stresses_window.py
--rw-rw-rw-   0        0        0     6365 2023-02-15 10:59:40.000000 ANYstructure-4.7/any_files/testCalc.py
--rw-rw-rw-   0        0        0      110 2023-02-15 12:07:54.893181 ANYstructure-4.7/setup.cfg
--rw-rw-rw-   0        0        0     1814 2023-02-15 12:04:38.000000 ANYstructure-4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:56:12.873189 ANYstructure-4.8/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:56:12.546122 ANYstructure-4.8/ANYstructure.egg-info/
+-rw-rw-rw-   0        0        0     2062 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3480 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:56:12.000000 ANYstructure-4.8/ANYstructure.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1097 2023-02-15 10:00:39.000000 ANYstructure-4.8/LICENSE
+-rw-rw-rw-   0        0        0     2974 2023-02-15 11:40:47.000000 ANYstructure-4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2062 2023-04-11 06:56:12.874189 ANYstructure-4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2439 2023-04-11 06:53:42.000000 ANYstructure-4.8/README.md
+-rw-rw-rw-   0        0        0     1365 2023-02-15 10:00:39.000000 ANYstructure-4.8/README.rst
+-rw-rw-rw-   0        0        0      141 2023-04-11 06:54:47.000000 ANYstructure-4.8/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-02-15 11:02:45.000000 ANYstructure-4.8/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:56:12.845975 ANYstructure-4.8/any_files/
+-rw-rw-rw-   0        0        0  1788080 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ANYstructure_documentation.pdf
+-rw-rw-rw-   0        0        0     3182 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/SN_curve_parameters.py
+-rw-rw-rw-   0        0        0        0 2023-02-15 11:00:07.000000 ANYstructure-4.8/any_files/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-02-15 11:24:06.000000 ANYstructure-4.8/any_files/__main__.py
+-rw-rw-rw-   0        0        0    20024 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/bulb_anglebar_tbar_flatbar.csv
+-rw-rw-rw-   0        0        0    18559 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/calc_loads.py
+-rw-rw-rw-   0        0        0   199022 2023-03-30 08:43:23.000000 ANYstructure-4.8/any_files/calc_structure.py
+-rw-rw-rw-   0        0        0     6673 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/compartment_window.py
+-rw-rw-rw-   0        0        0    79613 2023-03-24 13:11:10.000000 ANYstructure-4.8/any_files/example_data.py
+-rw-rw-rw-   0        0        0     3869 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/example_data_puls.py
+-rw-rw-rw-   0        0        0    10718 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/excel_inteface.py
+-rw-rw-rw-   0        0        0    17616 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/fatigue_window.py
+-rw-rw-rw-   0        0        0    12739 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/grid_window.py
+-rw-rw-rw-   0        0        0    32150 2023-03-22 09:51:57.000000 ANYstructure-4.8/any_files/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:56:12.858188 ANYstructure-4.8/any_files/images/
+-rw-rw-rw-   0        0        0    13325 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/ANYstructure_logo.jpg
+-rw-rw-rw-   0        0        0    28711 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/Buckling_Strength_of_Shells.png
+-rw-rw-rw-   0        0        0    23283 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/Panel_geometry_definitions.png
+-rw-rw-rw-   0        0        0    17342 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/current_comps_NONE.png
+-rw-rw-rw-   0        0        0    10668 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_T_L_FB.gif
+-rw-rw-rw-   0        0        0    32263 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_fixation_parameters.gif
+-rw-rw-rw-   0        0        0     3415 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_generate_report.gif
+-rw-rw-rw-   0        0        0     2698 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_int_pressure_button.gif
+-rw-rw-rw-   0        0        0     2565 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_int_pressure_button_search.gif
+-rw-rw-rw-   0        0        0     2175 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_multi_opt.gif
+-rw-rw-rw-   0        0        0     3219 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_optimize.gif
+-rw-rw-rw-   0        0        0    10465 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_plate_and_stiffener.gif
+-rw-rw-rw-   0        0        0     1495 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_stf_button.gif
+-rw-rw-rw-   0        0        0     5442 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_stiffener.gif
+-rw-rw-rw-   0        0        0     1949 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_stress_button.gif
+-rw-rw-rw-   0        0        0     5258 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_title.gif
+-rw-rw-rw-   0        0        0    15715 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/images/img_transverse_stress.gif
+-rw-rw-rw-   0        0        0     8961 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/load_factor_window.py
+-rw-rw-rw-   0        0        0    36341 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/load_window.py
+-rw-rw-rw-   0        0        0   456177 2023-04-11 06:52:15.000000 ANYstructure-4.8/any_files/main_application.py
+-rw-rw-rw-   0        0        0    16726 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/make_grid_numpy.py
+-rw-rw-rw-   0        0        0     1031 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/make_queue.py
+-rw-rw-rw-   0        0        0     1035 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/make_stack.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:56:12.873189 ANYstructure-4.8/any_files/ml_files/
+-rw-rw-rw-   0        0        0      785 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_CSR-Tank_req_cl_UP_scaler.pickle
+-rw-rw-rw-   0        0        0    85557 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_CSR-Tank_req_cl_predictor.pickle
+-rw-rw-rw-   0        0        0      857 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_SP_scaler.pickle
+-rw-rw-rw-   0        0        0    89722 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_predictor.pickle
+-rw-rw-rw-   0        0        0    95680 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_SP.pickle
+-rw-rw-rw-   0        0        0    91329 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_UP.pickle
+-rw-rw-rw-   0        0        0    95832 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_SP.pickle
+-rw-rw-rw-   0        0        0    90684 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_UP.pickle
+-rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_SP.pickle
+-rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_UP.pickle
+-rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_SP.pickle
+-rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_UP.pickle
+-rw-rw-rw-   0        0        0    95984 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_SP.pickle
+-rw-rw-rw-   0        0        0    90816 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_UP.pickle
+-rw-rw-rw-   0        0        0    97562 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_SP.pickle
+-rw-rw-rw-   0        0        0    92071 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_UP.pickle
+-rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_SP.pickle
+-rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_UP.pickle
+-rw-rw-rw-   0        0        0      833 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_SP.pickle
+-rw-rw-rw-   0        0        0      761 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_UP.pickle
+-rw-rw-rw-   0        0        0      925 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/opt_problem.py
+-rw-rw-rw-   0        0        0    86184 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/optimize.py
+-rw-rw-rw-   0        0        0    48607 2023-03-31 08:32:10.000000 ANYstructure-4.8/any_files/optimize_cylinder.py
+-rw-rw-rw-   0        0        0    98462 2023-02-15 11:40:06.000000 ANYstructure-4.8/any_files/optimize_geometry.py
+-rw-rw-rw-   0        0        0    87164 2023-02-15 11:40:06.000000 ANYstructure-4.8/any_files/optimize_multiple_window.py
+-rw-rw-rw-   0        0        0    66917 2023-02-15 11:40:06.000000 ANYstructure-4.8/any_files/optimize_window.py
+-rw-rw-rw-   0        0        0    27866 2023-03-22 09:51:57.000000 ANYstructure-4.8/any_files/pl_stf_window.py
+-rw-rw-rw-   0        0        0    52521 2023-03-28 13:00:33.000000 ANYstructure-4.8/any_files/report_generator.py
+-rw-rw-rw-   0        0        0     5615 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/sections.csv
+-rw-rw-rw-   0        0        0     4126 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/sesam_interface.py
+-rw-rw-rw-   0        0        0   495083 2023-02-15 10:00:39.000000 ANYstructure-4.8/any_files/ship_section_example.txt
+-rw-rw-rw-   0        0        0    13750 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/stresses_window.py
+-rw-rw-rw-   0        0        0     6365 2023-02-15 10:59:40.000000 ANYstructure-4.8/any_files/testCalc.py
+-rw-rw-rw-   0        0        0      110 2023-04-11 06:56:12.877188 ANYstructure-4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1814 2023-04-11 06:52:15.000000 ANYstructure-4.8/setup.py
```

### Comparing `ANYstructure-4.7/ANYstructure.egg-info/PKG-INFO` & `ANYstructure-4.8/ANYstructure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANYstructure
-Version: 4.7
+Version: 4.8
 Summary: A plate field optimization tool for offshore structures calculated according to DNV standards
 Home-page: https://github.com/audunarn/ANYstructure
 Author: Audun Arnesen Nyhus
 Author-email: audunarn@gmail.com
 License: MIT
 Keywords: dnvgl-gl-os-c101 naval_architecture structural_engineering steel buckling fatigue local_scantlings optimization weight
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ANYstructure-4.7/ANYstructure.egg-info/SOURCES.txt` & `ANYstructure-4.8/ANYstructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/LICENSE` & `ANYstructure-4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/MANIFEST.in` & `ANYstructure-4.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/PKG-INFO` & `ANYstructure-4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANYstructure
-Version: 4.7
+Version: 4.8
 Summary: A plate field optimization tool for offshore structures calculated according to DNV standards
 Home-page: https://github.com/audunarn/ANYstructure
 Author: Audun Arnesen Nyhus
 Author-email: audunarn@gmail.com
 License: MIT
 Keywords: dnvgl-gl-os-c101 naval_architecture structural_engineering steel buckling fatigue local_scantlings optimization weight
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ANYstructure-4.7/README.md` & `ANYstructure-4.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # ANYstructure #
 ANYstructure is the ultimate steel structure design tool for plate fields and cylinders! 
 Weight optimization for all structures with machine learning capabilities. 
 Calculations are based on DNV standards and rules
+### What's new in 4.8 ###
+* Reporting table on cylinders.
+* Color coding on come cylinder properties.
+* Corrected error on additional hoop stress input for cylinders.
 ### What's new in 4.7 ###
 * Corrected error on girder caluculation for cylinder buckling.
 * Added 1.10 load factor option for cylinder buckling.
 * Better compability with linux.
 * Python 3.11 based.
 ### What's new in 4.4 ###
 * Backup and restore feature added.
```

### Comparing `ANYstructure-4.7/README.rst` & `ANYstructure-4.8/README.rst`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/__main__.py` & `ANYstructure-4.8/__main__.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ANYstructure_documentation.pdf` & `ANYstructure-4.8/any_files/ANYstructure_documentation.pdf`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/SN_curve_parameters.py` & `ANYstructure-4.8/any_files/SN_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/__main__.py` & `ANYstructure-4.8/any_files/__main__.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/bulb_anglebar_tbar_flatbar.csv` & `ANYstructure-4.8/any_files/bulb_anglebar_tbar_flatbar.csv`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/calc_loads.py` & `ANYstructure-4.8/any_files/calc_loads.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/calc_structure.py` & `ANYstructure-4.8/any_files/calc_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 try:
     import any_files.helper as hlp
     import any_files.SN_curve_parameters as snc
 except ModuleNotFoundError:
     import ANYstructure.any_files.helper as hlp
     import ANYstructure.any_files.SN_curve_parameters as snc
 
-
 class Structure():
     '''
     Setting the properties for the plate and the stiffener. Takes a dictionary as argument.
     '''
     def __init__(self, main_dict, *args, **kwargs):
         super(Structure,self).__init__()
         self._main_dict = main_dict
@@ -139,28 +138,32 @@
             '\n Stf. fixation paramter,kps:    ' + str(self._stf_kps) + ' ' +
             '\n Global stress, sig_y1/sig_y2:  ' + str(round(self._sigma_y1,3))+'/'+str(round(self._sigma_y2,3))+ ' MPa' +
             '\n Global stress, sig_x1/sig_x2:   ' + str(round(self._sigma_x1,3))+'/'+str(round(self._sigma_x2,3))+ ' MPa' +
             '\n Global shear, tau_xy:          ' + str(round(self._tauxy,3)) + ' MPa' +
             '\n km1,km2,km3:                   ' + str(self._km1)+'/'+str(self._km2)+'/'+str(self._km3)+
             '\n Pressure side (p-plate/s-stf): ' + str(self._pressure_side) + ' ')
 
-    def get_beam_string(self):
+    def get_beam_string(self, short = False):
         ''' Returning a string. '''
         if type(self._stiffener_type) != str:
             print('error')
 
         base_name = self._stiffener_type+ '_' + str(round(self._web_height*1000, 0)) + 'x' + \
                    str(round(self._web_th*1000, 0))
         if self._stiffener_type == 'FB':
             ret_str = base_name
         elif self._stiffener_type in ['L-bulb', 'bulb', 'hp']:
-            ret_str = 'Bulb'+str(int(self._web_height*1000 + self._flange_th*1000))+'x'+\
-                      str(round(self._web_th*1000, 0))+ '_(' +str(round(self._web_height*1000, 0)) + 'x' + \
-                   str(round(self._web_th*1000, 0))+'_'+ str(round(self._flange_width*1000, 0)) + 'x' + \
-                      str(round(self._flange_th*1000, 0))+')'
+            if not short:
+                ret_str = 'Bulb'+str(int(self._web_height*1000 + self._flange_th*1000))+'x'+\
+                          str(round(self._web_th*1000, 0))+ '_(' +str(round(self._web_height*1000, 0)) + 'x' + \
+                       str(round(self._web_th*1000, 0))+'_'+ str(round(self._flange_width*1000, 0)) + 'x' + \
+                          str(round(self._flange_th*1000, 0))+')'
+            else:
+                ret_str = 'Bulb'+str(int(self._web_height*1000 + self._flange_th*1000))+'x'+\
+                      str(round(self._web_th*1000, 0))
         else:
             ret_str = base_name + '__' + str(round(self._flange_width*1000, 0)) + 'x' + \
                       str(round(self._flange_th*1000, 0))
 
         ret_str = ret_str.replace('.', '_')
 
         return ret_str
@@ -2391,15 +2394,15 @@
         # main_dict = {'sasd': 100, 'smsd': 100, 'tTsd': 50, 'tQsd':10, 'psd': -0.3, 'shsd': 0, 'geometry': 7,
         #              'material factor': self._mat_factor, 'lT': 0, 'delta0': 0.005, 'fab method ring stf': 1,
         #              'fab method ring girder': 2, 'E-module':2.1e11, 'poisson': 0.3, 'yield': 355e6}
 
         #if main_dict['geometry'][0] in [1,3,5,7]: # Need to convert from forces to stresses.
         self._sasd = main_dict['sasd'][0]
         self._smsd = main_dict['smsd'][0]
-        self._tTsd = main_dict['tTsd'][0]
+        self._tTsd = abs(main_dict['tTsd'][0])
         self._tQsd= main_dict['tQsd'][0]
         self._psd = main_dict['psd'][0]
         self._shsd = main_dict['shsd'][0]
         self._geometry = main_dict['geometry'][0]
         self._mat_factor = main_dict['material factor'][0]
         self._delta0 = main_dict['delta0'][0]
         self._fab_method_ring_stf = main_dict['fab method ring stf'][0]
@@ -2462,18 +2465,18 @@
     def smsd(self):
         return self._smsd
     @smsd.setter
     def smsd(self, val):
         self._smsd = val
     @property
     def tTsd(self):
-        return self._tTsd
+        return abs(self._tTsd)
     @tTsd.setter
     def tTsd(self, val):
-        self._tTsd = val
+        self._tTsd = abs(val)
     @property
     def tQsd(self):
         return self._tQsd
     @tQsd.setter
     def tQsd(self, val):
         self._tQsd = val
     @property
@@ -2616,14 +2619,16 @@
                                                            column_buckling_data=column_buckling_data)
                 results['Column stability check'] = column_buckling_data['Column stability check']
                 results['Need to check column buckling'] = column_buckling_data['Need to check column buckling']
                 results['Stiffener check'] = column_buckling_data['stiffener check']
                 results['Stiffener check detailed'] = column_buckling_data['stiffener check detailed']
                 results['Ring stiffened shell'] = ring_stf_shell[0]
 
+
+
                 if optimizing:
                     if not results['Column stability check']:
                         return False, 'Column stability', results
                     elif False in results['Stiffener check'].values():
                         return False, 'Stiffener check', results
                     elif results['Ring stiffened shell'] > 1:
                         return False, 'UF ring stiffeners', results
@@ -2653,20 +2658,21 @@
 
         if optimizing:
             return True, 'Check OK', results
 
         # print('Results for geometry', self._geometry)
         # print('UF',uf_unstf_shell, uf_long_stf, uf_ring_stf, uf_ring_frame)
         # print('Stiffeners', stiffener_check)
+
         return results
 
     def set_main_properties(self, main_dict):
         self._sasd = main_dict['sasd'][0]
         self._smsd = main_dict['smsd'][0]
-        self._tTsd = main_dict['tTsd'][0]
+        self._tTsd = abs(main_dict['tTsd'][0])
         self._tQsd= main_dict['tQsd'][0]
         self._psd = main_dict['psd'][0]
         self._shsd = main_dict['shsd'][0]
         self._geometry = main_dict['geometry'][0]
         self._mat_factor = main_dict['material factor'][0]
         self._delta0 = main_dict['delta0'][0]
         self._fab_method_ring_stf = main_dict['fab method ring stf'][0]
@@ -2740,15 +2746,15 @@
         sxsd, shsd, shRsd, tsd = list(), list(), list(), list()
 
         for idx, obj in stucture_objects.items():
             if obj is None:
                 shRsd.append(np.nan)
                 continue
             if idx == 'Unstiffened':
-                shsd.append((self._psd/1e6)*r/t+self._shsd/1e6)
+                shsd.append((self._psd/1e6)*r/t + self._shsd/1e6)
                 sxsd.append(self._sasd/1e6+self._smsd/1e6 if self._geometry in [2,6] else
                             min([self._sasd/1e6, self._sasd/1e6-self._smsd/1e6, self._sasd/1e6+self._smsd/1e6]))
                 tsd.append(self._tTsd/1e6 + self._tQsd/1e6)
             elif idx == 'Long Stiff.':
                 if stucture_objects['Ring Stiffeners'] == None:
                     shsd.append(shsd[0]+self._shsd/1e6)
                 else:
@@ -2785,18 +2791,19 @@
                     tsd.append(tsd[0])
                 else:
                     sxsd.append(np.nan)
                     tsd.append(np.nan)
 
         sxsd = np.array(sxsd)
         shsd = np.array(shsd)
-        tsd = np.array(tsd)
+        tsd = np.array(np.abs(tsd))
         sjsd = np.sqrt(sxsd**2 - sxsd*shsd + shsd**2+3*tsd**2)
 
-        return {'sjsd': sjsd, 'parameters': parameters, 'cross section data': cross_sec_data, 'shRsd': shRsd, 'shsd': shsd, 'sxsd': sxsd}
+        return {'sjsd': sjsd, 'parameters': parameters, 'cross section data': cross_sec_data,
+                'shRsd': shRsd, 'shsd': shsd, 'sxsd': sxsd}
 
     def unstiffened_shell(self, conical = False, shell_data = None):
 
         E = self._E/1e6
         t = self._Shell.thk*1000
 
         # get correct s
@@ -2806,20 +2813,21 @@
         v = self._v
         r = self._Shell.radius*1000
         l = self._Shell.dist_between_rings * 1000
         fy = self._yield/1e6
 
         sasd = self._sasd/1e6
         smsd = self._smsd/1e6
-        tsd = self._tTsd/1e6+self._tQsd/1e6
+        tsd = abs(self._tTsd/1e6+self._tQsd/1e6)
         psd = self._psd/1e6
-        if self._RingStf is not None:
-            shsd = shell_data['shsd'][1]
+
+        if self._RingStf is None:
+            shsd = shell_data['shsd'][0]
         else:
-            shsd = psd*r/t
+            shsd = shell_data['shsd'][1]
 
         provide_data = dict()
 
         '''
         	Selections for: Type of Structure Geometry:
         1	Unstiffened shell (Force input)
         2	Unstiffened panel (Stress input)
@@ -3102,14 +3110,15 @@
                     sasd_iter -= 10
                 else:
                     sasd_iter -= 20
 
             return 0 if len(logger) == 1 else max(logger[-2],0)
 
         provide_data['max axial stress - 3.4.2 Shell buckling'] = iter_table_2()
+        provide_data['shsd'] = shsd
         return provide_data
 
     def ring_stiffened_shell(self, data_shell_buckling = None, column_buckling_data = None):
 
         E = self._E/1e6
         t = self._Shell.thk*1000
         s = min([self._Shell.dist_between_rings, 2*math.pi*self._Shell.radius])*1000 if self._LongStf == None else \
@@ -3119,15 +3128,15 @@
         l = self._Shell.dist_between_rings * 1000
         fy = self._yield/1e6
 
         L = self._Shell.tot_cyl_length*1000
         LH = L
         sasd = self._sasd/1e6
         smsd = self._smsd/1e6
-        tsd = self._tTsd/1e6 + self._tQsd/1e6
+        tsd = abs(self._tTsd/1e6 + self._tQsd/1e6) # MAYBE MAYBE NOT.
         psd = self._psd/1e6
 
         data_shell_buckling = self.shell_buckling() if data_shell_buckling == None else data_shell_buckling
 
         #Pnt. 3.5:  Ring stiffened shell
 
         # Pnt. 3.5.2.1   Requirement for cross-sectional area:
@@ -3159,15 +3168,14 @@
         Ixreq = np.array([abs(worst_ax_comp) * t * (1 + alfaA) * math.pow(r0[0], 4) / (500 * E * l),
                           abs(worst_ax_comp) * t * (1 + alfaA) * math.pow(r0[1], 4) / (500 * E * l)])
 
         #Pnt. 3.5.2.5   Required Ixh for shell subjected to torsion and/or shear:
         Ixhreq = np.array([math.pow(tsd / E, (8 / 5)) * math.pow(r0[0] / L, 1 / 5) * L * r0[0] * t * l,
                            math.pow(tsd / E, (8 / 5)) * math.pow(r0[1] / L, 1 / 5) * L * r0[1] * t * l])
 
-
         #Pnt. 3.5.2.6   Simplified calculation of Ih for shell subjected to external pressure
         zt = np.array([data_shell_buckling['parameters'][0][6],data_shell_buckling['parameters'][1][6]])
         rf = np.array([data_shell_buckling['parameters'][0][4], data_shell_buckling['parameters'][1][4]])
 
         delta0 = r*self._delta0
 
         fb_ring_req_val = np.array([0 if self._RingStf is None else 0.4*self._RingStf.tw*math.sqrt(E/fy),
@@ -3286,17 +3294,18 @@
         l = self._Shell.dist_between_rings * 1000
         fy = self._yield/1e6
 
         L = self._Shell.tot_cyl_length*1000
         LH = L
         sasd = self._sasd/1e6
         smsd = self._smsd/1e6
-        tsd = self._tTsd/1e6 + self._tQsd/1e6
+        tsd = abs(self._tTsd/1e6 + self._tQsd/1e6)
         psd = self._psd/1e6
-        shsd = psd * r / t
+        shsd = unstiffened_shell['shsd']
+
 
         lightly_stf = s/t > math.sqrt(r/t)
         provide_data = dict()
 
         '''
         	Selections for: Type of Structure Geometry:
         1	Unstiffened shell (Force input)
@@ -3344,17 +3353,18 @@
         # Itot = Ishell + Istf_tot # Checked
 
         Iy = self._LongStf.get_moment_of_intertia(efficent_se=Se/1000, tf1=self._Shell.thk)*1000**4
 
         alpha = 12*(1-math.pow(v,2))*Iy/(s*math.pow(t,3))
         Zl = (math.pow(l, 2)/(r*t)) * math.sqrt(1-math.pow(v,2))
 
-        #print('Zl', Zl, 'alpha', alpha, 'Isef', Iy, 'Se', Se, 'sjsd', sjsd, 'sxsd', sxSd, 'fks', fks, 'As', As)
+        #|1print('Zl', Zl, 'alpha', alpha, 'Isef', Iy, 'Se', Se, 'sjsd', sjsd, 'sxsd', sxSd, 'fks', fks, 'As', As)
         # Table 3-3
 
+
         def table_3_3(chk):
             psi = {'Axial stress': 0 if Se == 0 else (1+alpha) / (1+A/(Se*t)),
                    'Torsion and shear stress': 5.54+1.82*math.pow(l/s, 4/3) * math.pow(alpha, 1/3),
                    'Lateral Pressure': 2*(1+math.sqrt(1+alpha))}                      # ψ
             epsilon = {'Axial stress': 0.702*Zl,
                    'Torsion and shear stress': 0.856*math.pow(Zl, 3/4),
                    'Lateral Pressure': 1.04*math.sqrt(Zl)}                             # ξ
@@ -3383,15 +3393,15 @@
 
         sasd = sasd*(A+s*t)/(A+Se*t) if A+Se*t>0 else 0
         smsd = smsd * (A + s * t) / (A + Se * t) if A + Se * t > 0 else 0
 
         sa0sd = -sasd if sasd < 0 else 0
         sm0sd = -smsd if smsd < 0 else 0
         sh0sd = -shsd if shsd < 0 else 0
-
+        #print('fy_used', fy_used,'sasd', sasd,'shsd', shsd, 'tsd', tsd)
         sjsd_panels = math.sqrt(math.pow(sasd+smsd,2)-(sasd+smsd)*shsd + math.pow(shsd,2)+  3*math.pow(tsd,2))
 
         worst_axial_comb = min(sasd-smsd,sasd+smsd)
         sjsd_shells = math.sqrt(math.pow(worst_axial_comb,2)-worst_axial_comb*shsd +math.pow(shsd,2)+3*math.pow(tsd,2))
         sxsd_used = worst_axial_comb
         provide_data['sxsd_used'] = sxsd_used
         sjsd_used = sjsd_panels if self._geometry in [2,6] else sjsd_shells
@@ -3402,15 +3412,15 @@
         lambda_s2_shell = fy_used/sjsd_shells*(max(0,-worst_axial_comb)/fEax+sh0sd/fElat+tsd/fEtors) if\
             sjsd_shells*fEax*fEtors*fElat>0 else 0
 
         shell_type = 2 if self._geometry in [1,5] else 1
         lambda_s = math.sqrt(lambda_s2_panel) if shell_type == 1 else math.sqrt(lambda_s2_shell)
 
         fks = fy_used/math.sqrt(1+math.pow(lambda_s,4))
-
+        #print('tsd',tsd, 'sasd', sasd, 'sjsd panels', sjsd_panels, 'fy_used', fy_used, 'lambda_T',data_col_buc['lambda_T'] )
         if lambda_s < 0.5:
             gammaM = self._mat_factor
         else:
             if self._mat_factor == 1.1:
                 if lambda_s > 1:
                     gammaM = 1.4
                 else:
@@ -3428,16 +3438,17 @@
 
         if self._uls_or_als == 'ALS':
             gammaM = gammaM/self._mat_factor
 
         # Design buckling strength:
         fksd = fks/gammaM
         provide_data['fksd'] = fksd
-        #print('fksd', fksd, 'fks', fks, 'gammaM', gammaM, 'lambda_s', lambda_s, 'lambda_s^2 panel', lambda_s2_panel, 'sjsd', sjsd_used, 'worst_axial_comb',worst_axial_comb, 'sm0sd',sm0sd)
-
+        # print('fksd', fksd, 'fks', fks, 'gammaM', gammaM, 'lambda_s', lambda_s, 'lambda_s^2 panel',
+        #       lambda_s2_panel, 'sjsd', sjsd_used, 'worst_axial_comb',worst_axial_comb, 'sm0sd',sm0sd)
+        #print('  ')
         return provide_data
 
     @staticmethod
     def get_Itot(hw, tw, b, tf, r, s, t):
 
         h = t+hw+tf
         As = hw*tw + b*tf  # checked
@@ -3486,15 +3497,15 @@
 
         L = self._Shell.tot_cyl_length*1000
         LH = L
         Lc = max([L, LH])
 
         sasd = self._sasd/1e6
         smsd = self._smsd/1e6
-        tsd = self._tTsd/1e6 + self._tQsd/1e6
+        tsd = abs(self._tTsd/1e6 + self._tQsd/1e6)
         psd = self._psd/1e6
         shsd = psd * r / t
 
         shell_buckling_data = self.shell_buckling(unstiffened_cylinder=unstf_shell_data) if\
             shell_bukcling_data is None else shell_bukcling_data
         data = self.unstiffened_shell() if unstf_shell_data is None else unstf_shell_data
 
@@ -3551,14 +3562,15 @@
             mu = 0.35*(lambdaT-0.6)
             fT = (1+mu+math.pow(lambdaT,2)-math.sqrt(math.pow(1+mu+math.pow(lambdaT,2),2)-4*math.pow(lambdaT,2)))\
                  /(2*math.pow(lambdaT,2))*fy if lambdaT > 0.6 else fy
 
             # General
 
             if key == 'Longitudinal stiff.':
+                #print('Column buckling', 'fET', fEt, 'mu', mu, 'lambdaT', lambdaT, 'hs', hs, 'It', It, 'Iz', Iz ,'Ipo', Ipo)
                 provide_data['lambda_T'] = lambdaT
                 provide_data['fT'] = fT
             fT_dict[key] = fT
             idx += 1
             # if key == 'Ring Stiff.':
             #     print(hs, It, Iz, Ipo, Iy)
             #     print('hello')
@@ -3725,15 +3737,16 @@
         chk4 = ef_div_tw < ef_div_tw_req
         chk4 = [np.nan if np.isnan(val) else chk4[idx] for idx, val in enumerate(ef_div_tw_req)]
 
         provide_data['stiffener check'] = {'longitudinal':all([chk1[0], chk2[0]]),
                                            'ring stiffener': None if self._RingStf is None else
                                            all([chk1[1],chk2[1],chk3[0],chk4[0]]),
                                            'ring frame': None if self._RingFrame is None else
-                                           all([chk1[2],chk2[2],chk3[1],chk4[1]])}
+                                           True}
+                                           #all([chk1[2],chk2[2],chk3[1],chk4[1]])} SKIP check for girders
         provide_data['stiffener check detailed'] = {'longitudinal':'Web height < ' + str(round(stf_req_h[0],1)) if not chk1[0]
         else '' + ' ' + 'flange width < ' +str(round(stf_req_b[0],1)) if not chk2[0] else ' ',
                                                    'ring stiffener': None if self._RingStf is None
                                                    else 'Web height < ' + str(round(stf_req_h[1],1)) if not chk1[1]
                                                    else '' + ' ' + 'flange width < ' +str(round(stf_req_b[1],1)) if not chk2[1]
                                                    else ' '  + ' ' + 'hw/tw >= ' + str(round(req_hw_div_tw[0],1))
                                                    if not chk3[0]
@@ -3771,15 +3784,15 @@
                     'Ring frame': None if self._RingFrame is None else
                     self._RingFrame.set_main_properties(all_prop_dict['Ring frame'])}
         return all_data
 
     def get_main_properties(self):
         main_dict = {'sasd': [self._sasd, 'Pa'],
                      'smsd': [self._smsd, 'Pa'],
-                     'tTsd': [self._tTsd, 'Pa'],
+                     'tTsd': [abs(self._tTsd), 'Pa'],
                      'tQsd': [self._tQsd, 'Pa'],
                      'psd': [self._psd, 'Pa'],
                      'shsd': [self._shsd, 'Pa'],
                      'geometry': [self._geometry, ''],
                      'material factor': [self._mat_factor, ''],
                      'delta0': [self._delta0, ''],
                      'fab method ring stf': [self._fab_method_ring_stf, '-'],
@@ -3795,15 +3808,15 @@
                      'ULS or ALS':[self._uls_or_als, '']}
 
         return main_dict
         
     def set_stresses_and_pressure(self, val):
         self._sasd = val['sasd']
         self._smsd = val['smsd']
-        self._tTsd = val['tTsd']
+        self._tTsd = abs(val['tTsd'])
         self._tQsd= val['tQsd']
         self._psd = val['psd']
         self._shsd = val['shsd']
         
     def get_x_opt(self):
         '''
         shell       (0.02, 2.5, 5, 5, 10, nan, nan, nan),
```

### Comparing `ANYstructure-4.7/any_files/compartment_window.py` & `ANYstructure-4.8/any_files/compartment_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/example_data.py` & `ANYstructure-4.8/any_files/example_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 structure_types = {'vertical': ['BBS', 'SIDE_SHELL', 'SSS'],
                          'horizontal': ['BOTTOM', 'BBT', 'HOPPER', 'MD'],
                          'non-wt': ['FRAME', 'GENERAL_INTERNAL_NONWT'],
                          'internals': ['INNER_SIDE', 'FRAME_WT', 'GENERAL_INTERNAL_WT',
                                        'INTERNAL_ZERO_STRESS_WT', 'INTERNAL_LOW_STRESS_WT']}
 
-obj_dict = {'mat_yield': [355e6, 'Pa'], 'mat_factor': [1.15, ''],'span': [3.7, 'm'], 'spacing': [0.75, 'm'],
-            'plate_thk': [0.018, 'm'],
-            'stf_web_height': [0.4, 'm'], 'stf_web_thk': [0.012, 'm'], 'stf_flange_width': [0.25, 'm'],
-            'stf_flange_thk': [0.014, 'm'], 'structure_type': ['BOTTOM', ''], 'plate_kpp': [1, ''],
+obj_dict = {'mat_yield': [355e6, 'Pa'], 'mat_factor': [1.10, ''],'span': [3.3, 'm'], 'spacing': [0.68, 'm'],
+            'plate_thk': [0.025, 'm'],
+            'stf_web_height': [0.250297358, 'm'], 'stf_web_thk': [0.012, 'm'], 'stf_flange_width': [0.52, 'm'],
+            'stf_flange_thk': [0.029702642, 'm'], 'structure_type': ['BOTTOM', ''], 'plate_kpp': [1, ''],
             'stf_kps': [1, ''], 'stf_km1': [12, ''], 'stf_km2': [24, ''], 'stf_km3': [12, ''],
             'sigma_y1': [100, 'MPa'], 'sigma_y2': [100, 'MPa'], 'sigma_x2': [102.7, 'MPa'], 'sigma_x1': [102.7, 'MPa'],
             'tau_xy': [5, 'MPa'],
             'stf_type': ['T', ''], 'structure_types': [structure_types, ''], 'zstar_optimization': [True, ''],
             'puls buckling method':[1,''], 'puls boundary':['Int',''], 'puls stiffener end':['C',''],
             'puls sp or up':['SP',''], 'puls up boundary' :['SSSS',''], 'panel or shell': ['panel', ''],
             'pressure side': ['both sides', ''], 'girder_lg': [5, 'm']}
```

### Comparing `ANYstructure-4.7/any_files/example_data_puls.py` & `ANYstructure-4.8/any_files/example_data_puls.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/excel_inteface.py` & `ANYstructure-4.8/any_files/excel_inteface.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/fatigue_window.py` & `ANYstructure-4.8/any_files/fatigue_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/grid_window.py` & `ANYstructure-4.8/any_files/grid_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/helper.py` & `ANYstructure-4.8/any_files/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 Helper funations to be used.
 '''
 
-import math, copy, csv
+import math, copy, csv, os
 import numpy as np
 
 print_it = True
-
+root_dir = os.path.dirname(os.path.abspath(__file__))
 def print_helper(properties, prop_text, units):
     '''
     Used to print out the properties
     '''
     dummy_i = 0
     print(' \n ')
     for prop_i in prop_text:
```

### Comparing `ANYstructure-4.7/any_files/images/ANYstructure_logo.jpg` & `ANYstructure-4.8/any_files/images/ANYstructure_logo.jpg`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/Buckling_Strength_of_Shells.png` & `ANYstructure-4.8/any_files/images/Buckling_Strength_of_Shells.png`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/Panel_geometry_definitions.png` & `ANYstructure-4.8/any_files/images/Panel_geometry_definitions.png`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/current_comps_NONE.png` & `ANYstructure-4.8/any_files/images/current_comps_NONE.png`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_T_L_FB.gif` & `ANYstructure-4.8/any_files/images/img_T_L_FB.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_fixation_parameters.gif` & `ANYstructure-4.8/any_files/images/img_fixation_parameters.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_generate_report.gif` & `ANYstructure-4.8/any_files/images/img_generate_report.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_int_pressure_button.gif` & `ANYstructure-4.8/any_files/images/img_int_pressure_button.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_int_pressure_button_search.gif` & `ANYstructure-4.8/any_files/images/img_int_pressure_button_search.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_multi_opt.gif` & `ANYstructure-4.8/any_files/images/img_multi_opt.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_optimize.gif` & `ANYstructure-4.8/any_files/images/img_optimize.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_plate_and_stiffener.gif` & `ANYstructure-4.8/any_files/images/img_plate_and_stiffener.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_stf_button.gif` & `ANYstructure-4.8/any_files/images/img_stf_button.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_stiffener.gif` & `ANYstructure-4.8/any_files/images/img_stiffener.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_stress_button.gif` & `ANYstructure-4.8/any_files/images/img_stress_button.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_title.gif` & `ANYstructure-4.8/any_files/images/img_title.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/images/img_transverse_stress.gif` & `ANYstructure-4.8/any_files/images/img_transverse_stress.gif`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/load_factor_window.py` & `ANYstructure-4.8/any_files/load_factor_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/load_window.py` & `ANYstructure-4.8/any_files/load_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/main_application.py` & `ANYstructure-4.8/any_files/main_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,14 @@
     import ANYstructure.any_files.pl_stf_window as struc
     import ANYstructure.any_files.stresses_window as stress
     import ANYstructure.any_files.fatigue_window as fatigue
     import ANYstructure.any_files.load_factor_window as load_factors
     from ANYstructure.any_files.report_generator import LetterMaker
     import ANYstructure.any_files.sesam_interface as sesam
 
-
-
 class Application():
     '''
     The Application class sets up the GUI using Tkinter.
     It is the main part of the code and calls up all other classes etc.
     '''
     def __init__(self, parent):
         '''
@@ -173,15 +171,15 @@
                               command=self.copy_property)
         undo_redo.add_command(label='Paste line propeties to active line (CTRL-D)',
                               command=self.paste_property)
 
         sub_report = tk.Menu(menu)
         menu.add_cascade(label = 'Reporting', menu = sub_report)
         sub_report.add_command(label = 'Generate PDF report', command = self.report_generate)
-        sub_report.add_command(label='Stiffened flat plate - Generate PDF result table', command=self.table_generate)
+        sub_report.add_command(label='Generate PDF result table', command=self.table_generate)
         sub_report.add_command(label='Stiffened flat plate - Weight development, plates and beams', command=self.on_plot_cog_dev)
 
         sub_sesam = tk.Menu(menu)
         menu.add_cascade(label = 'Interfaces', menu = sub_sesam)
         sub_sesam.add_command(label = 'Export geometry to SESAM GeniE JS', command = self.export_to_js)
         sub_sesam.add_command(label='Run all PULS lines', command=self.puls_run_all_lines)
         sub_sesam.add_command(label='Delete all PULS results', command=self.puls_delete_all)
@@ -200,14 +198,15 @@
         sub_colors.add_command(label = 'Colors - Light', command = lambda id = "light": self.set_colors(id))
         sub_colors.add_command(label='Colors - Grey', command = lambda id = "grey": self.set_colors(id))
         sub_colors.add_command(label='Colors - Dark', command = lambda id = "dark": self.set_colors(id))
         sub_colors.add_command(label='Colors - Unicorn', command=lambda id="pink": self.set_colors(id))
         sub_colors.add_command(label='Colors - Slava Ukraini', command=lambda id="SlavaUkraini": self.set_colors(id))
         sub_colors.add_command(label='Functional - All items', command=lambda id="all items": self.set_colors(id))
         sub_colors.add_command(label='Functional - Modelling', command=lambda id="modelling": self.set_colors(id))
+        sub_colors.add_command(label='Functional - Cylinder', command=lambda id="cylinder": self.set_colors(id))
 
         #base_mult = 1.2
         #base_canvas_dim = [int(1000 * base_mult),int(720*base_mult)]  #do not modify this, sets the "orignal" canvas dimensions.
         base_canvas_dim = [1000,720]  #do not modify this, sets the "orignal" canvas dimensions.
 
         self._canvas_dim = [int(base_canvas_dim[0] *1),
                            int(base_canvas_dim[1] *1)]
@@ -262,15 +261,16 @@
         self._prop_canvas.place(relx=x_canvas_place, rely=0.73, relwidth=0.38, relheight = 0.27)
         self._result_canvas.place(relx=x_canvas_place+0.38, rely=0.73, relwidth=0.36, relheight = 0.27)
 
 
 
         # Point frame
         self._pt_frame = tk.Frame(self._main_canvas, width=100, height=100, bg="black", relief='raised')
-
+        # Cylinder gui look placement of optmization button
+        self._gui_functional_look_cylinder_opt = [0.82, 0.008, 0.04, 0.175]
         #
         # -------------------------------------------------------------------------------------------------------------
         #
         # The dictionaries below are the main deictionaries used to define this application.
         self._point_dict = {} # Main point dictionary (point:coords) - see method new_point
         self._line_dict = {} # Main line dictionary (line:point,point) - see method new_line
         self._line_to_struc = {} # Main line assosiations (line:various objects) - see method new_structure
@@ -1738,17 +1738,16 @@
                                       'Flat plate, stiffened place': [[lc_x, lc_y - 6 * lc_y_delta, 0.04, 0.098],
                                                    [lc_x+0.1, lc_y - 6 * lc_y_delta, 0.04, 0.065],
                                                    [lc_x + 0.167, lc_y - 6 * lc_y_delta, 0.04, 0.04]],
                                       'Flat plate, unstiffened': [],
                                       'Flat plate, unstiffened place': [],
                                       'Flat plate, stiffened with girder': [],
                                       'Flat plate, stiffened with girder place': [],
-
-                                   'cylinder': [self._opt_cylinder],
-                                   'cylinder place' : [[lc_x, lc_y - 6 * lc_y_delta, 0.04, 0.175]]}
+                                       'cylinder': [self._opt_cylinder],
+                                       'cylinder place' : [[lc_x, lc_y - 6 * lc_y_delta, 0.04, 0.175]]}
 
         # Load information button
         ttk.Button(self._main_fr, text='Load info', command=self.button_load_info_click,style = "Bold.TButton")\
            .place(relx=0.78,rely=0.7, relwidth = 0.04)
 
         # Load information button
         ttk.Button(self._main_fr, text='Load factors', command=self.on_open_load_factor_window,style = "Bold.TButton")\
@@ -1802,16 +1801,25 @@
             tk.Misc.lift(self._main_canvas)
             self._gui_functional_look = 'modelling'
         elif theme == 'all items':
             self._gui_functional_look = 'all items'
             self._main_canvas.place_forget()
             x_canvas_place = 0.26
             self._main_canvas.place(relx=x_canvas_place, rely=0, relwidth=0.523, relheight=0.73)
+        elif theme == 'cylinder':
+            self._main_canvas.place_forget()
+            x_canvas_place = 0.26
+            self._main_canvas.place(relx=x_canvas_place, rely=0,relwidth=0.74, relheight = 0.73)
+            tk.Misc.lift(self._main_canvas)
+            self._gui_functional_look = 'cylinder'
+            placement = self._gui_functional_look_cylinder_opt # [0.786458333, 0.12962963000000005, 0.04, 0.175]
+            self._opt_cylinder.place(relx=placement[0], rely=placement[1], relheight=placement[2], relwidth=placement[3])
+            tk.Misc.lift(self._opt_cylinder)
 
-        if theme not in ['modelling', 'all items']:
+        if theme not in ['modelling', 'all items','cylinder']:
             self._style.configure("Bold.TButton", font=('Sans', '10', 'bold'))
             self._style.configure('TCheckbutton', background=self._general_color)
             self._style.configure('TFrame', background=self._general_color)
             self._style.configure('TLabel', background=self._general_color, foreground = self._color_text)
             self._style.configure('TScale', background=self._general_color)
             self._style.configure('TEntry', background=ent_bg)
             self._style.configure('TOptionMenu', background=ent_bg)
@@ -1987,15 +1995,15 @@
             ent_geo_y += delta_y*(len(self._shell_gui_items[1:])+1)
 
         if long_stf:
 
             self._lab_shell_long_stiffener.place(relx=hor_start, rely=ent_geo_y+ delta_y)
 
             tmp_unit_info = list()
-            for lab in ['Web, hw', 'Web, tw', 'Flange b', 'Flange, tw', 'Spacing, s', 'Stf. type', 'Load section']:
+            for lab in ['Web, hw', 'Web, tw', 'Flange b', 'Flange, tf', 'Spacing, s', 'Stf. type', 'Load section']:
                 tmp_unit_info.append(ttk.Label(self._tab_prop, text=lab))
 
             for lab, idx in zip(tmp_unit_info, range(len(tmp_unit_info))):
                 lab.place(relx=hor_start + idx * delta_x,rely=ent_geo_y+ delta_y*2)
                 self._unit_informations_dimensions.append(lab)
 
             for idx, entry in enumerate(self._shell_long_stf_gui_items[1:]):
@@ -2003,15 +2011,15 @@
 
             self._unit_informations_dimensions.append(self._lab_shell_long_stiffener)
             ent_geo_y += delta_y*3
 
         if ring_stf:
             self._lab_shell_ring_stiffener.place(relx=hor_start, rely=ent_geo_y+ delta_y*1)
             tmp_unit_info = list()
-            for lab in ['Web, hw', 'Web, tw', 'Flange, b', 'Flange, tw','tr. br. dist', 'Stf. type',
+            for lab in ['Web, hw', 'Web, tw', 'Flange, b', 'Flange, tf','tr. br. dist', 'Stf. type',
                         'Exclude', 'Load section prop.']:
                 tmp_unit_info.append(ttk.Label(self._tab_prop, text=lab))
 
             for lab, idx in zip(tmp_unit_info, range(len(tmp_unit_info))):
 
                 if idx in [6,7]:
                     lab.place(relx=hor_start + (idx-6) * delta_x*3, rely=ent_geo_y + delta_y * 4)
@@ -2039,15 +2047,15 @@
                 if idx in [7, 8]:
                     entry.place(relx=hor_start + (idx - 7) * delta_x * 4 + delta_x, rely=ent_geo_y + delta_y * 4,
                                 relwidth=geo_ent_width)
                 else:
                     entry.place(relx=hor_start + idx * delta_x, rely=ent_geo_y + delta_y * 3, relwidth=geo_ent_width)
 
             tmp_unit_info = list()
-            for lab in ['Web, hw', 'Web, tw', 'Flange, b', 'Flange, tw', 'tr. br. dist', 'L bet. Gird.',
+            for lab in ['Web, hw', 'Web, tw', 'Flange, b', 'Flange, tf', 'tr. br. dist', 'L bet. Gird.',
                         'Stf. type', 'Exclude', 'Load section prop.']:
                 tmp_unit_info.append(ttk.Label(self._tab_prop, text=lab))
 
             for lab, idx in zip(tmp_unit_info, range(len(tmp_unit_info))):
                 if idx in [7,8]:
                     lab.place(relx=hor_start + (idx-7) * delta_x*3, rely=ent_geo_y + delta_y * 4)
                 else:
@@ -2249,19 +2257,19 @@
                     sasd, smsd, tTsd, tQsd, shsd = hlp.helper_cylinder_stress_to_force_to_stress(
                         stresses=None, forces=forces, geometry=struc_obj.geometry, shell_t=self._new_shell_thk.get(),
                         shell_radius=self._new_shell_radius.get(), shell_spacing=self._new_stf_spacing.get(),
                         hw=self._new_stf_web_h.get(), tw=self._new_stf_web_t.get(), b=self._new_stf_fl_w.get(),
                         tf=self._new_stf_fl_t.get(), CylinderAndCurvedPlate=CylinderAndCurvedPlate)
                     self._new_shell_sasd.set(sasd)
                     self._new_shell_smsd.set(smsd)
-                    self._new_shell_tTsd.set(tTsd)
+                    self._new_shell_tTsd.set(abs(tTsd))
                     self._new_shell_tQsd.set(tQsd)
                     # self._new_shell_shsd.set(0)
                 else:
-                    stresses = [self._new_shell_sasd.get(), self._new_shell_smsd.get(), self._new_shell_tTsd.get(),
+                    stresses = [self._new_shell_sasd.get(), self._new_shell_smsd.get(), abs(self._new_shell_tTsd.get()),
                                 self._new_shell_tQsd.get(), self._new_shell_shsd.get()]
                     sasd, smsd, tTsd, tQsd, shsd = stresses
                     Nsd, Msd, Tsd, Qsd, shsd = hlp.helper_cylinder_stress_to_force_to_stress(
                         stresses=stresses, geometry=struc_obj.geometry, shell_t=self._new_shell_thk.get(),
                         shell_radius=self._new_shell_radius.get(), shell_spacing=self._new_stf_spacing.get(),
                         hw=self._new_stf_web_h.get(), tw=self._new_stf_web_t.get(), b=self._new_stf_fl_w.get(),
                         tf=self._new_stf_fl_t.get(), CylinderAndCurvedPlate=CylinderAndCurvedPlate)
@@ -2863,18 +2871,50 @@
         elif current_line is not None:
             line_iterator = [current_line, ]
         elif current_line not in self._line_to_struc.keys() and active_line_only:
             return return_dict
         else:
             return return_dict
         rec_for_color = {}
+
+        # Cylinder general
+        all_cyl_thk, recorded_cyl_long_stf = list(), list()
+        for obj_list in self._line_to_struc.values():
+            if obj_list[5] is not None:
+                all_cyl_thk.append(round(obj_list[5].ShellObj.thk * 1000, 2))
+                recorded_cyl_long_stf.append(obj_list[5].LongStfObj.get_beam_string())
+        all_cyl_thk = np.unique(all_cyl_thk)
+        all_cyl_thk = np.sort(all_cyl_thk)
+
         for current_line in line_iterator:
             rec_for_color[current_line]  = {}
             slamming_pressure = 0
             if current_line in self._line_to_struc.keys():
+
+
+                if self._line_to_struc[current_line][5] is not None:
+                    cyl_obj = self._line_to_struc[current_line][5]
+                    cyl_radius = round(cyl_obj.ShellObj.radius * 1000, 2)
+                    cyl_thickness = round(cyl_obj.ShellObj.thk * 1000, 2)
+                    cyl_long_str = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_ring_stf = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_heavy_ring = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_span = round(cyl_obj.ShellObj.dist_between_rings, 1)
+                    cyl_tot_length = round(cyl_obj.ShellObj.length_of_shell, 1)
+                    cyl_tot_cyl = round(cyl_obj.ShellObj.tot_cyl_length, 1)
+                    cyl_sigma_axial = cyl_obj.sasd / 1e6
+                    cyl_sigma_bend = cyl_obj.smsd / 1e6
+                    cyl_sigma_tors = cyl_obj.tTsd / 1e6
+                    cyl_tau_xy = cyl_obj.tQsd / 1e6
+                    cyl_lat_press = cyl_obj.psd / 1e6
+                    cyl_sigma_hoop = cyl_obj.shsd / 1e6
+                    cyl_results = cyl_obj.get_utilization_factors()
+                else:
+                    cyl_thickness = 0
+
                 all_obj = self._line_to_struc[current_line][0]
                 obj_scnt_calc_pl = all_obj.Plate #self._line_to_struc[current_line][1]
                 obj_scnt_calc_stf = all_obj.Stiffener  # self._line_to_struc[current_line][1]
                 obj_scnt_calc_girder = all_obj.Girder  # self._line_to_struc[current_line][1]
 
                 return_dict['all_obj'][current_line] = all_obj
 
@@ -2978,16 +3018,15 @@
                 return_dict['colors'][current_line] = {'buckling': color_buckling, 'fatigue': color_fatigue,
                                                        'section': color_sec, 'shear': color_shear,
                                                        'thickness': color_thk}
                 '''
                 Cylinder calculations
                 '''
                 if self._line_to_struc[current_line][5] is not None:
-                    cylinder_results = self._line_to_struc[current_line][5].get_utilization_factors()
-                    return_dict['cylinder'][current_line] = cylinder_results
+                    return_dict['cylinder'][current_line] = cyl_results
 
 
                 '''
                 PULS calculations
                 '''
                 if self._PULS_results != None:
                     res = self._PULS_results.get_puls_line_results(current_line)
@@ -3174,36 +3213,59 @@
 
                 # Color coding state
                 self._state_logger[current_line] = return_dict #  Logging the current state of the line.
                 self._line_to_struc[current_line][0].need_recalc = False
             else:
                 pass
 
-        sec_in_model, idx, recorded_sections = dict(), 0, list()
+        sec_in_model,  idx, recorded_sections = dict(), 0, list()
+        cyl_sec_in_model, idx_cyl, recorded_cyl_sections = dict(),  0, list()
+
         for data in self._line_to_struc.values():
             if data[0].Stiffener is not None:
                 if data[0].Stiffener.get_beam_string() not in recorded_sections:
                     sec_in_model[data[0].Stiffener.get_beam_string()] = idx
                     recorded_sections.append(data[0].Stiffener.get_beam_string())
                     idx += 1
+            if data[5] is not None:
+                if data[5].LongStfObj.get_beam_string() not in recorded_cyl_sections:
+                    cyl_sec_in_model[ data[5].LongStfObj.get_beam_string()] = idx_cyl
+                    recorded_cyl_sections.append(data[5].LongStfObj.get_beam_string())
+                    idx_cyl += 1
+
         sec_in_model['length'] = len(recorded_sections)
+        cyl_sec_in_model['length'] = len(recorded_cyl_sections)
 
         if self._line_to_struc != {}:
             sec_mod_map = np.arange(0,1.1,0.1)
             fat_map = np.arange(0,1.1,0.1)
             all_thicknesses = [round(objs[0].Plate.get_pl_thk(), 5) for objs in self._line_to_struc.values()]
             all_thicknesses = np.unique(all_thicknesses).tolist()
+            
+            
             thickest_plate = max(all_thicknesses)
             if len(all_thicknesses) > 1:
                 thk_map = np.arange(min(all_thicknesses), max(all_thicknesses) + (max(all_thicknesses) -
                                                                                   min(all_thicknesses)) / 10,
                                      (max(all_thicknesses) - min(all_thicknesses)) / 10)
             else:
                 thk_map = all_thicknesses
 
+            # if self._line_to_struc[current_line][5] is not None:
+            #     all_cyl_thk = all_cyl_thk.tolist()
+            #     if len(all_cyl_thk) > 1:
+            #         thk_map_cyl = np.arange(min(all_cyl_thk), max(all_cyl_thk) + (max(all_cyl_thk) -
+            #                                                                           min(all_cyl_thk)) / 10,
+            #                             (max(all_cyl_thk) - min(all_cyl_thk)) / 10)
+            #     else:
+            #         thk_map_cyl = all_cyl_thk
+            # else:
+            #     thk_map_cyl = [1,]
+
+
             try:
                 all_pressures = sorted([self.get_highest_pressure(line)['normal']
                                         for line in list(self._line_dict.keys())])
             except KeyError:
                 all_pressures = [0, 1]
 
             all_pressures = np.unique(all_pressures).tolist()
@@ -3271,30 +3333,32 @@
                 if self._line_to_struc[line][0].Stiffener is not None:
                     spacings.append(self._line_to_struc[line][0].Stiffener.get_s())
             spacing = np.unique(spacings).tolist()
             structure_type = [self._line_to_struc[line][0].Plate.get_structure_type() for line in
                               self._line_to_struc.keys()]
 
             return_dict['color code'] = {'thickest plate': thickest_plate, 'thickness map': thk_map,
-                                         'all thicknesses': all_thicknesses,
+                                         'all thicknesses': all_thicknesses, 'all cyl thicknesses': all_cyl_thk,
                                          'section modulus map': sec_mod_map,
                                          'fatigue map': fat_map,
                                          'highest pressure': highest_pressure, 'lowest pressure': lowest_pressure,
                                          'pressure map': press_map, 'all pressures':all_pressures,
                                          'all utilizations': all_utils, 'utilization map': util_map,
                                          'PULS utilization map': puls_util_map,
                                          'max sigma x': max(sig_x), 'min sigma x': min(sig_x), 'sigma x map': sig_x_map,
                                          'max sigma y1': max(sig_y1), 'min sigma y1': min(sig_y1),
                                          'sigma y1 map': sig_y1_map,
                                          'max sigma y2': max(sig_y2), 'min sigma y2': min(sig_y2),
                                          'sigma y2 map': sig_y2_map,
                                          'max tau xy': max(tau_xy), 'min tau xy': min(tau_xy), 'tau xy map': tau_xy_map,
                                          'structure types map': np.unique(structure_type).tolist(),
                                          'sections in model': sec_in_model,
+                                         'cyl sections in model': cyl_sec_in_model,
                                          'recorded sections': recorded_sections,
+                                         'recorded cylinder long sections' : recorded_cyl_sections,
                                          'spacings': spacing, 'max spacing': max(spacing), 'min spacing': min(spacing)}
             line_color_coding, puls_method_map, puls_sp_or_up_map = \
                 {}, {None: 0, 'buckling': 0.5, 'ultimate': 1}, {None:0, 'SP': 0.5, 'UP': 1}
             cmap_sections = plt.get_cmap('jet')
             thk_sort_unique = return_dict['color code']['all thicknesses']
             spacing_sort_unique = return_dict['color code']['spacings']
             structure_type_unique = return_dict['color code']['structure types map']
@@ -3309,14 +3373,47 @@
                     puls_method = self._line_to_struc[line][0].Plate.get_puls_method()
                     puls_uf = self._PULS_results.get_utilization(
                                                    line, puls_method,
                                                    self._new_puls_uf.get())
                     puls_color = matplotlib.colors.rgb2hex(cmap_sections(puls_uf))
                     puls_sp_or_up = self._line_to_struc[line][0].Plate.get_puls_sp_or_up()
 
+                # Cylinders
+                if self._line_to_struc[line][5] is not None:
+                    cyl_obj = self._line_to_struc[line][5]
+                    cyl_radius = round(cyl_obj.ShellObj.radius * 1000, 2)
+                    cyl_thickness = round(cyl_obj.ShellObj.thk * 1000, 2)
+                    cyl_long_str = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_ring_stf = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_heavy_ring = cyl_obj.LongStfObj.get_beam_string()
+                    cyl_span = round(cyl_obj.ShellObj.dist_between_rings, 1)
+                    cyl_tot_length = round(cyl_obj.ShellObj.length_of_shell, 1)
+                    cyl_tot_cyl = round(cyl_obj.ShellObj.tot_cyl_length, 1)
+                    cyl_sigma_axial = cyl_obj.sasd / 1e6
+                    cyl_sigma_bend = cyl_obj.smsd / 1e6
+                    cyl_sigma_tors = cyl_obj.tTsd / 1e6
+                    tau_xy = cyl_obj.tQsd / 1e6
+                    cyl_lat_press = cyl_obj.psd / 1e6
+                    cyl_sigma_hoop = cyl_obj.shsd / 1e6
+                    cyl_results = cyl_obj.get_utilization_factors()
+
+                    cyl_uf =  max([round(0 if cyl_results['Unstiffened shell'] is None else
+                                         cyl_results['Unstiffened shell'],2),
+                                   round(0 if cyl_results['Longitudinal stiffened shell'] is None else
+                                         cyl_results['Longitudinal stiffened shell'],2),
+                                   round(0 if cyl_results['Ring stiffened shell'] is None else
+                                         cyl_results['Ring stiffened shell'],2),
+                                   round(0 if cyl_results['Heavy ring frame'] is None else
+                                         cyl_results['Heavy ring frame'],2)])
+                else:
+                    cyl_uf = 0
+                    cyl_long_str = ' '
+                    cyl_long_str = None
+                    cyl_thickness = None
+
                 rp_uf = rec_for_color[line]['rp buckling']
 
                 tot_uf_rp = max([rec_for_color[line]['fatigue'], rp_uf,
                                  rec_for_color[line]['section modulus'], rec_for_color[line]['shear'],
                                  rec_for_color[line]['plate thickness']])
                 tot_uf_puls = max([rec_for_color[line]['fatigue'], puls_uf,
                                  rec_for_color[line]['section modulus'], rec_for_color[line]['shear'],
@@ -3324,39 +3421,46 @@
                 try:
                     this_pressure = self.get_highest_pressure(line)['normal']
                 except KeyError:
                     this_pressure = 0
                 rp_util = max(list(return_dict['utilization'][line].values()))
 
                 res = list()
+
                 for stress_list, this_stress in zip([sig_x, sig_y1, sig_y2, tau_xy],
                                                      [line_data[0].Plate.get_sigma_x1(), line_data[0].Plate.get_sigma_y1(),
                                                       line_data[0].Plate.get_sigma_y2(), line_data[0].Plate.get_tau_xy()]):
-                    if len(stress_list) == 1:
+                    if type(stress_list)==float:
+                        res.append(1)
+                    elif len(stress_list) == 1:
                         res.append(1)
                     elif max(stress_list) == 0 and min(stress_list) == 0:
                         res.append(0)
                     elif this_stress < 0:
                         res.append(this_stress /min(stress_list))
                     elif this_stress >= 0:
                         res.append(this_stress/ max(stress_list))
 
                 sig_x_uf, sig_y1_uf, sig_y2_uf , tau_xy_uf = res
-
+                if type(all_cyl_thk) is not list:
+                    all_cyl_thk = all_cyl_thk.tolist()
 
                 line_color_coding[line] = {'plate': matplotlib.colors.rgb2hex(cmap_sections(
                     thk_sort_unique.index(round(line_data[0].Plate.get_pl_thk(),10))/len(thk_sort_unique))),
                                            'spacing': 'black' if line_data[0].Stiffener is None else matplotlib.colors.rgb2hex(
                                                cmap_sections(spacing_sort_unique.index(round(line_data[0].Stiffener
                                                                                          .get_s(), 10)) / len(
                                                    spacing_sort_unique))),
                                            'section': 'black' if line_data[0].Stiffener is None else
                                            matplotlib.colors.rgb2hex(cmap_sections(sec_in_model[line_data[0]
                                                                                    .Stiffener.get_beam_string()]/
                                                                                    len(list(recorded_sections)))),
+                                            'section cyl': 'black' if cyl_long_str is None else
+                                            matplotlib.colors.rgb2hex(cmap_sections(cyl_sec_in_model[cyl_long_str] /
+                                                                                    len(list(recorded_cyl_sections)))),
                                            'structure type': matplotlib.colors.rgb2hex(
                                                cmap_sections(structure_type_unique.index(line_data[0].Plate.get_structure_type())
                                                              /len(structure_type_unique))),
                                            'pressure color': 'black' if all_pressures in [[0],[0,1]] else matplotlib.colors.rgb2hex(cmap_sections(
                                                this_pressure/highest_pressure)),
                                            'pressure': this_pressure,
                                            'rp uf color': matplotlib.colors.rgb2hex(cmap_sections(rp_util)),
@@ -3377,14 +3481,18 @@
                                            'PULS uf color': puls_color,
                                            'fatigue uf' : rec_for_color[line]['fatigue'],
                                            'section uf' : rec_for_color[line]['section modulus'],
                                            'sigma x': matplotlib.colors.rgb2hex(cmap_sections(sig_x_uf)),
                                            'sigma y1': matplotlib.colors.rgb2hex(cmap_sections(sig_y1_uf)),
                                            'sigma y2': matplotlib.colors.rgb2hex(cmap_sections(sig_y2_uf)),
                                            'tau xy':matplotlib.colors.rgb2hex(cmap_sections(tau_xy_uf)),
+                    'cylinder uf': matplotlib.colors.rgb2hex(cmap_sections(cyl_uf)),
+                    'cylinder plate' :  matplotlib.colors.rgb2hex
+                    (cmap_sections(0 if cyl_thickness is None else all_cyl_thk.index(cyl_thickness)/len(all_cyl_thk)))
+
                                            }
                 return_dict['color code']['lines'] = line_color_coding
 
                 # COG calculations
                 # Steel
                 tot_weight += return_dict['weights'][line]['line weight']
                 weight_mult_dist_x += return_dict['weights'][line]['line weight']\
@@ -3683,23 +3791,30 @@
                                               fill='black',
                                               anchor="nw")
                 self._main_canvas.create_text(10, start_text+20*idx, text=section,
                                               font=self._text_size["Text 10 bold"],
                                               fill=matplotlib.colors.rgb2hex(cmap_sections(idx/sec_in_model['length'])),
                                               anchor="nw")
         elif self._new_colorcode_plates.get() == True and self._line_to_struc != {}:
-
-            all_thicknesses = np.unique(cc_state['all thicknesses']).tolist()
+            cylinder = False
+            for obj_list in self._line_to_struc.values():
+                if obj_list[5] is not None:
+                    cylinder = True
+            if cylinder:
+                all_thicknesses = np.unique(cc_state['all cyl thicknesses']).tolist()
+            else:
+                all_thicknesses = np.unique(cc_state['all thicknesses']).tolist()
 
             for idx, thk in enumerate(np.unique(all_thicknesses).tolist()):
-                self._main_canvas.create_text(11, start_text_shift+20*idx, text=str('Plate '+ str(thk*1000) + ' mm'),
+                self._main_canvas.create_text(11, start_text_shift+20*idx, text=str('Plate '+
+                                                                                    str(thk if cylinder else thk*1000) + ' mm'),
                                               font=self._text_size["Text 10 bold"],
                                               fill='black',
                                               anchor="nw")
-                self._main_canvas.create_text(10, start_text+20*idx, text=str('Plate '+ str(thk*1000) + ' mm'),
+                self._main_canvas.create_text(10, start_text+20*idx, text=str('Plate '+ str(thk if cylinder else thk*1000) + ' mm'),
                                               font=self._text_size["Text 10 bold"],
                                               fill=matplotlib.colors.rgb2hex(cmap_sections(all_thicknesses.index(thk)
                                                                                            /len(all_thicknesses))),
                                               anchor="nw")
         elif self._new_colorcode_spacing.get() == True and self._line_to_struc != {}:
 
             all_spacings = cc_state['spacings']
@@ -3855,32 +3970,45 @@
                                               font=self._text_size["Text 10 bold"],
                                               fill='blue' if value == 'ultimate' else 'red',
                                               anchor="nw")
 
     def color_code_line(self, state, line, coord1, vector):
 
         cc_state = state['color code']
+
         if line not in state['color code']['lines'].keys():
             return 'black'
+
+
         if self._new_colorcode_beams.get() == True and line in list(self._line_to_struc.keys()):
             if self._line_to_struc[line][5] is not None or self._line_to_struc[line][0].Stiffener is None:
-                color = 'grey'
-                this_text = 'N/A'
+                if self._line_to_struc[line][5] is not None:
+                    cyl_obj = self._line_to_struc[line][5]
+                    if cyl_obj.LongStfObj is not None:
+                        this_text = cyl_obj.LongStfObj.get_beam_string(short = True)
+                        color = state['color code']['lines'][line]['section cyl']
+                    else:
+                        this_text = 'N/A'
+                        color = 'grey'
+                else:
+                    color = 'grey'
+                    this_text = 'N/A'
             elif self._line_to_struc[line][0].Plate is not None:
                 color = state['color code']['lines'][line]['section']
                 this_text = self._line_to_struc[line][0].Plate.get_beam_string()
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text ,
                                               font=self._text_size["Text 7"])
 
         elif self._new_colorcode_plates.get() == True and line in list(self._line_to_struc.keys()):
             if self._line_to_struc[line][5] is not None:
-                color = 'grey'
-                this_text = 'N/A'
+                cyl_obj = self._line_to_struc[line][5]
+                color = state['color code']['lines'][line]['cylinder plate']
+                this_text = str(round(cyl_obj.ShellObj.thk * 1000, 2))
             else:
                 color = state['color code']['lines'][line]['plate']
                 this_text = str(self._line_to_struc[line][0].Plate.get_pl_thk()*1000)
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text)
 
@@ -3891,15 +4019,14 @@
             else:
                 color = state['color code']['lines'][line]['spacing']
                 this_text = str(self._line_to_struc[line][0].Stiffener.get_s()*1000)
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text)
 
-
         elif self._new_colorcode_pressure.get() == True and line in list(self._line_to_struc.keys()):
             if self._line_to_struc[line][5] is not None:
                 color = 'grey'
                 this_text = 'N/A'
             else:
                 if cc_state['all pressures'] == [0, 1]:
                     color = 'black'
@@ -3907,33 +4034,47 @@
                     color = state['color code']['lines'][line]['pressure color']
                 this_text = str(state['color code']['lines'][line]['pressure'])
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text)
 
         elif self._new_colorcode_utilization.get() == True and self._new_buckling_method.get() == 'DNV-RP-C201 - prescriptive':
-            if self._line_to_struc[line][5] is not None:
-                color = 'grey'
+            if line not in list(self._line_to_struc.keys()):
+                color = 'black'
                 this_text = 'N/A'
+            elif self._line_to_struc[line][5] is not None:
+                cyl_obj = self._line_to_struc[line][5]
+                results = cyl_obj.get_utilization_factors()
+                ufs = [round(0 if results['Unstiffened shell'] is None else results['Unstiffened shell'], 2),
+                       round(0 if results['Longitudinal stiffened shell'] is None else results['Longitudinal stiffened shell'],2),
+                       round(0 if results['Ring stiffened shell'] is None else results['Ring stiffened shell'], 2),
+                       round(0 if results['Heavy ring frame'] is None else results['Heavy ring frame'], 2)]
+
+                color = state['color code']['lines'][line]['cylinder uf']
+                this_text = str(max(ufs))
+                if self._new_label_color_coding.get():
+                    self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
+                                                  text=this_text)
             else:
                 color = state['color code']['lines'][line]['rp uf color']
-            if self._new_label_color_coding.get():
-                self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
-                                              text=round(state['color code']['lines'][line]['rp uf'],2))
+                if self._new_label_color_coding.get():
+                    self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
+                                                  text=round(state['color code']['lines'][line]['rp uf'],2))
 
         elif self._new_colorcode_utilization.get() == True and self._new_buckling_method.get() == 'DNV PULS':
             if self._line_to_struc[line][5] is not None:
                 color = 'grey'
                 this_text = 'N/A'
             else:
                 color = state['color code']['lines'][line]['PULS uf color']
                 this_text = round(state['color code']['lines'][line]['PULS uf'],2)
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text)
+
         elif self._new_colorcode_utilization.get() == True and self._new_buckling_method.get() == 'ML-CL (PULS based)':
             color = 'black'
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text='N/A')
 
         elif self._new_colorcode_sigmax.get() == True:
@@ -4020,43 +4161,52 @@
                 this_text = round(state['color code']['lines'][line]['fatigue uf'],2)
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=this_text)
 
         elif self._new_colorcode_total.get() == True:
             if self._line_to_struc[line][5] is not None:
-                color = 'grey'
-                this_text = 'N/A'
+                cyl_obj = self._line_to_struc[line][5]
+                results = cyl_obj.get_utilization_factors()
+                ufs = [round(0 if results['Unstiffened shell'] is None else results['Unstiffened shell'], 2),
+                       round(0 if results['Longitudinal stiffened shell'] is None else results['Longitudinal stiffened shell'],2),
+                       round(0 if results['Ring stiffened shell'] is None else results['Ring stiffened shell'], 2),
+                       round(0 if results['Heavy ring frame'] is None else results['Heavy ring frame'], 2)]
+
+                color = state['color code']['lines'][line]['cylinder uf']
+                this_text = str(max(ufs))
                 if self._new_label_color_coding.get():
                     self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                                   text=this_text)
 
             elif self._new_buckling_method.get() == 'DNV PULS':
-                color = state['color code']['lines'][line]['Total uf color rp']
+                color = state['color code']['lines'][line]['Total uf color puls']
                 if self._new_label_color_coding.get():
                     self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                                   text=round(state['color code']['lines'][line]['Total uf puls'],2))
             elif self._new_buckling_method.get() == 'DNV-RP-C201 - prescriptive':
-                color = state['color code']['lines'][line]['Total uf color puls']
+                color = state['color code']['lines'][line]['Total uf color rp']
                 if self._new_label_color_coding.get():
                     self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                                   text=round(state['color code']['lines'][line]['Total uf rp'],2))
             elif self._new_buckling_method.get() == 'ML-CL (PULS based)':
                 color = 'black'
                 if self._new_label_color_coding.get():
                     self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                                   text='N/A')
+
         elif self._new_colorcode_puls_acceptance.get():
             if state['color code']['lines'][line]['PULS method'] == None:
                 color = 'black'
             else:
                 color = 'blue' if state['color code']['lines'][line]['PULS method'] == 'ultimate' else 'red'
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
                                               text=state['color code']['lines'][line]['PULS method'])
+
         elif self._new_colorcode_puls_sp_or_up.get():
             if state['color code']['lines'][line]['PULS sp or up'] == None:
                 color = 'black'
             else:
                 color = 'blue' if state['color code']['lines'][line]['PULS sp or up'] == 'SP' else 'red'
             if self._new_label_color_coding.get():
                 self._main_canvas.create_text(coord1[0] + vector[0] / 2 + 5, coord1[1] + vector[1] / 2 - 10,
@@ -4694,16 +4844,18 @@
                                                             anchor='nw',
                                                             fill = self._color_text)
                             y_location += 1
                             idx_y, idx_x = 0, 0
 
                             for stf_type, chk_bool in value.items():
                                 stf_text = stf_type
+                                if stf_type == 'ring frame':
+                                    continue
 
-                                chk_text = 'OK' if chk_bool == True else 'Not OK' if chk_bool == False else 'N/A'
+                                chk_text = 'OK' if chk_bool == True else 'failed' if chk_bool == False else 'N/A'
 
                                 self._result_canvas.create_text([15*dx*idx_x, dy*y_location],
                                                                 text=stf_text, font=self._text_size['Text 10 bold'],
                                                                 anchor='nw',
                                                                 fill=self._color_text if not value else 'black')
 
                                 self._result_canvas.create_text([15*dx*idx_x, y + (y_location+1)*dy],
@@ -4877,15 +5029,16 @@
                 # updating the span and deleting compartments (if not WT)
                 if get_num(self._active_point) in data:
                     coord1 = self._point_dict['point'+str(data[0])]
                     coord2 = self._point_dict['point'+str(data[1])]
                     if line in self._line_to_struc.keys():
                         self._line_to_struc[line][0].Plate.set_span(dist(coord1,coord2))
                         self._line_to_struc[line][0].Plate.set_span(dist(coord1, coord2))
-                        self._PULS_results.result_changed(line)
+                        if self._PULS_results is not None:
+                            self._PULS_results.result_changed(line)
                         if self._line_to_struc[line][0].Plate.get_structure_type() not in ['GENERAL_INTERNAL_NONWT',
                                                                                                 'FRAME']:
                             self._tank_dict = {}
                             self._main_grid.clear()
                             self._compartments_listbox.delete(0, 'end')
 
             for line, obj in self._line_to_struc.items():
@@ -5147,15 +5300,16 @@
                             tf=self._new_stf_fl_t.get(), CylinderAndCurvedPlate=CylinderAndCurvedPlate)
                         self._new_shell_sasd.set(sasd)
                         self._new_shell_smsd.set(smsd)
                         self._new_shell_tTsd.set(tTsd)
                         self._new_shell_tQsd.set(tQsd)
                         #self._new_shell_shsd.set(0)
                     else:
-                        stresses = [self._new_shell_sasd.get(), self._new_shell_smsd.get(), self._new_shell_tTsd.get(),
+                        stresses = [self._new_shell_sasd.get(), self._new_shell_smsd.get(),
+                                    abs(self._new_shell_tTsd.get()),
                                     self._new_shell_tQsd.get(), self._new_shell_shsd.get()]
                         sasd, smsd, tTsd, tQsd, shsd = stresses
                         Nsd, Msd, Tsd, Qsd, shsd = hlp.helper_cylinder_stress_to_force_to_stress(
                             stresses=stresses, geometry=geometry, shell_t=self._new_shell_thk.get(),
                             shell_radius=self._new_shell_radius.get(), shell_spacing=self._new_stf_spacing.get(),
                             hw=self._new_stf_web_h.get(), tw=self._new_stf_web_t.get(), b=self._new_stf_fl_w.get(),
                             tf=self._new_stf_fl_t.get(), CylinderAndCurvedPlate=CylinderAndCurvedPlate)
@@ -6314,15 +6468,16 @@
                 #'Flat plate, unstiffened', 'Flat plate, stiffened', 'Flat plate, stiffened with girder'
                 for dom in ['Flat plate, unstiffened', 'Flat plate, stiffened', 'Flat plate, stiffened with girder']:
                     for btn, placement in zip(self._optimization_buttons[dom],
                                               self._optimization_buttons[dom + ' place']):
                         btn.place_forget()
                 for btn, placement in zip(self._optimization_buttons['cylinder'],
                                           self._optimization_buttons['cylinder place']):
-
+                    if self._gui_functional_look == 'cylinder':
+                        placement = self._gui_functional_look_cylinder_opt
                     btn.place(relx = placement[0], rely= placement[1],relheight = placement[2], relwidth = placement[3])
 
             else:
                 self._new_calculation_domain.set(self._line_to_struc[self._active_line][0].calculation_domain)
                 self.calculation_domain_selected()
                 dom = self._line_to_struc[self._active_line][0].calculation_domain
                 for btn, placement in zip(self._optimization_buttons['cylinder'],
```

### Comparing `ANYstructure-4.7/any_files/make_grid_numpy.py` & `ANYstructure-4.8/any_files/make_grid_numpy.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/make_queue.py` & `ANYstructure-4.8/any_files/make_queue.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/make_stack.py` & `ANYstructure-4.8/any_files/make_stack.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_CSR-Tank_req_cl_UP_scaler.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_CSR-Tank_req_cl_UP_scaler.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_CSR-Tank_req_cl_predictor.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_CSR-Tank_req_cl_predictor.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_SP_scaler.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_SP_scaler.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_predictor.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_CSR_plate_cl,_CSR_web_cl,_CSR_web_flange_cl,_CSR_flange_cl_predictor.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_1_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_predictor_In-plane_support_cl_2,_3_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_1_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_buc_scaler_In-plane_support_cl_2,_3_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_1_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_predictor_In-plane_support_cl_2,_3_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_1_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_SP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_SP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_UP.pickle` & `ANYstructure-4.8/any_files/ml_files/CL_output_cl_ult_scaler_In-plane_support_cl_2,_3_UP.pickle`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/opt_problem.py` & `ANYstructure-4.8/any_files/opt_problem.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/optimize.py` & `ANYstructure-4.8/any_files/optimize.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/optimize_cylinder.py` & `ANYstructure-4.8/any_files/optimize_cylinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import numpy as np
 import time, os, datetime
 from tkinter import messagebox
 from tkinter.filedialog import askopenfilenames
 from multiprocessing import cpu_count
 
 try:
-    import any_files.main_application
+    import any_files.main_application as main_application
     import any_files.optimize as op
     import any_files.example_data as test
 except ModuleNotFoundError:
-    import ANYstructure.any_files.main_application
+    import ANYstructure.any_files.main_application as main_application
     import ANYstructure.any_files.optimize as op
     import ANYstructure.any_files.example_data as test
 
 class CreateOptimizeCylinderWindow():
     '''
     This class initiates the single optimization window.
     '''
 
     def __init__(self,master,app=None):
         super(CreateOptimizeCylinderWindow,self).__init__()
         if __name__ == '__main__':
             import pickle
+            import any_files.calc_structure as calc
             self._initial_structure_obj = test.get_structure_calc_object(heavy=True)
             self._initial_calc_obj = test.get_structure_calc_object(heavy=True)
             self._fatigue_object = test.get_fatigue_object()
             self._fatigue_pressure = test.get_fatigue_pressures()
             self._slamming_pressure = test.get_slamming_pressure()
             image_dir = os.path.dirname(__file__)+'\\images\\'
             self._PULS_object = None
```

### Comparing `ANYstructure-4.7/any_files/optimize_geometry.py` & `ANYstructure-4.8/any_files/optimize_geometry.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/optimize_multiple_window.py` & `ANYstructure-4.8/any_files/optimize_multiple_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/optimize_window.py` & `ANYstructure-4.8/any_files/optimize_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/pl_stf_window.py` & `ANYstructure-4.8/any_files/pl_stf_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     '''
     def __init__(self, master, app):
         super(CreateStructureWindow, self).__init__()
         self._frame = master
         self._frame.wm_title("Define structure properties")
         self._frame.geometry('1800x900')
         self._frame.grab_set()
+        self._root_dir = os.path.dirname(os.path.abspath(__file__))
         if __name__ == '__main__':
             self._initial_structure_obj = test.get_structure_calc_object()
             self._initial_calc_obj = test.get_structure_calc_object()
 
             self._section_list = []
             self._section_objects = []
             for section in hlp.helper_read_section_file('bulb_anglebar_tbar_flatbar.csv'):
@@ -388,15 +389,15 @@
         self.option_choose(None)
 
     def read_sections(self):
         '''
         Read a list.
         '''
         from tkinter import filedialog
-        import helper as hlp
+        import any_files.helper as hlp
         from pathlib import Path
 
         file = filedialog.askopenfile('r')
         file = Path(file.name)
         #m = self._ent_section_list.children['menu']
 
         for section in hlp.helper_read_section_file(file.name):
@@ -405,19 +406,20 @@
             self._section_objects.append(SecObj)
             #m.add_command(label=SecObj.__str__(), command=self.section_choose)
 
     def read_sections_built_in(self):
         '''
         Read a list.
         '''
-        import helper as hlp
+        import any_files.helper as hlp
         if pathlib.Path('bulb_anglebar_tbar_flatbar.csv').exists():
             libfile = 'bulb_anglebar_tbar_flatbar.csv'
         else:
             libfile = 'bulb_anglebar_tbar_flatbar.csv'
+            libfile = self._root_dir + '/' + libfile
         for section in hlp.helper_read_section_file(libfile):
             SecObj = Section(section)
             self._section_list = hlp.add_new_section(self._section_list, SecObj)
             self._section_objects.append(SecObj)
             #m.add_command(label=SecObj.__str__(), command=self.section_choose)
 
         self.regen_option_menu()
```

### Comparing `ANYstructure-4.7/any_files/report_generator.py` & `ANYstructure-4.8/any_files/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,15 @@
 
                     results = cyl_obj.get_utilization_factors()
                     textobject.textLine('Design axial stress/force:     ' + str(cyl_obj.sasd / 1e6) + ' MPa')
                     textobject.textLine('Design bending stress/moment:  ' + str(cyl_obj.smsd / 1e6) + ' MPa')
                     textobject.textLine('Design tosional stress/moment: ' + str(cyl_obj.tTsd / 1e6) + ' MPa')
                     textobject.textLine('Design shear stress/force:     ' + str(cyl_obj.tQsd / 1e6) + ' MPa')
                     textobject.textLine('Design lateral pressure        ' + str(cyl_obj.psd / 1e6) + ' MPa' )
+                    textobject.textLine('Additional hoop stress         ' + str(cyl_obj.shsd / 1e6) + ' MPa')
                     vpos -= 40
                     for key, value in results.items():
                         if key in ['Weight', 'Need to check column buckling']:
                             continue
                         if key not in ['Stiffener check', 'Stiffener check detailed']:
                             text_key = key
                             if key == 'Column stability check':
@@ -458,14 +459,16 @@
         else:
             origo = (50, 450)
         self.c.setLineWidth(2)
         self.c.setStrokeColor('red')
         idx, drawed_data = 0, list()
         all_line_data = self.data.get_color_and_calc_state()
         for line, pt in lines.items():
+            if line not in list(self.data._line_to_struc.keys()):
+                continue
             if draw_type == 'UF':
                 if self.data._new_buckling_method.get() == 'DNV-RP-C201 - prescriptive':
                     try:
                         self.c.setStrokeColor('red' if 'red' in colors[line].values() else 'green')
                     except KeyError:
                         self.c.setStrokeColor('black')
                 elif self.data._new_buckling_method.get() == 'DNV PULS':
@@ -771,80 +774,139 @@
 
     def createTable(self):
         '''
         Create a table of results for all lines.
         '''
 
         table_all = []
-        headers = ['Line', 'pl thk', 's', 'web h', 'web thk', 'fl. w', 'fl. thk', 'sig x1', 'sig x2', 'sig y1',
-                   'sig y2', 'tau xy', 'max press.', 'sec. mod', 'min sec.', 'min plt',
-                   'shr area', 'min shr A', 'fat uf', 'buc uf']
-        table_all.append(headers)
+        cylindersy, flat_plates, idx = False, False,-1
         for line in sorted(self.data._line_dict.keys()):
-            struc_obj = self.data._line_to_struc[line][0]
-            pressure = round(self.data.get_highest_pressure(line)['normal'] / 1000,0)
-
-            if self.data._PULS_results is not None:
-                puls_method = self.data._line_to_struc[line][0].Plate.get_puls_method()
-                if line in self.data._PULS_results.get_run_results().keys():
-                    if puls_method == 'buckling':
-                        buckling_uf = \
-                        self.data._PULS_results.get_run_results()[line]['Buckling strength']['Actual usage Factor'][0]
-                    else:
-                        buckling_uf = \
-                        self.data._PULS_results.get_run_results()[line]['Ultimate capacity']['Actual usage Factor'][0]
-            else:
-                buckling_uf = str(round(max(self.data.get_color_and_calc_state()['buckling'][line]), 2))
-
-            if self.data.get_color_and_calc_state()['fatigue'][line]['damage'] is not None:
-                fat_uf = self.data.get_color_and_calc_state()['fatigue'][line]['damage']
-                fat_uf = round(fat_uf, 3)
-            else:
-                fat_uf = self.data.get_color_and_calc_state()['fatigue'][line]['damage']
-
+            idx += 1
+            if self.data._line_to_struc[line][5] is None and cylinders is False:
+                flat_plates = True
+                if idx == 0:
+                    headers = ['Line', 'pl thk', 's', 'web h', 'web thk', 'fl. w', 'fl. thk', 'sig x1', 'sig x2', 'sig y1',
+                               'sig y2', 'tau xy', 'max press.', 'sec. mod', 'min sec.', 'min plt',
+                               'shr area', 'min shr A', 'fat uf', 'buc uf']
+                    table_all.append(headers)
+                if line not in list(self.data._line_to_struc.keys()):
+                    continue
+                struc_obj = self.data._line_to_struc[line][0]
+                pressure = round(self.data.get_highest_pressure(line)['normal'] / 1000,0)
 
-            data = [line,str(struc_obj.Plate.get_pl_thk() * 1000), str(struc_obj.Plate.get_s() * 1000),
-                    str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_web_h() * 1000),
-                    str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_web_thk() * 1000),
-                    str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_fl_w() * 1000),
-                    str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_fl_thk() * 1000),
-                    str(round(struc_obj.Plate.get_sigma_x1(), 0)), str(round(struc_obj.Plate.get_sigma_x2(), 0)),
-                    str(round(struc_obj.Plate.get_sigma_y1(), 0)),
-                    str(round(struc_obj.Plate.get_sigma_y2(), 0)),
-                    str(round(struc_obj.Plate.get_tau_xy(), 0)), str(round(pressure, 2) * 1000),
-                    str(int(min(self.data.get_color_and_calc_state()['section_modulus'][line]['sec_mod']) * 1000 ** 3)),
-                    str(int(self.data.get_color_and_calc_state()['section_modulus'][line]['min_sec_mod'] * 1000 ** 3)),
-                    str(round(self.data.get_color_and_calc_state()['thickness'][line]['min_thk'], 2)),
-                    str(int(self.data.get_color_and_calc_state()['shear_area'][line]['shear_area'] * 1000 ** 2)),
-                    str(int(self.data.get_color_and_calc_state()['shear_area'][line]['min_shear_area'] * 1000 ** 2)),
-                    fat_uf, buckling_uf]
-
-            table_all.append(data)
-
-        t = Table(table_all,colWidths=[0.55*inch])
-        t.setStyle(TableStyle([
-            ('GRID', (0, 0), (-1, -1), 0.5, colors.gray),
-            ('BACKGROUND', (0, 0), (-1, -1), colors.lightblue),
-            ('FONTSIZE', (0, 0), (-1, -1), 8),
-            ('FONTSIZE', (0, 4), (-1, 4), 8),
-            ('TEXTFONT', (0, 1), (-1, 1), 'Times-Bold'),
-            ('TEXTFONT', (0, 4), (-1, 4), 'Times-Bold'),
-        ]))
+                if self.data._PULS_results is not None:
+                    puls_method = self.data._line_to_struc[line][0].Plate.get_puls_method()
+                    if line in self.data._PULS_results.get_run_results().keys():
+                        if puls_method == 'buckling':
+                            buckling_uf = \
+                            self.data._PULS_results.get_run_results()[line]['Buckling strength']['Actual usage Factor'][0]
+                        else:
+                            buckling_uf = \
+                            self.data._PULS_results.get_run_results()[line]['Ultimate capacity']['Actual usage Factor'][0]
+                else:
+                    try:
+                        buckling_uf = str(round(max(self.data.get_color_and_calc_state()['buckling'][line]), 2))
+                    except TypeError:
+                        buckling_uf = None
+
+                if self.data.get_color_and_calc_state()['fatigue'][line]['damage'] is not None:
+                    fat_uf = self.data.get_color_and_calc_state()['fatigue'][line]['damage']
+                    fat_uf = round(fat_uf, 3)
+                else:
+                    fat_uf = self.data.get_color_and_calc_state()['fatigue'][line]['damage']
+
+
+                data = [line,str(struc_obj.Plate.get_pl_thk() * 1000), str(struc_obj.Plate.get_s() * 1000),
+                        str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_web_h() * 1000),
+                        str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_web_thk() * 1000),
+                        str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_fl_w() * 1000),
+                        str('' if struc_obj.Stiffener is None else struc_obj.Stiffener.get_fl_thk() * 1000),
+                        str(round(struc_obj.Plate.get_sigma_x1(), 0)), str(round(struc_obj.Plate.get_sigma_x2(), 0)),
+                        str(round(struc_obj.Plate.get_sigma_y1(), 0)),
+                        str(round(struc_obj.Plate.get_sigma_y2(), 0)),
+                        str(round(struc_obj.Plate.get_tau_xy(), 0)), str(round(pressure, 2) * 1000),
+                        str(int(min(self.data.get_color_and_calc_state()['section_modulus'][line]['sec_mod']) * 1000 ** 3)),
+                        str(int(self.data.get_color_and_calc_state()['section_modulus'][line]['min_sec_mod'] * 1000 ** 3)),
+                        str(round(self.data.get_color_and_calc_state()['thickness'][line]['min_thk'], 2)),
+                        str(int(self.data.get_color_and_calc_state()['shear_area'][line]['shear_area'] * 1000 ** 2)),
+                        str(int(self.data.get_color_and_calc_state()['shear_area'][line]['min_shear_area'] * 1000 ** 2)),
+                        fat_uf, buckling_uf]
+
+                table_all.append(data)
+
+            elif not flat_plates:
+                cylinders = True
+                if idx == 0:
+                    headers = ['Line', 'Radius', 'Thickness', 'Span', 'Tot. length',
+                               'Axial stress', 'Bend stress', 'Tors. stress', 'Shear stress', 'Lat. press.',
+                               'Hoop stress',
+                               'UF shell', 'UF long. stf.', 'UF ring. stf.', 'UF girder']
+                    table_all.append(headers)
+                cyl_obj = self.data._line_to_struc[line][5]
+                radius = round(cyl_obj.ShellObj.radius * 1000, 2)
+                thickness = round(cyl_obj.ShellObj.thk * 1000, 2)
+                long_str = cyl_obj.LongStfObj.get_beam_string()
+                ring_stf = cyl_obj.LongStfObj.get_beam_string()
+                heavy_ring = cyl_obj.LongStfObj.get_beam_string()
+                span = round(cyl_obj.ShellObj.dist_between_rings, 1)
+                tot_length = round(cyl_obj.ShellObj.length_of_shell, 1)
+                tot_cyl = round(cyl_obj.ShellObj.tot_cyl_length, 1)
+                sigma_axial = cyl_obj.sasd / 1e6
+                sigma_bend = cyl_obj.smsd / 1e6
+                sigma_tors = cyl_obj.tTsd / 1e6
+                tau_xy = cyl_obj.tQsd / 1e6
+                lat_press = cyl_obj.psd / 1e6
+                sigma_hoop = cyl_obj.shsd / 1e6
+                results = cyl_obj.get_utilization_factors()
+                data = [line, radius, thickness, span, tot_length,
+                        sigma_axial,
+                        sigma_bend,
+                        sigma_tors,
+                        tau_xy,
+                        lat_press,
+                        sigma_hoop,
+                        round(0 if results['Unstiffened shell'] is None else results['Unstiffened shell'],2),
+                        round(0 if results['Longitudinal stiffened shell'] is None else results['Longitudinal stiffened shell'],2),
+                        round(0 if results['Ring stiffened shell'] is None else results['Ring stiffened shell'],2),
+                        round(0 if results['Heavy ring frame'] is None else results['Heavy ring frame'],2)
+                        ]
+                table_all.append([str(data_item) for data_item in data])
+        if cylinders:
+            t = Table(table_all,colWidths=[0.7*inch])
+            t.setStyle(TableStyle([
+                ('GRID', (0, 0), (-1, -1), 0.5, colors.gray),
+                ('BACKGROUND', (0, 0), (-1, -1), colors.lightblue),
+                ('FONTSIZE', (0, 0), (-1, -1), 8),
+                ('FONTSIZE', (0, 4), (-1, 4), 8),
+                ('TEXTFONT', (0, 1), (-1, 1), 'Times-Bold'),
+                ('TEXTFONT', (0, 4), (-1, 4), 'Times-Bold'),
+            ]))
+        else:
+            t = Table(table_all,colWidths=[0.55*inch])
+            t.setStyle(TableStyle([
+                ('GRID', (0, 0), (-1, -1), 0.5, colors.gray),
+                ('BACKGROUND', (0, 0), (-1, -1), colors.lightblue),
+                ('FONTSIZE', (0, 0), (-1, -1), 8),
+                ('FONTSIZE', (0, 4), (-1, 4), 8),
+                ('TEXTFONT', (0, 1), (-1, 1), 'Times-Bold'),
+                ('TEXTFONT', (0, 4), (-1, 4), 'Times-Bold'),
+            ]))
 
         return [t,]
 
 
 if __name__ == '__main__':
     import multiprocessing, ctypes, tkinter
     import main_application as app
     multiprocessing.freeze_support()
     errorCode = ctypes.windll.shcore.SetProcessDpiAwareness(2)
     root = tkinter.Tk()
     my_app = app.Application(root)
     ship_example = r'C:\Github\ANYstructure\ship_section_example.txt'
     my_app.openfile(ship_example)
-    #my_app.table_generate()
-    my_app.report_generate(autosave=True)
+    #
+    my_app.table_generate()
+    #my_app.report_generate(autosave=True)
     # doc = LetterMaker("example.pdf", "The MVP", 10, to_report_gen)
     # doc.createDocument()
     # doc.savePDF()
```

### Comparing `ANYstructure-4.7/any_files/sections.csv` & `ANYstructure-4.8/any_files/sections.csv`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/sesam_interface.py` & `ANYstructure-4.8/any_files/sesam_interface.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/ship_section_example.txt` & `ANYstructure-4.8/any_files/ship_section_example.txt`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/stresses_window.py` & `ANYstructure-4.8/any_files/stresses_window.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/any_files/testCalc.py` & `ANYstructure-4.8/any_files/testCalc.py`

 * *Files identical despite different names*

### Comparing `ANYstructure-4.7/setup.py` & `ANYstructure-4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     with open('README.rst') as file:
         return file.read()
 
 setup(
     name='ANYstructure',  # Required
     url = 'https://github.com/audunarn/ANYstructure',
     entry_points={"console_scripts": ['ANYstructure = any_files.__main__:main']},
-    version='4.7',  # Required
+    version='4.8',  # Required
     license='MIT',
     description='A plate field optimization tool for offshore structures calculated according to DNV standards',
     long_description = readme(),
     author='Audun Arnesen Nyhus',  # Optional
     author_email='audunarn@gmail.com',  # Optional
     classifiers=[  # Optional
         'Development Status :: 5 - Production/Stable',
```

