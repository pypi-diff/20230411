# Comparing `tmp/fml40_reference_implementation-0.2.7-py3-none-any.whl.zip` & `tmp/fml40_reference_implementation-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,29 @@
-Zip file size: 150016 bytes, number of entries: 327
+Zip file size: 198449 bytes, number of entries: 439
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 16:18 dt_templates/__init__.py
+-rw-r--r--  2.0 unx      979 b- defN 23-Mar-24 14:23 dt_templates/chainsaw.py
+-rw-r--r--  2.0 unx     2259 b- defN 23-Mar-22 16:18 dt_templates/forwarder.py
+-rw-r--r--  2.0 unx      996 b- defN 23-Apr-11 07:53 dt_templates/forwarding_agency.py
+-rw-r--r--  2.0 unx     2139 b- defN 23-Mar-22 16:18 dt_templates/harvester.py
+-rw-r--r--  2.0 unx      988 b- defN 23-Apr-11 07:53 dt_templates/sawmill_entry.py
+-rw-r--r--  2.0 unx      979 b- defN 23-Apr-11 07:53 dt_templates/supplier.py
+-rw-r--r--  2.0 unx     2119 b- defN 23-Mar-24 14:23 dt_templates/truck.py
 -rw-r--r--  2.0 unx      360 b- defN 22-Jan-23 19:54 ml/__init__.py
--rw-r--r--  2.0 unx     1039 b- defN 21-Nov-09 12:38 ml/app_logger.py
--rw-r--r--  2.0 unx     2934 b- defN 22-Aug-05 12:49 ml/callback.py
--rw-r--r--  2.0 unx      693 b- defN 21-Nov-09 12:38 ml/ditto_feature.py
--rw-r--r--  2.0 unx    24704 b- defN 22-Nov-04 13:29 ml/dt_factory.py
--rw-r--r--  2.0 unx     6088 b- defN 21-Nov-09 12:38 ml/entry.py
--rw-r--r--  2.0 unx     3794 b- defN 21-Dec-16 08:43 ml/feature.py
--rw-r--r--  2.0 unx     1254 b- defN 21-Nov-09 12:38 ml/identifier.py
--rw-r--r--  2.0 unx     4598 b- defN 22-Feb-04 11:00 ml/parameters.py
--rw-r--r--  2.0 unx     2120 b- defN 22-Jan-19 08:16 ml/role.py
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jan-26 11:14 ml/app_logger.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-Jan-26 11:14 ml/callback.py
+-rw-r--r--  2.0 unx      693 b- defN 23-Jan-26 11:14 ml/ditto_feature.py
+-rw-r--r--  2.0 unx    33091 b- defN 23-Apr-11 07:53 ml/dt_factory.py
+-rw-r--r--  2.0 unx     6088 b- defN 23-Mar-22 16:18 ml/entry.py
+-rw-r--r--  2.0 unx     3794 b- defN 23-Jan-26 11:14 ml/feature.py
+-rw-r--r--  2.0 unx     1254 b- defN 23-Jan-26 11:14 ml/identifier.py
+-rw-r--r--  2.0 unx     4598 b- defN 23-Jan-26 11:14 ml/parameters.py
+-rw-r--r--  2.0 unx     2120 b- defN 23-Jan-26 11:14 ml/role.py
 -rw-r--r--  2.0 unx     8249 b- defN 22-Jan-23 19:54 ml/s3i_tools.py
--rw-r--r--  2.0 unx    32546 b- defN 22-Nov-04 09:38 ml/thing.py
--rw-r--r--  2.0 unx    10355 b- defN 22-Aug-03 12:25 ml/tools.py
+-rw-r--r--  2.0 unx    32710 b- defN 23-Mar-22 16:18 ml/thing.py
+-rw-r--r--  2.0 unx    10355 b- defN 23-Jan-26 11:14 ml/tools.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/functionalities/__init__.py
 -rw-r--r--  2.0 unx     1635 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_felling_jobs.py
 -rw-r--r--  2.0 unx      986 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_felling_support_jobs.py
 -rw-r--r--  2.0 unx      982 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_forwarding_jobs.py
 -rw-r--r--  2.0 unx      985 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_log_measurements.py
@@ -23,89 +31,113 @@
 -rw-r--r--  2.0 unx      872 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_moisture_measurement.py
 -rw-r--r--  2.0 unx      960 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_move_commands.py
 -rw-r--r--  2.0 unx      501 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_passability_report.py
 -rw-r--r--  2.0 unx      712 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_proximity_alert.py
 -rw-r--r--  2.0 unx      994 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_shield_commands.py
 -rw-r--r--  2.0 unx      583 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_single_tree_felling_jobs.py
 -rw-r--r--  2.0 unx      992 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_winch_command.py
+-rw-r--r--  2.0 unx      404 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/calculates_machine_operation_cost.py
 -rw-r--r--  2.0 unx      830 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/classifies_tree_species.py
+-rw-r--r--  2.0 unx      357 b- defN 23-Apr-11 07:53 ml/fml40/features/functionalities/controls_sawmill_production.py
 -rw-r--r--  2.0 unx      314 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/converts_data_formats.py
 -rw-r--r--  2.0 unx      333 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/converts_forest_gml.py
--rw-r--r--  2.0 unx      333 b- defN 22-Nov-04 09:42 ml/fml40/features/functionalities/converts_shapefile.py
+-rw-r--r--  2.0 unx      333 b- defN 22-Nov-17 10:47 ml/fml40/features/functionalities/converts_shapefile.py
 -rw-r--r--  2.0 unx      498 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/cuts.py
 -rw-r--r--  2.0 unx     1646 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/determines_passability.py
 -rw-r--r--  2.0 unx      544 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/displays_health_alarms.py
 -rw-r--r--  2.0 unx      316 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/evaluates_forest_rating.py
 -rw-r--r--  2.0 unx      693 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/evaluates_stand_attributes.py
 -rw-r--r--  2.0 unx     1209 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/fells.py
 -rw-r--r--  2.0 unx      556 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/forest_planning_evaluation.py
 -rw-r--r--  2.0 unx      982 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/forwards.py
 -rw-r--r--  2.0 unx      960 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/generates_afforestation_suggestions.py
 -rw-r--r--  2.0 unx      829 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/generates_felling_suggestions.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Apr-11 07:53 ml/fml40/features/functionalities/generates_log_delivery_note.py
+-rw-r--r--  2.0 unx      644 b- defN 23-Apr-11 07:53 ml/fml40/features/functionalities/generates_log_loading_note.py
 -rw-r--r--  2.0 unx      322 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/generates_typical_single_trees.py
 -rw-r--r--  2.0 unx      369 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/grabs.py
 -rw-r--r--  2.0 unx      493 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/harvests.py
 -rw-r--r--  2.0 unx      471 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/measure_wood.py
 -rw-r--r--  2.0 unx      365 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/monitor_health_status.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/plans_harvesting_job_list.py
 -rw-r--r--  2.0 unx      298 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/predicts_forest_development.py
+-rw-r--r--  2.0 unx      329 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/predicts_maintenance.py
+-rw-r--r--  2.0 unx      338 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/provides_emission_data.py
 -rw-r--r--  2.0 unx      511 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/provides_moisture_prediction.py
 -rw-r--r--  2.0 unx      391 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/provides_passability_information.py
 -rw-r--r--  2.0 unx      515 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/provides_production_data.py
 -rw-r--r--  2.0 unx      875 b- defN 22-Aug-03 12:25 ml/fml40/features/functionalities/provides_soil_data.py
+-rw-r--r--  2.0 unx      447 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/provides_stem_segment_data.py
 -rw-r--r--  2.0 unx      624 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/provides_tree_data.py
 -rw-r--r--  2.0 unx      314 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/provides_weather_data.py
 -rw-r--r--  2.0 unx      314 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/simulates_tree_growth.py
 -rw-r--r--  2.0 unx      469 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/supports_felling.py
 -rw-r--r--  2.0 unx      767 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/transports_logs.py
 -rw-r--r--  2.0 unx      289 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/visualizes_forest.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/__init__.py
 -rw-r--r--  2.0 unx      133 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/abstract_inventory.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/allow_wood_delivery_time_slot.py
 -rw-r--r--  2.0 unx      669 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/assortment.py
--rw-r--r--  2.0 unx      653 b- defN 22-Nov-04 09:42 ml/fml40/features/properties/values/basal_area.py
+-rw-r--r--  2.0 unx      653 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/basal_area.py
+-rw-r--r--  2.0 unx      531 b- defN 23-Mar-24 14:23 ml/fml40/features/properties/values/climbing_ability.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/cost_index_low_loader.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/customer_type.py
 -rw-r--r--  2.0 unx      643 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/dbh.py
 -rw-r--r--  2.0 unx      292 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/dominant_tree_species.py
 -rw-r--r--  2.0 unx      660 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/fell_indicator.py
 -rw-r--r--  2.0 unx      896 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/felling_period.py
+-rw-r--r--  2.0 unx      615 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/ground_clearance.py
 -rw-r--r--  2.0 unx      659 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/harvested_volume.py
 -rw-r--r--  2.0 unx      759 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/harvesting_parameter.py
 -rw-r--r--  2.0 unx      288 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/increment_volume.py
 -rw-r--r--  2.0 unx      679 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/interfering_branches.py
 -rw-r--r--  2.0 unx      718 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/inventory_data.py
--rw-r--r--  2.0 unx      652 b- defN 22-Nov-04 09:42 ml/fml40/features/properties/values/is_felled.py
+-rw-r--r--  2.0 unx      652 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/is_felled.py
+-rw-r--r--  2.0 unx      677 b- defN 23-Mar-24 14:23 ml/fml40/features/properties/values/log_loading_length.py
 -rw-r--r--  2.0 unx     1182 b- defN 22-Jul-19 15:56 ml/fml40/features/properties/values/maintenance_data.py
 -rw-r--r--  2.0 unx      283 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/mean_height.py
 -rw-r--r--  2.0 unx      286 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/number_of_stems.py
 -rw-r--r--  2.0 unx      695 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/overhang.py
+-rw-r--r--  2.0 unx      562 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/sawing_processing_step.py
+-rw-r--r--  2.0 unx      567 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/sawing_processing_time.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/sawing_setup_time.py
+-rw-r--r--  2.0 unx      307 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/sawmill_delivery_parking_area_status.py
+-rw-r--r--  2.0 unx      304 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/sawmill_entry_parking_area_status.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/stand_attribute_set.py
 -rw-r--r--  2.0 unx     1502 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/stem_segment_properties.py
--rw-r--r--  2.0 unx      657 b- defN 22-Nov-04 09:42 ml/fml40/features/properties/values/stock_volume.py
+-rw-r--r--  2.0 unx      657 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/stock_volume.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/suitable_tree_species.py
 -rw-r--r--  2.0 unx      287 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/thickness_class.py
--rw-r--r--  2.0 unx      944 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tilt.py
 -rw-r--r--  2.0 unx      281 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tree_data.py
--rw-r--r--  2.0 unx      284 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tree_species.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/tree_species.py
 -rw-r--r--  2.0 unx      684 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tree_type.py
--rw-r--r--  2.0 unx     3165 b- defN 22-Nov-04 09:38 ml/fml40/features/properties/values/vegetationindex.py
+-rw-r--r--  2.0 unx     3165 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/vegetationindex.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/vitality_status.py
 -rw-r--r--  2.0 unx      284 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/wood_quality.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/documents/contracts/__init__.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/documents/contracts/log_procurement_contract.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/jobs/__init__.py
 -rw-r--r--  2.0 unx      242 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/jobs/felling_job.py
 -rw-r--r--  2.0 unx      249 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/jobs/fellung_support_job.py
 -rw-r--r--  2.0 unx      245 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/jobs/forwarding_job.py
 -rw-r--r--  2.0 unx      448 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/jobs/log_transportation_job.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/documents/notes/__init__.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/documents/notes/log_delivery_note.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/__init__.py
 -rw-r--r--  2.0 unx      267 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/afforestation_suggestion.py
 -rw-r--r--  2.0 unx       77 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/felling_tool.py
 -rw-r--r--  2.0 unx      258 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/log_measurement.py
 -rw-r--r--  2.0 unx      267 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/log_transportation_report.py
 -rw-r--r--  2.0 unx      251 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/map_data.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/moisture_prediction_report.py
 -rw-r--r--  2.0 unx      261 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/passability_report.py
 -rw-r--r--  2.0 unx      267 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/reports/soil_moisture_measurement.py
+-rw-r--r--  2.0 unx      259 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/documents/reports/wood_certificate.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/forest/__init__.py
 -rw-r--r--  2.0 unx      253 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/forest/forest.py
 -rw-r--r--  2.0 unx      258 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/forest/forest_segment.py
 -rw-r--r--  2.0 unx      271 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/forest/tree.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/handheld_devices/__init__.py
@@ -116,21 +148,33 @@
 -rw-r--r--  2.0 unx      300 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/forwarder.py
 -rw-r--r--  2.0 unx      300 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/harvester.py
 -rw-r--r--  2.0 unx      299 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/log_truck.py
 -rw-r--r--  2.0 unx      280 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/mini_tractor.py
 -rw-r--r--  2.0 unx      298 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/skidder.py
 -rw-r--r--  2.0 unx      302 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/machines/wheel_loader.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/parts/__init__.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/band.py
+-rw-r--r--  2.0 unx      267 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/clam_bunk.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/front_bogie_lift.py
 -rw-r--r--  2.0 unx      266 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/grabber.py
 -rw-r--r--  2.0 unx      273 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/harvesting_head.py
 -rw-r--r--  2.0 unx      273 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/log_loading_area.py
+-rw-r--r--  2.0 unx      272 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/rear_bogie_lift.py
+-rw-r--r--  2.0 unx      269 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/rung_basket.py
 -rw-r--r--  2.0 unx      262 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/saw.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Apr-11 07:53 ml/fml40/roles/dts/parts/sawmill_entry.py
+-rw-r--r--  2.0 unx      301 b- defN 23-Apr-11 07:53 ml/fml40/roles/dts/parts/sawmill_entry_scale.py
+-rw-r--r--  2.0 unx      299 b- defN 23-Apr-11 07:53 ml/fml40/roles/dts/parts/sawmill_exit_scale.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Apr-11 07:53 ml/fml40/roles/dts/parts/sawmill_gate.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Apr-11 07:53 ml/fml40/roles/dts/parts/sawmill_storage_area.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/skidding_winch.py
 -rw-r--r--  2.0 unx      310 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/stacking_shield.py
--rw-r--r--  2.0 unx      264 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/parts/winch.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/parts/traction_winch.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/persons/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/persons/chain_saw_operator.py
 -rw-r--r--  2.0 unx      278 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/persons/forest_owner.py
 -rw-r--r--  2.0 unx      257 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/persons/forest_worker.py
 -rw-r--r--  2.0 unx      286 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/persons/mini_tractor_operator.py
 -rw-r--r--  2.0 unx      282 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/persons/skidder_operator.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sensors/__init__.py
 -rw-r--r--  2.0 unx      283 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/sensors/barkbeetle_sensor.py
 -rw-r--r--  2.0 unx      225 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sensors/calipers.py
@@ -139,128 +183,196 @@
 -rw-r--r--  2.0 unx      275 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/sites/forest_enterprise.py
 -rw-r--r--  2.0 unx      265 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/sites/hauler.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sites/mill/__init__.py
 -rw-r--r--  2.0 unx      213 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sites/mill/mill.py
 -rw-r--r--  2.0 unx      224 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sites/mill/papermill.py
 -rw-r--r--  2.0 unx      222 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/sites/mill/sawmill.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/ways/__init__.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Mar-24 14:23 ml/fml40/roles/dts/ways/forest_road.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/dts/woods/__init__.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Mar-24 14:23 ml/fml40/roles/dts/woods/log_loading_unit.py
+-rw-r--r--  2.0 unx      270 b- defN 23-Mar-22 16:18 ml/fml40/roles/dts/woods/loose_stack.py
 -rw-r--r--  2.0 unx      271 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/woods/stem_segment.py
 -rw-r--r--  2.0 unx      251 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/woods/wood.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Dec-16 08:43 ml/fml40/roles/dts/woods/wood_pile.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/hmis/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/services/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/functionalities/__init__.py
 -rw-r--r--  2.0 unx      680 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/accepts_jobs.py
 -rw-r--r--  2.0 unx      471 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/accepts_reports.py
 -rw-r--r--  2.0 unx      427 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/clears_jobs.py
 -rw-r--r--  2.0 unx      330 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/functionality.py
 -rw-r--r--  2.0 unx      633 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/manages_jobs.py
 -rw-r--r--  2.0 unx      510 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/plans_routes.py
