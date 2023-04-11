# Comparing `tmp/ScenarioGUI-0.2.0.tar.gz` & `tmp/ScenarioGUI-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScenarioGUI-0.2.0.tar", last modified: Thu Apr  6 13:23:03 2023, max compression
+gzip compressed data, was "ScenarioGUI-0.2.1.tar", last modified: Tue Apr 11 14:17:15 2023, max compression
```

## Comparing `ScenarioGUI-0.2.0.tar` & `ScenarioGUI-0.2.1.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.102604 ScenarioGUI-0.2.0/
--rw-rw-rw-   0        0        0     1550 2023-03-17 13:39:19.000000 ScenarioGUI-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    13181 2023-04-06 13:23:03.103605 ScenarioGUI-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    12496 2023-04-06 10:21:47.000000 ScenarioGUI-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:02.983487 ScenarioGUI-0.2.0/ScenarioGUI/
--rw-rw-rw-   0        0        0      283 2023-04-06 10:21:47.000000 ScenarioGUI-0.2.0/ScenarioGUI/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-06 10:21:47.000000 ScenarioGUI-0.2.0/ScenarioGUI/global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.004506 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/
--rw-rw-rw-   0        0        0        0 2023-03-15 21:01:46.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/__init__.py
--rw-rw-rw-   0        0        0    28668 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_base_class.py
--rw-rw-rw-   0        0        0     2655 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_calculation_thread.py
--rw-rw-rw-   0        0        0    57851 2023-04-03 06:43:48.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_combine_window.py
--rw-rw-rw-   0        0        0     4824 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_data_storage.py
--rw-rw-rw-   0        0        0     6963 2023-04-01 13:46:45.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.038546 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/
--rw-rw-rw-   0        0        0     1002 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py
--rw-rw-rw-   0        0        0     5894 2023-04-01 13:42:53.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/aim.py
--rw-rw-rw-   0        0        0     9672 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py
--rw-rw-rw-   0        0        0     9951 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/category.py
--rw-rw-rw-   0        0        0     3535 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py
--rw-rw-rw-   0        0        0     7199 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py
--rw-rw-rw-   0        0        0    14527 2023-03-30 05:40:29.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py
--rw-rw-rw-   0        0        0     9396 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py
--rw-rw-rw-   0        0        0     5335 2023-04-01 13:38:11.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py
--rw-rw-rw-   0        0        0     5030 2023-03-27 21:12:41.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/functions.py
--rw-rw-rw-   0        0        0     4092 2023-03-28 05:52:35.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/hint.py
--rw-rw-rw-   0        0        0     8872 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py
--rw-rw-rw-   0        0        0     7816 2023-03-28 07:47:58.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
--rw-rw-rw-   0        0        0    10309 2023-04-01 13:45:00.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/option.py
--rw-rw-rw-   0        0        0    14296 2023-04-06 13:05:56.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/page.py
--rw-rw-rw-   0        0        0     3047 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
--rw-rw-rw-   0        0        0    10412 2023-04-03 07:51:18.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
--rw-rw-rw-   0        0        0     4670 2023-03-28 07:47:58.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
--rw-rw-rw-   0        0        0     5841 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
--rw-rw-rw-   0        0        0     1482 2023-04-06 10:21:47.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/status_bar_logger.py
--rw-rw-rw-   0        0        0     8448 2023-03-28 05:52:35.000000 ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/translation_class.py
--rw-rw-rw-   0        0        0     1513 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/ScenarioGUI/translation_csv_to_py.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:02.990493 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/
--rw-rw-rw-   0        0        0    13181 2023-04-06 13:23:02.000000 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-04-06 13:23:02.000000 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:23:02.000000 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-06 13:23:02.000000 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-06 13:23:02.000000 ScenarioGUI-0.2.0/ScenarioGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1732 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      985 2023-04-06 13:23:03.104606 ScenarioGUI-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      113 2023-03-28 07:47:58.000000 ScenarioGUI-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.042550 ScenarioGUI-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-16 09:51:14.000000 ScenarioGUI-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     7096 2023-04-06 11:50:27.000000 ScenarioGUI-0.2.0/tests/gui_structure_for_tests.py
--rw-rw-rw-   0        0        0     1618 2023-03-31 17:17:03.000000 ScenarioGUI-0.2.0/tests/result_creating_class_for_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.068565 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/
--rw-rw-rw-   0        0        0        0 2023-03-16 09:51:14.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/__init__.py
--rw-rw-rw-   0        0        0      917 2023-04-06 10:21:47.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_aim.py
--rw-rw-rw-   0        0        0     1644 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_button_box.py
--rw-rw-rw-   0        0        0     1360 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_category.py
--rw-rw-rw-   0        0        0     1873 2023-04-06 10:52:05.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_filename.py
--rw-rw-rw-   0        0        0     5178 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_flexible_amount_option.py
--rw-rw-rw-   0        0        0     2246 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_float_box.py
--rw-rw-rw-   0        0        0     1424 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_function_button.py
--rw-rw-rw-   0        0        0     2067 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_int_box.py
--rw-rw-rw-   0        0        0     2047 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_list_box.py
--rw-rw-rw-   0        0        0     1187 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_page.py
--rw-rw-rw-   0        0        0     1311 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_repr.py
--rw-rw-rw-   0        0        0     2076 2023-04-06 12:27:05.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_result_export.py
--rw-rw-rw-   0        0        0     1428 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_results_figure.py
--rw-rw-rw-   0        0        0     1362 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_results_text.py
--rw-rw-rw-   0        0        0     1366 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_text_box.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.093588 ScenarioGUI-0.2.0/tests/test_main_window_functions/
--rw-rw-rw-   0        0        0        0 2023-04-06 12:27:30.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/__init__.py
--rw-rw-rw-   0        0        0     2414 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_auto_save.py
--rw-rw-rw-   0        0        0     2354 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_backup.py
--rw-rw-rw-   0        0        0     2946 2023-04-06 12:02:31.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_close.py
--rw-rw-rw-   0        0        0     1309 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_datastorage.py
--rw-rw-rw-   0        0        0     2121 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_double_naming.py
--rw-rw-rw-   0        0        0     2769 2023-04-06 11:46:02.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_global_settings.py
--rw-rw-rw-   0        0        0     2100 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_move_scenario.py
--rw-rw-rw-   0        0        0     6098 2023-04-06 10:51:01.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_new_save_load.py
--rw-rw-rw-   0        0        0     1414 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_no_file.py
--rw-rw-rw-   0        0        0     1908 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_push_button_change.py
--rw-rw-rw-   0        0        0     4332 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_rename_scenario.py
--rw-rw-rw-   0        0        0     5156 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_run.py
--rw-rw-rw-   0        0        0     6402 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_scenario_change.py
--rw-rw-rw-   0        0        0     1961 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_scenario_properties.py
--rw-rw-rw-   0        0        0     2876 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_main_window_functions/test_toggle_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:23:03.101594 ScenarioGUI-0.2.0/tests/test_translations/
--rw-rw-rw-   0        0        0        0 2023-03-16 13:35:34.000000 ScenarioGUI-0.2.0/tests/test_translations/__init__.py
--rw-rw-rw-   0        0        0      913 2023-03-29 05:42:57.000000 ScenarioGUI-0.2.0/tests/test_translations/test_language_change.py
--rw-rw-rw-   0        0        0      624 2023-04-06 12:28:47.000000 ScenarioGUI-0.2.0/tests/test_translations/test_translation_csv_2_py.py
--rw-rw-rw-   0        0        0     8795 2023-04-06 12:28:41.000000 ScenarioGUI-0.2.0/tests/test_translations/translation_class.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.616012 ScenarioGUI-0.2.1/
+-rw-rw-rw-   0        0        0     1550 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    13181 2023-04-11 14:17:15.617015 ScenarioGUI-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12496 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.457484 ScenarioGUI-0.2.1/ScenarioGUI/
+-rw-rw-rw-   0        0        0      283 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/ScenarioGUI/__init__.py
+-rw-rw-rw-   0        0        0     3629 2023-04-11 14:12:38.000000 ScenarioGUI-0.2.1/ScenarioGUI/global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.522491 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/__init__.py
+-rw-rw-rw-   0        0        0    29594 2023-04-11 12:51:29.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_base_class.py
+-rw-rw-rw-   0        0        0     2655 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_calculation_thread.py
+-rw-rw-rw-   0        0        0    59525 2023-04-11 13:59:04.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_combine_window.py
+-rw-rw-rw-   0        0        0     4824 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_data_storage.py
+-rw-rw-rw-   0        0        0     8207 2023-04-11 12:59:59.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.547486 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/
+-rw-rw-rw-   0        0        0     1002 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py
+-rw-rw-rw-   0        0        0     6283 2023-04-11 12:58:07.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/aim.py
+-rw-rw-rw-   0        0        0     9824 2023-04-11 11:44:38.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py
+-rw-rw-rw-   0        0        0    10352 2023-04-11 13:00:40.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/category.py
+-rw-rw-rw-   0        0        0     3535 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py
+-rw-rw-rw-   0        0        0     7673 2023-04-11 12:50:25.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py
+-rw-rw-rw-   0        0        0    15245 2023-04-11 13:49:17.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py
+-rw-rw-rw-   0        0        0     9433 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py
+-rw-rw-rw-   0        0        0     5770 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py
+-rw-rw-rw-   0        0        0     5028 2023-04-11 11:30:06.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/functions.py
+-rw-rw-rw-   0        0        0     4524 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/hint.py
+-rw-rw-rw-   0        0        0     8909 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py
+-rw-rw-rw-   0        0        0     7894 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
+-rw-rw-rw-   0        0        0    10794 2023-04-11 14:10:30.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/option.py
+-rw-rw-rw-   0        0        0    15083 2023-04-11 11:58:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/page.py
+-rw-rw-rw-   0        0        0     3047 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
+-rw-rw-rw-   0        0        0    10748 2023-04-11 13:50:58.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
+-rw-rw-rw-   0        0        0     4670 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
+-rw-rw-rw-   0        0        0     5841 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
+-rw-rw-rw-   0        0        0     1569 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/status_bar_logger.py
+-rw-rw-rw-   0        0        0     8448 2023-03-27 13:57:20.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/translation_class.py
+-rw-rw-rw-   0        0        0     1513 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/translation_csv_to_py.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.551003 ScenarioGUI-0.2.1/ScenarioGUI/utils/
+-rw-rw-rw-   0        0        0      130 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-11 11:30:06.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/change_font_size.py
+-rw-rw-rw-   0        0        0      838 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/set_default_font.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.503482 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/
+-rw-rw-rw-   0        0        0    13181 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3924 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1732 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      985 2023-04-11 14:17:15.619014 ScenarioGUI-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      113 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.554014 ScenarioGUI-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-03 14:37:38.000000 ScenarioGUI-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     7096 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/gui_structure_for_tests.py
+-rw-rw-rw-   0        0        0     1618 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/tests/result_creating_class_for_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.574016 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:08.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/__init__.py
+-rw-rw-rw-   0        0        0      917 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_aim.py
+-rw-rw-rw-   0        0        0     1644 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_button_box.py
+-rw-rw-rw-   0        0        0     1360 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_category.py
+-rw-rw-rw-   0        0        0     1873 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_filename.py
+-rw-rw-rw-   0        0        0     5178 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_flexible_amount_option.py
+-rw-rw-rw-   0        0        0     2246 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_float_box.py
+-rw-rw-rw-   0        0        0     1424 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_function_button.py
+-rw-rw-rw-   0        0        0     2067 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_int_box.py
+-rw-rw-rw-   0        0        0     2047 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_list_box.py
+-rw-rw-rw-   0        0        0     1187 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_page.py
+-rw-rw-rw-   0        0        0     1311 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_repr.py
+-rw-rw-rw-   0        0        0     2076 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_result_export.py
+-rw-rw-rw-   0        0        0     1428 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_figure.py
+-rw-rw-rw-   0        0        0     1362 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_text.py
+-rw-rw-rw-   0        0        0     1366 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_text_box.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.596021 ScenarioGUI-0.2.1/tests/test_main_window_functions/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:00:55.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/__init__.py
+-rw-rw-rw-   0        0        0     2414 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_auto_save.py
+-rw-rw-rw-   0        0        0     2354 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_backup.py
+-rw-rw-rw-   0        0        0     3698 2023-04-11 14:05:28.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_change_font_size.py
+-rw-rw-rw-   0        0        0     2946 2023-04-11 14:12:17.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_close.py
+-rw-rw-rw-   0        0        0     1309 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_datastorage.py
+-rw-rw-rw-   0        0        0     2121 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_double_naming.py
+-rw-rw-rw-   0        0        0     6263 2023-04-11 14:05:28.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_global_settings.py
+-rw-rw-rw-   0        0        0     2100 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_move_scenario.py
+-rw-rw-rw-   0        0        0     6100 2023-04-11 14:11:35.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_new_save_load.py
+-rw-rw-rw-   0        0        0     1414 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_no_file.py
+-rw-rw-rw-   0        0        0     1908 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_push_button_change.py
+-rw-rw-rw-   0        0        0     4332 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_rename_scenario.py
+-rw-rw-rw-   0        0        0     5156 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_run.py
+-rw-rw-rw-   0        0        0     6402 2023-03-28 11:53:59.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_change.py
+-rw-rw-rw-   0        0        0     1961 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_properties.py
+-rw-rw-rw-   0        0        0     2876 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_toggle_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.615015 ScenarioGUI-0.2.1/tests/test_translations/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:09.000000 ScenarioGUI-0.2.1/tests/test_translations/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_translations/test_language_change.py
+-rw-rw-rw-   0        0        0      624 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_translations/test_translation_csv_2_py.py
+-rw-rw-rw-   0        0        0     8795 2023-04-11 14:13:13.000000 ScenarioGUI-0.2.1/tests/test_translations/translation_class.py
```

### Comparing `ScenarioGUI-0.2.0/LICENSE` & `ScenarioGUI-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/PKG-INFO` & `ScenarioGUI-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScenarioGUI
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for a scenario based GUI
 Home-page: https://github.com/tblanke/ScenarioGUI
 Author: Tobias Blanke
 Author-email: blanke@fh-aachen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ScenarioGUI-0.2.0/README.md` & `ScenarioGUI-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/global_settings.py` & `ScenarioGUI-0.2.1/ScenarioGUI/global_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from platform import system
 
 path = Path(__file__).parent.absolute()
 config = ConfigParser()
 
 
 def get_path_for_file(start_path: Path, filename: str) -> Path:
