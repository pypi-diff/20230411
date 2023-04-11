# Comparing `tmp/neer-0.0.7.tar.gz` & `tmp/neer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neer-0.0.7.tar", last modified: Mon Feb 27 01:29:00 2023, max compression
+gzip compressed data, was "neer-0.0.8.tar", last modified: Tue Apr 11 01:31:38 2023, max compression
```

## Comparing `neer-0.0.7.tar` & `neer-0.0.8.tar`

### file list

```diff
@@ -1,309 +1,314 @@
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:29:00.139964 neer-0.0.7/
--rw-r--r--   0 spectralartist   (501) staff       (20)      429 2023-02-27 01:29:00.139702 neer-0.0.7/PKG-INFO
--rw-r--r--   0 spectralartist   (501) staff       (20)       96 2023-02-10 13:28:08.000000 neer-0.0.7/README.md
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.960512 neer-0.0.7/neer/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-15 06:19:11.000000 neer-0.0.7/neer/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      126 2023-02-10 23:35:30.000000 neer-0.0.7/neer/base.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.963898 neer-0.0.7/neer/predictions/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-10 13:51:35.000000 neer-0.0.7/neer/predictions/__init__.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.995028 neer-0.0.7/neer/predictions/predictions/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:57.000000 neer-0.0.7/neer/predictions/predictions/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1667 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/event_analysis_results.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      764 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_link_bre.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1355 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_link_cof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1149 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_link_lof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1364 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_1d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_1h.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1746 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_30d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_5m.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1450 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_1d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_1h.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1824 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_30d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_5m.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      764 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_node_bre.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1355 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_node_cof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1388 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_node_lof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1413 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_1d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_1h.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1905 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_30d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_5m.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1308 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_1d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_1h.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1466 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_30d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_5m.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1484 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_1d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_1h.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2220 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_30d.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_5m.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1143 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_conduit_surcharge_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1413 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_flow_classification_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1180 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_link_dw_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1187 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_link_flow_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1211 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_node_depth_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1342 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_node_dw_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1171 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_node_flooding_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1296 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_node_inflow_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1053 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_node_surcharge_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1048 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_outfall_loading_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1344 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_pumping_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1403 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_storage_volume_summaries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1415 2023-02-15 06:39:33.000000 neer-0.0.7/neer/predictions/predictions/spark_rpt_subcatchment_runoff_summaries.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.995400 neer-0.0.7/neer/primary/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-10 13:51:28.000000 neer-0.0.7/neer/primary/__init__.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.995804 neer-0.0.7/neer/primary/cswr/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:49.000000 neer-0.0.7/neer/primary/cswr/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      832 2023-02-27 01:16:39.000000 neer-0.0.7/neer/primary/cswr/features.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:29:00.131163 neer-0.0.7/neer/primary/public/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:43.000000 neer-0.0.7/neer/primary/public/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      779 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/announcements.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      856 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/api_jobs.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1006 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/api_tokens.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      908 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/auto_simulation_schedule.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      978 2023-02-27 01:19:18.000000 neer-0.0.7/neer/primary/public/auto_snapshot_schedule.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      961 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/back_testing_schedule.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      749 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/billed_water_usage.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      942 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/calibration_data.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      800 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/calibration_data_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      745 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/client_teams.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      713 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/client_users.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      842 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/clients.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      548 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/cof_cost.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      622 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/cof_cost_items.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      772 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/cof_model_predictions.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      839 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/cof_models.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1244 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/customer_survey_form.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      715 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/datum_adjustments.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      828 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/discount_requests.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      664 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/draw_layer.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      746 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/failed_jobs.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      728 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/feature_stations.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      740 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/fileuploads.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      607 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/general_us_crit_ratings.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      695 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/geometries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1388 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_adjust.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1274 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_aquifer.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      670 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_backdrop.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12366 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_bridge_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      938 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_buildup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      886 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_calibration_files.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1755 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_conduit.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      602 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_control.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      545 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_control_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11539 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_control_valve_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      893 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_coordinate.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      721 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_coverage.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12368 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_culvert_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    10858 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_curb_stop_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      789 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_curve.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      816 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_curve_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12360 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_dam_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      746 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_demand_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     9551 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_detention_basin_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1358 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_divider.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      919 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_dwf.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12385 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_enclosed_gravity_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11535 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_end_section_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_energy_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12389 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_engineered_channel_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1330 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_evaporation.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_event.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      733 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_file.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_fire_hydrant_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12373 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_force_main_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12377 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_gravity_main_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     9561 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_green_infrastructure_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1286 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_groundwater.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_gwf.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      668 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_hydrograph.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1163 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_hydrograph_values.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      893 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_infiltration.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      990 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_inflow.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_inlet_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2024 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_junction.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_junction_box_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1392 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_junction_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      728 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_label.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      792 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_landuse.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12055 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lateral_inventory_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12364 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_levee_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      658 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lid_control.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      750 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lid_control_subvalues.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      650 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lid_control_values.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1209 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lid_usage.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11598 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_lift_station_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    10290 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_link_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      723 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_loading.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      871 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_losses.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_manhole_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      660 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_map.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_meter_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12383 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_natural_channel_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     9530 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_node_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      666 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_option.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_option_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1188 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_orifice.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1169 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_outfall.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_outfall_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1259 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_outlet.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11545 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_outlet_structure_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      705 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pattern.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      596 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pattern_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      890 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pattern_multipliers.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pattern_multipliers_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1383 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pipe_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1151 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pollutant.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      895 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_polygon.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      655 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_profile.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1140 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pump.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    10475 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pump_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1439 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pump_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11598 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_pump_station_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      663 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_quality_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1219 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_raingage.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      709 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_rdii.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      665 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_reaction_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      666 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_report.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     9540 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_reservoir_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1219 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_reservoir_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      536 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_rule_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12928 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_service_lateral_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11543 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_simple_junction_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      601 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_snowpack.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1146 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_snowpack_values.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      762 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_source_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_status_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1583 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_storage.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_storage_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11539 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_storage_basin_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_storage_tank_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11562 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_stormwater_treatment_unit_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      999 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_subarea.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1198 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_subcatchment.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      831 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_symbol.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      708 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_tag.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1664 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_tank_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1007 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temp.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      820 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature_adcimpervious.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      816 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature_adcpervious.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      810 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature_snowmelt.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      765 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature_timeseries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      836 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_temperature_windspeed_monthly.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      657 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_time_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      660 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_timeseries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      767 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_timeseries_values.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      599 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_title.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      603 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_transect.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      788 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_transects_gr.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_transects_nc.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1221 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_transects_x1.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      711 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_treatment.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_valve_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1325 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_valve_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      889 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_vertices.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      942 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_washoff.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    10952 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_wastewater_treatment_plant_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    12489 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_water_main_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)    10942 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_water_treatment_plant_am.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1486 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_weir.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      977 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/inp_xsection.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/invitations.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1111 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/invoices.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      813 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/jobs.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      707 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/land_use_code_scores.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      779 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/layer_files.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      732 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/layers.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1072 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/leak_detection_program.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2020 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/likely_leak_locations.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1556 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/lof_models.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      797 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/maps.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/material_service_life.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      555 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/migrations.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1034 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/ml_models_groups.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      701 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/ml_models_groups_items.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      553 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/ml_models_names.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      826 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/ml_models_predictions.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      588 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/months.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      722 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/my_layer_files.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      729 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/my_layers.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      770 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/my_layers_features.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1135 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/noaa_frequency_tables.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      752 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/non_revenue_water.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1137 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/non_revenue_water_loss.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      960 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/notifications.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      771 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/outfall_replacement_cost_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      682 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/password_resets.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      879 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/performance_indicators.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      963 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/pipe_cost_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      763 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/pred_lof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      844 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/processed_cof.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      890 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/processed_cof_buffer.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1094 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/processed_cof_facility_distance.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      774 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/processed_cof_transportation_rating.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      658 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/project_settings.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      526 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/projection_list.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     3741 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/projects.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/projects_models.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      623 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/projects_old.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1616 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/rainfall_analysis.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1167 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/rainfall_analysis_gauge_results.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      590 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/rainfall_analysis_gauges.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      568 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/rating_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      970 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/rcb_pipe_cost_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      530 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/roles.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      537 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/roles_old.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      712 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/simulation_schedule.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     4937 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/simulations.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      653 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/spatial_ref_sys.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      753 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/structure_replacement_unit_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      832 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/structure_unit_cost_lookup.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1062 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/subscriptions.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      721 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/team_api_keys.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      551 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/team_models.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1071 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/team_subscriptions.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      678 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/team_users.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1729 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/teams.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      510 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/test.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      731 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/testingspatial.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      797 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/typeorm_metadata.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      678 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/us_counties.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1156 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/us_states.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      733 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/user_project_mapping.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      597 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/user_project_mapping_old.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2514 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/users.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1250 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/utility_inspection_form.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      870 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/public/water_balance.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:29:00.132123 neer-0.0.7/neer/primary/topology/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:02.000000 neer-0.0.7/neer/primary/topology/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      892 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/topology/layer.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.7/neer/primary/topology/topology.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:29:00.132491 neer-0.0.7/neer/timescale/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:14:12.000000 neer-0.0.7/neer/timescale/__init__.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:29:00.139273 neer-0.0.7/neer/timescale/timeseries/
--rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:14:26.000000 neer-0.0.7/neer/timescale/timeseries/__init__.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      925 2023-02-27 01:15:19.000000 neer-0.0.7/neer/timescale/timeseries/calibration_data.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      930 2023-02-27 01:15:19.000000 neer-0.0.7/neer/timescale/timeseries/calibration_data_dw.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     2604 2023-02-27 01:23:56.000000 neer-0.0.7/neer/timescale/timeseries/forecasts.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1344 2023-02-27 01:23:48.000000 neer-0.0.7/neer/timescale/timeseries/historical_weather.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      783 2023-02-27 01:15:18.000000 neer-0.0.7/neer/timescale/timeseries/inp_timeseries.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      807 2023-02-27 01:15:16.000000 neer-0.0.7/neer/timescale/timeseries/inp_timeseries_back_testing.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      886 2023-02-27 01:15:18.000000 neer-0.0.7/neer/timescale/timeseries/inp_timeseries_values.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      910 2023-02-27 01:15:16.000000 neer-0.0.7/neer/timescale/timeseries/inp_timeseries_values_back_testing.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      810 2023-02-27 01:15:17.000000 neer-0.0.7/neer/timescale/timeseries/site_sensor_measurements.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1458 2023-02-27 01:25:31.000000 neer-0.0.7/neer/timescale/timeseries/site_sensors.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      965 2023-02-27 01:26:07.000000 neer-0.0.7/neer/timescale/timeseries/sites.py
--rw-r--r--   0 spectralartist   (501) staff       (20)      980 2023-02-27 01:15:15.000000 neer-0.0.7/neer/timescale/timeseries/timeseries_file_data.py
--rw-r--r--   0 spectralartist   (501) staff       (20)     1004 2023-02-27 01:15:17.000000 neer-0.0.7/neer/timescale/timeseries/timeseries_file_data_back_testing.py
-drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:28:59.963376 neer-0.0.7/neer.egg-info/
--rw-r--r--   0 spectralartist   (501) staff       (20)      429 2023-02-27 01:28:59.000000 neer-0.0.7/neer.egg-info/PKG-INFO
--rw-r--r--   0 spectralartist   (501) staff       (20)    12365 2023-02-27 01:28:59.000000 neer-0.0.7/neer.egg-info/SOURCES.txt
--rw-r--r--   0 spectralartist   (501) staff       (20)        1 2023-02-27 01:28:59.000000 neer-0.0.7/neer.egg-info/dependency_links.txt
--rw-r--r--   0 spectralartist   (501) staff       (20)       55 2023-02-27 01:28:59.000000 neer-0.0.7/neer.egg-info/requires.txt
--rw-r--r--   0 spectralartist   (501) staff       (20)        5 2023-02-27 01:28:59.000000 neer-0.0.7/neer.egg-info/top_level.txt
--rw-r--r--   0 spectralartist   (501) staff       (20)      533 2023-02-27 01:28:30.000000 neer-0.0.7/pyproject.toml
--rw-r--r--   0 spectralartist   (501) staff       (20)       38 2023-02-27 01:29:00.140038 neer-0.0.7/setup.cfg
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:38.200935 neer-0.0.8/
+-rw-r--r--   0 spectralartist   (501) staff       (20)      429 2023-04-11 01:31:38.200437 neer-0.0.8/PKG-INFO
+-rw-r--r--   0 spectralartist   (501) staff       (20)       96 2023-02-10 13:28:08.000000 neer-0.0.8/README.md
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.934639 neer-0.0.8/neer/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-15 06:19:11.000000 neer-0.0.8/neer/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      126 2023-02-10 23:35:30.000000 neer-0.0.8/neer/base.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.938469 neer-0.0.8/neer/predictions/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-10 13:51:35.000000 neer-0.0.8/neer/predictions/__init__.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.974926 neer-0.0.8/neer/predictions/predictions/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:57.000000 neer-0.0.8/neer/predictions/predictions/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1667 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/event_analysis_results.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      764 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_link_bre.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1355 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_link_cof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1149 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_link_lof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1364 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_1d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_1h.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1746 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_30d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1744 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_5m.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1450 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_1d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_1h.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1824 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_30d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1822 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_5m.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      764 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_node_bre.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1355 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_node_cof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1388 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_node_lof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1413 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_1d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_1h.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1905 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_30d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1903 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_5m.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1308 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_1d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_1h.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1466 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_30d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1464 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_5m.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1484 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_1d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_1h.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2220 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_30d.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2218 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_5m.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1143 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_conduit_surcharge_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1413 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_flow_classification_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1180 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_link_dw_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1187 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_link_flow_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1211 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_node_depth_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1342 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_node_dw_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1171 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_node_flooding_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1296 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_node_inflow_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1053 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_node_surcharge_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1048 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_outfall_loading_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1344 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_pumping_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1403 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_storage_volume_summaries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1415 2023-02-15 06:39:33.000000 neer-0.0.8/neer/predictions/predictions/spark_rpt_subcatchment_runoff_summaries.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.975411 neer-0.0.8/neer/primary/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-10 13:51:28.000000 neer-0.0.8/neer/primary/__init__.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.975731 neer-0.0.8/neer/primary/aqueduct/
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1251 2023-04-11 01:29:35.000000 neer-0.0.8/neer/primary/aqueduct/arcgis_features.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.977594 neer-0.0.8/neer/primary/cswr/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:49.000000 neer-0.0.8/neer/primary/cswr/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      832 2023-02-27 01:16:39.000000 neer-0.0.8/neer/primary/cswr/features.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:38.184811 neer-0.0.8/neer/primary/public/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:43.000000 neer-0.0.8/neer/primary/public/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      779 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/announcements.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      856 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/api_jobs.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1006 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/api_tokens.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      908 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/auto_simulation_schedule.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      978 2023-02-27 01:19:18.000000 neer-0.0.8/neer/primary/public/auto_snapshot_schedule.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      961 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/back_testing_schedule.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      749 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/billed_water_usage.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      942 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/calibration_data.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      800 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/calibration_data_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      745 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/client_teams.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      713 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/client_users.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      842 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/clients.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      548 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/cof_cost.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      622 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/cof_cost_items.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      772 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/cof_model_predictions.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      839 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/cof_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1244 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/customer_survey_form.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      715 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/datum_adjustments.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      828 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/discount_requests.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      664 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/draw_layer.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      746 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/failed_jobs.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      728 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/feature_stations.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      740 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/fileuploads.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      607 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/general_us_crit_ratings.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      695 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/geometries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1388 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_adjust.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1274 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_aquifer.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      670 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_backdrop.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12366 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_bridge_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      938 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_buildup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      886 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_calibration_files.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1755 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_conduit.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      602 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_control.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      545 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_control_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11539 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_control_valve_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      893 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_coordinate.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      721 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_coverage.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12368 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_culvert_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    10858 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_curb_stop_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      789 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_curve.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      816 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_curve_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12360 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_dam_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      746 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_demand_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     9551 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_detention_basin_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1358 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_divider.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      919 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_dwf.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12385 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_enclosed_gravity_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11535 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_end_section_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_energy_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12389 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_engineered_channel_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1330 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_evaporation.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_event.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      733 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_file.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_fire_hydrant_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12373 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_force_main_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12377 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_gravity_main_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     9561 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_green_infrastructure_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1286 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_groundwater.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_gwf.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      668 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_hydrograph.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1163 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_hydrograph_values.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      893 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_infiltration.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      990 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_inflow.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_inlet_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2024 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_junction.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_junction_box_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1392 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_junction_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      728 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_label.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      792 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_landuse.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12055 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lateral_inventory_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12364 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_levee_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      658 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lid_control.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      750 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lid_control_subvalues.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      650 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lid_control_values.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1209 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lid_usage.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11598 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_lift_station_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    10290 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_link_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      723 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_loading.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      871 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_losses.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_manhole_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      660 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_map.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_meter_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12383 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_natural_channel_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     9530 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_node_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      666 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_option.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_option_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1188 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_orifice.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1169 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_outfall.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_outfall_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1259 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_outlet.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11545 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_outlet_structure_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      705 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pattern.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      596 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pattern_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      890 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pattern_multipliers.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pattern_multipliers_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1383 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pipe_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1151 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pollutant.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      895 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_polygon.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      655 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_profile.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1140 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pump.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    10475 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pump_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1439 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pump_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11598 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_pump_station_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      663 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_quality_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1219 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_raingage.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      709 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_rdii.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      665 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_reaction_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      666 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_report.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     9540 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_reservoir_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1219 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_reservoir_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      536 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_rule_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12928 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_service_lateral_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11543 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_simple_junction_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      601 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_snowpack.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1146 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_snowpack_values.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      762 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_source_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      661 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_status_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1583 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_storage.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11528 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_storage_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11539 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_storage_basin_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11537 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_storage_tank_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11562 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_stormwater_treatment_unit_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      999 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_subarea.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1198 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_subcatchment.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      831 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_symbol.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      708 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_tag.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1664 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_tank_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1007 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temp.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      820 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature_adcimpervious.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      816 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature_adcpervious.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      810 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature_snowmelt.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      765 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature_timeseries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      836 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_temperature_windspeed_monthly.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      657 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_time_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      660 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_timeseries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      767 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_timeseries_values.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      599 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_title.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      603 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_transect.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      788 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_transects_gr.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_transects_nc.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1221 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_transects_x1.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      711 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_treatment.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    11524 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_valve_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1325 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_valve_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      889 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_vertices.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      942 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_washoff.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    10952 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_wastewater_treatment_plant_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12489 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_water_main_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)    10942 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_water_treatment_plant_am.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1486 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_weir.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      977 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/inp_xsection.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      846 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/invitations.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1111 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/invoices.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      813 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/jobs.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      707 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/land_use_code_scores.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      779 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/layer_files.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      732 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/layers.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1072 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/leak_detection_program.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2020 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/likely_leak_locations.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      650 2023-04-11 01:17:46.000000 neer-0.0.8/neer/primary/public/lof_model_teams.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1556 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/lof_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      797 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/maps.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      725 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/material_service_life.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      555 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/migrations.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1034 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/ml_models_groups.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      701 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/ml_models_groups_items.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      553 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/ml_models_names.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      826 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/ml_models_predictions.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      588 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/months.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      722 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/my_layer_files.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      729 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/my_layers.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      770 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/my_layers_features.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      701 2023-04-11 01:08:47.000000 neer-0.0.8/neer/primary/public/new_lof_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      751 2023-04-11 01:11:12.000000 neer-0.0.8/neer/primary/public/new_ml_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1135 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/noaa_frequency_tables.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      752 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/non_revenue_water.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1137 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/non_revenue_water_loss.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      960 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/notifications.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      771 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/outfall_replacement_cost_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      682 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/password_resets.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      879 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/performance_indicators.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      963 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/pipe_cost_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      763 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/pred_lof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      844 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/processed_cof.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      890 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/processed_cof_buffer.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1094 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/processed_cof_facility_distance.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      774 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/processed_cof_transportation_rating.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      658 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/project_settings.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      526 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/projection_list.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     3741 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/projects.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/projects_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      623 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/projects_old.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1616 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/rainfall_analysis.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1167 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/rainfall_analysis_gauge_results.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      590 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/rainfall_analysis_gauges.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      568 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/rating_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      970 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/rcb_pipe_cost_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      530 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/roles.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      537 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/roles_old.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      712 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/simulation_schedule.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     4937 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/simulations.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      653 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/spatial_ref_sys.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      753 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/structure_replacement_unit_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      832 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/structure_unit_cost_lookup.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1062 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/subscriptions.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      721 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/team_api_keys.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      551 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/team_models.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1071 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/team_subscriptions.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      678 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/team_users.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1729 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/teams.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      510 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/test.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      731 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/testingspatial.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      797 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/typeorm_metadata.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      678 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/us_counties.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1156 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/us_states.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      733 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/user_project_mapping.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      597 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/user_project_mapping_old.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2514 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/users.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1250 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/utility_inspection_form.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      870 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/public/water_balance.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:38.187393 neer-0.0.8/neer/primary/topology/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-14 14:17:02.000000 neer-0.0.8/neer/primary/topology/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      892 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/topology/layer.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      684 2023-02-15 06:39:33.000000 neer-0.0.8/neer/primary/topology/topology.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:38.188164 neer-0.0.8/neer/timescale/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:14:12.000000 neer-0.0.8/neer/timescale/__init__.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:38.199006 neer-0.0.8/neer/timescale/timeseries/
+-rw-r--r--   0 spectralartist   (501) staff       (20)        0 2023-02-27 01:14:26.000000 neer-0.0.8/neer/timescale/timeseries/__init__.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      925 2023-02-27 01:15:19.000000 neer-0.0.8/neer/timescale/timeseries/calibration_data.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      930 2023-02-27 01:15:19.000000 neer-0.0.8/neer/timescale/timeseries/calibration_data_dw.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     2604 2023-02-27 01:23:56.000000 neer-0.0.8/neer/timescale/timeseries/forecasts.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1344 2023-02-27 01:23:48.000000 neer-0.0.8/neer/timescale/timeseries/historical_weather.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      783 2023-02-27 01:15:18.000000 neer-0.0.8/neer/timescale/timeseries/inp_timeseries.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      807 2023-02-27 01:15:16.000000 neer-0.0.8/neer/timescale/timeseries/inp_timeseries_back_testing.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      886 2023-02-27 01:15:18.000000 neer-0.0.8/neer/timescale/timeseries/inp_timeseries_values.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      910 2023-02-27 01:15:16.000000 neer-0.0.8/neer/timescale/timeseries/inp_timeseries_values_back_testing.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      810 2023-02-27 01:15:17.000000 neer-0.0.8/neer/timescale/timeseries/site_sensor_measurements.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1458 2023-02-27 01:25:31.000000 neer-0.0.8/neer/timescale/timeseries/site_sensors.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      965 2023-02-27 01:26:07.000000 neer-0.0.8/neer/timescale/timeseries/sites.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)      980 2023-02-27 01:15:15.000000 neer-0.0.8/neer/timescale/timeseries/timeseries_file_data.py
+-rw-r--r--   0 spectralartist   (501) staff       (20)     1004 2023-02-27 01:15:17.000000 neer-0.0.8/neer/timescale/timeseries/timeseries_file_data_back_testing.py
+drwxr-xr-x   0 spectralartist   (501) staff       (20)        0 2023-04-11 01:31:37.937922 neer-0.0.8/neer.egg-info/
+-rw-r--r--   0 spectralartist   (501) staff       (20)      429 2023-04-11 01:31:37.000000 neer-0.0.8/neer.egg-info/PKG-INFO
+-rw-r--r--   0 spectralartist   (501) staff       (20)    12520 2023-04-11 01:31:37.000000 neer-0.0.8/neer.egg-info/SOURCES.txt
+-rw-r--r--   0 spectralartist   (501) staff       (20)        1 2023-04-11 01:31:37.000000 neer-0.0.8/neer.egg-info/dependency_links.txt
+-rw-r--r--   0 spectralartist   (501) staff       (20)       55 2023-04-11 01:31:37.000000 neer-0.0.8/neer.egg-info/requires.txt
+-rw-r--r--   0 spectralartist   (501) staff       (20)        5 2023-04-11 01:31:37.000000 neer-0.0.8/neer.egg-info/top_level.txt
+-rw-r--r--   0 spectralartist   (501) staff       (20)      533 2023-04-11 01:31:13.000000 neer-0.0.8/pyproject.toml
+-rw-r--r--   0 spectralartist   (501) staff       (20)       38 2023-04-11 01:31:38.201057 neer-0.0.8/setup.cfg
```

### Comparing `neer-0.0.7/neer/predictions/predictions/event_analysis_results.py` & `neer-0.0.8/neer/predictions/predictions/event_analysis_results.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_link_bre.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_link_bre.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_link_cof.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_link_cof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_link_lof.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_link_lof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_1d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_1d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_1h.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_1h.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_30d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_30d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_5m.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_5m.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_dw.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_1d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_1d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_1h.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_1h.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_30d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_30d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_links_dw_5m.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_links_dw_5m.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_node_bre.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_node_bre.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_node_cof.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_node_cof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_node_lof.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_node_lof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_1d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_1d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_1h.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_1h.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_30d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_30d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_5m.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_5m.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_1d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_1d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_1h.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_1h.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_30d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_30d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_nodes_dw_5m.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_nodes_dw_5m.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_1d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_1d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_1h.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_1h.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_30d.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_30d.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_report_subcatchments_5m.py` & `neer-0.0.8/neer/predictions/predictions/spark_report_subcatchments_5m.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_conduit_surcharge_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_conduit_surcharge_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_flow_classification_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_flow_classification_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_link_dw_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_link_dw_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_link_flow_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_link_flow_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_node_depth_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_node_depth_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_node_dw_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_node_dw_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_node_flooding_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_node_flooding_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_node_inflow_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_node_inflow_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_node_surcharge_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_node_surcharge_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_outfall_loading_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_outfall_loading_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_pumping_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_pumping_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_storage_volume_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_storage_volume_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/predictions/predictions/spark_rpt_subcatchment_runoff_summaries.py` & `neer-0.0.8/neer/predictions/predictions/spark_rpt_subcatchment_runoff_summaries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/cswr/features.py` & `neer-0.0.8/neer/primary/cswr/features.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/announcements.py` & `neer-0.0.8/neer/primary/public/announcements.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/api_jobs.py` & `neer-0.0.8/neer/primary/public/api_jobs.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/api_tokens.py` & `neer-0.0.8/neer/primary/public/api_tokens.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/auto_simulation_schedule.py` & `neer-0.0.8/neer/primary/public/auto_simulation_schedule.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/auto_snapshot_schedule.py` & `neer-0.0.8/neer/primary/public/auto_snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/back_testing_schedule.py` & `neer-0.0.8/neer/primary/public/back_testing_schedule.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/billed_water_usage.py` & `neer-0.0.8/neer/primary/public/billed_water_usage.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/calibration_data.py` & `neer-0.0.8/neer/primary/public/calibration_data.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/calibration_data_dw.py` & `neer-0.0.8/neer/primary/public/calibration_data_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/client_teams.py` & `neer-0.0.8/neer/primary/public/client_teams.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/client_users.py` & `neer-0.0.8/neer/primary/public/client_users.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/clients.py` & `neer-0.0.8/neer/primary/public/clients.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/cof_cost.py` & `neer-0.0.8/neer/primary/public/cof_cost.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/cof_cost_items.py` & `neer-0.0.8/neer/primary/public/cof_cost_items.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/cof_model_predictions.py` & `neer-0.0.8/neer/primary/public/cof_model_predictions.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/cof_models.py` & `neer-0.0.8/neer/primary/public/cof_models.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/customer_survey_form.py` & `neer-0.0.8/neer/primary/public/customer_survey_form.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/datum_adjustments.py` & `neer-0.0.8/neer/primary/public/datum_adjustments.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/discount_requests.py` & `neer-0.0.8/neer/primary/public/discount_requests.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/draw_layer.py` & `neer-0.0.8/neer/primary/public/draw_layer.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/failed_jobs.py` & `neer-0.0.8/neer/primary/public/failed_jobs.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/feature_stations.py` & `neer-0.0.8/neer/primary/public/feature_stations.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/fileuploads.py` & `neer-0.0.8/neer/primary/public/fileuploads.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/general_us_crit_ratings.py` & `neer-0.0.8/neer/primary/public/general_us_crit_ratings.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/geometries.py` & `neer-0.0.8/neer/primary/public/geometries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_adjust.py` & `neer-0.0.8/neer/primary/public/inp_adjust.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_aquifer.py` & `neer-0.0.8/neer/primary/public/inp_aquifer.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_backdrop.py` & `neer-0.0.8/neer/primary/public/inp_backdrop.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_bridge_am.py` & `neer-0.0.8/neer/primary/public/inp_bridge_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_buildup.py` & `neer-0.0.8/neer/primary/public/inp_buildup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_calibration_files.py` & `neer-0.0.8/neer/primary/public/inp_calibration_files.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_conduit.py` & `neer-0.0.8/neer/primary/public/inp_conduit.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_control.py` & `neer-0.0.8/neer/primary/public/inp_control.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_control_dw.py` & `neer-0.0.8/neer/primary/public/inp_control_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_control_valve_am.py` & `neer-0.0.8/neer/primary/public/inp_control_valve_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_coordinate.py` & `neer-0.0.8/neer/primary/public/inp_coordinate.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_coverage.py` & `neer-0.0.8/neer/primary/public/inp_coverage.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_culvert_am.py` & `neer-0.0.8/neer/primary/public/inp_culvert_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_curb_stop_am.py` & `neer-0.0.8/neer/primary/public/inp_curb_stop_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_curve.py` & `neer-0.0.8/neer/primary/public/inp_curve.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_curve_dw.py` & `neer-0.0.8/neer/primary/public/inp_curve_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_dam_am.py` & `neer-0.0.8/neer/primary/public/inp_dam_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_demand_dw.py` & `neer-0.0.8/neer/primary/public/inp_demand_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_detention_basin_am.py` & `neer-0.0.8/neer/primary/public/inp_detention_basin_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_divider.py` & `neer-0.0.8/neer/primary/public/inp_divider.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_dwf.py` & `neer-0.0.8/neer/primary/public/inp_dwf.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_enclosed_gravity_am.py` & `neer-0.0.8/neer/primary/public/inp_enclosed_gravity_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_end_section_am.py` & `neer-0.0.8/neer/primary/public/inp_end_section_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_energy_dw.py` & `neer-0.0.8/neer/primary/public/inp_energy_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_engineered_channel_am.py` & `neer-0.0.8/neer/primary/public/inp_engineered_channel_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_evaporation.py` & `neer-0.0.8/neer/primary/public/inp_evaporation.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_event.py` & `neer-0.0.8/neer/primary/public/inp_event.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_file.py` & `neer-0.0.8/neer/primary/public/inp_file.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_fire_hydrant_am.py` & `neer-0.0.8/neer/primary/public/inp_fire_hydrant_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_force_main_am.py` & `neer-0.0.8/neer/primary/public/inp_force_main_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_gravity_main_am.py` & `neer-0.0.8/neer/primary/public/inp_gravity_main_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_green_infrastructure_am.py` & `neer-0.0.8/neer/primary/public/inp_green_infrastructure_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_groundwater.py` & `neer-0.0.8/neer/primary/public/inp_groundwater.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_gwf.py` & `neer-0.0.8/neer/primary/public/inp_gwf.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_hydrograph.py` & `neer-0.0.8/neer/primary/public/inp_hydrograph.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_hydrograph_values.py` & `neer-0.0.8/neer/primary/public/inp_hydrograph_values.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_infiltration.py` & `neer-0.0.8/neer/primary/public/inp_infiltration.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_inflow.py` & `neer-0.0.8/neer/primary/public/inp_inflow.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_inlet_am.py` & `neer-0.0.8/neer/primary/public/inp_inlet_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_junction.py` & `neer-0.0.8/neer/primary/public/inp_junction.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_junction_box_am.py` & `neer-0.0.8/neer/primary/public/inp_junction_box_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_junction_dw.py` & `neer-0.0.8/neer/primary/public/inp_junction_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_label.py` & `neer-0.0.8/neer/primary/public/inp_label.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_landuse.py` & `neer-0.0.8/neer/primary/public/inp_landuse.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lateral_inventory_am.py` & `neer-0.0.8/neer/primary/public/inp_lateral_inventory_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_levee_am.py` & `neer-0.0.8/neer/primary/public/inp_levee_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lid_control.py` & `neer-0.0.8/neer/primary/public/inp_lid_control.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lid_control_subvalues.py` & `neer-0.0.8/neer/primary/public/inp_lid_control_subvalues.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lid_control_values.py` & `neer-0.0.8/neer/primary/public/inp_lid_control_values.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lid_usage.py` & `neer-0.0.8/neer/primary/public/inp_lid_usage.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_lift_station_am.py` & `neer-0.0.8/neer/primary/public/inp_lift_station_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_link_am.py` & `neer-0.0.8/neer/primary/public/inp_link_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_loading.py` & `neer-0.0.8/neer/primary/public/inp_loading.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_losses.py` & `neer-0.0.8/neer/primary/public/inp_losses.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_manhole_am.py` & `neer-0.0.8/neer/primary/public/inp_manhole_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_map.py` & `neer-0.0.8/neer/primary/public/inp_map.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_meter_am.py` & `neer-0.0.8/neer/primary/public/inp_meter_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_natural_channel_am.py` & `neer-0.0.8/neer/primary/public/inp_natural_channel_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_node_am.py` & `neer-0.0.8/neer/primary/public/inp_node_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_option.py` & `neer-0.0.8/neer/primary/public/inp_option.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_option_dw.py` & `neer-0.0.8/neer/primary/public/inp_option_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_orifice.py` & `neer-0.0.8/neer/primary/public/inp_orifice.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_outfall.py` & `neer-0.0.8/neer/primary/public/inp_outfall.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_outfall_am.py` & `neer-0.0.8/neer/primary/public/inp_outfall_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_outlet.py` & `neer-0.0.8/neer/primary/public/inp_outlet.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_outlet_structure_am.py` & `neer-0.0.8/neer/primary/public/inp_outlet_structure_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pattern.py` & `neer-0.0.8/neer/primary/public/inp_pattern.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pattern_dw.py` & `neer-0.0.8/neer/primary/public/inp_pattern_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pattern_multipliers.py` & `neer-0.0.8/neer/primary/public/inp_pattern_multipliers.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pattern_multipliers_dw.py` & `neer-0.0.8/neer/primary/public/inp_pattern_multipliers_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pipe_dw.py` & `neer-0.0.8/neer/primary/public/inp_pipe_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pollutant.py` & `neer-0.0.8/neer/primary/public/inp_pollutant.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_polygon.py` & `neer-0.0.8/neer/primary/public/inp_polygon.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_profile.py` & `neer-0.0.8/neer/primary/public/inp_profile.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pump.py` & `neer-0.0.8/neer/primary/public/inp_pump.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pump_am.py` & `neer-0.0.8/neer/primary/public/inp_pump_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pump_dw.py` & `neer-0.0.8/neer/primary/public/inp_pump_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_pump_station_am.py` & `neer-0.0.8/neer/primary/public/inp_pump_station_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_quality_dw.py` & `neer-0.0.8/neer/primary/public/inp_quality_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_raingage.py` & `neer-0.0.8/neer/primary/public/inp_raingage.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_rdii.py` & `neer-0.0.8/neer/primary/public/inp_rdii.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_reaction_dw.py` & `neer-0.0.8/neer/primary/public/inp_reaction_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_report.py` & `neer-0.0.8/neer/primary/public/inp_report.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_reservoir_am.py` & `neer-0.0.8/neer/primary/public/inp_reservoir_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_reservoir_dw.py` & `neer-0.0.8/neer/primary/public/inp_reservoir_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_rule_dw.py` & `neer-0.0.8/neer/primary/public/inp_rule_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_service_lateral_am.py` & `neer-0.0.8/neer/primary/public/inp_service_lateral_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_simple_junction_am.py` & `neer-0.0.8/neer/primary/public/inp_simple_junction_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_snowpack.py` & `neer-0.0.8/neer/primary/public/inp_snowpack.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_snowpack_values.py` & `neer-0.0.8/neer/primary/public/inp_snowpack_values.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_source_dw.py` & `neer-0.0.8/neer/primary/public/inp_source_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_status_dw.py` & `neer-0.0.8/neer/primary/public/inp_status_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_storage.py` & `neer-0.0.8/neer/primary/public/inp_storage.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_storage_am.py` & `neer-0.0.8/neer/primary/public/inp_storage_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_storage_basin_am.py` & `neer-0.0.8/neer/primary/public/inp_storage_basin_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_storage_tank_am.py` & `neer-0.0.8/neer/primary/public/inp_storage_tank_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_stormwater_treatment_unit_am.py` & `neer-0.0.8/neer/primary/public/inp_stormwater_treatment_unit_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_subarea.py` & `neer-0.0.8/neer/primary/public/inp_subarea.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_subcatchment.py` & `neer-0.0.8/neer/primary/public/inp_subcatchment.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_symbol.py` & `neer-0.0.8/neer/primary/public/inp_symbol.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_tag.py` & `neer-0.0.8/neer/primary/public/inp_tag.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_tank_dw.py` & `neer-0.0.8/neer/primary/public/inp_tank_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temp.py` & `neer-0.0.8/neer/primary/public/inp_temp.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature.py` & `neer-0.0.8/neer/primary/public/inp_temperature.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature_adcimpervious.py` & `neer-0.0.8/neer/primary/public/inp_temperature_adcimpervious.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature_adcpervious.py` & `neer-0.0.8/neer/primary/public/inp_temperature_adcpervious.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature_snowmelt.py` & `neer-0.0.8/neer/primary/public/inp_temperature_snowmelt.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature_timeseries.py` & `neer-0.0.8/neer/primary/public/inp_temperature_timeseries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_temperature_windspeed_monthly.py` & `neer-0.0.8/neer/primary/public/inp_temperature_windspeed_monthly.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_time_dw.py` & `neer-0.0.8/neer/primary/public/inp_time_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_timeseries.py` & `neer-0.0.8/neer/primary/public/inp_timeseries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_timeseries_values.py` & `neer-0.0.8/neer/primary/public/inp_timeseries_values.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_title.py` & `neer-0.0.8/neer/primary/public/inp_title.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_transect.py` & `neer-0.0.8/neer/primary/public/inp_transect.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_transects_gr.py` & `neer-0.0.8/neer/primary/public/inp_transects_gr.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_transects_nc.py` & `neer-0.0.8/neer/primary/public/inp_transects_nc.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_transects_x1.py` & `neer-0.0.8/neer/primary/public/inp_transects_x1.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_treatment.py` & `neer-0.0.8/neer/primary/public/inp_treatment.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_valve_am.py` & `neer-0.0.8/neer/primary/public/inp_valve_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_valve_dw.py` & `neer-0.0.8/neer/primary/public/inp_valve_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_vertices.py` & `neer-0.0.8/neer/primary/public/inp_vertices.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_washoff.py` & `neer-0.0.8/neer/primary/public/inp_washoff.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_wastewater_treatment_plant_am.py` & `neer-0.0.8/neer/primary/public/inp_wastewater_treatment_plant_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_water_main_am.py` & `neer-0.0.8/neer/primary/public/inp_water_main_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_water_treatment_plant_am.py` & `neer-0.0.8/neer/primary/public/inp_water_treatment_plant_am.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_weir.py` & `neer-0.0.8/neer/primary/public/inp_weir.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/inp_xsection.py` & `neer-0.0.8/neer/primary/public/inp_xsection.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/invitations.py` & `neer-0.0.8/neer/primary/public/invitations.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/invoices.py` & `neer-0.0.8/neer/primary/public/invoices.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/jobs.py` & `neer-0.0.8/neer/primary/public/jobs.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/land_use_code_scores.py` & `neer-0.0.8/neer/primary/public/land_use_code_scores.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/layer_files.py` & `neer-0.0.8/neer/primary/public/layer_files.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/layers.py` & `neer-0.0.8/neer/primary/public/layers.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/leak_detection_program.py` & `neer-0.0.8/neer/primary/public/leak_detection_program.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/likely_leak_locations.py` & `neer-0.0.8/neer/primary/public/likely_leak_locations.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/lof_models.py` & `neer-0.0.8/neer/primary/public/lof_models.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/maps.py` & `neer-0.0.8/neer/primary/public/maps.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/material_service_life.py` & `neer-0.0.8/neer/primary/public/material_service_life.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/migrations.py` & `neer-0.0.8/neer/primary/public/migrations.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/ml_models_groups.py` & `neer-0.0.8/neer/primary/public/ml_models_groups.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/ml_models_groups_items.py` & `neer-0.0.8/neer/primary/public/ml_models_groups_items.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/ml_models_names.py` & `neer-0.0.8/neer/primary/public/ml_models_names.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/ml_models_predictions.py` & `neer-0.0.8/neer/primary/public/ml_models_predictions.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/months.py` & `neer-0.0.8/neer/primary/public/months.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/my_layer_files.py` & `neer-0.0.8/neer/primary/public/my_layer_files.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/my_layers.py` & `neer-0.0.8/neer/primary/public/my_layers.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/my_layers_features.py` & `neer-0.0.8/neer/primary/public/my_layers_features.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/noaa_frequency_tables.py` & `neer-0.0.8/neer/primary/public/noaa_frequency_tables.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/non_revenue_water.py` & `neer-0.0.8/neer/primary/public/non_revenue_water.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/non_revenue_water_loss.py` & `neer-0.0.8/neer/primary/public/non_revenue_water_loss.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/notifications.py` & `neer-0.0.8/neer/primary/public/notifications.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/outfall_replacement_cost_lookup.py` & `neer-0.0.8/neer/primary/public/outfall_replacement_cost_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/password_resets.py` & `neer-0.0.8/neer/primary/public/password_resets.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/performance_indicators.py` & `neer-0.0.8/neer/primary/public/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/pipe_cost_lookup.py` & `neer-0.0.8/neer/primary/public/pipe_cost_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/pred_lof.py` & `neer-0.0.8/neer/primary/public/pred_lof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/processed_cof.py` & `neer-0.0.8/neer/primary/public/processed_cof.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/processed_cof_buffer.py` & `neer-0.0.8/neer/primary/public/processed_cof_buffer.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/processed_cof_facility_distance.py` & `neer-0.0.8/neer/primary/public/processed_cof_facility_distance.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/processed_cof_transportation_rating.py` & `neer-0.0.8/neer/primary/public/processed_cof_transportation_rating.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/project_settings.py` & `neer-0.0.8/neer/primary/public/project_settings.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/projection_list.py` & `neer-0.0.8/neer/primary/public/projection_list.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/projects.py` & `neer-0.0.8/neer/primary/public/projects.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/projects_models.py` & `neer-0.0.8/neer/primary/public/projects_models.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/projects_old.py` & `neer-0.0.8/neer/primary/public/projects_old.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/rainfall_analysis.py` & `neer-0.0.8/neer/primary/public/rainfall_analysis.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/rainfall_analysis_gauge_results.py` & `neer-0.0.8/neer/primary/public/rainfall_analysis_gauge_results.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/rainfall_analysis_gauges.py` & `neer-0.0.8/neer/primary/public/rainfall_analysis_gauges.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/rating_lookup.py` & `neer-0.0.8/neer/primary/public/rating_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/rcb_pipe_cost_lookup.py` & `neer-0.0.8/neer/primary/public/rcb_pipe_cost_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/roles.py` & `neer-0.0.8/neer/primary/public/roles.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/roles_old.py` & `neer-0.0.8/neer/primary/public/roles_old.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/simulation_schedule.py` & `neer-0.0.8/neer/primary/public/simulation_schedule.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/simulations.py` & `neer-0.0.8/neer/primary/public/simulations.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/spatial_ref_sys.py` & `neer-0.0.8/neer/primary/public/spatial_ref_sys.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/structure_replacement_unit_lookup.py` & `neer-0.0.8/neer/primary/public/structure_replacement_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/structure_unit_cost_lookup.py` & `neer-0.0.8/neer/primary/public/structure_unit_cost_lookup.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/subscriptions.py` & `neer-0.0.8/neer/primary/public/subscriptions.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/team_api_keys.py` & `neer-0.0.8/neer/primary/public/team_api_keys.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/team_models.py` & `neer-0.0.8/neer/primary/public/team_models.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/team_subscriptions.py` & `neer-0.0.8/neer/primary/public/team_subscriptions.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/team_users.py` & `neer-0.0.8/neer/primary/public/team_users.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/teams.py` & `neer-0.0.8/neer/primary/public/teams.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/testingspatial.py` & `neer-0.0.8/neer/primary/public/testingspatial.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/typeorm_metadata.py` & `neer-0.0.8/neer/primary/public/typeorm_metadata.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/us_counties.py` & `neer-0.0.8/neer/primary/public/us_counties.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/us_states.py` & `neer-0.0.8/neer/primary/public/us_states.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/user_project_mapping.py` & `neer-0.0.8/neer/primary/public/user_project_mapping.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/user_project_mapping_old.py` & `neer-0.0.8/neer/primary/public/user_project_mapping_old.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/users.py` & `neer-0.0.8/neer/primary/public/users.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/utility_inspection_form.py` & `neer-0.0.8/neer/primary/public/utility_inspection_form.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/public/water_balance.py` & `neer-0.0.8/neer/primary/public/water_balance.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/topology/layer.py` & `neer-0.0.8/neer/primary/topology/layer.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/primary/topology/topology.py` & `neer-0.0.8/neer/primary/topology/topology.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/calibration_data.py` & `neer-0.0.8/neer/timescale/timeseries/calibration_data.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/calibration_data_dw.py` & `neer-0.0.8/neer/timescale/timeseries/calibration_data_dw.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/forecasts.py` & `neer-0.0.8/neer/timescale/timeseries/forecasts.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/historical_weather.py` & `neer-0.0.8/neer/timescale/timeseries/historical_weather.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/inp_timeseries.py` & `neer-0.0.8/neer/timescale/timeseries/inp_timeseries.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/inp_timeseries_back_testing.py` & `neer-0.0.8/neer/timescale/timeseries/inp_timeseries_back_testing.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/inp_timeseries_values.py` & `neer-0.0.8/neer/timescale/timeseries/inp_timeseries_values.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/inp_timeseries_values_back_testing.py` & `neer-0.0.8/neer/timescale/timeseries/inp_timeseries_values_back_testing.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/site_sensor_measurements.py` & `neer-0.0.8/neer/timescale/timeseries/site_sensor_measurements.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/site_sensors.py` & `neer-0.0.8/neer/timescale/timeseries/site_sensors.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/sites.py` & `neer-0.0.8/neer/timescale/timeseries/sites.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/timeseries_file_data.py` & `neer-0.0.8/neer/timescale/timeseries/timeseries_file_data.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer/timescale/timeseries/timeseries_file_data_back_testing.py` & `neer-0.0.8/neer/timescale/timeseries/timeseries_file_data_back_testing.py`

 * *Files identical despite different names*

### Comparing `neer-0.0.7/neer.egg-info/SOURCES.txt` & `neer-0.0.8/neer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 neer/predictions/predictions/spark_rpt_node_inflow_summaries.py
 neer/predictions/predictions/spark_rpt_node_surcharge_summaries.py
 neer/predictions/predictions/spark_rpt_outfall_loading_summaries.py
 neer/predictions/predictions/spark_rpt_pumping_summaries.py
 neer/predictions/predictions/spark_rpt_storage_volume_summaries.py
 neer/predictions/predictions/spark_rpt_subcatchment_runoff_summaries.py
 neer/primary/__init__.py