--rw-r--r--  2.0 unx      377 b- defN 22-Nov-04 13:29 ml/ml40/features/functionalities/predicts_maintenance.py
+-rw-r--r--  2.0 unx      377 b- defN 23-Apr-11 07:53 ml/ml40/features/functionalities/predicts_consumption.py
+-rw-r--r--  2.0 unx      377 b- defN 22-Nov-17 10:47 ml/ml40/features/functionalities/predicts_maintenance.py
+-rw-r--r--  2.0 unx      327 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/predicts_purchase.py
+-rw-r--r--  2.0 unx      387 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/provides_emissions_data.py
+-rw-r--r--  2.0 unx      384 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/provides_machine_data.py
 -rw-r--r--  2.0 unx      515 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/provides_map_data.py
 -rw-r--r--  2.0 unx      482 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/provides_operational_data.py
+-rw-r--r--  2.0 unx      340 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/provides_settlement.py
 -rw-r--r--  2.0 unx      656 b- defN 22-Aug-03 12:25 ml/ml40/features/functionalities/provides_weather_data.py
 -rw-r--r--  2.0 unx      398 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/renders.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/__init__.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/property.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/associations/__init__.py
 -rw-r--r--  2.0 unx      285 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/associations/association.py
 -rw-r--r--  2.0 unx      805 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/associations/composite.py
--rw-r--r--  2.0 unx      865 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/associations/shared.py
+-rw-r--r--  2.0 unx      865 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/associations/shared.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/__init__.py
--rw-r--r--  2.0 unx      284 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/acceleration.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/acceleration.py
 -rw-r--r--  2.0 unx      287 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/accoustic_indices.py
 -rw-r--r--  2.0 unx      996 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/address.py
--rw-r--r--  2.0 unx      283 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/air_pressure.py
+-rw-r--r--  2.0 unx      537 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/air_pressure.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/air_volume.py
 -rw-r--r--  2.0 unx      276 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/area.py
+-rw-r--r--  2.0 unx      769 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/bank_account.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/brand.py
 -rw-r--r--  2.0 unx      282 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/brightness.py
+-rw-r--r--  2.0 unx      315 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/contacts.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/cost.py
 -rw-r--r--  2.0 unx      795 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/count.py
--rw-r--r--  2.0 unx      872 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/dimensions.py
+-rw-r--r--  2.0 unx      280 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/current_load.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/current_weight.py
+-rw-r--r--  2.0 unx      526 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/description.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/diameter.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/dimensions.py
 -rw-r--r--  2.0 unx      663 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/distance.py
+-rw-r--r--  2.0 unx      278 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/empty_load.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/empty_weight.py
 -rw-r--r--  2.0 unx     1053 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/expansion_length.py
--rw-r--r--  2.0 unx      963 b- defN 22-Nov-04 09:42 ml/ml40/features/properties/values/financial_value.py
+-rw-r--r--  2.0 unx      963 b- defN 22-Nov-17 10:47 ml/ml40/features/properties/values/financial_value.py
 -rw-r--r--  2.0 unx     1214 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/force.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/fuel.py
+-rw-r--r--  2.0 unx      733 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/fuel_comsumption.py
+-rw-r--r--  2.0 unx      110 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/fuel_type.py
 -rw-r--r--  2.0 unx      531 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/generic_property.py
 -rw-r--r--  2.0 unx      313 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/gyroscope_value.py
 -rw-r--r--  2.0 unx     1745 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/heart_rate.py
 -rw-r--r--  2.0 unx     2173 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/high_speed_image_value.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/idling_operating_hours.py
+-rw-r--r--  2.0 unx      797 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/imu_quaternion.py
 -rw-r--r--  2.0 unx      280 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/infrared.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/land_velocity.py
 -rw-r--r--  2.0 unx      711 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/last_service_check.py
 -rw-r--r--  2.0 unx      973 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/lidar_frame.py
 -rw-r--r--  2.0 unx     1286 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/lift.py
 -rw-r--r--  2.0 unx      420 b- defN 22-Aug-03 12:25 ml/ml40/features/properties/values/linestring.py
 -rw-r--r--  2.0 unx      690 b- defN 22-Aug-04 07:53 ml/ml40/features/properties/values/linestring_wkt.py
 -rw-r--r--  2.0 unx      685 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/liquid_filling_level.py
--rw-r--r--  2.0 unx     1943 b- defN 22-Nov-04 09:42 ml/ml40/features/properties/values/location.py
+-rw-r--r--  2.0 unx      482 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/load.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/load_index.py
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/loading_volume.py
+-rw-r--r--  2.0 unx     1943 b- defN 22-Nov-17 10:47 ml/ml40/features/properties/values/location.py
 -rw-r--r--  2.0 unx      275 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/lot.py
+-rw-r--r--  2.0 unx      541 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/machine_operating_status.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/machine_operating_status_type.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/maintenance_due.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/maintenance_remaining_hours.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/manufacturing_year.py
+-rw-r--r--  2.0 unx      760 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/measure.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/model.py
 -rw-r--r--  2.0 unx      999 b- defN 22-Aug-03 12:25 ml/ml40/features/properties/values/moisture.py
--rw-r--r--  2.0 unx      676 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/operating_hours.py
+-rw-r--r--  2.0 unx      546 b- defN 23-Mar-24 14:23 ml/ml40/features/properties/values/motor_vehicle_license_plate_number.py
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/opening_hours.py
+-rw-r--r--  2.0 unx      912 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/operating_hours.py
 -rw-r--r--  2.0 unx     1201 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/orientation_rpy.py
--rw-r--r--  2.0 unx      652 b- defN 22-Nov-04 09:42 ml/ml40/features/properties/values/percentage.py
+-rw-r--r--  2.0 unx      652 b- defN 22-Nov-17 10:47 ml/ml40/features/properties/values/percentage.py
 -rw-r--r--  2.0 unx      669 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/personal_name.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/pressure.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/price_list.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/purchase_cost.py
 -rw-r--r--  2.0 unx      280 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/rgb_color.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/road_velocity.py
 -rw-r--r--  2.0 unx      655 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/rotational_speed.py
 -rw-r--r--  2.0 unx      277 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/route.py
+-rw-r--r--  2.0 unx      527 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/serial_number.py
 -rw-r--r--  2.0 unx      282 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/sound_level.py
 -rw-r--r--  2.0 unx      276 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/srid.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/status.py
 -rw-r--r--  2.0 unx     1512 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/std_deviation_rpy.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/steering_angle.py
 -rw-r--r--  2.0 unx     1026 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/stereo_camera_config.py
 -rw-r--r--  2.0 unx      279 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/surface.py
 -rw-r--r--  2.0 unx      288 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/surface_wkt.py
 -rw-r--r--  2.0 unx     1304 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/switching_stage.py
--rw-r--r--  2.0 unx     1122 b- defN 22-Aug-03 12:25 ml/ml40/features/properties/values/temperature.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/tax_number.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/temperature.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/tilt.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/time.py
 -rw-r--r--  2.0 unx      626 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/time_slot.py
--rw-r--r--  2.0 unx      646 b- defN 22-Nov-04 09:42 ml/ml40/features/properties/values/unit.py
--rw-r--r--  2.0 unx      990 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/value.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/torque.py
+-rw-r--r--  2.0 unx      519 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/type.py
+-rw-r--r--  2.0 unx      646 b- defN 22-Nov-17 10:47 ml/ml40/features/properties/values/unit.py
+-rw-r--r--  2.0 unx     1013 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/value.py
+-rw-r--r--  2.0 unx      703 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/velocity.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/volume.py
 -rw-r--r--  2.0 unx     2793 b- defN 22-Aug-03 12:25 ml/ml40/features/properties/values/weatherdata.py
 -rw-r--r--  2.0 unx      669 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/weight.py
 -rw-r--r--  2.0 unx      309 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/white_level.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/__init__.py
 -rw-r--r--  2.0 unx      280 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/document.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/contracts/__init__.py
+-rw-r--r--  2.0 unx      299 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/contracts/contract.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/jobs/__init__.py
 -rw-r--r--  2.0 unx      695 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/jobs/generic_job.py
--rw-r--r--  2.0 unx      782 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/jobs/job.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/documents/jobs/job.py
 -rw-r--r--  2.0 unx      288 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/jobs/job_list.py
 -rw-r--r--  2.0 unx       99 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/jobs/job_status.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/notes/__init__.py
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/notes/note.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/reports/__init__.py
 -rw-r--r--  2.0 unx      307 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/reports/production_data.py
 -rw-r--r--  2.0 unx      297 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/reports/report.py
 -rw-r--r--  2.0 unx        1 b- defN 21-Nov-09 12:38 ml/ml40/roles/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/__init__.py
 -rw-r--r--  2.0 unx      217 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/dt.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/handheld_devices/__init__.py
 -rw-r--r--  2.0 unx      260 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/handheld_devices/handheld_device.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/machines/__init__.py
 -rw-r--r--  2.0 unx      261 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/machines/machine.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/organisations/__init__.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Apr-11 07:53 ml/ml40/roles/dts/organisations/forwarding_agency.py
+-rw-r--r--  2.0 unx      322 b- defN 23-Apr-11 07:53 ml/ml40/roles/dts/organisations/funding_agency.py
+-rw-r--r--  2.0 unx      276 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/organisations/organisation.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/organisations/production_team.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/organisations/supplier.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/parts/__init__.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/parts/chain.py
 -rw-r--r--  2.0 unx      274 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/crane.py
 -rw-r--r--  2.0 unx      276 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/engine.py
 -rw-r--r--  2.0 unx      260 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/part.py
 -rw-r--r--  2.0 unx      274 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/scale.py
 -rw-r--r--  2.0 unx      272 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/tank.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/parts/wheel.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/parts/winch.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/persons/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/persons/machine_operator.py
 -rw-r--r--  2.0 unx      242 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/persons/person.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/__init__.py
 -rw-r--r--  2.0 unx      279 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/accelerometer.py
 -rw-r--r--  2.0 unx      290 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/air_sensor.py
+-rw-r--r--  2.0 unx      298 b- defN 23-Apr-11 07:53 ml/ml40/roles/dts/sensors/counter_sensor.py
 -rw-r--r--  2.0 unx      290 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/gyroscope.py
 -rw-r--r--  2.0 unx      274 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/high_speed_camera.py
 -rw-r--r--  2.0 unx      295 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/imu.py
 -rw-r--r--  2.0 unx      321 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/laser_range_finder.py
 -rw-r--r--  2.0 unx      254 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/lidar.py
 -rw-r--r--  2.0 unx      294 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/light_sensor.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/sensors/pressure_sensor.py
 -rw-r--r--  2.0 unx      252 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/sensor.py
 -rw-r--r--  2.0 unx      298 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/sensor_network.py
 -rw-r--r--  2.0 unx      292 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/soil_sensor.py
 -rw-r--r--  2.0 unx      294 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/sound_sensor.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/stereo_camera.py
+-rw-r--r--  2.0 unx      306 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/sensors/temperature_sensor.py
+-rw-r--r--  2.0 unx      334 b- defN 23-Apr-11 07:53 ml/ml40/roles/dts/sensors/vehicle_counter_sensor.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sites/__init__.py
 -rw-r--r--  2.0 unx      260 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sites/site.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/ways/__init__.py
 -rw-r--r--  2.0 unx      258 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/ways/way.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/hmis/__init__.py
 -rw-r--r--  2.0 unx      262 b- defN 21-Dec-16 08:43 ml/ml40/roles/hmis/app.py
 -rw-r--r--  2.0 unx      274 b- defN 21-Dec-16 08:43 ml/ml40/roles/hmis/dashboard.py
@@ -269,15 +381,15 @@
 -rw-r--r--  2.0 unx      259 b- defN 21-Dec-16 08:43 ml/ml40/roles/hmis/machine_ui.py
 -rw-r--r--  2.0 unx        1 b- defN 22-Aug-03 12:25 ml/ml40/roles/services/__init__.py
 -rw-r--r--  2.0 unx      289 b- defN 22-Aug-03 12:25 ml/ml40/roles/services/openweather_service.py
 -rw-r--r--  2.0 unx      257 b- defN 22-Aug-03 12:25 ml/ml40/roles/services/service.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/mml40/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/mml40/features/__init__.py
 -rw-r--r--  2.0 unx      526 b- defN 21-Dec-16 08:43 ml/mml40/features/functionalities/CantileverConfigure.py
--rw-r--r--  2.0 unx      468 b- defN 22-Nov-04 13:29 ml/mml40/features/functionalities/EstimatesLoading.py
+-rw-r--r--  2.0 unx      468 b- defN 22-Nov-17 10:47 ml/mml40/features/functionalities/EstimatesLoading.py
 -rw-r--r--  2.0 unx      785 b- defN 21-Dec-16 08:43 ml/mml40/features/functionalities/ProvidesDisplacementData.py
 -rw-r--r--  2.0 unx      727 b- defN 21-Dec-16 08:43 ml/mml40/features/functionalities/ProvidesForceData.py
 -rw-r--r--  2.0 unx      737 b- defN 21-Dec-16 08:43 ml/mml40/features/functionalities/ProvidesStretchData.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/mml40/features/functionalities/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/mml40/features/properties/__init__.py
 -rw-r--r--  2.0 unx     1671 b- defN 21-Nov-09 12:38 ml/mml40/features/properties/values/Displacement.py
 -rw-r--r--  2.0 unx     1938 b- defN 21-Nov-09 12:38 ml/mml40/features/properties/values/GeometryProperties.py
@@ -317,13 +429,13 @@
 -rw-r--r--  2.0 unx      252 b- defN 22-Aug-03 12:25 ml/wml40/roles/dts/water/water.py
 -rw-r--r--  2.0 unx      277 b- defN 22-Aug-03 12:25 ml/wml40/roles/dts/water/waterreservoir.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-03 12:25 ml/wml40/roles/hmis/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-03 12:25 ml/wml40/roles/services/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 tests/test_async.py
 -rw-r--r--  2.0 unx       48 b- defN 22-Aug-03 12:25 tests/test_entry.py
--rw-rw-rw-  2.0 unx     7651 b- defN 22-Nov-04 13:52 fml40_reference_implementation-0.2.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8893 b- defN 22-Nov-04 13:52 fml40_reference_implementation-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-04 13:52 fml40_reference_implementation-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Nov-04 13:52 fml40_reference_implementation-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    33142 b- defN 22-Nov-04 13:52 fml40_reference_implementation-0.2.7.dist-info/RECORD
-327 files, 285262 bytes uncompressed, 95182 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 unx     7651 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8893 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    45031 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/RECORD
+439 files, 356503 bytes uncompressed, 123853 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,7 +1,31 @@
+Filename: dt_templates/__init__.py
+Comment: 
+
+Filename: dt_templates/chainsaw.py
+Comment: 
+
+Filename: dt_templates/forwarder.py
+Comment: 
+
+Filename: dt_templates/forwarding_agency.py
+Comment: 
+
+Filename: dt_templates/harvester.py
+Comment: 
+
+Filename: dt_templates/sawmill_entry.py
+Comment: 
+
+Filename: dt_templates/supplier.py
+Comment: 
+
+Filename: dt_templates/truck.py
+Comment: 
+
 Filename: ml/__init__.py
 Comment: 
 
 Filename: ml/app_logger.py
 Comment: 
 
 Filename: ml/callback.py
@@ -78,17 +102,23 @@
 
 Filename: ml/fml40/features/functionalities/accepts_single_tree_felling_jobs.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/accepts_winch_command.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/calculates_machine_operation_cost.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/classifies_tree_species.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/controls_sawmill_production.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/converts_data_formats.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/converts_forest_gml.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/converts_shapefile.py
@@ -120,14 +150,20 @@
 
 Filename: ml/fml40/features/functionalities/generates_afforestation_suggestions.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/generates_felling_suggestions.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/generates_log_delivery_note.py
+Comment: 
+
+Filename: ml/fml40/features/functionalities/generates_log_loading_note.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/generates_typical_single_trees.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/grabs.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/harvests.py
@@ -135,29 +171,41 @@
 
 Filename: ml/fml40/features/functionalities/measure_wood.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/monitor_health_status.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/plans_harvesting_job_list.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/predicts_forest_development.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/predicts_maintenance.py
+Comment: 
+
+Filename: ml/fml40/features/functionalities/provides_emission_data.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/provides_moisture_prediction.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/provides_passability_information.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/provides_production_data.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/provides_soil_data.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/provides_stem_segment_data.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/provides_tree_data.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/provides_weather_data.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/simulates_tree_growth.py
@@ -177,32 +225,47 @@
 
 Filename: ml/fml40/features/properties/values/__init__.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/abstract_inventory.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/allow_wood_delivery_time_slot.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/assortment.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/basal_area.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/climbing_ability.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/cost_index_low_loader.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/customer_type.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/dbh.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/dominant_tree_species.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/fell_indicator.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/felling_period.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/ground_clearance.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/harvested_volume.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/harvesting_parameter.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/increment_volume.py