-    path_i = start_path
+    path_i = start_path.absolute()
     for i in range(6):
         items = [item.parent for item in path_i.glob(f"**/{filename}")]
         if items:
             return items[0]
         path_i = path_i.parent
     raise FileNotFoundError
 
@@ -28,24 +28,27 @@
 LIGHT: str = "rgb(0,0,0)"
 LIGHT_SELECT: str = "rgb(0,0,0)"
 DARK: str = "rgb(0,0,0)"
 GREY: str = "rgb(0,0,0)"
 WARNING: str = "rgb(0,0,0)"
 BLACK: str = "rgb(0,0,0)"
 
-FONT = "None"
-FONT_SIZE = 6
+FONT = "Arial"
+FONT_SIZE = 10
 
-FILE_EXTENSION: str = "nothing"
-GUI_NAME: str = "None"
+FILE_EXTENSION: str = "yourGUI"
+GUI_NAME: str = "Your GUI Name"
 ICON_NAME: str = "icon"
 
 # get current version
-config.read(config.read(get_path_for_file(path, "setup.cfg").joinpath("setup.cfg")))
-VERSION = config.get("metadata", "version")
+try:
+    config.read(config.read(get_path_for_file(path, "setup.cfg").joinpath("setup.cfg")))
+    VERSION = config.get("metadata", "version")
+except FileNotFoundError:  # pragma: no cover
+    VERSION = "0.0.0"
 
 
 def load(gui_file: str | Path):
     config.read(gui_file)
 
     global FOLDER
     global WHITE
@@ -56,16 +59,20 @@
     global WARNING
     global BLACK
     global FONT
     global FONT_SIZE
     global FILE_EXTENSION
     global GUI_NAME
     global ICON_NAME
+    global VERSION
 
-    FOLDER = get_path_for_file(get_path_for_file(path, config['DEFAULT']["PATH_2_ICONS"]).joinpath(config['DEFAULT']["PATH_2_ICONS"]), "icons")
+    FOLDER = get_path_for_file(get_path_for_file(Path(gui_file).parent.parent, config['DEFAULT']["PATH_2_ICONS"]).joinpath(config['DEFAULT']["PATH_2_ICONS"]), "icons")
+
+    config.read(config.read(get_path_for_file(Path(gui_file).parent.parent, "setup.cfg").joinpath("setup.cfg")))
+    VERSION = config.get("metadata", "version")
 
     WHITE = config['COLORS']["WHITE"]
     LIGHT = config['COLORS']["LIGHT"]
     LIGHT_SELECT = config['COLORS']["LIGHT_SELECT"]
     DARK = config['COLORS']["DARK"]
     GREY = config['COLORS']["GREY"]
     WARNING = config['COLORS']["WARNING"]
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_base_class.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_base_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import PySide6.QtCore as QtC
 import PySide6.QtGui as QtG
 import PySide6.QtWidgets as QtW
 
 import ScenarioGUI.global_settings as globs
 
 from .status_bar_logger import StatusBar
+from ..utils import set_default_font
 
 
 class BaseUI:
     """
     This class contains the framework of the GUI, with the top bar,
     the scenario/run/ ... buttons and the shortcuts.
     """