+neer/primary/aqueduct/arcgis_features.py
 neer/primary/cswr/__init__.py
 neer/primary/cswr/features.py
 neer/primary/public/__init__.py
 neer/primary/public/announcements.py
 neer/primary/public/api_jobs.py
 neer/primary/public/api_tokens.py
 neer/primary/public/auto_simulation_schedule.py
@@ -214,26 +215,29 @@
 neer/primary/public/invoices.py
 neer/primary/public/jobs.py
 neer/primary/public/land_use_code_scores.py
 neer/primary/public/layer_files.py
 neer/primary/public/layers.py
 neer/primary/public/leak_detection_program.py
 neer/primary/public/likely_leak_locations.py
+neer/primary/public/lof_model_teams.py
 neer/primary/public/lof_models.py
 neer/primary/public/maps.py
 neer/primary/public/material_service_life.py
 neer/primary/public/migrations.py
 neer/primary/public/ml_models_groups.py
 neer/primary/public/ml_models_groups_items.py
 neer/primary/public/ml_models_names.py
 neer/primary/public/ml_models_predictions.py
 neer/primary/public/months.py
 neer/primary/public/my_layer_files.py
 neer/primary/public/my_layers.py
 neer/primary/public/my_layers_features.py
+neer/primary/public/new_lof_models.py
+neer/primary/public/new_ml_models.py
 neer/primary/public/noaa_frequency_tables.py
 neer/primary/public/non_revenue_water.py
 neer/primary/public/non_revenue_water_loss.py
 neer/primary/public/notifications.py
 neer/primary/public/outfall_replacement_cost_lookup.py
 neer/primary/public/password_resets.py
 neer/primary/public/performance_indicators.py
```

### Comparing `neer-0.0.7/pyproject.toml` & `neer-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neer"
-version = "0.0.7"
+version = "0.0.8"
 authors = []
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