@@ -213,39 +276,57 @@
 
 Filename: ml/fml40/features/properties/values/inventory_data.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/is_felled.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/log_loading_length.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/maintenance_data.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/mean_height.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/number_of_stems.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/overhang.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/sawing_processing_step.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/sawing_processing_time.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/sawing_setup_time.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/sawmill_delivery_parking_area_status.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/sawmill_entry_parking_area_status.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/stand_attribute_set.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/stem_segment_properties.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/stock_volume.py
 Comment: 
 
-Filename: ml/fml40/features/properties/values/thickness_class.py
+Filename: ml/fml40/features/properties/values/suitable_tree_species.py
 Comment: 
 
-Filename: ml/fml40/features/properties/values/tilt.py
+Filename: ml/fml40/features/properties/values/thickness_class.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/tree_data.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/tree_species.py
 Comment: 
@@ -261,14 +342,20 @@
 
 Filename: ml/fml40/features/properties/values/wood_quality.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/__init__.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/documents/contracts/__init__.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/documents/contracts/log_procurement_contract.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/documents/jobs/__init__.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/jobs/felling_job.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/jobs/fellung_support_job.py
@@ -276,14 +363,20 @@
 
 Filename: ml/fml40/features/properties/values/documents/jobs/forwarding_job.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/jobs/log_transportation_job.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/documents/notes/__init__.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/documents/notes/log_delivery_note.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/documents/reports/__init__.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/reports/afforestation_suggestion.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/reports/felling_tool.py
@@ -303,14 +396,17 @@
 
 Filename: ml/fml40/features/properties/values/documents/reports/passability_report.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/documents/reports/soil_moisture_measurement.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/documents/reports/wood_certificate.py
+Comment: 
+
 Filename: ml/fml40/roles/__init__.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/__init__.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/forest/__init__.py
@@ -357,35 +453,71 @@
 
 Filename: ml/fml40/roles/dts/machines/wheel_loader.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/parts/__init__.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/parts/band.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/clam_bunk.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/front_bogie_lift.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/parts/grabber.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/parts/harvesting_head.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/parts/log_loading_area.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/parts/rear_bogie_lift.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/rung_basket.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/parts/saw.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/parts/sawmill_entry.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/sawmill_entry_scale.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/sawmill_exit_scale.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/sawmill_gate.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/sawmill_storage_area.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/parts/skidding_winch.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/parts/stacking_shield.py
 Comment: 
 
-Filename: ml/fml40/roles/dts/parts/winch.py
+Filename: ml/fml40/roles/dts/parts/traction_winch.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/persons/__init__.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/persons/chain_saw_operator.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/persons/forest_owner.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/persons/forest_worker.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/persons/mini_tractor_operator.py
@@ -426,17 +558,26 @@
 
 Filename: ml/fml40/roles/dts/sites/mill/sawmill.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/ways/__init__.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/ways/forest_road.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/woods/__init__.py
 Comment: 
 
+Filename: ml/fml40/roles/dts/woods/log_loading_unit.py
+Comment: 
+
+Filename: ml/fml40/roles/dts/woods/loose_stack.py
+Comment: 
+
 Filename: ml/fml40/roles/dts/woods/stem_segment.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/woods/wood.py
 Comment: 
 
 Filename: ml/fml40/roles/dts/woods/wood_pile.py
@@ -471,23 +612,38 @@
 
 Filename: ml/ml40/features/functionalities/manages_jobs.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/plans_routes.py
 Comment: 
 
+Filename: ml/ml40/features/functionalities/predicts_consumption.py
+Comment: 
+
 Filename: ml/ml40/features/functionalities/predicts_maintenance.py
 Comment: 
 
+Filename: ml/ml40/features/functionalities/predicts_purchase.py
+Comment: 
+
+Filename: ml/ml40/features/functionalities/provides_emissions_data.py
+Comment: 
+
+Filename: ml/ml40/features/functionalities/provides_machine_data.py
+Comment: 
+
 Filename: ml/ml40/features/functionalities/provides_map_data.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/provides_operational_data.py
 Comment: 
 
+Filename: ml/ml40/features/functionalities/provides_settlement.py
+Comment: 
+
 Filename: ml/ml40/features/functionalities/provides_weather_data.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/renders.py
 Comment: 
 
 Filename: ml/ml40/features/properties/__init__.py
@@ -519,53 +675,104 @@
 
 Filename: ml/ml40/features/properties/values/address.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/air_pressure.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/air_volume.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/area.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/bank_account.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/brand.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/brightness.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/contacts.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/cost.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/count.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/current_load.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/current_weight.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/description.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/diameter.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/dimensions.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/distance.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/empty_load.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/empty_weight.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/expansion_length.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/financial_value.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/force.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/fuel.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/fuel_comsumption.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/fuel_type.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/generic_property.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/gyroscope_value.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/heart_rate.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/high_speed_image_value.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/idling_operating_hours.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/imu_quaternion.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/infrared.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/land_velocity.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/last_service_check.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/lidar_frame.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/lift.py
@@ -576,77 +783,155 @@
 
 Filename: ml/ml40/features/properties/values/linestring_wkt.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/liquid_filling_level.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/load.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/load_index.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/loading_volume.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/location.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/lot.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/machine_operating_status.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/machine_operating_status_type.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/maintenance_due.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/maintenance_remaining_hours.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/manufacturing_year.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/measure.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/model.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/moisture.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/motor_vehicle_license_plate_number.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/opening_hours.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/operating_hours.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/orientation_rpy.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/percentage.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/personal_name.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/pressure.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/price_list.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/purchase_cost.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/rgb_color.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/road_velocity.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/rotational_speed.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/route.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/serial_number.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/sound_level.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/srid.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/status.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/std_deviation_rpy.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/steering_angle.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/stereo_camera_config.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/surface.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/surface_wkt.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/switching_stage.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/tax_number.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/temperature.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/tilt.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/time.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/time_slot.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/torque.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/type.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/unit.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/value.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/velocity.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/volume.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/weatherdata.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/weight.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/white_level.py
@@ -654,14 +939,20 @@
 
 Filename: ml/ml40/features/properties/values/documents/__init__.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/document.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/documents/contracts/__init__.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/documents/contracts/contract.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/documents/jobs/__init__.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/jobs/generic_job.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/jobs/job.py
@@ -669,14 +960,20 @@
 
 Filename: ml/ml40/features/properties/values/documents/jobs/job_list.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/jobs/job_status.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/documents/notes/__init__.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/documents/notes/note.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/documents/reports/__init__.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/reports/production_data.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/reports/report.py
@@ -699,17 +996,38 @@
 
 Filename: ml/ml40/roles/dts/machines/__init__.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/machines/machine.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/organisations/__init__.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/organisations/forwarding_agency.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/organisations/funding_agency.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/organisations/organisation.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/organisations/production_team.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/organisations/supplier.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/parts/__init__.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/parts/chain.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/parts/crane.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/parts/engine.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/parts/part.py
@@ -717,14 +1035,20 @@
 
 Filename: ml/ml40/roles/dts/parts/scale.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/parts/tank.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/parts/wheel.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/parts/winch.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/persons/__init__.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/persons/machine_operator.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/persons/person.py
@@ -735,14 +1059,17 @@
 
 Filename: ml/ml40/roles/dts/sensors/accelerometer.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/air_sensor.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/sensors/counter_sensor.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/sensors/gyroscope.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/high_speed_camera.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/imu.py
@@ -753,14 +1080,17 @@
 
 Filename: ml/ml40/roles/dts/sensors/lidar.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/light_sensor.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/sensors/pressure_sensor.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/sensors/sensor.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/sensor_network.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/soil_sensor.py
@@ -768,14 +1098,20 @@
 
 Filename: ml/ml40/roles/dts/sensors/sound_sensor.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/stereo_camera.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/sensors/temperature_sensor.py
+Comment: 
+
+Filename: ml/ml40/roles/dts/sensors/vehicle_counter_sensor.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/sites/__init__.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sites/site.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/ways/__init__.py
@@ -960,23 +1296,23 @@
 
 Filename: tests/test_async.py
 Comment: 
 
 Filename: tests/test_entry.py
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.7.dist-info/LICENSE.txt
+Filename: fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.7.dist-info/METADATA
+Filename: fml40_reference_implementation-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.7.dist-info/WHEEL
+Filename: fml40_reference_implementation-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.7.dist-info/top_level.txt
+Filename: fml40_reference_implementation-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.7.dist-info/RECORD
+Filename: fml40_reference_implementation-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ml/dt_factory.py