@@ -76,29 +77,26 @@
         font.setBold(False)
         font.setItalic(False)
         ghe_tool.setFont(font)
         icon = QtG.QIcon()
         icon.addFile(f"{globs.FOLDER}/icons/{globs.ICON_NAME}", QtC.QSize(), QtG.QIcon.Normal, QtG.QIcon.Off)
         ghe_tool.setWindowIcon(icon)
         ghe_tool.setStyleSheet(
-            f"*{'{'}color: {globs.WHITE}; font: {globs.FONT_SIZE}pt '{globs.FONT}';background-color: {globs.DARK};selection-background-color: {globs.LIGHT};"
+            f"*{'{'}color: {globs.WHITE};background-color: {globs.DARK};selection-background-color: {globs.LIGHT};"
             f"alternate-background-color: {globs.LIGHT};{'}'}\n"
             f"QPushButton{'{'}border: 3px solid {globs.LIGHT};border-radius: 5px;color:{globs.WHITE};gridline-color:{globs.LIGHT};"
-            f"background-color:{globs.LIGHT};"
-            f"font: 700 {globs.FONT_SIZE}pt '{globs.FONT}';{'}'}"
+            f"background-color:{globs.LIGHT};font-weight:700;{'}'}"
             f"QPushButton:hover{'{'}background-color: {globs.DARK};{'}'}\n"
             f"QPushButton:disabled{'{'}border: 3px solid {globs.GREY};border-radius: 5px;color: {globs.WHITE};gridline-color: {globs.GREY};"
             f"background-color: {globs.GREY};{'}'}\n"
             f"QPushButton:disabled:hover{'{'}background-color: {globs.DARK};{'}'}\n"
             f"QComboBox{'{'}border: 1px solid {globs.WHITE};border-bottom-left-radius: 0px;border-bottom-right-radius: 0px;{'}'}\n"
-            f"QSpinBox{'{'}selection-color: {globs.WHITE};selection-background-color: {globs.LIGHT};border: 1px solid {globs.WHITE}; "
-            f"font: {globs.FONT_SIZE}pt '{globs.FONT}';{'}'}\n"
+            f"QSpinBox{'{'}selection-color: {globs.WHITE};selection-background-color: {globs.LIGHT};border: 1px solid {globs.WHITE};{'}'}\n"
             f"QLineEdit{'{'}border: 3px solid {globs.LIGHT};border-radius: 5px;color: {globs.WHITE};gridline-color: {globs.LIGHT};background-color: "
-            f"{globs.LIGHT};font-weight:700;\n"
-            f"selection-background-color: {globs.LIGHT_SELECT};{'}'}\n"
+            f"{globs.LIGHT};selection-background-color: {globs.LIGHT_SELECT};{'}'}\n"
             f"QLineEdit:hover{'{'}background-color: {globs.DARK};{'}'}"
             f"QToolTip{'{'}color: {globs.WHITE}; background-color: {globs.DARK}; border: 1px solid {globs.LIGHT};border-radius: 4px;{'}'}"
             f"QTabBar::tab{'{'}background-color: {globs.DARK};padding-top:5px;padding-bottom:5px;padding-left:5px;padding-right:5px;color: {globs.WHITE};{'}'}"
             f"QTabBar::tab:selected, QTabBar::tab:hover{'{'}background-color: {globs.LIGHT};{'}'}"
             f"QTabBar::tab:selected{'{'}background-color: {globs.LIGHT};{'}'}"
             f"QTabBar::tab:!selected{'{'}background-color:  {globs.DARK};{'}'}"
             f"QTabWidget::pane{'{'}border: 1px solid {globs.WHITE};{'}'}"
@@ -400,14 +398,15 @@
             f"QtG.QAction::icon {'{'} background-color:{globs.LIGHT};selection-background-color: {globs.LIGHT};{'}'}\n"
             f"*{'{'}	background-color: {globs.DARK};{'}'}\n"
             f"*:hover{'{'}background-color: {globs.LIGHT};{'}'}"
         )
         self.menu_file.setTearOffEnabled(False)
         self.menu_calculation = QtW.QMenu(self.menubar)
         self.menu_calculation.setObjectName("menuCalculation")
+        self.menu_calculation.setFont(font)
         self.menu_settings = QtW.QMenu(self.menubar)
         self.menu_settings.setObjectName("menuSettings")
         self.menu_language = QtW.QMenu(self.menu_settings)
         self.menu_language.setObjectName("menuLanguage")
         self.menu_language.setEnabled(True)
         icon35 = QtG.QIcon()
         icon35.addFile(f"{globs.FOLDER}/icons/Language.svg", QtC.QSize(), QtG.QIcon.Normal, QtG.QIcon.Off)
@@ -435,21 +434,24 @@
         self.menubar.addAction(self.menu_calculation.menuAction())
         self.menubar.addAction(self.menu_scenario.menuAction())
         self.menubar.addAction(self.menu_settings.menuAction())
         self.menu_file.addAction(self.action_new)
         self.menu_file.addAction(self.action_save)
         self.menu_file.addAction(self.action_save_as)
         self.menu_file.addAction(self.action_open)
+        self.menu_file.setFont(font)
         self.menu_calculation.addAction(self.action_start_multiple)
         self.menu_calculation.addAction(self.action_start_single)
         self.menu_settings.addAction(self.menu_language.menuAction())
+        self.menu_settings.setFont(font)
         self.menu_scenario.addAction(self.action_update_scenario)
         self.menu_scenario.addAction(self.action_add_scenario)
         self.menu_scenario.addAction(self.action_delete_scenario)
         self.menu_scenario.addAction(self.action_rename_scenario)
+        self.menu_scenario.setFont(font)
         self.tool_bar.addAction(self.action_new)
         self.tool_bar.addAction(self.action_save)
         self.tool_bar.addAction(self.action_save_as)
         self.tool_bar.addAction(self.action_open)
         self.tool_bar.addAction(self.action_start_single)
         self.tool_bar.addAction(self.action_start_multiple)
         self.tool_bar.addAction(self.action_update_scenario)
@@ -462,14 +464,32 @@
         self.push_button_start_multiple.clicked.connect(self.action_start_multiple.trigger)
         self.push_button_add_scenario.clicked.connect(self.action_add_scenario.trigger)
         self.push_button_delete_scenario.clicked.connect(self.action_delete_scenario.trigger)
         self.push_button_save_scenario.clicked.connect(self.action_update_scenario.trigger)
         self.list_widget_scenario.itemDoubleClicked.connect(self.action_rename_scenario.trigger)
         self.push_button_start_single.clicked.connect(self.action_start_single.trigger)
 
+        set_default_font(self.list_widget_scenario)
+
+        set_default_font(self.push_button_save_scenario, bold=True)
+        set_default_font(self.push_button_add_scenario, bold=True)
+        set_default_font(self.push_button_delete_scenario, bold=True)
+        set_default_font(self.button_rename_scenario, bold=True)
+        set_default_font(self.push_button_cancel, bold=True)
+        set_default_font(self.push_button_start_single, bold=True)
+        set_default_font(self.push_button_start_multiple, bold=True)
+        set_default_font(self.menu_scenario)
+        set_default_font(self.menu_calculation)
+        set_default_font(self.menu_file)
+        set_default_font(self.menu_settings)
+        set_default_font(self.menu_language)
+        set_default_font(self.menubar)
+        set_default_font(self.list_widget_scenario)
+        set_default_font(self.status_bar.widget)
+
         self.stacked_widget.setCurrentIndex(0)
         QtC.QMetaObject.connectSlotsByName(ghe_tool)
 
         ghe_tool.setWindowTitle("GHEtool")
         self.action_new.setText("New")
         # if QT_CONFIG(tooltip)
         self.action_new.setToolTip("Create new project file")
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_calculation_thread.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_calculation_thread.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_combine_window.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_combine_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 from pathlib import Path, PurePath
 from sys import path
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC
 import PySide6.QtGui as QtG
 import PySide6.QtWidgets as QtW
+from matplotlib import rcParams
+
 import ScenarioGUI.global_settings as globs
 
 from .gui_base_class import BaseUI
 from .gui_calculation_thread import CalcProblem
 from .gui_data_storage import DataStorage
 from .gui_structure_classes import FigureOption, Option, ResultExport
 from .gui_structure_classes.functions import check_aim_options, show_linked_options
+from ..utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Protocol
 
     from ScenarioGUI.gui_classes.gui_structure import GuiStructure
 
@@ -234,14 +237,15 @@
         for option, _ in self.gui_structure.list_of_aims:
             option.change_event(self.change)
 
         for option, name in setting_options:
             option.change_event(ft_partial(self._change_settings_in_all_data_storages, name))
 
         self.gui_structure.option_language.change_event(self.change_language)