```diff
@@ -13,53 +13,89 @@
 from ml.ml40.roles.hmis.app import App
 from ml.ml40.roles.hmis.dashboard import Dashboard
 from ml.ml40.roles.hmis.machine_ui import MachineUI
 from ml.ml40.roles.hmis.hmd import HMD
 from ml.ml40.roles.hmis.hmi import HMI
 from ml.ml40.roles.dts.handheld_devices.handheld_device import HandheldDevice
 from ml.ml40.roles.dts.machines.machine import Machine
+from ml.ml40.roles.dts.organisations.organisation import Organisation
+from ml.ml40.roles.dts.organisations.forwarding_agency import ForwardingAgency
+from ml.ml40.roles.dts.organisations.funding_agency import FundingAgency
+from ml.ml40.roles.dts.organisations.production_team import ProductionTeam
+from ml.ml40.roles.dts.organisations.supplier import Supplier
+from ml.ml40.roles.dts.parts.chain import Chain
 from ml.ml40.roles.dts.parts.crane import Crane
 from ml.ml40.roles.dts.parts.part import Part
 from ml.ml40.roles.dts.parts.engine import Engine
 from ml.ml40.roles.dts.parts.scale import Scale
 from ml.ml40.roles.dts.parts.tank import Tank
+from ml.ml40.roles.dts.parts.winch import Winch
+from ml.ml40.roles.dts.parts.wheel import Wheel
 from ml.ml40.roles.dts.persons.machine_operator import MachineOperator
 from ml.ml40.roles.dts.persons.person import Person
 from ml.ml40.roles.dts.sensors.sensor import Sensor
 from ml.ml40.roles.dts.sensors.air_sensor import AirSensor
+from ml.ml40.roles.dts.sensors.accelerometer import Accelerometer
+from ml.ml40.roles.dts.sensors.counter_sensor import CounterSensor
+from ml.ml40.roles.dts.sensors.gyroscope import Gyroscope
+from ml.ml40.roles.dts.sensors.high_speed_camera import HighSpeedCamera
+from ml.ml40.roles.dts.sensors.imu import IMU
+from ml.ml40.roles.dts.sensors.laser_range_finder import LaserRangeFinder
+from ml.ml40.roles.dts.sensors.lidar import LiDAR
+from ml.ml40.roles.dts.sensors.pressure_sensor import PressureSensor
+from ml.ml40.roles.dts.sensors.sensor import Sensor
 from ml.ml40.roles.dts.sensors.soil_sensor import SoilSensor
+from ml.ml40.roles.dts.sensors.sound_sensor import SoundSensor
+from ml.ml40.roles.dts.sensors.stereo_camera import StereoCamera
+from ml.ml40.roles.dts.sensors.temperature_sensor import TemperatureSensor
+from ml.ml40.roles.dts.sensors.vehicle_counter_sensor import VehicleCounterSensor
 from ml.ml40.roles.dts.sites.site import Site
 from ml.ml40.roles.dts.ways.way import Way
 
 from ml.fml40.roles.dts.handheld_devices.brushcutter import Brushcutter
 from ml.fml40.roles.dts.handheld_devices.chainsaw import Chainsaw
 from ml.fml40.roles.dts.machines.forest_machine import ForestMachine
 from ml.fml40.roles.dts.machines.forwarder import Forwarder
 from ml.fml40.roles.dts.machines.harvester import Harvester
 from ml.fml40.roles.dts.machines.log_truck import LogTruck
 from ml.fml40.roles.dts.machines.mini_tractor import MiniTractor
 from ml.fml40.roles.dts.machines.skidder import Skidder
 from ml.fml40.roles.dts.machines.wheel_loader import WheelLoader
+from ml.fml40.roles.dts.parts.band import Band
+from ml.fml40.roles.dts.parts.clam_bunk import ClamBunk
+from ml.fml40.roles.dts.parts.front_bogie_lift import FrontBogieLift
 from ml.fml40.roles.dts.parts.grabber import Grabber
 from ml.fml40.roles.dts.parts.harvesting_head import HarvestingHead
 from ml.fml40.roles.dts.parts.log_loading_area import LogLoadingArea
+from ml.fml40.roles.dts.parts.rear_bogie_lift import RearBogieLift
+from ml.fml40.roles.dts.parts.rung_basket import RungBasket
 from ml.fml40.roles.dts.parts.saw import Saw
+from ml.fml40.roles.dts.parts.sawmill_entry import SawmillEntry
+from ml.fml40.roles.dts.parts.sawmill_entry_scale import SawmillEntryScale
+from ml.fml40.roles.dts.parts.sawmill_exit_scale import SawmillExitScale
+from ml.fml40.roles.dts.parts.sawmill_gate import SawmillGate
+from ml.fml40.roles.dts.parts.sawmill_storage_area import SawmillStorageArea
+from ml.fml40.roles.dts.parts.skidding_winch import SkiddingWinch
 from ml.fml40.roles.dts.parts.stacking_shield import StackingShield
-from ml.fml40.roles.dts.parts.winch import Winch
+from ml.fml40.roles.dts.parts.traction_winch import TractionWinch
+from ml.fml40.roles.dts.persons.chain_saw_operator import ChainsawOperator
 from ml.fml40.roles.dts.persons.forest_owner import ForestOwner
 from ml.fml40.roles.dts.persons.forest_worker import ForestWorker
 from ml.fml40.roles.dts.persons.mini_tractor_operator import MiniTractorOperator
 from ml.fml40.roles.dts.persons.skidder_operator import SkidderOperator
 from ml.fml40.roles.dts.sensors.vitality_sensor import VitalitySensor
 from ml.fml40.roles.dts.sensors.barkbeetle_sensor import BarkbeetleSensor
 from ml.fml40.roles.dts.sites.forest_enterprise import ForestEnterprise
 from ml.fml40.roles.dts.sites.hauler import Hauler
 from ml.fml40.roles.dts.sites.mill.mill import Mill
 from ml.fml40.roles.dts.sites.mill.papermill import Papermill
 from ml.fml40.roles.dts.sites.mill.sawmill import Sawmill
+from ml.fml40.roles.dts.ways.forest_road import ForestRoad
+from ml.fml40.roles.dts.woods.log_loading_unit import LogLoadingUnit
+from ml.fml40.roles.dts.woods.loose_stack import LooseStack
 from ml.fml40.roles.dts.woods.wood import Wood
 from ml.fml40.roles.dts.woods.stem_segment import StemSegment
 from ml.fml40.roles.dts.woods.wood_pile import WoodPile
 from ml.fml40.roles.dts.forest.forest import Forest
 from ml.fml40.roles.dts.forest.forest_segment import ForestSegment
 from ml.fml40.roles.dts.forest.tree import Tree
 
@@ -75,90 +111,149 @@
 from ml.wml40.roles.dts.water.water import Water
 from ml.wml40.roles.dts.water.waterreservoir import WaterReservoir
 
 from ml.ml40.features.properties.associations.association import Association
 from ml.ml40.features.properties.associations.composite import Composite
 from ml.ml40.features.properties.property import Property
 from ml.ml40.features.properties.associations.shared import Shared
+from ml.ml40.features.properties.values.acceleration import Acceleration
 from ml.ml40.features.properties.values.address import Address
+from ml.ml40.features.properties.values.air_volume import AirVolume
+from ml.ml40.features.properties.values.bank_account import BankAccount
+from ml.ml40.features.properties.values.brand import Brand
+from ml.ml40.features.properties.values.contacts import Contacts
+from ml.ml40.features.properties.values.cost import Cost
 from ml.ml40.features.properties.values.count import Count
+from ml.ml40.features.properties.values.current_load import CurrentLoad
+from ml.ml40.features.properties.values.current_weight import CurrentWeight
+from ml.ml40.features.properties.values.description import Description
+from ml.ml40.features.properties.values.diameter import Diameter
 from ml.ml40.features.properties.values.dimensions import Dimensions
 from ml.ml40.features.properties.values.distance import Distance
+from ml.ml40.features.properties.values.empty_load import EmptyLoad
+from ml.ml40.features.properties.values.empty_weight import EmptyWeight
 from ml.ml40.features.properties.values.expansion_length import ExpansionLength
 from ml.ml40.features.properties.values.financial_value import FinancialValue
 from ml.ml40.features.properties.values.force import Force
+from ml.ml40.features.properties.values.fuel import Fuel
+from ml.ml40.features.properties.values.fuel_comsumption import FuelConsumption
+from ml.ml40.features.properties.values.fuel_type import FuelType
 from ml.ml40.features.properties.values.generic_property import GenericProperty
+from ml.ml40.features.properties.values.idling_operating_hours import IdlingOperatingHours
+from ml.ml40.features.properties.values.imu_quaternion import IMUQuaternion
+from ml.ml40.features.properties.values.land_velocity import LandVelocity
 from ml.ml40.features.properties.values.last_service_check import LastServiceCheck
-from ml.ml40.features.properties.values.lot import Lot
 from ml.ml40.features.properties.values.lift import Lift
 from ml.ml40.features.properties.values.linestring import LineString
 from ml.ml40.features.properties.values.linestring_wkt import LineStringWKT
 from ml.ml40.features.properties.values.liquid_filling_level import LiquidFillingLevel
+from ml.ml40.features.properties.values.load import Load
+from ml.ml40.features.properties.values.load_index import LoadIndex
+from ml.ml40.features.properties.values.loading_volume import LoadingVolume
+from ml.ml40.features.properties.values.lot import Lot
 from ml.ml40.features.properties.values.location import Location
+from ml.ml40.features.properties.values.machine_operating_status import MachineOperatingStatus
+from ml.ml40.features.properties.values.machine_operating_status_type import MachineOperatingStatusType
+from ml.ml40.features.properties.values.maintenance_due import MaintenanceDue
+from ml.ml40.features.properties.values.maintenance_remaining_hours import MaintenanceRemainingHours
+from ml.ml40.features.properties.values.manufacturing_year import ManufacturingYear
+from ml.ml40.features.properties.values.measure import Measure
+from ml.ml40.features.properties.values.model import Model
 from ml.ml40.features.properties.values.moisture import Moisture
+from ml.ml40.features.properties.values.motor_vehicle_license_plate_number import MotorVehicleLicensePlateNumber
+from ml.ml40.features.properties.values.opening_hours import OpeningHours
 from ml.ml40.features.properties.values.operating_hours import OperatingHours
 from ml.ml40.features.properties.values.orientation_rpy import OrientationRPY
 from ml.ml40.features.properties.values.percentage import Percentage
 from ml.ml40.features.properties.values.personal_name import PersonalName
+from ml.ml40.features.properties.values.pressure import Pressure
+from ml.ml40.features.properties.values.price_list import PriceList
+from ml.ml40.features.properties.values.purchase_cost import PurchaseCost
+from ml.ml40.features.properties.values.road_velocity import RoadVelocity
 from ml.ml40.features.properties.values.rotational_speed import RotationalSpeed
 from ml.ml40.features.properties.values.route import Route
+from ml.ml40.features.properties.values.serial_number import SerialNumber
 from ml.ml40.features.properties.values.srid import SRID
+from ml.ml40.features.properties.values.status import Status
+from ml.ml40.features.properties.values.steering_angle import SteeringAngle
 from ml.ml40.features.properties.values.surface import Surface
 from ml.ml40.features.properties.values.surface_wkt import SurfaceWKT
 from ml.ml40.features.properties.values.switching_stage import SwitchingStage
+from ml.ml40.features.properties.values.tax_number import TaxNumber
 from ml.ml40.features.properties.values.temperature import Temperature
+from ml.ml40.features.properties.values.time import Time
 from ml.ml40.features.properties.values.time_slot import TimeSlot
+from ml.ml40.features.properties.values.tilt import Tilt
+from ml.ml40.features.properties.values.torque import Torque
+from ml.ml40.features.properties.values.type import Type
 from ml.ml40.features.properties.values.unit import Unit
+from ml.ml40.features.properties.values.velocity import Velocity
+from ml.ml40.features.properties.values.volume import Volume
 from ml.ml40.features.properties.values.weatherdata import WeatherData
 from ml.ml40.features.properties.values.weight import Weight
+from ml.ml40.features.properties.values.documents.contracts.contract import Contract
 from ml.ml40.features.properties.values.documents.jobs.generic_job import GenericJob
 from ml.ml40.features.properties.values.documents.jobs.job import Job
 from ml.ml40.features.properties.values.documents.jobs.job_list import JobList
 from ml.ml40.features.properties.values.documents.jobs.job_status import JobStatus
+from ml.ml40.features.properties.values.documents.notes.note import Note
 from ml.ml40.features.properties.values.documents.reports.report import Report
 from ml.ml40.features.properties.values.documents.reports.production_data import ProductionData
 
+
 from ml.fml40.features.properties.values.abstract_inventory import AbstractInventory
+from ml.fml40.features.properties.values.allow_wood_delivery_time_slot import AllowWoodDeliveryTimeSlot
 from ml.fml40.features.properties.values.assortment import Assortment
 from ml.fml40.features.properties.values.basal_area import BasalArea
+from ml.fml40.features.properties.values.climbing_ability import ClimbingAbility
+from ml.fml40.features.properties.values.cost_index_low_loader import CostIndexLowLoader
+from ml.fml40.features.properties.values.customer_type import CustomerType
 from ml.fml40.features.properties.values.dbh import DBH
 from ml.fml40.features.properties.values.fell_indicator import FellIndicator
 from ml.fml40.features.properties.values.felling_period import FellingPeriod
+from ml.fml40.features.properties.values.ground_clearance import GroundClearance
 from ml.fml40.features.properties.values.harvesting_parameter import HarvestingParameters
 from ml.fml40.features.properties.values.harvested_volume import HarvestedVolume
 from ml.fml40.features.properties.values.interfering_branches import InterferingBranches
 from ml.fml40.features.properties.values.inventory_data import InventoryData
 from ml.fml40.features.properties.values.is_felled import IsFelled
+from ml.fml40.features.properties.values.log_loading_length import LogLoadingLength
 from ml.fml40.features.properties.values.maintenance_data import MaintenanceData
 from ml.fml40.features.properties.values.mean_height import MeanHeight
 from ml.fml40.features.properties.values.overhang import Overhang
+from ml.fml40.features.properties.values.sawing_processing_step import SawingProcessingStep
+from ml.fml40.features.properties.values.sawing_processing_time import SawingProcessingTime
+from ml.fml40.features.properties.values.sawing_setup_time import SawingSetupTime
+from ml.fml40.features.properties.values.sawmill_delivery_parking_area_status import SawmillDeliveryParkingAreaStatus
+from ml.fml40.features.properties.values.sawmill_entry_parking_area_status import SawmillEntryParkingAreaStatus
 from ml.fml40.features.properties.values.stem_segment_properties import StemSegmentProperties
 from ml.fml40.features.properties.values.stock_volume import StockVolume
+from ml.fml40.features.properties.values.suitable_tree_species import SuitableTreeSpecies
 from ml.fml40.features.properties.values.thickness_class import ThicknessClass
-from ml.fml40.features.properties.values.tilt import Tilt
 from ml.fml40.features.properties.values.tree_data import TreeData
 from ml.fml40.features.properties.values.tree_species import TreeSpecies
 from ml.fml40.features.properties.values.tree_type import TreeType
 from ml.fml40.features.properties.values.vegetationindex import VegetationIndex
 from ml.fml40.features.properties.values.vitality_status import VitalityStatus
 from ml.fml40.features.properties.values.wood_quality import WoodQuality
-
+from ml.fml40.features.properties.values.documents.contracts.log_procurement_contract import LogProcurementContract
 from ml.fml40.features.properties.values.documents.jobs.felling_job import FellingJob
 from ml.fml40.features.properties.values.documents.jobs.fellung_support_job import FellingSupportJob
 from ml.fml40.features.properties.values.documents.jobs.forwarding_job import ForwardingJob
 from ml.fml40.features.properties.values.documents.jobs.log_transportation_job import LogTransportationJob
-
+from ml.fml40.features.properties.values.documents.notes.log_delivery_note import LogDeliveryNote
 from ml.fml40.features.properties.values.documents.reports.afforestation_suggestion import AfforestationSuggestion
 from ml.fml40.features.properties.values.documents.reports.felling_tool import FellingTool
 from ml.fml40.features.properties.values.documents.reports.log_measurement import LogMeasurement
 from ml.fml40.features.properties.values.documents.reports.log_transportation_report import LogTransportationReport
 from ml.fml40.features.properties.values.documents.reports.map_data import MapData
 from ml.fml40.features.properties.values.documents.reports.moisture_prediction_report import MoisturePredictionReport
 from ml.fml40.features.properties.values.documents.reports.passability_report import PassabilityReport
 from ml.fml40.features.properties.values.documents.reports.soil_moisture_measurement import SoilMoistureMeasurement
+from ml.fml40.features.properties.values.documents.reports.wood_certificate import WoodCertificate
 
 from ml.mml40.features.properties.values.Displacement import Displacement
 from ml.mml40.features.properties.values.GeometryProperties import GeometryProperties
 from ml.mml40.features.properties.values.LoadAlarm import LoadAlarm
 from ml.mml40.features.properties.values.MaterialProperties import MaterialProperties
 from ml.mml40.features.properties.values.Stretch import Stretch
 
@@ -169,17 +264,23 @@
 
 from ml.ml40.features.functionalities.accepts_jobs import AcceptsJobs
 from ml.ml40.features.functionalities.accepts_reports import AcceptsReports
 from ml.ml40.features.functionalities.clears_jobs import ClearsJobs
 from ml.ml40.features.functionalities.functionality import Functionality
 from ml.ml40.features.functionalities.manages_jobs import ManagesJobs
 from ml.ml40.features.functionalities.plans_routes import PlansRoutes
+from ml.ml40.features.functionalities.predicts_consumption import PredictsConsumption
 from ml.ml40.features.functionalities.predicts_maintenance import PredictsMaintenance
+from ml.ml40.features.functionalities.predicts_purchase import PredictsPurchase
+from ml.ml40.features.functionalities.provides_emissions_data import ProvidesEmissionsData
+from ml.ml40.features.functionalities.provides_machine_data import ProvidesMachineData
 from ml.ml40.features.functionalities.provides_map_data import ProvidesMapData
 from ml.ml40.features.functionalities.provides_operational_data import ProvidesOperationalData
+from ml.ml40.features.functionalities.predicts_purchase import PredictsPurchase
+from ml.ml40.features.functionalities.provides_settlement import ProvidesSettlement
 from ml.ml40.features.functionalities.provides_weather_data import ProvidesWeatherData
 from ml.ml40.features.functionalities.renders import Renders
 
 from ml.fml40.features.functionalities.accepts_felling_jobs import AcceptsFellingJobs
 from ml.fml40.features.functionalities.accepts_felling_support_jobs import AcceptsFellingSupportJobs
 from ml.fml40.features.functionalities.accepts_forwarding_jobs import AcceptsForwardingJobs
 from ml.fml40.features.functionalities.accepts_log_measurements import AcceptsLogMeasurements
@@ -187,33 +288,43 @@
 from ml.fml40.features.functionalities.accepts_moisture_measurement import AcceptsMoistureMeasurement
 from ml.fml40.features.functionalities.accepts_move_commands import AcceptsMoveCommands
 from ml.fml40.features.functionalities.accepts_passability_report import AcceptsPassabilityReport
 from ml.fml40.features.functionalities.accepts_proximity_alert import AcceptsProximityAlert
 from ml.fml40.features.functionalities.accepts_shield_commands import AcceptsShieldCommands
 from ml.fml40.features.functionalities.accepts_single_tree_felling_jobs import AcceptsSingleTreeFellingJobs
 from ml.fml40.features.functionalities.accepts_winch_command import AcceptsWinchCommands
+from ml.fml40.features.functionalities.calculates_machine_operation_cost import CalculatesMachineOperationCost
 from ml.fml40.features.functionalities.classifies_tree_species import ClassifiesTreeSpecies
+from ml.fml40.features.functionalities.controls_sawmill_production import ControlsSawmillProduction
 from ml.fml40.features.functionalities.converts_shapefile import ConvertsShapefile
 from ml.fml40.features.functionalities.cuts import Cuts
 from ml.fml40.features.functionalities.determines_passability import DeterminesPassability
 from ml.fml40.features.functionalities.displays_health_alarms import DisplaysHealthAlarms
 from ml.fml40.features.functionalities.evaluates_stand_attributes import EvaluatesStandAttributes
 from ml.fml40.features.functionalities.fells import Fells
 from ml.fml40.features.functionalities.forest_planning_evaluation import ForestPlanningEvaluation
 from ml.fml40.features.functionalities.forwards import Forwards
 from ml.fml40.features.functionalities.generates_afforestation_suggestions import GeneratesAfforestationSuggestions
 from ml.fml40.features.functionalities.generates_felling_suggestions import GeneratesFellingSuggestions
+from ml.fml40.features.functionalities.generates_log_delivery_note import GeneratesLogDeliveryNote
+from ml.fml40.features.functionalities.generates_log_loading_note import GeneratesLogLoadingNote
 from ml.fml40.features.functionalities.grabs import Grabs
 from ml.fml40.features.functionalities.harvests import Harvests
 from ml.fml40.features.functionalities.measure_wood import MeasuresWood
 from ml.fml40.features.functionalities.monitor_health_status import MonitorsHealthStatus
+from ml.fml40.features.functionalities.plans_harvesting_job_list import PlansHarvestingJobList
+from ml.fml40.features.functionalities.predicts_forest_development import PredictsForestDevelopment
+from ml.fml40.features.functionalities.predicts_maintenance import PredictsMaintenance
+from ml.fml40.features.functionalities.provides_emission_data import ProvidesEmissionData
 from ml.fml40.features.functionalities.provides_moisture_prediction import ProvidesMoisturePrediction
 from ml.fml40.features.functionalities.provides_passability_information import ProvidesPassabilityInformation
 from ml.fml40.features.functionalities.provides_production_data import ProvidesProductionData
+from ml.fml40.features.functionalities.provides_stem_segment_data import ProvidesStemSegmentData
 from ml.fml40.features.functionalities.provides_soil_data import ProvidesSoilData
+
 from ml.fml40.features.functionalities.provides_tree_data import ProvidesTreeData
 from ml.fml40.features.functionalities.provides_weather_data import ProvidesWeatherData
 from ml.fml40.features.functionalities.simulates_tree_growth import SimulatesTreeGrowth
 from ml.fml40.features.functionalities.supports_felling import SupportsFelling
 from ml.fml40.features.functionalities.transports_logs import TransportsLogs
 
 from ml.mml40.features.functionalities.CantileverConfigure import CantileverConfigure
```

## ml/thing.py

```diff
@@ -48,14 +48,15 @@
         self.__grant_type = grant_type
         self.__username = username
         self.__password = password
         self.__token = None
         self.__is_repository = is_repository
         self.__is_broker = is_broker
         self.__is_broker_rest = is_broker_rest
+        self.__broker_msg_list = []
         self.loop = loop
         self.__resGetValue = []
 
         self.callbacks = CallbackManager()
         self.parameters = parameters
 
     @property
@@ -66,17 +67,21 @@
     def token(self):
         return self.__token
 
     @property
     def identifier(self):
         return self.__entry.identifier
 
+    @property
+    def broker_msg_list(self):
+        return self.__broker_msg_list
+
     def run_forever(self):
         try:
-            self.__setup_thing_json_sync()
+            self.setup_thing_json_sync()
             self.connect_to_s3i()
             self.loop.run_forever()
 
         except KeyboardInterrupt:
             APP_LOGGER.info("[S3I]: Disconnect from S3I")
             self.loop.close()
 
@@ -219,15 +224,15 @@
                              self.__refresh_token_recur)
 
     def __get_remaining_time_to_refresh(self):
         remaining_time = self.idp._time_until_token_valid()
         safety_margin = 5
         return remaining_time - safety_margin
 
-    def __setup_thing_json_sync(self):
+    def setup_thing_json_sync(self):
         APP_LOGGER.info("[S3I]: Start the thing")
         self.__recursively_update_dt_json(frequency=self.parameters.thing_sync_freq)
         self.callbacks.process(
             prefix=self._ON_THING_START_OK,
             loop=self.loop
         )
 
@@ -356,14 +361,15 @@
 
         # Add S3I-B Message validate
         try:
             body = raise_error_from_s3ib_msg(body, S3IBMessageError)
         except S3IBMessageError as e:
             APP_LOGGER.error("[S3I]: {}".format(e))
         else:
+            self.__broker_msg_list.append(body)
             message_type = body.get("messageType")
 
             __log = "[S3I]: Received a S3I-B {}: {}".format(
                 message_type, json.dumps(body, indent=2)
             )
             APP_LOGGER.info(__log)
```