+        self.gui_structure.option_font_size.change_event(self.change_font_size)
         self.gui_structure.page_result.button.clicked.connect(self.display_results)
         self.action_add_scenario.triggered.connect(self.add_scenario)
         self.action_update_scenario.triggered.connect(self.save_scenario)
         self.action_delete_scenario.triggered.connect(self.delete_scenario)
         self.action_start_multiple.triggered.connect(self.start_multiple_scenarios_calculation)
         self.action_start_single.triggered.connect(self.start_current_scenario_calculation)
         self.action_save.triggered.connect(self.fun_save)
@@ -251,14 +255,36 @@
         self.action_rename_scenario.triggered.connect(lambda: self.fun_rename_scenario())
         self.list_widget_scenario.setDragDropMode(QtW.QAbstractItemView.InternalMove)
         self.list_widget_scenario.model().rowsMoved.connect(self.fun_move_scenario)
         self.list_widget_scenario.currentItemChanged.connect(self.scenario_is_changed)
         self.list_widget_scenario.itemSelectionChanged.connect(self._always_scenario_selected)
         self.dia.closeEvent = self.closeEvent
 
+    def change_font_size(self):
+        size = self.gui_structure.option_font_size.get_value()
+        globs.FONT_SIZE = size
+        rcParams.update({'font.size': size})
+        self.gui_structure.change_font_size_2(size)
+        change_font_size(self.push_button_save_scenario, size)
+        change_font_size(self.push_button_add_scenario, size)
+        change_font_size(self.push_button_delete_scenario, size)
+        change_font_size(self.button_rename_scenario, size)
+        change_font_size(self.push_button_cancel, size)
+        change_font_size(self.push_button_start_single, size)
+        change_font_size(self.push_button_start_multiple, size)
+        change_font_size(self.menu_scenario, size)
+        change_font_size(self.menu_calculation, size)
+        change_font_size(self.menu_file, size)
+        change_font_size(self.menu_settings, size)
+        change_font_size(self.menu_language, size)
+        change_font_size(self.menubar, size)
+        change_font_size(self.list_widget_scenario, size)
+        change_font_size(self.status_bar.widget, size)
+        self.remove_previous_calculated_results()
+
     def export_results(self, result_export: ResultExport):
         filename: tuple = QtW.QFileDialog.getSaveFileName(
             self.central_widget,
             caption=result_export.caption,
             filter=f".{result_export.file_extension} (*.{result_export.file_extension})",
             dir=str(self.default_path),
         )
@@ -463,14 +489,15 @@
             return
         # get test of old scenario (item)
         text = old_row_item.text()
         # check if the old scenario is unsaved then create message box
         if text[-1] == "*":
             # create message box
             self.dialog: QtW.QMessageBox = QtW.QMessageBox(self.dia)
+            set_default_font(self.dialog)
             # set Icon to question mark icon
             self.dialog.setIcon(QtW.QMessageBox.Question)
             # set label text to leave scenario text depending on language selected
             self.dialog.setText(self.translations.label_LeaveScenarioText[self.gui_structure.option_language.get_value()[0]])
             # set window text to  leave scenario text depending on language selected
             self.dialog.setWindowTitle(self.translations.label_CancelTitle[self.gui_structure.option_language.get_value()[0]])
             # set standard buttons to save, close and cancel
@@ -483,14 +510,15 @@
             button_s.setText(f"{self.translations.push_button_save_scenario[self.gui_structure.option_language.get_value()[0]]} ")
             button_cl.setText(f"{self.translations.label_LeaveScenario[self.gui_structure.option_language.get_value()[0]]} ")
             button_ca.setText(f"{self.translations.label_StayScenario[self.gui_structure.option_language.get_value()[0]]} ")
             # set  save, close and cancel button icon
             self.set_push_button_icon(button_s, "Save_Inv")
             self.set_push_button_icon(button_cl, "Exit")
             self.set_push_button_icon(button_ca, "Abort")
+            [set_default_font(button) for button in self.dialog.findChildren(QtW.QPushButton)]
             # execute message box and save response
             reply = self.dialog.exec()
             # check if closing should be canceled
             if reply == QtW.QMessageBox.Cancel:
                 return_2_old_item()
                 return
             # save scenario if wanted
@@ -579,21 +607,23 @@
         item = self.list_widget_scenario.item(0) if item is None else item
         if name:
             set_name(name)
             return
 
         # create dialog box to ask for a new name
         self.dialog = QtW.QInputDialog(self.dia)
+        set_default_font(self.dialog)
         self.dialog.setWindowTitle(self.translations.label_new_scenario[self.gui_structure.option_language.get_value()[0]])
         self.dialog.setLabelText(f"{self.translations.new_name[self.gui_structure.option_language.get_value()[0]]}{item.text()}")
         self.dialog.setOkButtonText(self.translations.label_okay[self.gui_structure.option_language.get_value()[0]])  # +++
         self.dialog.setCancelButtonText(self.translations.label_abort[self.gui_structure.option_language.get_value()[0]])  # +++
         li = self.dialog.findChildren(QtW.QPushButton)
         self.set_push_button_icon(li[0], "Okay")
         self.set_push_button_icon(li[1], "Abort")
+        [set_default_font(button) for button in li]
         # set new name if the dialog is not canceled and the text is not None
         if self.dialog.exec() == QtW.QDialog.Accepted:
             set_name(self.dialog.textValue())
 
         self.dialog = None
 
     def check_results(self) -> None:
@@ -1344,26 +1374,28 @@
         """
         # close app if nothing has been changed
         if not self.changedFile:
             event.accept()
             return
         # create message box
         self.dialog: QtW.QMessageBox = QtW.QMessageBox(self.dia)
+        set_default_font(self.dialog)
         # set Icon to question mark icon
         self.dialog.setIcon(QtW.QMessageBox.Question)
         # set label text to cancel text depending on language selected
         self.dialog.setText(self.translations.label_CancelText[self.gui_structure.option_language.get_value()[0]])
         # set window text to cancel text depending on language selected
         self.dialog.setWindowTitle(self.translations.label_CancelTitle[self.gui_structure.option_language.get_value()[0]])
         # set standard buttons to save, close and cancel
         self.dialog.setStandardButtons(QtW.QMessageBox.Save | QtW.QMessageBox.Close | QtW.QMessageBox.Cancel)
         # get save, close and cancel button
         button_s = self.dialog.button(QtW.QMessageBox.Save)
         button_cl = self.dialog.button(QtW.QMessageBox.Close)
         button_ca = self.dialog.button(QtW.QMessageBox.Cancel)
+        [set_default_font(button) for button in self.dialog.findChildren(QtW.QPushButton)]
         # set save, close and cancel button text depending on language selected
         button_s.setText(f"{self.translations.label_Save[self.gui_structure.option_language.get_value()[0]]} ")
         button_cl.setText(f"{self.translations.label_close[self.gui_structure.option_language.get_value()[0]]} ")
         button_ca.setText(f"{self.translations.label_cancel[self.gui_structure.option_language.get_value()[0]]} ")
         # set  save, close and cancel button icon
         self.set_push_button_icon(button_s, "Save_Inv")
         self.set_push_button_icon(button_cl, "Exit")
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_data_storage.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_data_storage.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     IntBox,
     ListBox,
     Option,
     Page,
     ResultExport, ResultFigure,
     ResultText,
 )
+from ScenarioGUI import global_settings as globs
 
 if TYPE_CHECKING:
     import PySide6.QtWidgets as QtW
 
     from ScenarioGUI.gui_classes.translation_class import Translations
 
 
@@ -55,18 +56,20 @@
         # self.page_settings = None
         # self.category_language = None
         # self.option_language = None
         # self.category_save_scenario = None
         # self.option_toggle_buttons = None
         # self.option_auto_saving = None
         # self.hint_saving = None
+        self.option_font_size = None
 
         self.list_of_aims: list[tuple[Aim, str]] = []
         self.list_of_options: list[tuple[Option, str]] = []
         self.list_of_pages: list[Page] = []
+        self.list_of_rest: list[Hint | FunctionButton | Category] = []
 
         self.list_of_result_texts: list[tuple[ResultText, str]] = []
         self.list_of_result_figures: list[tuple[ResultFigure, str]] = []
         self.list_of_result_exports: list[tuple[ResultExport, str]] = []
 
         self.list_of_options_with_dependent_results: list[tuple[Option, str]] = []
 
@@ -105,14 +108,16 @@
             label=self.translations.option_toggle_buttons,
             default_index=1,
             entries=[" no ", " yes "],
             category=self.category_save_scenario,
         )
         self.option_toggle_buttons.change_event(self.change_toggle_button)
         self.option_n_threads = IntBox(label=self.translations.option_n_threads, default_value=2, category=self.category_save_scenario, minimal_value=1)
+        self.option_font_size = IntBox(label="Font Size", default_value= globs.FONT_SIZE, category= self.category_save_scenario, minimal_value=8,
+                                       maximal_value=14)
         self.option_auto_saving = ButtonBox(
             label=self.translations.option_auto_saving,
             default_index=0,
             entries=[" no ", " yes "],
             category=self.category_save_scenario,
         )
         self.hint_saving = Hint(
@@ -120,31 +125,48 @@
             hint=self.translations.hint_saving,
         )
 
     def create_lists(self):
         """
         creates the lists with the different elements
         """
-        self.list_of_aims: list[tuple[Aim, str]] = [(getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), Aim)]
-        self.list_of_options: list[tuple[Option, str]] = [(getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), Option)]
-        self.list_of_pages: list[Page] = [getattr(self, name) for name in self.__dict__ if isinstance(getattr(self, name), Page)]
+        self.list_of_aims = [(getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), Aim)]
+        self.list_of_options = [(getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), Option)]
+        self.list_of_pages = [getattr(self, name) for name in self.__dict__ if isinstance(getattr(self, name), Page)]
+        self.list_of_rest = [getattr(self, name) for name in self.__dict__ if isinstance(getattr(self, name), (Hint,
+                                                                                                                                             FunctionButton,
+                                                                                                                                            Category))]
 
         self.list_of_result_texts: list[tuple[ResultText, str]] = [
             (getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), ResultText)
         ]
         self.list_of_result_figures: list[tuple[ResultFigure, str]] = [
             (getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), ResultFigure)
         ]
         self.list_of_result_exports: list[tuple[ResultExport, str]] = [
             (getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), ResultExport)
         ]
         self.list_of_options_with_dependent_results: list[tuple[Option, str]] = [
             (getattr(self, name), name) for name in self.__dict__ if isinstance(getattr(self, name), Option) if getattr(self, name).linked_options
         ]
 
+    def change_font_size_2(self, size: int) -> None:
+        """
+        changes the font size to the size value
+
+        Parameters
+        ----------
+        size: int
+            new font size
+        """
+        _ = [option.set_font_size(size) for option, _ in self.list_of_options]
+        _ = [aim.set_font_size(size) for aim, _ in self.list_of_aims]
+        _ = [item.set_font_size(size) for item in self.list_of_rest]
+        _ = [page.set_font_size(size) for page in self.list_of_pages]
+
 
     def change_toggle_button(self) -> None:
         """
         This function changes the behaviour of both the ButtonBox and aim selection
         from either toggle behaviour to not-change behaviour.
 
         Returns
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/aim.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/aim.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, Protocol
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -79,14 +80,28 @@
 
         Returns
         -------
         None
         """
         self.widget.setText(name)
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the new font size to button
+
+        Parameters
+        ----------
+        size: new font size in points
+
+        Returns
+        -------
+            None
+        """
+        change_font_size(self.widget, size)
+
     def change_event(self, function_to_be_called: Callable, *args) -> None:
         """
         This function calls the function_to_be_called whenever the Aim is changed.
 
         Parameters
         ----------
         function_to_be_called : callable
@@ -144,21 +159,22 @@
         self.widget.setParent(frame)
         push_button = self.widget
         push_button.setIcon(icon11)
         push_button.setMinimumSize(QtC.QSize(0, 60))
         push_button.setMaximumSize(QtC.QSize(16777215, 60))
         push_button.setStyleSheet(
             f"QPushButton{'{'}border: 3px solid {globs.DARK};border-radius: 15px;color:{globs.WHITE};gridline-color: {globs.LIGHT};"
-            f"background-color: {globs.GREY};font-weight:700;{'}'}"
+            f"background-color: {globs.GREY};{'}'}"
             f"QPushButton:hover{'{'}border: 3px solid {globs.DARK};background-color:{globs.LIGHT};{'}'}"
             f"QPushButton:checked{'{'}border:3px solid {globs.LIGHT};background-color:{globs.LIGHT};{'}'}\n"
             f"QPushButton:disabled{'{'}border: 3px solid {globs.GREY};border-radius: 5px;color: {globs.WHITE};gridline-color: {globs.GREY};"
             f"background-color: {globs.GREY};{'}'}\n"
             f"QPushButton:disabled:hover{'{'}background-color: {globs.DARK};{'}'}"
         )
+        set_default_font(push_button, bold=True)
         push_button.setIconSize(QtC.QSize(30, 30))
         push_button.setCheckable(True)
         push_button.setText(self.label[0])
         layout.addWidget(push_button, int(idx / 2), 0 if divmod(idx, 2)[1] == 0 else 1, 1, 1)
 
     def translate(self, idx: int) -> None:
         """
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import partial as ft_partial
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
-from .functions import _update_opponent_not_change, _update_opponent_toggle, check
+from .functions import update_opponent_not_change, update_opponent_toggle, check
 from .option import Option
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
@@ -241,14 +241,18 @@
                 f"QPushButton:disabled{'{'}border: 3px solid {globs.GREY};border-radius: 5px;color: {globs.WHITE};"
                 f"gridline-color: {globs.GREY};background-color: {globs.GREY};{'}'}\n"
                 f"QPushButton:disabled:hover{'{'}background-color: {globs.DARK};{'}'}"
             )
             widget.setCheckable(True)
             widget.setChecked(idx == self.default_value)
             widget.setMinimumHeight(30)