## ml/fml40/features/properties/values/tree_species.py

```diff
@@ -2,7 +2,22 @@
 
 
 class TreeSpecies(Value):
     def __init__(self, namespace="fml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
+        self.__tree_species = []
+
+    @property
+    def tree_species(self):
+        return self.__tree_species
+
+    @tree_species.setter
+    def tree_species(self, value):
+        self.__tree_species = value
+
+    def to_json(self):
+        self.__json_out = super().to_json()
+        if self.__tree_species is not None:
+            self.__json_out["treeSpecies"] = self.__tree_species
+        return self.__json_out
```

## ml/ml40/features/properties/values/acceleration.py

```diff
@@ -2,7 +2,21 @@
 
 
 class Acceleration(Value):
     def __init__(self, namespace="ml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
+        self.x = None
+        self.y = None
+        self.z = None
+        self.__json_out = dict()
+
+    def to_json(self):
+        self.__json_out = super().to_json()
+        if self.x is not None:
+            self.__json_out["x"] = self.x
+        if self.y is not None:
+            self.__json_out["y"] = self.y
+        if self.z is not None:
+            self.__json_out["z"] = self.z
+        return self.__json_out
```

## ml/ml40/features/properties/values/air_pressure.py

```diff
@@ -2,7 +2,15 @@
 
 
 class AirPressure(Value):
     def __init__(self, namespace="ml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
+        self.pressure = None
+        self.__json_out = dict()
+
+    def to_json(self):
+        self.__json_out = super().to_json()
+        if self.pressure is not None:
+            self.__json_out["pressure"] = self.pressure
+        return self.__json_out
```

## ml/ml40/features/properties/values/dimensions.py

```diff
@@ -5,23 +5,20 @@
     def __init__(self, namespace="ml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
 
         self.height = None
         self.length = None
-        self.weight = None
         self.width = None
         self.__json_out = dict()
 
     def to_json(self):
         self.__json_out = super().to_json()
         if self.height is not None:
             self.__json_out["height"] = self.height
         if self.length is not None:
             self.__json_out["length"] = self.length
-        if self.weight is not None:
-            self.__json_out["weight"] = self.weight
         if self.width is not None:
             self.__json_out["width"] = self.width
 
         return self.__json_out
```

## ml/ml40/features/properties/values/operating_hours.py

```diff
@@ -4,22 +4,32 @@
 class OperatingHours(Value):
     def __init__(self, namespace="ml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
 
         self.__total = None
+        self.__current = None
         self.__json_out = dict()
 
     @property
     def total(self):
         return self.__total
 
     @total.setter
     def total(self, value):
         self.__total = value
 
+    @property
+    def current(self):
+        return self.__current
+
+    @current.setter
+    def current(self, value):
+        self.__current = value
+
     def to_json(self):
         self.__json_out = super().to_json()
         if self.__total is not None:
             self.__json_out["total"] = self.__total
+            self.__json_out["current"] = self.__current
         return self.__json_out
```

## ml/ml40/features/properties/values/temperature.py

```diff
@@ -2,37 +2,15 @@
 
 
 class Temperature(Value):
     def __init__(self, namespace="ml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
-        self.__temperature = None
-        self.__latestTime = None
+        self.temperature = None
         self.__json_out = dict()
 
-    @property
-    def temperature(self):
-        return self.__temperature
-
-    @temperature.setter
-    def temperature(self, value):
-        if isinstance(value, (float, int)):
-            self.__temperature = value
-        else:
-            raise TypeError
-            
-    @property
-    def latestTime(self):
-        return self.__latestTime
-
-    @latestTime.setter
-    def latestTime(self, value):
-        self.__latestTime = value
-
     def to_json(self):
         self.__json_out = super().to_json()
         if self.temperature is not None:
             self.__json_out["temperature"] = self.temperature
-        if self.latestTime is not None:
-            self.__json_out["latestTime"] = self.latestTime
         return self.__json_out
```

## ml/ml40/features/properties/values/value.py

```diff
@@ -19,14 +19,15 @@
     def valid_to(self, value):
         self.__valid_to = value
 
     @property
     def valid_from(self):
         return self.__valid_from
 
+    @valid_from.setter
     def valid_from(self, value):
         self.__valid_from = value
 
     def to_json(self):
         self.__json_out = super().to_json()
         if self.valid_from and self.valid_to:
             self.__json_out["valid_from"] = self.valid_from
```

## Comparing `ml/fml40/features/properties/values/tilt.py` & `ml/ml40/features/properties/values/tilt.py`

 * *Files identical despite different names*

## Comparing `fml40_reference_implementation-0.2.7.dist-info/LICENSE.txt` & `fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fml40_reference_implementation-0.2.7.dist-info/METADATA` & `fml40_reference_implementation-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fml40-reference-implementation
-Version: 0.2.7
+Version: 0.2.8
 Summary: fml40 reference implementation basic functions
 Home-page: https://www.kwh40.de/
 Author: Kompetenzzentrum Wald und Holz 4.0
 Author-email: s3i@kwh40.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

## Comparing `fml40_reference_implementation-0.2.7.dist-info/RECORD` & `fml40_reference_implementation-0.2.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+dt_templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dt_templates/chainsaw.py,sha256=ton9eRu5l5tL1mUuB_qPFVq_hFT9y1kBW5XHr54lI5M,979
+dt_templates/forwarder.py,sha256=kLqICn3w3ld0uHQEf-NXAoKQcKRNY9VE0LMDfACTzFc,2259
+dt_templates/forwarding_agency.py,sha256=WtzUGqHobuvUcCDinJRP244aSlRx0ghX2geZ0kxlRgI,996
+dt_templates/harvester.py,sha256=RhAG2dMWpGKFR-V4AywtNnynDcJ86k_SLzILjWXIF5w,2139
+dt_templates/sawmill_entry.py,sha256=oKpTDaM_x3wzufint70kvubJVbiKTmnKf11J6XaYv6U,988
+dt_templates/supplier.py,sha256=m2K2wCHrMev8eDl8lOaBJEl99rXE-mUn0PrE0xWEEI4,979
+dt_templates/truck.py,sha256=I1sZ67G0PEIn_GEAhXyMT3I_azZ_logNN9xi8t5WfSk,2119
 ml/__init__.py,sha256=QlspklRgPqi7uUxePGa-uJuTWPcwL0qHImVpbQJQKFs,360
 ml/app_logger.py,sha256=lsICIYTOADyMnisDaI2_KO1mGVFxkl1OYSsNK3JTlE4,1039
 ml/callback.py,sha256=PQxNdevMdI_fEUsAmRKNpZmnZs5MqY7ZTUx8vIZW1lw,2934
 ml/ditto_feature.py,sha256=OjvKNRSYYNxYW1QgbwSeLHPd2xxTFUud2CEFt2U46Fk,693
-ml/dt_factory.py,sha256=x7uSBySqAkT_8dTxXjRkS9-F_3otpteI9pCK6kbWGFY,24704
+ml/dt_factory.py,sha256=qYAiS5C-Oi2rkFt4oP7K5wgN-LCPXAKLG1tL0VPEaX8,33091
 ml/entry.py,sha256=Q6OiJO8Vwj5ztCtYXaZSb3BzqmIyHgkdWp0iv6I3kGM,6088
 ml/feature.py,sha256=Z1q6sb0V0Buk3HvSSISOQfapZMsWxP2htKiIPv1g1xk,3794
 ml/identifier.py,sha256=4tVvLEH8fnLHAWe1rfuF3QuPd-TvMbaAElKvo7K5j3s,1254
 ml/parameters.py,sha256=GiK3n-AavnRy7Myz2LVlkvqSyZD7oJrPmqd0SfgNpHI,4598
 ml/role.py,sha256=gkK2-7QlARGICzjKwVxfcxvGm1BzZzTaPEVUbgXh71Q,2120
 ml/s3i_tools.py,sha256=e1TIqxspHw5-qOb3ptFbJb5hWVidI-0VMMVIqFvUXV8,8249
-ml/thing.py,sha256=SAhNiIJ2tyBAq-nokVAYQGvE2VXasEARauoAO2ufzoQ,32546
+ml/thing.py,sha256=TvVOyICgYLRLhBd_2s3TgnqiHFAQa0Q1rVs6tOTrMac,32710
 ml/tools.py,sha256=oIyixHmXwSsghka4vdIXPE6ofr_lmyNl-_hzZu4A-jg,10355
 ml/fml40/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/functionalities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/functionalities/accepts_felling_jobs.py,sha256=OG8fmKM8HeetsZQiQngdkpE8nfIgd99oV_2TzMvM8dU,1635
 ml/fml40/features/functionalities/accepts_felling_support_jobs.py,sha256=lLVssji7aut_7IzFKeg9H175L27_5tLCfNmoQOEB7mI,986
 ml/fml40/features/functionalities/accepts_forwarding_jobs.py,sha256=VtigSxGp9TZBaoSsmjZWQ47BtC-pVPtgDAk_R_LUotw,982
@@ -22,89 +30,113 @@
 ml/fml40/features/functionalities/accepts_moisture_measurement.py,sha256=i8zKb0UFe-crKrlnkN1ZtbuKydx5LP4yEiLe7_H2Hp8,872
 ml/fml40/features/functionalities/accepts_move_commands.py,sha256=kxMZiUWQVrdDOhlw52RTDaSbpkwNcAOUhCXWAQglk9I,960
 ml/fml40/features/functionalities/accepts_passability_report.py,sha256=a449SYeo5DMWTgVAW-zPSldwwhL2WJza1ypUDGh02dI,501
 ml/fml40/features/functionalities/accepts_proximity_alert.py,sha256=KrfSCbcLY8j5leHI__6rBHP1v-ok45XfsqpKRP1UN1I,712
 ml/fml40/features/functionalities/accepts_shield_commands.py,sha256=WuGYv-Y2MvtjYU8gXZIqOkdLnswDNoe0ZhycDl9gyvc,994
 ml/fml40/features/functionalities/accepts_single_tree_felling_jobs.py,sha256=RI0igTsjqrIWW9nK8G_RBF40dMNJDEp3iQmB6xFdNEQ,583
 ml/fml40/features/functionalities/accepts_winch_command.py,sha256=SKQ0aky32cKwqaK1Us_cHHuRpf2VY-FGZNw4FZ4_dXg,992
+ml/fml40/features/functionalities/calculates_machine_operation_cost.py,sha256=wVrnD5ijxGM17hj1mzdVK8cNwAp3icMBFRSkhAd9sjA,404
 ml/fml40/features/functionalities/classifies_tree_species.py,sha256=IGtyo2JJMo8W3LTY4VvLEP2uP-mrpqZ0aU_fjVBs_Hs,830
+ml/fml40/features/functionalities/controls_sawmill_production.py,sha256=F1ESPVIFr-ul6tZULcSIngZQDaxqeX-7eVkTPDnOHXA,357
 ml/fml40/features/functionalities/converts_data_formats.py,sha256=asiMttzY5r0Z0Ae2Iwbss7AjRKVGhJg13X1e28Dl3SY,314
 ml/fml40/features/functionalities/converts_forest_gml.py,sha256=4wUKKfQ0J4AnV6kB29Dc8HgJ4FxXHwWIaXLOYuc0_Ns,333
 ml/fml40/features/functionalities/converts_shapefile.py,sha256=-FTyWWqFYvzvZJSZobDltKWNgpZ3n7-vSYod0xiYfJU,333
 ml/fml40/features/functionalities/cuts.py,sha256=elyaf4IDS_63oq6jiqnniJxpaH9FR5vxTPLO945rRTs,498
 ml/fml40/features/functionalities/determines_passability.py,sha256=Wc1-kP6t4m8tXJS7TMLmmh98a2-Re04ZrGH5eKjcpNM,1646
 ml/fml40/features/functionalities/displays_health_alarms.py,sha256=U9y6GwBVho_Lg9AJA5iys5xZATnUqLsp9yKMkS2NPKA,544
 ml/fml40/features/functionalities/evaluates_forest_rating.py,sha256=UEwft8CY8jeXTrEmfZeUOU7hxMOhiHXpX4W6QJibXUE,316
 ml/fml40/features/functionalities/evaluates_stand_attributes.py,sha256=wGzBL5UEpHTsNEOJjT6qWZBrrYa7_GsZehw1dnyjzYo,693
 ml/fml40/features/functionalities/fells.py,sha256=fPLrhLXi_HutYWekUIR6nE0H06DKvi-OGkFb1a8tH8s,1209
 ml/fml40/features/functionalities/forest_planning_evaluation.py,sha256=0yGkMyazKL6DloyLWqkRxnkI3A3BdreF0oE4b9ZTtYI,556
 ml/fml40/features/functionalities/forwards.py,sha256=Q1-VeFA1p59YtbmWdoPMjd3TY8wRxpcYwX2UEhcIsoE,982
 ml/fml40/features/functionalities/generates_afforestation_suggestions.py,sha256=ira_5RLpbXjNFi-iWXDbU7f5nQh__NqA_F-3VCDdJcM,960
 ml/fml40/features/functionalities/generates_felling_suggestions.py,sha256=jwxoTv8iOSuAabeUyFSnnQutuS7kSVe0jvDZTUp9Aq0,829
+ml/fml40/features/functionalities/generates_log_delivery_note.py,sha256=vvx9wVrZIL5peKX0j2TRQvu8Pp_RzaNsOnxQZDNnUh0,646
+ml/fml40/features/functionalities/generates_log_loading_note.py,sha256=O6ZltihUr9x9D_3HHaeQ1R3bH9kYqQ0p9C6DrzGZSe0,644
 ml/fml40/features/functionalities/generates_typical_single_trees.py,sha256=PMFEC9KTAmZAnvHiNaMheaEh3FN1eIxkfbtg9RCecRc,322
 ml/fml40/features/functionalities/grabs.py,sha256=l0l5GHrtY2uVo6-C_t5ZLnh4v9eraSYFQmzCP7SFJB0,369
 ml/fml40/features/functionalities/harvests.py,sha256=ixFfhSRszMyRUD8N2eI6qyGL6zQkLgCq2w70b-wc_UM,493
 ml/fml40/features/functionalities/measure_wood.py,sha256=8eRR0UsRloOoNMvEmxA3BkIu3STKc56cH6x-8IvdlaM,471
 ml/fml40/features/functionalities/monitor_health_status.py,sha256=1e9kwy99ENS8FhxUhvz63EOn_L5iHSHFvg4p86lB7Xg,365
+ml/fml40/features/functionalities/plans_harvesting_job_list.py,sha256=ugOZC6L8Di8JZjyKVeA1VzmRFz0h3X7xhqSofP3Umcw,328
 ml/fml40/features/functionalities/predicts_forest_development.py,sha256=rNtfv_Cm-sur5zVKAycxv3sleefOQB4FswHaBA-e5ew,298
+ml/fml40/features/functionalities/predicts_maintenance.py,sha256=D97vbnIvWO2zAIRNF_pGvUECTANGR2ywjbEG3yOQbg8,329
+ml/fml40/features/functionalities/provides_emission_data.py,sha256=BKEiEdBlo-wCjjA1wqgk5Pa7Td-gINyHn3CaytwwZzA,338
 ml/fml40/features/functionalities/provides_moisture_prediction.py,sha256=JsGTDMTQyR13j3Nsmh6RpdeBDhODtrFgVYR0jmgUqxg,511
 ml/fml40/features/functionalities/provides_passability_information.py,sha256=xiM3bW9Md9xibib1sb8CEUN6FP37G3Um1aiU3cCOE08,391
 ml/fml40/features/functionalities/provides_production_data.py,sha256=umLJ05HwdkMpXY5UFrESFS53YoyHQ_KQQPDZOa_rjaE,515
 ml/fml40/features/functionalities/provides_soil_data.py,sha256=RGUv2e5P1WCsZMWIRxVIjrLVyaO1kAy_guTy1TcL5t0,875