+            font = widget.font()
+            font.setFamily(globs.FONT)
+            font.setPointSize(globs.FONT_SIZE)
+            widget.setFont(font)
             layout.addWidget(widget)
 
     def update_function(
         self,
         button: QtW.QPushButton,
         button_opponent: QtW.QPushButton,
         false_button_list: list[QtW.QPushButton] = None,
@@ -267,10 +271,10 @@
             List with other buttons which aren't active
 
         Returns
         -------
         None
         """
         if self.TOGGLE:
-            _update_opponent_toggle(button, button_opponent, false_button_list)
+            update_opponent_toggle(button, button_opponent, false_button_list)
             return
-        _update_opponent_not_change(button, [*false_button_list, button_opponent])
+        update_opponent_not_change(button, [*false_button_list, button_opponent])
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/category.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .hint import Hint
 from .result_text import ResultText
+from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from .function_button import FunctionButton
     from .option import Option
     from .page import Page
 
 
@@ -153,14 +154,15 @@
         self.label.setText(self.label_text[0])
         self.label.setStyleSheet(
             f"QLabel {'{'}border: 1px solid  {globs.LIGHT};border-top-left-radius: 15px;border-top-right-radius: 15px;"
             f"background-color:  {globs.LIGHT};padding: 5px 0px;\n"
             f"	color:  {globs.WHITE};font-weight:700;{'}'}"
         )
         self.label.setAlignment(QtC.Qt.AlignCenter | QtC.Qt.AlignVCenter)
+        set_default_font(self.label, bold=True)
         layout.addWidget(self.label)
         self.frame.setParent(page)
         self.frame.setStyleSheet(
             f"QFrame{'{'}border: 1px solid {globs.LIGHT};border-bottom-left-radius: 15px;border-bottom-right-radius: 15px;{'}'}\n"
             f"QLabel{'{'}border: 0px solid {globs.WHITE};{'}'}"
         )
         self.frame.setFrameShape(QtW.QFrame.StyledPanel)
@@ -220,15 +222,14 @@
         graphic_view = QtW.QGraphicsView(self.frame)
         graphic_view.setMinimumSize(QtC.QSize(0, 0))
         graphic_view.setMaximumSize(QtC.QSize(100, 16777215))
         graphic_view.setStyleSheet(
             f"QFrame{'{'}border: 1px solid {globs.LIGHT};border-bottom-left-radius: 0px;border-bottom-right-radius: 0px;{'}'}\n"
             f"QLabel{'{'}border: 0px solid {globs.WHITE};{'}'}"
         )
-
         layout.addWidget(graphic_view)
         return graphic_view
 
     def hide(self, **kwargs) -> None:
         """
         This function makes the current category invisible and everything on them.
         It makes sure that it only hides the objects that were not already hidden
@@ -289,9 +290,23 @@
 
         Returns
         -------
         None
         """
         self.set_text(self.label_text[idx])
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the new font size to button
+
+        Parameters
+        ----------
+        size: new font size in points
+
+        Returns
+        -------
+            None
+        """
+        change_font_size(self.label, size)
+
     def __repr__(self):
         return f"{type(self).__name__}; Label: {self.label_text[0]}"
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .option import Option
+from ...utils import set_default_font, change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
 
 
@@ -188,27 +189,44 @@
         -------
         None
         """
         layout = self.create_frame(frame, layout_parent, False)
         self.widget.setParent(self.frame)
         self.widget.setStyleSheet(
             f"QLineEdit{'{'}border: 3px solid {globs.LIGHT};border-radius: 5px;color: {globs.WHITE};gridline-color: {globs.LIGHT};"
-            f"background-color: {globs.LIGHT};font-weight:500;\n"
+            f"background-color: {globs.LIGHT};\n"
             f"selection-background-color: {globs.LIGHT_SELECT};{'}'}\n"
             f"QLineEdit:hover{'{'}background-color: {globs.DARK};{'}'}"
         )
         self.widget.setText(self.default_value)
+        set_default_font(self.widget)
         layout.addWidget(self.widget)
         self.button.setParent(self.frame)
         self.button.setMinimumSize(QtC.QSize(30, 30))
         self.button.setMaximumSize(QtC.QSize(30, 30))
         self.button.setText("...")
+        set_default_font(self.button)
         self.button.clicked.connect(self.fun_choose_file)  # pylint: disable=E1101
         layout.addWidget(self.button)
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the new font size to label, text box and button
+
+        Parameters
+        ----------
+        size: new font size in points
+
+        Returns
+        -------
+            None
+        """
+        super().set_font_size(size)
+        change_font_size(self.button, size)
+
     def fun_choose_file(self) -> None:
         """
         This function opens a file selector, with which the filename path can be selected.
         This is automatically added to the FileNameBox.
 
         Returns
         -------
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .option import Option
+from ...utils import set_default_font, change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -80,26 +81,30 @@
     def add_option(self, option: type[Option], name: str, **kwargs):
         self.option_classes.append((option, kwargs, name))
 
     def _add_entry(self) -> None:
         length = len(self.option_entries)
         label = QtW.QLabel(self.frame)
         label.setText(f"{self.entry_name} {length + 1}")
+        set_default_font(label)
         self.frame.layout().addWidget(label, length + 1, 0)
         options = []
         i = 2
         for option, kwargs, _ in self.option_classes:
             option_i = option(**kwargs, category=self, label="")
             option_i.change_event(self.func_on_change)
             option_i.create_widget(self.frame, self.frame.layout(), column=length + 1, row=i)
+            set_default_font(option_i.widget)
             options.append(option_i)
             i += 1
         self.option_entries.append(options)
         add_button: QtW.QPushButton = QtW.QPushButton(text=" + ", parent=self.frame, clicked=partial(self._add_entry_at_row, row=length))
         delete_button: QtW.QPushButton = QtW.QPushButton(text=" - ", parent=self.frame, clicked=partial(self._del_entry, row=length))
+        set_default_font(add_button, bold=True)
+        set_default_font(delete_button, bold=True)
         self.frame.layout().addWidget(add_button, length + 1, i)
         self.frame.layout().addWidget(delete_button, length + 1, i + 1)
 
     def _add_entry_at_row(self, row: int):
         values = self.get_value()
         values.insert(row + 1, values[row]) if row + 1 < len(values) else values.append(values[row])
         self.set_value(values)
@@ -316,14 +321,29 @@
         -------
         None
         """
         self.func_on_change = function_to_be_called
         for option in self.list_of_options:
             option.change_event(function_to_be_called)
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the new font size to button
+
+        Parameters
+        ----------
+        size: new font size in points
+
+        Returns
+        -------
+            None
+        """
+        change_font_size(self.label, size)
+        [change_font_size(widget, size) for widget in self.frame.children() if isinstance(widget, QtW.QWidget)]
+
     def create_widget(
             self,
             frame: QtW.QFrame,
             layout_parent: QtW.QLayout,
             *,
             row: int = None,
             column: int = None,
@@ -358,16 +378,17 @@
         layout_parent_i.setContentsMargins(0, 0, 0, 0)
         self.label.setParent(frame_i)
         self.label.setText(self.label_text[0])
         self.label.setStyleSheet(
             f"QLabel {'{'}border: 1px solid  {globs.LIGHT};border-top-left-radius: 15px;border-top-right-radius: 15px;"
             f"border-bottom-left-radius: 0px;border-top-right-radius: 0px;"
             f"background-color:  {globs.LIGHT};padding: 5px 0px;\n"
-            f"	color:  {globs.WHITE};font-weight:700;{'}'}"
+            f"	color:  {globs.WHITE};{'}'}"
         )
+        set_default_font(self.label, bold=True)
         self.label.setAlignment(QtC.Qt.AlignCenter | QtC.Qt.AlignVCenter)
         layout_parent_i.addWidget(self.label)
         self.frame.setParent(frame_i)
         self.frame.setStyleSheet(
             f"QFrame{'{'}border: 1px solid {globs.LIGHT};border-bottom-left-radius: 15px;border-bottom-right-radius: 15px;{'}'}\n"
             f"QLabel{'{'}border: 0px solid {globs.WHITE};{'}'}"
         )
@@ -382,12 +403,13 @@
 
         spacer = QtW.QSpacerItem(1, 1, QtW.QSizePolicy.Expanding, QtW.QSizePolicy.Minimum)
         self.frame.layout().addItem(spacer)
         i = 2
         for _, _, name in self.option_classes:
             label = QtW.QLabel(frame)
             label.setText(name)
+            set_default_font(label)
             self.frame.layout().addWidget(label, 0, i)
             i += 1
 
         _ = [self._add_entry() for _ in range(self.default_value)]
         layout_parent_i.addWidget(self.frame)
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .option import Option
+from ...utils import set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -257,24 +258,25 @@
         -------
         None
         """
         layout = self.create_frame(frame, layout_parent)
         self.widget.setParent(self.frame)
         self.widget.setStyleSheet(
             f'QDoubleSpinBox{"{"}selection-color: {globs.WHITE};selection-background-color: {globs.LIGHT};'
-            f'border: 1px solid {globs.WHITE};font: {globs.FONT_SIZE}pt "{globs.FONT}";{"}"}'
+            f'border: 1px solid {globs.WHITE};{"}"}'
         )
         self.widget.setAlignment(QtC.Qt.AlignRight | QtC.Qt.AlignTrailing | QtC.Qt.AlignVCenter)
         self.widget.setProperty("showGroupSeparator", True)
         self.widget.setMinimum(self.minimal_value)
         self.widget.setMaximum(self.maximal_value)
         self.widget.setDecimals(self.decimal_number)
         self.widget.setValue(self.default_value)
         self.widget.setSingleStep(self.step)
         if self.limit_size:
             self.widget.setMaximumWidth(100)
             self.widget.setMinimumWidth(100)
         self.widget.setMinimumHeight(28)
+        set_default_font(self.widget)
         if row is not None and isinstance(layout_parent, QtW.QGridLayout):
             layout_parent.addWidget(self.widget, column, row)
             return
         layout.addWidget(self.widget)
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from ..gui_structure_classes import Category
 
 
@@ -75,14 +76,15 @@
         icon = QtG.QIcon()
         # icon11.addPixmap(QtGui_QPixmap(icon), QtGui_QIcon.Normal, QtGui_QIcon.Off)
         icon.addFile(f"{globs.FOLDER}/icons/{self.icon}")
         self.button.setIcon(icon)
         self.button.setIconSize(QtC.QSize(20, 20))
         self.button.setMinimumWidth(100)
         self.button.setMinimumHeight(35)
+        set_default_font(self.button)
         self.frame.setParent(frame)
         self.frame.setFrameShape(QtW.QFrame.StyledPanel)
         self.frame.setFrameShadow(QtW.QFrame.Raised)
         self.frame.setStyleSheet(f"QFrame{'{'}border: 0px solid {globs.WHITE};border-radius: 0px;{'}'}")
         layout = QtW.QHBoxLayout(self.frame)
         layout.setSpacing(6)
         layout.setContentsMargins(0, 0, 0, 0)
@@ -154,14 +156,29 @@
 
         Returns
         -------
         None
         """
         self.button.clicked.connect(lambda: function_to_be_called(*args))
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the text size of hint
+
+        Parameters
+        ----------
+        size: int
+            new font size as points
+        Returns
+        -------
+
+        """
+        if self.button is not None:
+            change_font_size(self.button, size, False)
+
     def translate(self, idx: int) -> None:
         """
         Translates the label.
 
         Parameters
         ----------
         idx: int
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/functions.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if TYPE_CHECKING:
     import PySide6.QtWidgets as QtW  # type: ignore
 
     from .aim import Aim
     from .option import Option
 
 
-def _update_opponent_not_change(button: QtW.QPushButton, false_button_list: list[QtW.QPushButton] = None):
+def update_opponent_not_change(button: QtW.QPushButton, false_button_list: list[QtW.QPushButton] = None):
     """
     This function controls the behaviour of the buttons.
     This function makes sure that whenever a button is active, all other buttons except the current one,
     are inactive. If the current button is already active, nothing changes.
 
     Parameters
     ----------
@@ -33,15 +33,15 @@
         button.setChecked(True)
         return
     for but in false_button_list:
         if but != button:
             but.setChecked(False)
 
 
-def _update_opponent_toggle(
+def update_opponent_toggle(
     button: QtW.QPushButton,
     button_opponent: QtW.QPushButton,
     false_button_list: list[QtW.QPushButton] = None,
 ):
     """
     This function controls the behaviour of the buttons, specifically the toggle behaviour.
     This function makes sure that whenever a button is pressed, all other buttons except the current one,
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/hint.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/hint.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from .category import Category
 
 
 class Hint:
     """
@@ -76,14 +77,15 @@
         -------
         None
         """
         self.label.setParent(frame)
         self.label.setText(self.hint[0])
         if self.warning:
             self.label.setStyleSheet(f"color: {globs.WARNING};")
+        set_default_font(self.label)
         self.label.setWordWrap(True)
         if row is not None and isinstance(layout_parent, QtW.QGridLayout):
             layout_parent.addWidget(self.label, column, row)
             return
         layout_parent.addWidget(self.label)
 
     def hide(self) -> None:
@@ -128,14 +130,29 @@
 
         Returns
         -------
         None
         """
         self.label.setText(name)
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the text size of hint
+
+        Parameters
+        ----------
+        size: int
+            new font size as points
+        Returns
+        -------
+
+        """
+        if self.label is not None:
+            change_font_size(self.label, size, False)
+
     def translate(self, idx: int) -> None:
         """
         Translates the label.
 
         Parameters
         ----------
         idx: int
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .option import Option
+from ...utils import set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -252,21 +253,22 @@
         -------
         None
         """
         layout = self.create_frame(frame, layout_parent)
         self.widget.setParent(self.frame)
         self.widget.setStyleSheet(
             f'QSpinBox{"{"}selection-color: {globs.WHITE};selection-background-color: {globs.LIGHT};'
-            f'border: 1px solid {globs.WHITE};font: {globs.FONT_SIZE}pt "{globs.FONT}";{"}"}'
+            f'border: 1px solid {globs.WHITE};{"}"}'
         )
         self.widget.setAlignment(QtC.Qt.AlignRight | QtC.Qt.AlignTrailing | QtC.Qt.AlignVCenter)
         self.widget.setMinimum(self.minimal_value)
         self.widget.setMaximum(self.maximal_value)
         self.widget.setValue(self.default_value)
         self.widget.setSingleStep(self.step)
         self.widget.setMaximumWidth(100)
         self.widget.setMinimumWidth(100)
         self.widget.setMinimumHeight(28)
+        set_default_font(self.widget)
         if row is not None and isinstance(layout_parent, QtW.QGridLayout):
             layout_parent.addWidget(self.widget, column, row)
             return
         layout.addWidget(self.widget)
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .functions import check
 from .option import Option
+from ...utils import set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -231,11 +232,12 @@
         self.widget.addItems(self.entries)
         self.widget.setCurrentIndex(self.default_value)
         if self.limit_size:
             # self.widget.setMaximumWidth(100)
             self.widget.setMinimumWidth(100)
         self.widget.currentIndexChanged.connect(ft_partial(check, self.linked_options, self))  # pylint: disable=E1101
         self.widget.setMinimumHeight(28)
+        set_default_font(self.widget)
         if row is not None and isinstance(layout_parent, QtW.QGridLayout):
             layout_parent.addWidget(self.widget, column, row)
             return
         layout.addWidget(self.widget)
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/option.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import abc
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+from ScenarioGUI.utils import change_font_size, set_default_font
 
 from .aim import Aim
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
     from typing import Protocol
 
@@ -227,24 +228,26 @@
         QtW.QHBoxLayout
             The frame created for this option
         """
 
         if self.label_text == [""]:
             self.frame.setParent(None)
             self.frame = frame
+            self.label = None
             return frame.layout()
         self.frame.setParent(frame)
         self.frame.setFrameShape(QtW.QFrame.StyledPanel)
         self.frame.setFrameShadow(QtW.QFrame.Raised)
         self.frame.setStyleSheet("QFrame {\n" f"	border: 0px solid {globs.WHITE};\n" "	border-radius: 0px;\n" "  }\n")
         layout = QtW.QHBoxLayout(self.frame)
         layout.setSpacing(6)
         layout.setContentsMargins(0, 0, 0, 0)
         self.label.setParent(frame)
         self.label.setText(self.label_text[0])
+        set_default_font(self.label)
         layout.addWidget(self.label)
         if create_spacer:
             spacer = QtW.QSpacerItem(1, 1, QtW.QSizePolicy.Expanding, QtW.QSizePolicy.Minimum)
             layout.addItem(spacer)
         layout_parent.addWidget(self.frame)
         return layout
 
@@ -317,14 +320,23 @@
             Function which should be called
 
         Returns
         -------
         None
         """
 
+    def set_font_size(self, size: int) -> None:
+        if self.label is not None:
+            change_font_size(self.label, size, False)
+        if isinstance(self.widget, list):
+            for widget in self.widget:
+                change_font_size(widget, size, True)
+            return
+        change_font_size(self.widget, size, True)
+
     def translate(self, idx: int) -> None:
         """
         Translates the label.
 
         Parameters
         ----------
         idx: int
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/page.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
 from .aim import Aim
-from .functions import _update_opponent_not_change, _update_opponent_toggle, check_aim_options
+from .functions import update_opponent_not_change, update_opponent_toggle, check_aim_options
+from ...utils import set_default_font, change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
 
 
@@ -161,16 +162,16 @@
         None
         """
         self.page.setParent(central_widget)
         layout = QtW.QVBoxLayout(self.page)
         layout.setSpacing(0)
         self.label.setParent(central_widget)
         label: QtW.QLabel = self.label
-        label.setStyleSheet(f'font: {globs.FONT_SIZE+4}pt "{globs.FONT}";font-weight:700;')
         label.setText(self.name[0].split(",")[0])
+        set_default_font(label, bold=True, add_2_size=4)
         layout.addWidget(label)
         spacer_label = QtW.QLabel(self.page)
         spacer_label.setMinimumHeight(6)
         spacer_label.setMaximumHeight(6)
         layout.addWidget(spacer_label)
         scroll_area = QtW.QScrollArea(self.page)
         scroll_area.setFrameShape(QtW.QFrame.NoFrame)
@@ -203,24 +204,44 @@
         self.button.setParent(central_widget)
         self.button.setMinimumSize(QtC.QSize(100, 100))
         icon23 = QtG.QIcon()
         icon23.addFile(f"{globs.FOLDER}/icons/{self.icon}", QtC.QSize(), QtG.QIcon.Normal, QtG.QIcon.Off)
         self.button.setIcon(icon23)
         self.button.setIconSize(QtC.QSize(24, 24))
         self.button.setText(self.button_name)
+        set_default_font(self.button, bold=True)
         self.label_gap.setParent(central_widget)
         self.label_gap.setMinimumSize(QtC.QSize(0, 6))
         self.label_gap.setMaximumSize(QtC.QSize(16777215, 6))
 
         vertical_layout_menu.addWidget(self.button)
         vertical_layout_menu.addWidget(self.label_gap)
         self.button.clicked.connect(ft_partial(stacked_widget.setCurrentWidget, self.page))  # pylint: disable=E1101
         for function_2_be_called in self.functions_button_clicked:
             self.button.clicked.connect(function_2_be_called)  # pylint: disable=E1101
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the text size of hint
+
+        Parameters
+        ----------
+        size: int
+            new font size as points
+        Returns
+        -------
+
+        """
+        change_font_size(self.label, size + 4, False)
+        change_font_size(self.button, size, False)
+        if self.push_button_previous is not None:
+            change_font_size(self.push_button_previous, size, False)
+        if self.push_button_next is not None:
+            change_font_size(self.push_button_next, size, False)
+
     def create_upper_frame(self, scroll_area_content: QtW.QWidget, scroll_area_layout: QtW.QVBoxLayout):
         """
         This function creates the upper frame of the GUI, i.e. the first visible screen.
 
         Parameters
         ----------
         scroll_area_content : QtW.QWidget
@@ -283,17 +304,17 @@
             List with other buttons which aren't active
 
         Returns
         -------
         None
         """
         if self.TOGGLE:
-            _update_opponent_toggle(button, button_opponent, false_button_list)
+            update_opponent_toggle(button, button_opponent, false_button_list)
             return
-        _update_opponent_not_change(button, [*false_button_list, button_opponent])
+        update_opponent_not_change(button, [*false_button_list, button_opponent])
 
     def create_navigation_buttons(self, central_widget: QtW.QWidget, scroll_area_layout: QtW.QVBoxLayout) -> None:
         """
         This function creates the navigation button (previous and next) on the bottom of each Page.
 
         Parameters
         ----------
@@ -321,14 +342,15 @@
                 QtC.QSize(),
                 QtG.QIcon.Normal,
                 QtG.QIcon.Off,
             )
             self.push_button_previous.setIcon(icon)
             self.push_button_previous.setIconSize(QtC.QSize(20, 20))
             self.push_button_previous.setText(f"  {self.previous_label}  ")
+            set_default_font(self.push_button_previous, bold=True)
 
             horizontal_layout.addWidget(self.push_button_previous)
             self.push_button_previous.clicked.connect(self.previous_page.button.click)  # pylint: disable=E1101
 
         horizontal_spacer = QtW.QSpacerItem(1, 1, QtW.QSizePolicy.Expanding, QtW.QSizePolicy.Minimum)
 
         horizontal_layout.addItem(horizontal_spacer)
@@ -343,14 +365,15 @@
                 QtC.QSize(),
                 QtG.QIcon.Normal,
                 QtG.QIcon.Off,
             )
             self.push_button_next.setIcon(icon)
             self.push_button_next.setIconSize(QtC.QSize(20, 20))
             self.push_button_next.setText(f"  {self.next_label}  ")
+            set_default_font(self.push_button_next, bold=True)
 
             horizontal_layout.addWidget(self.push_button_next)
             self.push_button_next.clicked.connect(self.next_page.button.click)  # pylint: disable=E1101
 
         scroll_area_layout.addLayout(horizontal_layout)
 
     def translate(self, idx: int) -> None:
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 import ScenarioGUI.global_settings as globs
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
 from .category import Category
+from ...utils import change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from .page import Page
 
 
 class ResultFigure(Category):
     """
@@ -258,14 +259,28 @@
         """
         if self.to_show:
             super().show()
         if results:
             return
         self.to_show = True
 
+    def set_font_size(self, size: int) -> None:
+        """
+        set the new font size to button
+
+        Parameters
+        ----------
+        size: new font size in points
+
+        Returns
+        -------
+            None
+        """
+        change_font_size(self.label, size)
+
     def hide(self, results: bool = False) -> None:
         """
         This function hides the ResultFigure option.
         It also sets the to_show parameter to False, so the Figure is not randomly showed
         when the result page is opened.
 
         Parameters
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/status_bar_logger.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/status_bar_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from logging import Handler
 from typing import TYPE_CHECKING
 
 from PySide6.QtWidgets import QStatusBar
 
 import ScenarioGUI.global_settings as globs
+from ScenarioGUI.utils import set_default_font
 
 if TYPE_CHECKING:
     from logging import LogRecord
 
     from PySide6.QtWidgets import QWidget
 
 
@@ -28,14 +29,15 @@
         Parameters
         ----------
         parent: QtW.QWidget
             parent to create QStatusBar in
         """
         super().__init__()
         self.widget: QStatusBar = QStatusBar(parent)
+        set_default_font(self.widget)
         self.level_2_color: dict[str, str] = {
             "DEBUG": f"{globs.WHITE}",
             "INFO": f"{globs.WHITE}",
             "ERROR": "rgb(255,0,0)",
             "CRITICAL": "rgb(255,0,0)",
             "WARNING": f"{globs.WARNING}",
         }
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/gui_classes/translation_class.py` & `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/translation_class.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI/translation_csv_to_py.py` & `ScenarioGUI-0.2.1/ScenarioGUI/translation_csv_to_py.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI.egg-info/PKG-INFO` & `ScenarioGUI-0.2.1/ScenarioGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScenarioGUI
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for a scenario based GUI
 Home-page: https://github.com/tblanke/ScenarioGUI
 Author: Tobias Blanke
 Author-email: blanke@fh-aachen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ScenarioGUI-0.2.0/ScenarioGUI.egg-info/SOURCES.txt` & `ScenarioGUI-0.2.1/ScenarioGUI.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
 ScenarioGUI/gui_classes/gui_structure_classes/option.py
 ScenarioGUI/gui_classes/gui_structure_classes/page.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
 ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
+ScenarioGUI/utils/__init__.py
+ScenarioGUI/utils/change_font_size.py
+ScenarioGUI/utils/set_default_font.py
 tests/__init__.py
 tests/gui_structure_for_tests.py
 tests/result_creating_class_for_tests.py
 tests/test_gui_structure_elements/__init__.py
 tests/test_gui_structure_elements/test_aim.py
 tests/test_gui_structure_elements/test_button_box.py
 tests/test_gui_structure_elements/test_category.py
@@ -56,14 +59,15 @@
 tests/test_gui_structure_elements/test_result_export.py
 tests/test_gui_structure_elements/test_results_figure.py
 tests/test_gui_structure_elements/test_results_text.py
 tests/test_gui_structure_elements/test_text_box.py
 tests/test_main_window_functions/__init__.py
 tests/test_main_window_functions/test_auto_save.py
 tests/test_main_window_functions/test_backup.py
+tests/test_main_window_functions/test_change_font_size.py
 tests/test_main_window_functions/test_close.py
 tests/test_main_window_functions/test_datastorage.py
 tests/test_main_window_functions/test_double_naming.py
 tests/test_main_window_functions/test_global_settings.py
 tests/test_main_window_functions/test_move_scenario.py
 tests/test_main_window_functions/test_new_save_load.py
 tests/test_main_window_functions/test_no_file.py
```

### Comparing `ScenarioGUI-0.2.0/pyproject.toml` & `ScenarioGUI-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/setup.cfg` & `ScenarioGUI-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 6365 6e61 7269 6f47 5549 0d0a   = ScenarioGUI..
-00000020: 7665 7273 696f 6e20 3d20 302e 322e 300d  version = 0.2.0.
+00000020: 7665 7273 696f 6e20 3d20 302e 322e 310d  version = 0.2.1.
 00000030: 0a61 7574 686f 7220 3d20 546f 6269 6173  .author = Tobias
 00000040: 2042 6c61 6e6b 650d 0a61 7574 686f 725f   Blanke..author_
 00000050: 656d 6169 6c20 3d20 626c 616e 6b65 4066  email = blanke@f
 00000060: 682d 6161 6368 656e 2e64 650d 0a64 6573  h-aachen.de..des
 00000070: 6372 6970 7469 6f6e 203d 2050 7974 686f  cription = Pytho
 00000080: 6e20 7061 636b 6167 6520 666f 7220 6120  n package for a 
 00000090: 7363 656e 6172 696f 2062 6173 6564 2047  scenario based G
```

### Comparing `ScenarioGUI-0.2.0/tests/gui_structure_for_tests.py` & `ScenarioGUI-0.2.1/tests/gui_structure_for_tests.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/result_creating_class_for_tests.py` & `ScenarioGUI-0.2.1/tests/result_creating_class_for_tests.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_aim.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_aim.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_button_box.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_button_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_category.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_category.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_filename.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_filename.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_flexible_amount_option.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_flexible_amount_option.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_float_box.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_float_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_function_button.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_function_button.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_int_box.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_int_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_list_box.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_list_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_page.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_page.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_repr.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_repr.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_result_export.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_result_export.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_results_figure.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_figure.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_results_text.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_text.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_gui_structure_elements/test_text_box.py` & `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_text_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_auto_save.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_auto_save.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_backup.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_backup.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_close.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_close.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,25 +57,25 @@
     def save():
         while main_window.dialog is None:  # pragma: no cover
             QtW.QApplication.processEvents()
         # handle dialog now
         if isinstance(main_window.dialog, QtW.QMessageBox):
             main_window.dialog.buttons()[0].click()
 
-    QtC.QTimer.singleShot(250, close)
+    QtC.QTimer.singleShot(500, close)
     main_window.close()
 
-    QtC.QTimer.singleShot(250, cancel)
+    QtC.QTimer.singleShot(500, cancel)
     main_window.close()
 
-    QtC.QTimer.singleShot(250, save)
+    QtC.QTimer.singleShot(500, save)
     
     def get_save_file_name(*args, **kwargs):
         """getSaveFileName proxy"""
         return kwargs["return_value"]
     
     QtW.QFileDialog.getSaveFileName = partial(get_save_file_name, return_value=(f"{filename_1}", f"{main_window.filename_default[1]}"))
     main_window.close()
 
-    QtC.QTimer.singleShot(250, exit_window)
+    QtC.QTimer.singleShot(500, exit_window)
     main_window.close()
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_datastorage.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_datastorage.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_double_naming.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_double_naming.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_move_scenario.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_move_scenario.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_new_save_load.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_new_save_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,11 +107,11 @@
     f"{main_window.default_path.joinpath(filename_3)}", f"{global_vars.FILE_EXTENSION} (*.{global_vars.FILE_EXTENSION})"))
     main_window.action_new.trigger()
     assert (Path(main_window.filename[0]), main_window.filename[1]) == (
         main_window.default_path.joinpath(filename_3),
         f"{global_vars.FILE_EXTENSION} (*.{global_vars.FILE_EXTENSION})",
     )
     assert len(main_window.list_ds) < 1
-    main_window.filename = (filename_1, filename_1)
+    main_window.filename = ("filename_1", filename_1)
     main_window.fun_load_known_filename()
     assert main_window.status_bar.widget.currentMessage() == main_window.translations.no_file_selected[0]
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_no_file.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_no_file.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_push_button_change.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_push_button_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_rename_scenario.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_rename_scenario.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_run.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_run.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_scenario_change.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_scenario_properties.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_properties.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_main_window_functions/test_toggle_buttons.py` & `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_toggle_buttons.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_translations/test_language_change.py` & `ScenarioGUI-0.2.1/tests/test_translations/test_language_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_translations/test_translation_csv_2_py.py` & `ScenarioGUI-0.2.1/tests/test_translations/test_translation_csv_2_py.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.0/tests/test_translations/translation_class.py` & `ScenarioGUI-0.2.1/tests/test_translations/translation_class.py`

 * *Files identical despite different names*