+ml/fml40/features/functionalities/provides_stem_segment_data.py,sha256=YjaZ6v4uEgRhfsrhNoUysE3qfV0JqxZMuAB0DQ34jcA,447
 ml/fml40/features/functionalities/provides_tree_data.py,sha256=XXaziILTFrjMIdpqF-_xvlzIRbzNKCSO0MV_g0OLRcc,624
 ml/fml40/features/functionalities/provides_weather_data.py,sha256=eVPUtiDgAXkakCfSK2y97P6Bp0zuJdRvyJtQFijOCrc,314
 ml/fml40/features/functionalities/simulates_tree_growth.py,sha256=fcUFzSlHilr3_MQ6RGsBHGc1y42OQ4jrdGVz5hyDha8,314
 ml/fml40/features/functionalities/supports_felling.py,sha256=6w6JopbJOM4Ckebbdhu82oawTsRwzU_GUBjI3JvwK8w,469
 ml/fml40/features/functionalities/transports_logs.py,sha256=3H7kbezsyGP4Qo4lUhwc4VonBhGkvKZuQfh4LjtBPKA,767
 ml/fml40/features/functionalities/visualizes_forest.py,sha256=IRKtYPPf23t2wv0g6nhhlv_xSbu6f5zz3JrOKjZfSPY,289
 ml/fml40/features/properties/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/properties/values/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/properties/values/abstract_inventory.py,sha256=NWZ4bC3SKxqThzsK1WzQif9BxZOWID6XiKhXEL-RQiU,133
+ml/fml40/features/properties/values/allow_wood_delivery_time_slot.py,sha256=1g7JQ6MjEs5gxyuAwJqUlJDjf-l3-FflqmGA3By88eM,308
 ml/fml40/features/properties/values/assortment.py,sha256=nLMja-rwqv1Fv7r5flTniTzmFRNCsFTs5AwDSuw2Pm8,669
 ml/fml40/features/properties/values/basal_area.py,sha256=17gh5rWibugM-kQrm85-QXd4R436U3sdkpElmW3ewgA,653
+ml/fml40/features/properties/values/climbing_ability.py,sha256=yAj_VItWJ1SU79jl2P-IghddGO_UhrWRxWxPMVGUAEM,531
+ml/fml40/features/properties/values/cost_index_low_loader.py,sha256=St_KHZQsR0kZpPXSK2UT9tCNLsA-N_dqQPsXV247Fs4,288
+ml/fml40/features/properties/values/customer_type.py,sha256=k6LW3hSw7JXT8xWSBacNS_y7yuuKnV6SECjlj_QSiDk,130
 ml/fml40/features/properties/values/dbh.py,sha256=JTCGfeawQMYXLbKJtz_W0Q1PMJFfZcsVttxCAeJ4Qqk,643
 ml/fml40/features/properties/values/dominant_tree_species.py,sha256=LkxapxuAnyudMYO2K10ZMcm7YfdhiisqYEJCHNO2SKw,292
 ml/fml40/features/properties/values/fell_indicator.py,sha256=bd8_S6qNmkrXv7mIT8_UWDocz3gOMLbFPLNy0n4w-Vc,660
 ml/fml40/features/properties/values/felling_period.py,sha256=LNk8TidqdvMvmvFkor8L_1r6nNgMKlOlFUWlw1WMPRg,896
+ml/fml40/features/properties/values/ground_clearance.py,sha256=PoVFnRPvM3lvRlvXXNdsat6IS5VoXV1uk7QQY9WEmYY,615
 ml/fml40/features/properties/values/harvested_volume.py,sha256=QiLjetrGQTPusweE-mQe3bII4zuTHxdb1AFumRvoDpY,659
 ml/fml40/features/properties/values/harvesting_parameter.py,sha256=d1uF3bsSDNdiznPKYtiM1TqAhnz_cKPnbk4zXm74vhM,759
 ml/fml40/features/properties/values/increment_volume.py,sha256=GYh96wcfMpKHs6fLi5vT3Q9yTtn3Nm3XoBKOP6nHfek,288
 ml/fml40/features/properties/values/interfering_branches.py,sha256=dHc0D-cpdQeyJ9i9fveoCdNExyVC8HGAMETpsVWfSTw,679
 ml/fml40/features/properties/values/inventory_data.py,sha256=-xdu3K4ATIw5sbEZAlR_Cl0Yq94vZqqMP_7vThYeUWU,718
 ml/fml40/features/properties/values/is_felled.py,sha256=54DxU1rlPIiPlCojJgwAkF54lJcUnbh6WgzbnwwqpYM,652
+ml/fml40/features/properties/values/log_loading_length.py,sha256=82Axp3hC8fSmtnqr1dxG6LzIUIF-ywWWR939dZhvTSU,677
 ml/fml40/features/properties/values/maintenance_data.py,sha256=IOvAsT50TvjNh1uggBYmx-mSUxrVxAuwBzmLEKVF-5c,1182
 ml/fml40/features/properties/values/mean_height.py,sha256=Cnx0S82Q33cypAjuol2y81kYyKcMsTXw5n0e3LI-kVU,283
 ml/fml40/features/properties/values/number_of_stems.py,sha256=9I9CpwskqAbJOvbiiqEIOzRny6QjkIGvxypdo2Bia4s,286
 ml/fml40/features/properties/values/overhang.py,sha256=sKCK_OjVRDpvqSz0Lc6aMuvm0pSKLYW2S3TWNoeCF_g,695
+ml/fml40/features/properties/values/sawing_processing_step.py,sha256=lkN2qTqrI1Nq---rCMVBbA4CmjsOzy2Tvu-WFHix9pk,562
+ml/fml40/features/properties/values/sawing_processing_time.py,sha256=uFRgMBHlH9_Y3ER6vdfby__NbsCS8kBLGGGuvIGXpPo,567
+ml/fml40/features/properties/values/sawing_setup_time.py,sha256=JHpOh-wjHC2EJt3B3lJ4uR69BLP5lJHuoqeO2aWzrEQ,284
+ml/fml40/features/properties/values/sawmill_delivery_parking_area_status.py,sha256=1cL7_72TWgOCGiibZVSUwbrNc9VB2emx5PjHpCYRdu4,307
+ml/fml40/features/properties/values/sawmill_entry_parking_area_status.py,sha256=FPH4rr_mH4bvxoYujJF63PqIrVc28hYUQ8hM8cjZRg4,304
 ml/fml40/features/properties/values/stand_attribute_set.py,sha256=wB0lXJkBTh6RjFr5nNAOIaJnf-DPHkrjkCy8LLoqh5g,268
 ml/fml40/features/properties/values/stem_segment_properties.py,sha256=TL_CKO-QqYtyGxD9kdzKsquiIPGdlPg_9c5dpHb07YE,1502
 ml/fml40/features/properties/values/stock_volume.py,sha256=jT1H1NONCDtbpGtvggoPlc8N8YKYhVV94z6o9TTuJKc,657
+ml/fml40/features/properties/values/suitable_tree_species.py,sha256=0prkntmaaoFufi-mcijw_gS4vei7bnwM86r6e4ayHxM,312
 ml/fml40/features/properties/values/thickness_class.py,sha256=tMhnDWmXpv9u7qddXpgNPgmZATHzUJIQmP9bJQfL6Fc,287
-ml/fml40/features/properties/values/tilt.py,sha256=_K1H5FtxDUBLNYL6tqeOtyFl5S7CqG9UcbT1683THhI,944
 ml/fml40/features/properties/values/tree_data.py,sha256=TLVkUsce2qIIggxNz62fYyDMulcgqAC-meLj5cTa0Jw,281
-ml/fml40/features/properties/values/tree_species.py,sha256=6tvPpEHZRd0M318jn8vqZjACJkuUUd2OaMg-lJgFzzM,284
+ml/fml40/features/properties/values/tree_species.py,sha256=SVlhlsf4t6JGNwQXVk8EXfv4Z-5M_7NpBVUjBl1Hjrs,700
 ml/fml40/features/properties/values/tree_type.py,sha256=rpClFBJElYLKn_lwn5YymANRjJjAB4lYT1QEV04WEKs,684
 ml/fml40/features/properties/values/vegetationindex.py,sha256=A6n07rGC8InBMYrsQAI4m5bKqjUFQk1Fw_ogE9OHJjk,3165
 ml/fml40/features/properties/values/vitality_status.py,sha256=kXha5zwQknosLdyOiuZKWvwI7enpmRI7Nocs3d-p-VA,649
 ml/fml40/features/properties/values/wood_quality.py,sha256=zstocRCM_wKMLAN-slmUPAwWki1rh21zWH2gsBXSLiE,284
 ml/fml40/features/properties/values/documents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/features/properties/values/documents/contracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/features/properties/values/documents/contracts/log_procurement_contract.py,sha256=UNkiICo3dTiexFAQggzUIIUjctqu1bDyqVfu7iPmeoI,323
 ml/fml40/features/properties/values/documents/jobs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/properties/values/documents/jobs/felling_job.py,sha256=OLqze8EN_tdQjCC-CzOIjN-d1G2u0wJF2I4iYrUgy1k,242
 ml/fml40/features/properties/values/documents/jobs/fellung_support_job.py,sha256=ioOdCl__l7YQanEo7Qt9CVeW-J30CWc1j9A_dz1Easg,249
 ml/fml40/features/properties/values/documents/jobs/forwarding_job.py,sha256=n2cA8n7z1DSrVzCDfWCTBj1SPHovyAkikP4MstcQqHc,245
 ml/fml40/features/properties/values/documents/jobs/log_transportation_job.py,sha256=_2bQh0swt4YYImEsdQvQSkQOI0rRrvQyX5ofehhwqQ4,448
+ml/fml40/features/properties/values/documents/notes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/features/properties/values/documents/notes/log_delivery_note.py,sha256=KIgQIxjTTyUkDheAVscWbW0OF4MKduWsbmRMxuhA6Oo,300
 ml/fml40/features/properties/values/documents/reports/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/features/properties/values/documents/reports/afforestation_suggestion.py,sha256=806xcaCxKpCMOWjnG0bWnaOOePmjq7XEjJPqCDNGJCI,267
 ml/fml40/features/properties/values/documents/reports/felling_tool.py,sha256=x9ea_ChWB2EBfrrS6WC-w4ZWKqyOEpkk0cxuSpEG_TA,77
 ml/fml40/features/properties/values/documents/reports/log_measurement.py,sha256=wYWSxMmx5MB43mBZC60dIZ0X3_co0fYwHnuJ6X7cKSs,258
 ml/fml40/features/properties/values/documents/reports/log_transportation_report.py,sha256=68Cb0LoPSInmQfUEsxr_Y6T1WuyPCBkJxW9T9hu_WfE,267
 ml/fml40/features/properties/values/documents/reports/map_data.py,sha256=WUGaEgbblJ50AhZH2XLttbxdCjitX18wHNd9tNNuyRw,251
 ml/fml40/features/properties/values/documents/reports/moisture_prediction_report.py,sha256=o-1IcqTi0kExXgVIzhZywro1OnZNkonVYujGmaHw9Xc,268
 ml/fml40/features/properties/values/documents/reports/passability_report.py,sha256=jnfzcEWODV0Sl8ZD1ppuZ4GzOuq3xpYeq34OWnx1_4U,261
 ml/fml40/features/properties/values/documents/reports/soil_moisture_measurement.py,sha256=itEVifSSC4ztugkfLs7nvRClmQoyge-OA2cdEvQqc2w,267
+ml/fml40/features/properties/values/documents/reports/wood_certificate.py,sha256=Cqpdt29BY6xp0d69tj24MyQnVz5f4kUu_JUHpPlfggU,259
 ml/fml40/roles/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/dts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/dts/forest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/dts/forest/forest.py,sha256=2TfmOKrwXP_9eyeihpyL8-c2cbOwzWU2mBMz_VYarOI,253
 ml/fml40/roles/dts/forest/forest_segment.py,sha256=u2jb0jLhLswpz-AIT4YN_jnZY7ZAd_2HHxHAaO0EvaY,258
 ml/fml40/roles/dts/forest/tree.py,sha256=VF7-mzKpWI-Q5vkvVBjXht5PJbfK8fjjNdM5ubAtrZ8,271
 ml/fml40/roles/dts/handheld_devices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -115,21 +147,33 @@
 ml/fml40/roles/dts/machines/forwarder.py,sha256=wxlm0_33Mez2SAgRkF0zuud0z4bOqzpB_ulGvLHtnIM,300
 ml/fml40/roles/dts/machines/harvester.py,sha256=7DP86fs_yhhjm_rnvZQLFza6MDTKXr2rAxTywxOx56o,300
 ml/fml40/roles/dts/machines/log_truck.py,sha256=6Tw2K4MDHo8peBSkQAI9k3ZH_V2bt3Pu89g5R6gE2kk,299
 ml/fml40/roles/dts/machines/mini_tractor.py,sha256=32S42qOX9ngSk3eKd_uR4Mej6oX039k81MTsV7uwj3g,280
 ml/fml40/roles/dts/machines/skidder.py,sha256=oyDrp2nQAHYlQw_O_ic4j7ZIKeOIPO2uejlQRWoqU14,298
 ml/fml40/roles/dts/machines/wheel_loader.py,sha256=rDt5QXcOCOGPhY3FmDVIr0RZW0NwTLIcmkcS0oTZwIE,302
 ml/fml40/roles/dts/parts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/roles/dts/parts/band.py,sha256=FXyltOPi-5oxNpfvar4ChgxQ2nVQZQYcQnuQW4y4sz8,263
+ml/fml40/roles/dts/parts/clam_bunk.py,sha256=NIeKXX9k52WTQ87HwPYbV53yjGLKwkMLEoMNJXAsZEg,267
+ml/fml40/roles/dts/parts/front_bogie_lift.py,sha256=J5J1WiVYcRsVPAlbwSs5MB91pKHael2bhDUNkJUbOIw,273
 ml/fml40/roles/dts/parts/grabber.py,sha256=KyVS_B0M_JySoav0sLTQbDvmhe3HHy4Lef0PWXfbTvQ,266
 ml/fml40/roles/dts/parts/harvesting_head.py,sha256=_oe8vjoDPLJlYfQMeGzOfh5OGkp7kCfxIX5zb61BjAo,273
 ml/fml40/roles/dts/parts/log_loading_area.py,sha256=EG-E1K6ZoxJY8KeZd749fLEi4zmWZOQxvW0SozL4_HY,273
+ml/fml40/roles/dts/parts/rear_bogie_lift.py,sha256=CPk4b2Svr4aPQhqco0NOWBrtOwZEdleloALNTIpwrTE,272
+ml/fml40/roles/dts/parts/rung_basket.py,sha256=Rf4jfyvU1OBfR4oWg1EaK0fwtda8KdwlQsM5crFxJVk,269
 ml/fml40/roles/dts/parts/saw.py,sha256=qmETVxAWX33RZw-KVh8j01hEin3fqfLF7P-Et3e1f9w,262
+ml/fml40/roles/dts/parts/sawmill_entry.py,sha256=EMAraUJiYrH67O2H0J4krytQw1uiLgVoM6queYxTMZg,288
+ml/fml40/roles/dts/parts/sawmill_entry_scale.py,sha256=0iR6A0n3j3br0nPwaOlc4J6TUWWkBmogrjX1WxelOa4,301
+ml/fml40/roles/dts/parts/sawmill_exit_scale.py,sha256=UUFvyZFuIcylT5qVc6dXSGB7YnEZeWx2XgzumDYAyI8,299
+ml/fml40/roles/dts/parts/sawmill_gate.py,sha256=Ph9XHq4hOK5qARzzcQkkTG2B-a7uU8WrrFDUHL5-99w,286
+ml/fml40/roles/dts/parts/sawmill_storage_area.py,sha256=cmmjWe7-xSw2o64FKje2uH7D2RePM1l-Sv7bFFFjc0Y,300
+ml/fml40/roles/dts/parts/skidding_winch.py,sha256=vvjOZEhvCA1J_CBqyKQ8c_ZV_B0oDaCltpSkhT_-4j8,293
 ml/fml40/roles/dts/parts/stacking_shield.py,sha256=0HWNDnUUlldrOyy59212NdlVJRR0uobG0PaD6W71TOs,310
-ml/fml40/roles/dts/parts/winch.py,sha256=-f7VUeU1-ptf2SgDXoq4ibkql6cQK7hoDwfFQZqCmXM,264
+ml/fml40/roles/dts/parts/traction_winch.py,sha256=NjdvNxKOBDRmRymhOQEwWiZWigFuvao2EHu8Io2yES0,293
 ml/fml40/roles/dts/persons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/roles/dts/persons/chain_saw_operator.py,sha256=T0Px3VfvwLrryyj8OezCZ0fscRLqbLXp5hREIg0iO9E,283
 ml/fml40/roles/dts/persons/forest_owner.py,sha256=TncH6gnNaBbdIhH84HGzjI7xcauWF4B9pQGl314NNIQ,278
 ml/fml40/roles/dts/persons/forest_worker.py,sha256=eySniKuBGVW1zU6ySffewDPvXwvjhAuIsx7dzAbW6j0,257
 ml/fml40/roles/dts/persons/mini_tractor_operator.py,sha256=YKL7ULYYVu0p1kKos0bVN2rYaI_igvajsqlRTpW3Jd0,286
 ml/fml40/roles/dts/persons/skidder_operator.py,sha256=xQSUyc0NbYsTtrmNR_ujCu63wmxLM0xUrYdlCKWHwHs,282
 ml/fml40/roles/dts/sensors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/dts/sensors/barkbeetle_sensor.py,sha256=FqoFzBESQhryBUyOar4SxtPJPGe0unMDX4GSvZAETh8,283
 ml/fml40/roles/dts/sensors/calipers.py,sha256=3rj0crwg_RZ4NjkBUa_eoCZt1SnVyPoRLik03kZ66eI,225
@@ -138,128 +182,196 @@
 ml/fml40/roles/dts/sites/forest_enterprise.py,sha256=XFxVht0Z_PW_Sunyg5W3Kc3-y9B-_7PVyIc8l9LMcLI,275
 ml/fml40/roles/dts/sites/hauler.py,sha256=bLDvSzgTeQd1OshAI_sbcRXQJ44IV8QKE1ll98jm-dM,265
 ml/fml40/roles/dts/sites/mill/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/dts/sites/mill/mill.py,sha256=bWWVhUVE0u45s2W4NgoI73QIL0STPtKaVR5dCHTihLk,213
 ml/fml40/roles/dts/sites/mill/papermill.py,sha256=h8GRvBaEN9eouYvS1fCAdV3SBsw0D15n52rRjvJuK8k,224
 ml/fml40/roles/dts/sites/mill/sawmill.py,sha256=j7YBr18_vVi65CJVb0lJgVC7ftCqNzBZzZVG44p4OU8,222
 ml/fml40/roles/dts/ways/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/roles/dts/ways/forest_road.py,sha256=Z6TR-G0nOuzZo_9CzRCUfHWuMg4iyvIuNoMzIsfsNiM,265
 ml/fml40/roles/dts/woods/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/fml40/roles/dts/woods/log_loading_unit.py,sha256=1Yn6WnywZSX3ebSIjiqbaJxK_oGjEYQbrlHFj2HY25o,274
+ml/fml40/roles/dts/woods/loose_stack.py,sha256=p2xqnaKZgvMUdBohLIKtIAqBK_JWFDoe4VVfa6MglpY,270
 ml/fml40/roles/dts/woods/stem_segment.py,sha256=w4elNLCNSdacrBSyspHD1ua69xLnVyvKv2izsBHZOio,271
 ml/fml40/roles/dts/woods/wood.py,sha256=7ZZKRsiP3-18faQmhNr0pMW-w0wtEX0MRJHNquohtFw,251
 ml/fml40/roles/dts/woods/wood_pile.py,sha256=JA1OMclulXEFE0KFillDM9uQE0mF0mLtGdEjZRHTjkQ,268
 ml/fml40/roles/hmis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/fml40/roles/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/functionalities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/functionalities/accepts_jobs.py,sha256=MxfoCdi-ELnb7Cwqh2q9W6QbjrNBC0UhtFYBn3PdCyo,680
 ml/ml40/features/functionalities/accepts_reports.py,sha256=5ExZtfvs9K5dkvrSiF6QZDjHpfNzaZeTeOSVLyZZnyg,471
 ml/ml40/features/functionalities/clears_jobs.py,sha256=kXzb2WDAipPWjxHKh0y5qf6FlY98PO4Zs7wikxA4xh8,427
 ml/ml40/features/functionalities/functionality.py,sha256=hseOzQH126xKMurdFSVN_s2g_HUD_Ju7g6ZUTo3VUe0,330
 ml/ml40/features/functionalities/manages_jobs.py,sha256=33Jd3bPufS3-ED0xneQTx_DwIubN1ZGYBYoLLOJIzHE,633
 ml/ml40/features/functionalities/plans_routes.py,sha256=KWaKgLgdD0ScXrlI19bMHVzLj1x7OkPpZiNIijiPnps,510
+ml/ml40/features/functionalities/predicts_consumption.py,sha256=gYOZS9018MUg_dJ3XEYST1If7jSAgEcRACiSpVU1K8c,377
 ml/ml40/features/functionalities/predicts_maintenance.py,sha256=XD4QCnjSZGMaYRcMjFsVqhNnh2S95iYyxKqyLWZNLC8,377
+ml/ml40/features/functionalities/predicts_purchase.py,sha256=WxTWhiMrrBjjNJAM1EvlCLYVzMXjfjm9AnRujbBVD88,327
+ml/ml40/features/functionalities/provides_emissions_data.py,sha256=Ou_LzS3Jhmc2Db5WpRFZ4HBj3HJKNfBp8WONQLhqNpg,387
+ml/ml40/features/functionalities/provides_machine_data.py,sha256=hHQNQF93cz1UUMuVAvIU5CrTOgLD8oabPlamNNzMWtM,384
 ml/ml40/features/functionalities/provides_map_data.py,sha256=H-itYaLRB7yrM3V-UF1fHBifRLgSf9kFTR6NUrKqZLg,515
 ml/ml40/features/functionalities/provides_operational_data.py,sha256=HU1kXSMMY7WHQHR6TkWwBynw3m52699-9mA9LCuAqnc,482
+ml/ml40/features/functionalities/provides_settlement.py,sha256=AZAadBHH_98RNWl5s8Y6QehIwfpuggima9D5Ucpkbdw,340
 ml/ml40/features/functionalities/provides_weather_data.py,sha256=GQ9PllJpd7luaOzIEsaSbNbBFR-SYahnip5cVps-jhQ,656
 ml/ml40/features/functionalities/renders.py,sha256=DWlH1bJqm5dfAxrkbKF_NyF52sGrp-g9lQJyqttGToE,398
 ml/ml40/features/properties/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/property.py,sha256=Ul3rmY2ptnOPpdnkJCukTJWvcd6HvHmjF27nzgwjA8Q,268
 ml/ml40/features/properties/associations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/associations/association.py,sha256=4gIrF-Tt9kea9N6QtN2G4SZa4-xfoDJUqaunlx7VcI0,285
 ml/ml40/features/properties/associations/composite.py,sha256=-lAuPSnNtk58o06PWFE1GG-BwQp9_4xAaKSYCdPbROg,805
 ml/ml40/features/properties/associations/shared.py,sha256=oPkJEhC9JZ_xXs6KMhkyC89isfT2HZYKp4mk4uoch8o,865
 ml/ml40/features/properties/values/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ml/ml40/features/properties/values/acceleration.py,sha256=wCwg2XEOti0oyp5Hh9KrCzSIe1fk8VZ33rElfM_Sejc,284
+ml/ml40/features/properties/values/acceleration.py,sha256=tEjmWjmXkAqwfO94AbTk8x_9SDNiYNsHQHXhlwvprpg,700
 ml/ml40/features/properties/values/accoustic_indices.py,sha256=Cz--j5gloIYRSYV7wyYGCTj4TrvS0BL0QDU5Wl4csEk,287
 ml/ml40/features/properties/values/address.py,sha256=UjrbKJMloafMO-lZhrF5FFh0WXAB7NTeudrkKQdcIDY,996
-ml/ml40/features/properties/values/air_pressure.py,sha256=h1Bg71vtzoziNKH99oHvo-VIuwVAwoFgxPnWLRfNfI0,283
+ml/ml40/features/properties/values/air_pressure.py,sha256=XzJah_YWnQlJNRaqYftmuzKQ3SJbR8xE_tbX6kjPpJo,537
+ml/ml40/features/properties/values/air_volume.py,sha256=P9zP6XZSAY2v1TBb3oCoKjA28bI9Vxi4pY8e_lqVmNI,528
 ml/ml40/features/properties/values/area.py,sha256=0IBAtAeQtX8UwMTVK6JrC0-2Cj5qjD2rhxLWZe-qRzM,276
+ml/ml40/features/properties/values/bank_account.py,sha256=ZPihA14Zyi7JCRoYTwiGt_L3KP2P5Hg5G0og2jG9BVg,769
+ml/ml40/features/properties/values/brand.py,sha256=wxKk08jevADlf-ivC-OWcw2pUA1FY2PDgHb6r1n-GbM,516
 ml/ml40/features/properties/values/brightness.py,sha256=beMCxTOrKMoxaXkMFa-X5QSR_oNPKPDZ4xLMG_3ewFI,282
+ml/ml40/features/properties/values/contacts.py,sha256=dYC4Oxg-RPT0WfhkLTBifIWcNmQtpgI1ardOaPwgp50,315
+ml/ml40/features/properties/values/cost.py,sha256=2vgTf-umhBXHoWjLZcv8OEIoMpJsglHCkMN1lbzLcwk,515
 ml/ml40/features/properties/values/count.py,sha256=rxgydZ4hyHpuVNxkykpARNyIE_edwmOMbh0dKYtAu9g,795
-ml/ml40/features/properties/values/dimensions.py,sha256=QGFeWa1z7CcAHIoFfqIExgAi5slhYsrZSr2fww6k2aI,872
+ml/ml40/features/properties/values/current_load.py,sha256=GAUth78GEQPJeW6JTTEDxJSThhF7HhwOQP7zpUuccDI,280
+ml/ml40/features/properties/values/current_weight.py,sha256=5j9NCco9k3iNblxXjNf0edhHPUkBHD-50sIi8-yaXds,288
+ml/ml40/features/properties/values/description.py,sha256=lhZA1OTrXnk3QBGfdeNxtOqFr_JWNiyQIF4HpehYkQc,526
+ml/ml40/features/properties/values/diameter.py,sha256=kLQi7P5U5jyVkDRkpfEraNHpXO20ycx4Fgf_YRqLhOY,524
+ml/ml40/features/properties/values/dimensions.py,sha256=iuyTG-pWgdN4wSEn8R1lMAAKXRE4rGxn31VKg3od0Uw,757
 ml/ml40/features/properties/values/distance.py,sha256=owX4JBrcxMNoMyiLl7cobU8TnZroF4azCJq4eehIpRg,663
+ml/ml40/features/properties/values/empty_load.py,sha256=qsCPSdjJR11ac3kRatEXWdPw9TMSK8gwDP5F8MZI4bk,278
+ml/ml40/features/properties/values/empty_weight.py,sha256=e9TI6x6hL2EcFpIwfkYQnh7Mms8DXwEsRVTmIDyWRg4,286
 ml/ml40/features/properties/values/expansion_length.py,sha256=JWAhu6nblFlr3hZP9WfwudYvl-OzxxdyOHUWXNfCNgY,1053
 ml/ml40/features/properties/values/financial_value.py,sha256=pz47yud8pDn6SEXg0_IzJv8ej0nKzJVFeWRZxkYBVHw,963
 ml/ml40/features/properties/values/force.py,sha256=nbE-TFtvrs1H4sUKOG01HvVIvOQqefTP5Z1Bof1PeAI,1214
+ml/ml40/features/properties/values/fuel.py,sha256=LXn2LS2oeOsc2a9WQWDP7zvNzQcUF_LEe0mVsnfhcc8,515
+ml/ml40/features/properties/values/fuel_comsumption.py,sha256=YHzM2V1xzMdvb100iiU8RROrCPWFOXgIyeQoGX8VPtw,733
+ml/ml40/features/properties/values/fuel_type.py,sha256=sfv0C-3OcLHZrq2Yc3PNGfWq1-SJ304HpPPMp52UUJ8,110
 ml/ml40/features/properties/values/generic_property.py,sha256=ZH-WUdAaf2BLE8jjktEDsGxhSJ7ZLanQ3sqkp_81MAU,531
 ml/ml40/features/properties/values/gyroscope_value.py,sha256=6e_haFUjeyR9rnhBXvcKsHiHaSkYYoAHdwXp1na0i7Y,313
 ml/ml40/features/properties/values/heart_rate.py,sha256=Wcri3rFc_fAQpRW4NnKbat-cqWSLkVUYyv39WngknTY,1745
 ml/ml40/features/properties/values/high_speed_image_value.py,sha256=R57j00x8Vc8J4UH_xYBzPJcXKU_lcnjJkr3yNyLxXEU,2173
+ml/ml40/features/properties/values/idling_operating_hours.py,sha256=d3CtvckPbVngP-YPWQM3HbGKCJW8_wgjstSg2a6heeg,535
+ml/ml40/features/properties/values/imu_quaternion.py,sha256=BPQIkLVweDQrgbW7Q2HeUxUGZcvtS8_TzCucHRF54Ms,797
 ml/ml40/features/properties/values/infrared.py,sha256=aCj9sAQpfRq8LLjm4QT7rcvO33H77inBTTySdw3Cdhg,280
+ml/ml40/features/properties/values/land_velocity.py,sha256=4dRgyMdmAEdy51pxkdpZkf1VOmbNp5_dxjdfOmukA5g,293
 ml/ml40/features/properties/values/last_service_check.py,sha256=EccUBUjCAeo_o6U-o1HZxhAWYhLi_omlrgBhJ29tbvQ,711
 ml/ml40/features/properties/values/lidar_frame.py,sha256=s5nUBqSmbVEoxn6uIupYjIuX9GUc3jflYoxPH08nbVk,973
 ml/ml40/features/properties/values/lift.py,sha256=7KqgzOGuNs1kReKa2D_4M80KzkPSVCk1KjMKWXXSyO8,1286
 ml/ml40/features/properties/values/linestring.py,sha256=62zkQncwFyuVnGfWSB-Ncy_dkFtbTRsRVXCBl-cfUmw,420
 ml/ml40/features/properties/values/linestring_wkt.py,sha256=bQNxTXmtJmGl21WavokCAM9zaZj0py-mvnNW9c8mdh8,690
 ml/ml40/features/properties/values/liquid_filling_level.py,sha256=SHI8xnMOpAJtx8umuw8kpfh5zVbxkY82HpeFqqLe9nM,685
+ml/ml40/features/properties/values/load.py,sha256=SqD9gxtNLvnmfqSQz379OWPkAxQOCRGHkxnFtSuuJsU,482
+ml/ml40/features/properties/values/load_index.py,sha256=xkgzArM7KYcIIjrpLPjGv-ADSkIvWMixS1duEMGEmxw,487
+ml/ml40/features/properties/values/loading_volume.py,sha256=NMQuaZgmigjMOX8sBZUo9OX_y1Q8mVIPrp5bhnSQjTk,289
 ml/ml40/features/properties/values/location.py,sha256=xbyB9pZEVujCJLEsKk8bCUTARG2R2dm0yGnALIDrnpg,1943
 ml/ml40/features/properties/values/lot.py,sha256=iXdAhnhpaj1uCsJce5GUK8cbjyjd_MZvKm9OEhKVP4c,275
+ml/ml40/features/properties/values/machine_operating_status.py,sha256=53CiDK_cy0Dr21gds_QTll__EsVZ743tlzUClsh9M2M,541
+ml/ml40/features/properties/values/machine_operating_status_type.py,sha256=yvVohQbp-TLHqqmvjOJt9NsNZrQWLIDzoitMljzJ5AI,133
+ml/ml40/features/properties/values/maintenance_due.py,sha256=SP6lfZUJhVQEYCJPDikZwmMw0ioUWKavSd6vfvIO6rU,529
+ml/ml40/features/properties/values/maintenance_remaining_hours.py,sha256=5d9fs3BZQZDqFqVukC-EVJQJmiZwkkfWQb1dd5bnTVQ,540
+ml/ml40/features/properties/values/manufacturing_year.py,sha256=dE5-hvuBHf92HeMA8tk3ui4-MnY_licIwIRPar_B_gw,528
+ml/ml40/features/properties/values/measure.py,sha256=EoGGO9eo4GUf1lgRzjQLktJUl66bi_Q0U46eDhYmhDs,760
+ml/ml40/features/properties/values/model.py,sha256=jZilTwjodt1lsw3IE8GPCYKFAZ7z4UMd0WVv6-Sg7-8,516
 ml/ml40/features/properties/values/moisture.py,sha256=ZyzBRwWCELUBzRZv36E3MGbStGhjPDnf7WZUxKeBZ1o,999
-ml/ml40/features/properties/values/operating_hours.py,sha256=RntTMYflXnWU5G6lSXoGTRUT-DcWKk5DXK5zQkZ5-f8,676
+ml/ml40/features/properties/values/motor_vehicle_license_plate_number.py,sha256=AdikkWhZo-gxr8KyP7rLVKqttuxF5NIBCDwpf7flKYs,546
+ml/ml40/features/properties/values/opening_hours.py,sha256=vWlTM7vayvhgtktqWeXD0rpMqsWHUzrLXiJ9fFv6oVc,295
+ml/ml40/features/properties/values/operating_hours.py,sha256=G_4ePt6LkK0EaJXL227-CRe2z9Dx6X52IvL-4CO901Y,912
 ml/ml40/features/properties/values/orientation_rpy.py,sha256=sq4CvyD3LAsKwXfasxmLqfwg19e9b9tWex-4iav2U10,1201
 ml/ml40/features/properties/values/percentage.py,sha256=tBUWESbmStBFdXXdcj607VbuKtnh7UC9XeaIL9vLvD4,652
 ml/ml40/features/properties/values/personal_name.py,sha256=GF5MQ2wjwafDDWxT8SLabttxP2nPcTonTEoq6Fw6VQY,669
+ml/ml40/features/properties/values/pressure.py,sha256=NIJUxSuiRNL7_QrGjCsZwguwAkehGfEvaNsvVSQb0Js,535
+ml/ml40/features/properties/values/price_list.py,sha256=GD2bg9baxz6_O9cYPto8m8tnfMyAVIvQunIiolT42bw,524
+ml/ml40/features/properties/values/purchase_cost.py,sha256=CaPTByt2k76pz7EIji7fN7Dtj13C_f5dMyFwgIJQWCs,314
 ml/ml40/features/properties/values/rgb_color.py,sha256=fGmeql9p9pmg23V5nh-9c6TEhlWCssqwTqRFHkmzbOI,280
+ml/ml40/features/properties/values/road_velocity.py,sha256=fybIcA9MDbA4SYOMTxbc5wYsZ8qIesWSbGAfu8lG1pk,293
 ml/ml40/features/properties/values/rotational_speed.py,sha256=dbrqCazRH7pg2XYQ2PG0sJ25dtp5RTfhu7fkngkmZgM,655
 ml/ml40/features/properties/values/route.py,sha256=WVxurIuGSTjU6Ib4p8nGUE41fprwvfzyU0BzAkk4VkA,277
+ml/ml40/features/properties/values/serial_number.py,sha256=Gx0YiG6u3u7EbYcgzzeFBz0cMoZqr-0K6KY7nuin2Lg,527
 ml/ml40/features/properties/values/sound_level.py,sha256=mteUz_09gTrjAfar3XomAuAqunuVmxUDw19t8kXznNI,282
 ml/ml40/features/properties/values/srid.py,sha256=epWBWcGWtpKF06fiZAjAE4Kaai-b7pGk-9K8USwUn8A,276
+ml/ml40/features/properties/values/status.py,sha256=ouUefdMzVN1oM34BqOByKFVQO_-hxlRU55qrW40Seg8,525
 ml/ml40/features/properties/values/std_deviation_rpy.py,sha256=mLH1Rp7fDbscSJLgzQ-MFUDW1Et3hH8rCBbmH1d74mY,1512
+ml/ml40/features/properties/values/steering_angle.py,sha256=BBVu49EB_3Y2IlpDKoNGSLxFCVmIkcFAUN9M2JTSkHc,528
 ml/ml40/features/properties/values/stereo_camera_config.py,sha256=vlGMeMiuDdeyy-9nrxbGI454wyt0a5mIQjY-8PEWb4U,1026
 ml/ml40/features/properties/values/surface.py,sha256=_uYzl5C3Lom7ox_nm_Rswp5bpWql62TlJz3jb3-Svrk,279
 ml/ml40/features/properties/values/surface_wkt.py,sha256=Gyh6Nycznu7QgGskfSIOYtCbI0yrsF-UrNlt3Uj0BXk,288
 ml/ml40/features/properties/values/switching_stage.py,sha256=w2JV2fKg1v0lUmb7EQopqNef6xQMObGIU-_QF_uMjfU,1304
-ml/ml40/features/properties/values/temperature.py,sha256=imRp9PS3u2uVqZJgk0tjihM9iYBBMAXpstqIfjlQSwA,1122
+ml/ml40/features/properties/values/tax_number.py,sha256=pRueAO4l9GNmQJIYgqxc8f6JDBUgI9LnqrjDjc49vdw,524
+ml/ml40/features/properties/values/temperature.py,sha256=xAWn-w_gYexjuo8sZwKPc32kAr4B49dHhu8l0Nv4-qo,550
+ml/ml40/features/properties/values/tilt.py,sha256=_K1H5FtxDUBLNYL6tqeOtyFl5S7CqG9UcbT1683THhI,944
+ml/ml40/features/properties/values/time.py,sha256=wdQeSO4WQikqZyCN7SgwqiQXbOhEJonATv3FjL3rutQ,515
 ml/ml40/features/properties/values/time_slot.py,sha256=OHkxa02ongIA6dBd-cKI_8JCafiaKwhcZF2J9Z8x7Zw,626
+ml/ml40/features/properties/values/torque.py,sha256=tqI1qkIxZ9-XnhWyjKT9gl3UrmDQfMuPn-XJPCIx3pM,665
+ml/ml40/features/properties/values/type.py,sha256=Wc0pIkrl_u_nvQQ3naO9UjYzTwqj5N-Nt0fgfScGxwo,519
 ml/ml40/features/properties/values/unit.py,sha256=r0OPg-Fg7dQAVa_FnkzinAUsG6zYPs9BVoFJZi6ZCwY,646
-ml/ml40/features/properties/values/value.py,sha256=-_mM7S3HvO4ShMX4BsOcl1ow-0dBXy-d6CPlvGWXctk,990
+ml/ml40/features/properties/values/value.py,sha256=RIfcfNyFG0I0IQxiiBv7ftXMoOmekfTfl3iDzhYvlEY,1013
+ml/ml40/features/properties/values/velocity.py,sha256=AVrl-c5HaOOkgGekQP8W4IsA0-nd9k5mJbsGGJKK_0Q,703
+ml/ml40/features/properties/values/volume.py,sha256=_NEZaarXQNHYpUHm4Ozuffaz2pO43hSXyi5guZrHT7E,522
 ml/ml40/features/properties/values/weatherdata.py,sha256=OxHVAiTDkd2GQPcb9aonsazsu_Ci0Johh40FbBqGJU8,2793
 ml/ml40/features/properties/values/weight.py,sha256=ci5RC8UAQkVO3YM5d2iSLBPtTufXicwyUU4W-d49KFE,669
 ml/ml40/features/properties/values/white_level.py,sha256=rlGQ9CVlTVf-yp2tTsBwkq_255E9MYM0drLt0Vl5ZFU,309
 ml/ml40/features/properties/values/documents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/document.py,sha256=tUGqNBu690MWHly0QnPDR1bLOOBtFU5etM_tBhFlT4A,280
+ml/ml40/features/properties/values/documents/contracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/ml40/features/properties/values/documents/contracts/contract.py,sha256=XFb2iCKavtCCuLDyfooX0YpogZwlA7jkS3RZzMih8s0,299
 ml/ml40/features/properties/values/documents/jobs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/jobs/generic_job.py,sha256=8j9iyYkyP_vDccLqXBOdCtDX3xdRUDRQ26DS9asIVEw,695
 ml/ml40/features/properties/values/documents/jobs/job.py,sha256=ouLcrOVA5tkB9NZufh3R3KEkhL25hZTK-4Ik18hxxsc,782
 ml/ml40/features/properties/values/documents/jobs/job_list.py,sha256=n6hS2-x4NLTZa4sGlyS6Q54oKZ5idoXBxjHf-SVv5pM,288
 ml/ml40/features/properties/values/documents/jobs/job_status.py,sha256=GoRxfx0nxiw3cZDBxGwPBOaqdhcx9-VuhVrLuf2BX30,99
+ml/ml40/features/properties/values/documents/notes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/ml40/features/properties/values/documents/notes/note.py,sha256=9bXwLh9G14-cOI3moFETZOON8jcpvfPuXBJwsjTUsxU,295
 ml/ml40/features/properties/values/documents/reports/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/reports/production_data.py,sha256=nCWHNIBdrXKETBh8kZM64ntJNhFRmOargeg_uG2Bm30,307
 ml/ml40/features/properties/values/documents/reports/report.py,sha256=Ed_RN3Hiqb-S27EBHXc_BL6UKBIPimCk6_ELuUyzUlg,297
 ml/ml40/roles/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 ml/ml40/roles/dts/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 ml/ml40/roles/dts/dt.py,sha256=-TjodAuL-H4oOBApAjRGaVMrldwDll_ZLys7SHsS3Y0,217
 ml/ml40/roles/dts/handheld_devices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/handheld_devices/handheld_device.py,sha256=0So8Pa9Sx5bg3-aYN52XF0xvKlLJYr7EFWIEhVVMvRI,260
 ml/ml40/roles/dts/machines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/machines/machine.py,sha256=SeyVigVr-gnOV6rOM7Ao3wP2-KWKXOj8-62dERJb7MM,261
+ml/ml40/roles/dts/organisations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/ml40/roles/dts/organisations/forwarding_agency.py,sha256=6j3x48jUH0QQ2qfjK6iwYulUeiYaOmsRvl90u9nTcYE,328
+ml/ml40/roles/dts/organisations/funding_agency.py,sha256=Qa1eOetgf3gbEV4tcsopqevJHnK8ygyojKmXUbmQvj0,322
+ml/ml40/roles/dts/organisations/organisation.py,sha256=SPzT87llYG_s8SzGu6KtCbq8i9jlDS9jiDvjdWk_OqU,276
+ml/ml40/roles/dts/organisations/production_team.py,sha256=88GleZfiFI5Xah0noCa7j_k7aodGLlzo7NRTmxdXgb4,324
+ml/ml40/roles/dts/organisations/supplier.py,sha256=hYwrCkZaR9pFN9rkgNREtymEkEcRYHauvPnLaSISRAM,312
 ml/ml40/roles/dts/parts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/ml40/roles/dts/parts/chain.py,sha256=jsEI6G5pBzqVyYWBgQXI8l86paqdCrYuKt-4uoZmsvs,274
 ml/ml40/roles/dts/parts/crane.py,sha256=aE0u7rkAGihtnB1Z7rV2Dq4oCQQc1I0m-obqWBdcjQk,274
 ml/ml40/roles/dts/parts/engine.py,sha256=ex5OY--oeO3vCA7H5rt8chaHZjcztRN_na-FxELcwEI,276
 ml/ml40/roles/dts/parts/part.py,sha256=9nuoe9kSHroTGElOeKGrqkajSn4_UvpjS42D5do66vw,260
 ml/ml40/roles/dts/parts/scale.py,sha256=0Q8onMR9dx2kvD9eZuwOSj5YzL5NFaZDfVTFuJLznq4,274
 ml/ml40/roles/dts/parts/tank.py,sha256=me9B25qLBBw6tvmmaM7LPHXY7wQ99rCB3DhDhImmeE4,272
+ml/ml40/roles/dts/parts/wheel.py,sha256=smsQznwaHy2D58_1r5tgAPG6Z-B1tk2Ayz5fJP7Dsx0,274
+ml/ml40/roles/dts/parts/winch.py,sha256=YQywNVwhPMfZqaa-QrNGrfOMoUV63uDW3D1DMJrVpEs,274
 ml/ml40/roles/dts/persons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/persons/machine_operator.py,sha256=MZZ3Vss3nlm5DIHK8OpNBKI2uaOf1um2HvMDHbrRUs8,302
 ml/ml40/roles/dts/persons/person.py,sha256=arDzt_2VLq9uWflZ2FlOqhcsk-ldmxsFnROu86Qj7mQ,242
 ml/ml40/roles/dts/sensors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/sensors/accelerometer.py,sha256=fQQTS5YtmBPpkGd65-6QuSQ4f_aI2--R8Y7jtCPYx9E,279
 ml/ml40/roles/dts/sensors/air_sensor.py,sha256=6NRY9eFpWXD1z0BYBtFcT-OZ0s9nOOfAoCfIJw7Exjc,290
+ml/ml40/roles/dts/sensors/counter_sensor.py,sha256=XM1rjyA866ZmMJjGSKw9FqlSE9A1lNXuuSkMrtxNGbA,298
 ml/ml40/roles/dts/sensors/gyroscope.py,sha256=Fd4b_puUZ2cm6kS_0_AAVcliaZxulzblEMPWltVyyg0,290
 ml/ml40/roles/dts/sensors/high_speed_camera.py,sha256=L8ACQQx_q-HPXnd0WCxcTTtZEaoOA92_7H3aYZWKSNQ,274
 ml/ml40/roles/dts/sensors/imu.py,sha256=Y5AafN2HO8Ly-oa6sib6_Efv3CAY68-hxcx5cL4LDVw,295
 ml/ml40/roles/dts/sensors/laser_range_finder.py,sha256=Khf5PRpORNMee5BP1XNiPuIH9Z1CDePyV1ArDfEFACs,321
 ml/ml40/roles/dts/sensors/lidar.py,sha256=udA0BbKNcnM7jShR0gmyaw1xWFeJ94sN-875Aqy6ZZQ,254
 ml/ml40/roles/dts/sensors/light_sensor.py,sha256=POtlxEf5kl4JqtEMLv0i6GxMbx5jVuBRIbgY-6bI_l8,294
+ml/ml40/roles/dts/sensors/pressure_sensor.py,sha256=w5bIxDDkLY9QPNvxdVKiSBd5U18KSb1dExwOWvTF83g,300
 ml/ml40/roles/dts/sensors/sensor.py,sha256=6NvdOyQwWac3e33zb8yd-L2gF85wungxQFRMbFTrX-A,252
 ml/ml40/roles/dts/sensors/sensor_network.py,sha256=mnLEbX-WWXL5AI67Ag_-_0V4zHswnhba8glxTXRJ9jQ,298
 ml/ml40/roles/dts/sensors/soil_sensor.py,sha256=UMUogGpPdRRGouL0LGpBZtrpc-ZuR85syMa1fN822BI,292
 ml/ml40/roles/dts/sensors/sound_sensor.py,sha256=8IAy9hFGsAN5Pn8OxCfeMVzBvMsvTDxzwF1BGmS-1X8,294
 ml/ml40/roles/dts/sensors/stereo_camera.py,sha256=A8LN9ResBpGK9wv4BufZclddMrxnr1n7wI2NR9CKNGg,268
+ml/ml40/roles/dts/sensors/temperature_sensor.py,sha256=8z5TRTtn3wu2AuFNiBV828VK3luv00eXsXdIfkpr6Uk,306
+ml/ml40/roles/dts/sensors/vehicle_counter_sensor.py,sha256=pZeApwXqzw411aecKcVjolGF625n2ppYB5k4jngx3Mg,334
 ml/ml40/roles/dts/sites/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/sites/site.py,sha256=Ye8nN_HCnpQCqj6l4ZwSYLmO_-VvKaMw6SbMf-lOC8c,260
 ml/ml40/roles/dts/ways/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/ways/way.py,sha256=_DDZIKkfnrAsVWWHL52baYVl-IVxiAcR8vc1_iQ7TJc,258
 ml/ml40/roles/hmis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/hmis/app.py,sha256=Q_qGmiw2JofjgsED_KGIfFI45ZE3j7MLzSpfWqtpAHE,262
 ml/ml40/roles/hmis/dashboard.py,sha256=KEF97MI5dtN2_-vLCfTAQlW3NneeztNfRGdMvy-S3v0,274
@@ -316,12 +428,12 @@
 ml/wml40/roles/dts/water/water.py,sha256=EkIdLUwG6NFFk0eFuooIv2Aa_MZzGm7WXAblFktqQWw,252
 ml/wml40/roles/dts/water/waterreservoir.py,sha256=BiXgiP7EFtV43RiI_xwdsVyz9QFSzJj59r_a26Sd8ec,277
 ml/wml40/roles/hmis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/wml40/roles/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_async.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_entry.py,sha256=r9lHxwSp6WbRu9fvh15q5hmMCEUC-P6MjlSekCiXibc,48
-fml40_reference_implementation-0.2.7.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
-fml40_reference_implementation-0.2.7.dist-info/METADATA,sha256=0RNI-bJmK3eIE5VmilABygC-jCywLsPw6sW9VBut8HU,8893
-fml40_reference_implementation-0.2.7.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
-fml40_reference_implementation-0.2.7.dist-info/top_level.txt,sha256=Txv1lgjX0CJ7-VPm6Uv5WJ2XYyNfE4K4M3jUQ2uDXZE,9
-fml40_reference_implementation-0.2.7.dist-info/RECORD,,
+fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
+fml40_reference_implementation-0.2.8.dist-info/METADATA,sha256=NB-7wfVqrj6zj9kKMDhK8hUxH3l4bXyxbf_6pHEZci8,8893
+fml40_reference_implementation-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fml40_reference_implementation-0.2.8.dist-info/top_level.txt,sha256=zi2IoIakYFZNb4sNVwCx-zsTTM-9E_fUQkhRTH7Tivs,22
+fml40_reference_implementation-0.2.8.dist-info/RECORD,,
```

