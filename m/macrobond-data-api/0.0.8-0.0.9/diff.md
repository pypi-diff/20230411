# Comparing `tmp/macrobond-data-api-0.0.8.tar.gz` & `tmp/macrobond-data-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-ub8pw8x1/macrobond-data-api-0.0.8.tar", last modified: Wed Mar  1 08:16:36 2023, max compression
+gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-twqbz4ne/macrobond-data-api-0.0.9.tar", last modified: Wed Mar  1 14:26:43 2023, max compression
```

## Comparing `macrobond-data-api-0.0.8.tar` & `macrobond-data-api-0.0.9.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/_fill_metadata_from_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_weekdays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/util/save_credential_to_keyring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/subscription_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-01 08:16:36.000000 macrobond-data-api-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-01 08:15:17.000000 macrobond-data-api-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_fill_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_weekdays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/save_credential_to_keyring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/subscription_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/setup.py
```

### Comparing `macrobond-data-api-0.0.8/LICENSE` & `macrobond-data-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/PKG-INFO` & `macrobond-data-api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.8 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.9 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-0.0.8/README.md` & `macrobond-data-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/__init__.py` & `macrobond-data-api-0.0.9/macrobond_data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/_generated.py` & `macrobond-data-api-0.0.9/macrobond_data_api/_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
     Returns
     -------
     `Generator[macrobond_data_api.common.types.series_with_vintages.SeriesWithVintages]`
     """
     return _get_api().get_many_series_with_revisions(requests, include_not_modified)
 
 
-def get_nth_release(nth: int, *series_names: str, raise_error: bool = None) -> Sequence[Series]:
+def get_nth_release(
+    nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> Sequence[Series]:
     """
     Fetcha series where each value is the nth change of the value.
 
     Parameters
     ----------
     time : nth
         The nth change of each value.
@@ -202,15 +204,17 @@
         If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
     Returns
     -------
     `Sequence[macrobond_data_api.common.types.series.Series]`
     The result is in the same order as in the request.
     """
-    return _get_api().get_nth_release(nth, *series_names, raise_error=raise_error)
+    return _get_api().get_nth_release(
+        nth, *series_names, include_times_of_change=include_times_of_change, raise_error=raise_error
+    )
 
 
 def get_observation_history(series_name: str, *times: datetime) -> Sequence[SeriesObservationHistory]:
     """
     Get the revision of an observation.
 
     Parameters
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/_get_api.py` & `macrobond-data-api-0.0.9/macrobond_data_api/_get_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_revision.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     SeriesWithVintagesErrorCode,
     RevisionHistoryRequest,
     VintageValues,
 )
 
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
 
-from ._fill_metadata_from_entity import _fill_metadata_from_entity
+from ._fill_metadata import _fill_metadata_from_entity, _fill_values_metadata_from_series
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from .com_types import SeriesWithRevisions
 
     from .com_types import Series as ComSeries, Entity as ComEntity
@@ -77,93 +77,104 @@
             time_stamp_of_first_revision,
             time_stamp_of_last_revision,
             vintage_time_stamps,
         )
 
     series = self.database.FetchSeriesWithRevisions(series_names)
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.ErrorMessage if y.IsError else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.ErrorMessage) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence([to_obj(x, y) for x, y in zip(series_names, series)])
 
 
 def get_vintage_series(
     self: "ComApi", time: datetime, *series_names: str, raise_error: bool = None
 ) -> Sequence[VintageSeries]:
     def to_obj(series_name: str) -> VintageSeries:
         series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
         if series_with_revisions.IsError:
-            return VintageSeries(series_name, series_with_revisions.ErrorMessage, None, None, None, None)
+            return VintageSeries(series_name, series_with_revisions.ErrorMessage, None, None, None, None, None)
 
         try:
             series = series_with_revisions.GetVintage(time)
         except OSError as os_error:
             if os_error.errno == 22 and os_error.strerror == "Invalid argument":
                 raise ValueError("Invalid time") from os_error
             raise os_error
 
         if series.IsError:
-            return VintageSeries(series_name, series.ErrorMessage, None, None, None, None)
+            return VintageSeries(series_name, series.ErrorMessage, None, None, None, None, None)
 
         values, dates = _remove_padding(series)
 
         return VintageSeries(
-            series_name, "", _fill_metadata_from_entity(series), values, _datetime_to_datetime_timezone(dates), None
+            series_name,
+            "",
+            _fill_metadata_from_entity(series),
+            None,
+            values,
+            _datetime_to_datetime_timezone(dates),
+            None,
         )
 
     series = [to_obj(x) for x in series_names]
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
-def get_nth_release(self: "ComApi", nth: int, *series_names: str, raise_error: bool = None) -> Sequence[Series]:
+def get_nth_release(
+    self: "ComApi", nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> Sequence[Series]:
+    if len(series_names) == 0:
+        raise ValueError("No series names")
+
     def to_obj(series_name: str) -> Series:
         series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
         if series_with_revisions.IsError:
-            return Series(series_name, series_with_revisions.ErrorMessage, None, None, None)
+            return Series(series_name, series_with_revisions.ErrorMessage, None, None, None, None)
 
         series = series_with_revisions.GetNthRelease(nth)
         if series.IsError:
-            return Series(series_name, series.ErrorMessage, None, None, None)
+            return Series(series_name, series.ErrorMessage, None, None, None, None)
 
         values = [None if isnan(x) else x for x in series.Values]  # type: ignore
-
         dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
+        values_metadata = _fill_values_metadata_from_series(series) if include_times_of_change else None
 
-        return Series(series_name, None, _fill_metadata_from_entity(series), values, dates)
+        return Series(series_name, None, _fill_metadata_from_entity(series), values_metadata, values, dates)
 
     series = [to_obj(x) for x in series_names]
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
 def get_all_vintage_series(self: "ComApi", series_name: str) -> GetAllVintageSeriesResult:
     def to_obj(com_series: "ComSeries", name: str) -> VintageSeries:
         if com_series.IsError:
-            return VintageSeries(name, com_series.ErrorMessage, None, None, None, None)
+            return VintageSeries(name, com_series.ErrorMessage, None, None, None, None, None)
 
         values, dates = _remove_padding(com_series)
 
         return VintageSeries(
-            name, None, _fill_metadata_from_entity(com_series), values, _datetime_to_datetime_timezone(dates), None
+            name,
+            None,
+            _fill_metadata_from_entity(com_series),
+            None,
+            values,
+            _datetime_to_datetime_timezone(dates),
+            None,
         )
 
     series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
     if series_with_revisions.IsError:
         if series_with_revisions.ErrorMessage == "Not found":
             raise ValueError("Series not found: " + series_name)
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, TYPE_CHECKING
 
 from macrobond_data_api.common.types import SearchResult
-from ._fill_metadata_from_entity import _fill_metadata_from_entity
+from ._fill_metadata import _fill_metadata_from_entity
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from macrobond_data_api.common.types import SearchFilter
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 
 from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode
 
 from macrobond_data_api.common.types import (
     SeriesEntry,
     GetEntitiesError,
+    EntityErrorInfo,
     Series,
     Entity,
     UnifiedSeriesList,
     UnifiedSeries,
 )
 
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
 
-from ._fill_metadata_from_entity import _fill_metadata_from_entity
+from ._fill_metadata import _fill_metadata_from_entity
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from macrobond_data_api.common.types import StartOrEndPoint
 
     from .com_types import Series as ComSeries, Entity as ComEntity
@@ -35,49 +36,46 @@
     if com_entity.IsError:
         return Entity(name, com_entity.ErrorMessage, None)
     return Entity(name, None, _fill_metadata_from_entity(com_entity))
 
 
 def _create_series(com_series: "ComSeries", name: str) -> Series:
     if com_series.IsError:
-        return Series(name, com_series.ErrorMessage, None, None, None)
+        return Series(name, com_series.ErrorMessage, None, None, None, None)
     return Series(
         name,
         None,
         _fill_metadata_from_entity(com_series),
+        None,
         list(com_series.Values),
         _datetime_to_datetime(com_series.DatesAtStartOfPeriod),
     )
 
 
 def get_one_series(self: "ComApi", series_name: str, raise_error: bool = None) -> Series:
     return self.get_series(series_name, raise_error=raise_error)[0]
 
 
 def get_series(self: "ComApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[Series]:
     com_series = self.database.FetchSeries(series_names)
     series = [_create_series(x, y) for x, y in zip(com_series, series_names)]
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
     return _ReprHtmlSequence(series)
 
 
 def get_one_entity(self: "ComApi", entity_name: str, raise_error: bool = None) -> Entity:
     return self.get_entities(entity_name, raise_error=raise_error)[0]
 
 
 def get_entities(self: "ComApi", *entity_names: str, raise_error: bool = None) -> Sequence[Entity]:
     com_entitys = self.database.FetchEntities(entity_names)
     entitys = [_create_entity(x, y) for x, y in zip(com_entitys, entity_names)]
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), entity_names, entitys),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(entity_names, entitys)])
     return _ReprHtmlSequence(entitys)
 
 
 def get_many_series(self: "ComApi", *series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
     if len(series) == 0:
         yield from ()
 
@@ -89,15 +87,15 @@
     for serie, serie_info in zip(self.get_series(*[x[0] for x in series], raise_error=False), series):
         if serie.is_error:
             yield serie
             continue
 
         last_modified_time = serie.metadata["LastModifiedTimeStamp"]
         if last_modified_time <= serie_info[1]:
-            yield Series(serie_info[0], "Not modified", None, None, None)
+            yield Series(serie_info[0], "Not modified", None, None, None, None)
             continue
 
         yield serie
 
 
 def get_unified_series(
     self: "ComApi",
@@ -159,13 +157,13 @@
             "",
             _fill_metadata_from_entity(com_one_series),
             [None if x is not None and isnan(x) else x for x in com_one_series.Values],
         )
 
     ret = UnifiedSeriesList([to_obj(request.AddedSeries[x].Name, y) for x, y in enumerate(com_series)], dates)
 
-    errors = ret.get_errors()
-    raise_error = self.raise_error if raise_error is None else raise_error
-    if raise_error and len(errors) != 0:
-        raise GetEntitiesError(errors)
+    if self.raise_error if raise_error is None else raise_error:
+        errors = [EntityErrorInfo(x, y) for x, y in ret.get_errors().items()]
+        if errors:
+            raise GetEntitiesError(errors)
 
     return ret
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/_fill_metadata_from_entity.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/_fill_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from typing import Any, TYPE_CHECKING, Sequence
+from typing import Any, TYPE_CHECKING, Sequence, Dict
 from datetime import datetime, timezone
 
 
 try:
     from pywintypes import TimeType
 except ImportError as ex:
     ...
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_types import Entity as ComEntity
+    from .com_types import Series as ComSeries
+    from .com_types import Metadata as ComMetadata
     from macrobond_data_api.common.types.metadata import Metadata
+    from macrobond_data_api.common.types.values_metadata import ValuesMetadata
 
 
 def _get_val(name: str, values: Sequence[Any]) -> Any:
     if isinstance(values[0], TimeType):
         if name == "LastModifiedTimeStamp":
             datetime_ = values[0]
             return datetime(
@@ -40,14 +43,19 @@
         values = [
             datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond, timezone.utc) for x in values
         ]
         return values[0] if len(values) == 1 else values
     return values[0] if len(values) == 1 else list(values)
 
 
+def _fill_metadata_from_metadata(com_metadata: "ComMetadata") -> Dict:
+    return {x: _get_val(x, com_metadata.GetValues(x)) for x, _ in com_metadata.ListNames()}
+
+
 def _fill_metadata_from_entity(com_entity: "ComEntity") -> "Metadata":
-    metadata = com_entity.Metadata
-    ret = {x: _get_val(x, metadata.GetValues(x)) for x, _ in metadata.ListNames()}
-    # ret = {x: metadata.GetValues(x) for x in (x[0] for x in metadata.ListNames())}
+    ret = _fill_metadata_from_metadata(com_entity.Metadata)
     ret.setdefault("FullDescription", com_entity.Title)
-
     return ret
+
+
+def _fill_values_metadata_from_series(com_series: "ComSeries") -> "ValuesMetadata":
+    return [_fill_metadata_from_metadata(x) for x in com_series.ValuesMetadata]
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_api.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_client.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from typing import TYPE_CHECKING, List, Optional, cast
+from typing import TYPE_CHECKING, List, Optional, Tuple, cast
 
 from macrobond_data_api.common import Client
 
 from .com_api import ComApi
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_types import Connection
@@ -24,14 +24,18 @@
 try:
     # winreg is not available on linux so mypy will fail on build server as it is runiong on linux
     from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT, HKEY_CURRENT_USER  # type: ignore
 except ImportError:
     ...
 
 
+class ComClientVersionException(Exception):
+    pass
+
+
 class ComClient(Client["ComApi"]):
     """
     ComClient to get data via the Macrobond desktop API
 
     Returns
     -------
     ComClient
@@ -98,17 +102,36 @@
                 for hint in hints:
                     print("\n" + hint, file=sys.stderr)
 
                 if len(hints) != 0:
                     print("", file=sys.stderr)
 
                 raise
+
+            ComClient._test_version(connection.Version)
+
             self.__api = ComApi(connection)
         return self.__api
 
+    @staticmethod
+    def _test_version(version: Tuple[int, int, int]) -> None:
+        if version == (0, 0, 0):
+            return
+
+        major, minor, _ = version
+
+        if major > 1:
+            return
+
+        if major == 0:
+            raise ComClientVersionException("Unsupported version " + (".".join([str(x) for x in version])))
+
+        if minor < 25:
+            raise ComClientVersionException("Unsupported version " + (".".join([str(x) for x in version])))
+
     def close(self) -> None:
         """
         free all resources used by the Macrobond API.
         Opening and closing sessions can be slow,
         so it is usually not a good idea to open and close them for each request
         """
         if self.__api:
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Interface for a Macrobond connection."""
 
     @property
     def Database(self) -> Database:
         """This property returns a reference to the database interface."""
 
     @property
-    def Version(self) -> Tuple[int]:
+    def Version(self) -> Tuple[int, int, int]:
         """
         Version	Returns an array of three values for the version of the installed API.
         For example, for the version 1.23.3 it will return [1, 23, 3].
         """
 
     def Close(self) -> None:
         """
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/api.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,17 @@
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.vintage_series.VintageSeries]`
         The result is in the same order as in the request.
         """
 
     @abstractmethod
-    def get_nth_release(self, nth: int, *series_names: str, raise_error: bool = None) -> Sequence[Series]:
+    def get_nth_release(
+        self, nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+    ) -> Sequence[Series]:
         """
         Fetcha series where each value is the nth change of the value.
 
         Parameters
         ----------
         time : nth
             The nth change of each value.
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/client.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/__init__.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_info.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, MutableMapping, TYPE_CHECKING, List, Sequence, overload
+from typing import Any, Mapping, TYPE_CHECKING, List, Sequence, overload
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame  # type: ignore
     from .metadata import Metadata
 
 __pdoc__ = {
     "SearchResult.__init__": False,
@@ -28,15 +28,15 @@
         A sequence of the metadata of the entities found.
         """
         self.is_truncated = is_truncated
         """
         Indicates whether the search result was too long and truncated.
         """
 
-    def to_dict(self) -> List[MutableMapping[str, Any]]:
+    def to_dict(self) -> List[Mapping[str, Any]]:
         """
         Return the result as a dictionary.
         """
         return list(self)
 
     def to_pd_data_frame(self) -> "DataFrame":
         """
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result_long.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,39 +10,46 @@
 SeriesColumnsLiterals = Literal[EntityColumnsLiterals, "Values", "Dates"]
 
 SeriesColumns = List[SeriesColumnsLiterals]
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import Series as PdSeries  # type: ignore
     from .metadata import Metadata
+    from .values_metadata import ValuesMetadata
 
 __pdoc__ = {
     "Series.__init__": False,
 }
 
 
 @dataclass(init=False)
 class Series(Entity):
     """Represents a Macrobond time series."""
 
-    __slots__ = ("values", "dates")
+    __slots__ = ("values_metadata", "values", "dates")
 
     values: Sequence[Optional[float]]
     dates: Sequence[datetime]
 
     def __init__(
         self,
         name: str,
         error_message: Optional[str],
         metadata: Optional["Metadata"],
+        values_metadata: Optional["ValuesMetadata"],
         values: Optional[List[Optional[float]]],
         dates: Optional[List[datetime]],
     ) -> None:
         super().__init__(name, error_message, metadata)
 
+        self.values_metadata = values_metadata
+        """
+        The meta data for the values.
+        """
+
         self.values = ...  # type: ignore
         """
         The values of the series.
         The number of values is the same as the number of `Series.dates`. 
         """
         self.dates = ...  # type: ignore
         """
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_observation_history.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/unified_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/common/types/vintage_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing_extensions import Literal
 from dateutil import parser
 
 from .series import Series, SeriesColumnsLiterals
 
 if TYPE_CHECKING:  # pragma: no cover
     from .metadata import Metadata
+    from .values_metadata import ValuesMetadata
 
 
 VintageSeriesColumns = List[Literal[SeriesColumnsLiterals, "VintageTimeStamp", "TimesOfChange"]]
 
 
 __pdoc__ = {
     "VintageSeries.__init__": False,
@@ -26,19 +27,20 @@
     __slots__ = ("_revision_time_stamp",)
 
     def __init__(
         self,
         name: str,
         error_message: Optional[str],
         metadata: Optional["Metadata"],
+        values_metadata: Optional["ValuesMetadata"],
         values: Optional[List[Optional[float]]],
         dates: Optional[List[datetime]],
         _revision_time_stamp: Optional[datetime],
     ) -> None:
-        super().__init__(name, error_message, metadata, values, dates)
+        super().__init__(name, error_message, metadata, values_metadata, values, dates)
         self._revision_time_stamp = _revision_time_stamp
 
     @property
     def revision_time_stamp(self) -> Optional[datetime]:
         """The vintage of the series."""
         if self._revision_time_stamp:
             return self._revision_time_stamp
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/util/save_credential_to_keyring.py` & `macrobond-data-api-0.0.9/macrobond_data_api/util/save_credential_to_keyring.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_revision.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from .web_api import WebApi
 
     from .web_types import (
         SeriesWithRevisionsInfoResponse,
         VintageSeriesResponse,
         SeriesWithVintagesResponse,
         RevisionHistoryRequest as WebRevisionHistoryRequest,
-        SeriesResponse,
+        SeriesWithTimesOfChangeResponse,
         VintageValuesResponse,
     )
 
 
 def _optional_str_to_datetime(datetime_str: Optional[str]) -> Optional[datetime]:
     return parser.parse(datetime_str) if datetime_str else None
 
@@ -54,27 +54,14 @@
     return parser.parse(datetime_str, ignoretz=True) if datetime_str else None
 
 
 def int_to_float_or_none(int_: Optional[int]) -> Optional[float]:
     return float(int_) if int_ else None
 
 
-def _create_series(response: "SeriesResponse", name: str, session: Session) -> Series:
-    error_text = response.get("errorText")
-
-    if error_text:
-        return Series(name, error_text, None, None, None)
-
-    dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
-    values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
-    metadata = session._create_metadata(response["metadata"])
-
-    return Series(name, "", cast(Dict[str, Any], metadata), values, dates)
-
-
 def get_revision_info(self: "WebApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[RevisionInfo]:
     def to_obj(name: str, serie: "SeriesWithRevisionsInfoResponse") -> RevisionInfo:
         error_text = serie.get("errorText")
         if error_text:
             return RevisionInfo(name, error_text, False, False, None, None, [])
 
         time_stamp_of_first_revision = _optional_str_to_datetime(serie.get("timeStampOfFirstRevision"))
@@ -93,29 +80,27 @@
             time_stamp_of_first_revision,
             time_stamp_of_last_revision,
             vintage_time_stamps,
         )
 
     response = self.session.series.get_revision_info(*series_names)
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.get("errorText")), series_names, response),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.get("errorText")) for x, y in zip(series_names, response)])
 
     return _ReprHtmlSequence([to_obj(x, y) for x, y in zip(series_names, response)])
 
 
 def get_vintage_series(
     self: "WebApi", time: datetime, *series_names: str, raise_error: Optional[bool] = None
 ) -> Sequence[VintageSeries]:
     def to_obj(response: "VintageSeriesResponse", series_name: str) -> VintageSeries:
         error_message = response.get("errorText")
         if error_message:
-            return VintageSeries(series_name, error_message, None, None, None, None)
+            return VintageSeries(series_name, error_message, None, None, None, None, None)
 
         metadata = self.session._create_metadata(response["metadata"])
 
         revision_time_stamp = cast(str, metadata.get("RevisionTimeStamp"))
 
         if not revision_time_stamp or time != revision_time_stamp:
             raise ValueError("Invalid time")
@@ -123,58 +108,80 @@
         values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
         dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
 
         vintage_time_stamp = (
             _str_to_datetime(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
         )
 
-        return VintageSeries(series_name, None, metadata, values, dates, vintage_time_stamp)
+        return VintageSeries(series_name, None, metadata, None, values, dates, vintage_time_stamp)
 
     response = self.session.series.fetch_vintage_series(time, *series_names, get_times_of_change=False)
 
     series = [to_obj(x, y) for x, y in zip(response, series_names)]
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
 def get_nth_release(
-    self: "WebApi", nth: int, *series_names: str, raise_error: Optional[bool] = None
+    self: "WebApi",
+    nth: int,
+    *series_names: str,
+    include_times_of_change: bool = False,
+    raise_error: Optional[bool] = None
 ) -> Sequence[Series]:
-    response = self.session.series.fetch_nth_release_series(nth, *series_names)
+    def to_obj(response: "SeriesWithTimesOfChangeResponse", name: str, session: Session) -> Series:
+        error_text = response.get("errorText")
+
+        if error_text:
+            return Series(name, error_text, None, None, None, None)
+
+        dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
+        values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
+        metadata = session._create_metadata(response["metadata"])
+        values_metadata = (
+            [{"timesOfChange": _optional_str_to_datetime(x)} for x in cast(List[str], response["timesOfChange"])]
+            if include_times_of_change and "timesOfChange" in response
+            else None
+        )
+
+        return Series(name, "", cast(Dict[str, Any], metadata), values_metadata, values, dates)
 
-    series = [_create_series(x, y, self.session) for x, y in zip(response, series_names)]
+    if len(series_names) == 0:
+        raise ValueError("No series names")
 
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
+    response = self.session.series.fetch_nth_release_series(
+        nth, *series_names, get_times_of_change=include_times_of_change
     )
 
+    series = [to_obj(x, y, self.session) for x, y in zip(response, series_names)]
+
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
+
     return _ReprHtmlSequence(series)
 
 
 def get_all_vintage_series(self: "WebApi", series_name: str) -> GetAllVintageSeriesResult:
     def to_obj(response: "VintageSeriesResponse", series_name: str) -> VintageSeries:
         error_message = response.get("errorText")
         if error_message:
-            return VintageSeries(series_name, error_message, None, None, None, None)
+            return VintageSeries(series_name, error_message, None, None, None, None, None)
 
         metadata = self.session._create_metadata(response["metadata"])
         values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
         dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
 
         vintage_time_stamp = (
             _str_to_datetime(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
         )
 
-        return VintageSeries(series_name, None, metadata, values, dates, vintage_time_stamp)
+        return VintageSeries(series_name, None, metadata, None, values, dates, vintage_time_stamp)
 
     try:
         response = self.session.series.get_fetch_all_vintage_series(series_name)
     except ProblemDetailsException as ex:
         if ex.status == 404:
             raise ValueError("Series not found: " + series_name) from ex
         raise ex
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from macrobond_data_api.common.types import SeriesEntry
 
 from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode
 
 from macrobond_data_api.common.types import (
     GetEntitiesError,
+    EntityErrorInfo,
     Series,
     Entity,
     UnifiedSeries,
     UnifiedSeriesList,
 )
 
 from .session import Session
@@ -58,51 +59,47 @@
     return Entity(name, None, cast(Dict[str, Any], metadata))
 
 
 def _create_series(response: "SeriesResponse", name: str, session: Session) -> Series:
     error_text = response.get("errorText")
 
     if error_text:
-        return Series(name, error_text, None, None, None)
+        return Series(name, error_text, None, None, None, None)
 
     dates = [_str_to_datetime_no_utc(x) for x in cast(List[str], response["dates"])]
 
     values = [float(x) if x else None for x in cast(List[Optional[float]], response["values"])]
 
     metadata = session._create_metadata(response["metadata"])
 
     # values = cast(Tuple[Optional[float]], response["values"])
-    return Series(name, "", metadata, values, dates)
+    return Series(name, "", metadata, None, values, dates)
 
 
 def get_one_series(self: "WebApi", series_name: str, raise_error: Optional[bool] = None) -> Series:
     return self.get_series(series_name, raise_error=raise_error)[0]
 
 
 def get_series(self: "WebApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[Series]:
     response = self.session.series.get_fetch_series(*series_names)
     series = [_create_series(x, y, self.session) for x, y in zip(response, series_names)]
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), series_names, series),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
     return _ReprHtmlSequence(series)
 
 
 def get_one_entity(self: "WebApi", entity_name: str, raise_error: Optional[bool] = None) -> Entity:
     return self.get_entities(entity_name, raise_error=raise_error)[0]
 
 
 def get_entities(self: "WebApi", *entity_names: str, raise_error: Optional[bool] = None) -> Sequence[Entity]:
     response = self.session.series.fetch_entities(*entity_names)
     entitys = [_create_entity(x, y, self.session) for x, y in zip(response, entity_names)]
-    GetEntitiesError._raise_if(
-        self.raise_error if raise_error is None else raise_error,
-        map(lambda x, y: (x, y.error_message if y.is_error else None), entity_names, entitys),
-    )
+    if self.raise_error if raise_error is None else raise_error:
+        GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(entity_names, entitys)])
     return _ReprHtmlSequence(entitys)
 
 
 def get_many_series(self: "WebApi", *series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
     if len(series) == 0:
         yield from ()
 
@@ -178,13 +175,13 @@
 
             metadata = self.session._create_metadata(one_series["metadata"])
 
             series.append(UnifiedSeries(name, "", metadata, values))
 
     ret = UnifiedSeriesList(series, dates)
 
-    errors = ret.get_errors()
-    raise_error = self.raise_error if raise_error is None else raise_error
-    if raise_error and len(errors) != 0:
-        raise GetEntitiesError(errors)
+    if self.raise_error if raise_error is None else raise_error:
+        errors = [EntityErrorInfo(x, y) for x, y in ret.get_errors().items()]
+        if errors:
+            raise GetEntitiesError(errors)
 
     return ret
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_only_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/session.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/session.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/subscription_list_poller.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/subscription_list_poller.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_api.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_client.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/status_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_body.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_body.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_list.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/subscription_list_state.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_state.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api/web/web_types/vintage_values_response.py` & `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/vintage_values_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-0.0.9/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.8 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.9 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-0.0.9/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 macrobond_data_api.egg-info/requires.txt
 macrobond_data_api.egg-info/top_level.txt
 macrobond_data_api/com/__init__.py
 macrobond_data_api/com/_com_api_metadata.py
 macrobond_data_api/com/_com_api_revision.py
 macrobond_data_api/com/_com_api_search.py
 macrobond_data_api/com/_com_api_series.py
-macrobond_data_api/com/_fill_metadata_from_entity.py
+macrobond_data_api/com/_fill_metadata.py
 macrobond_data_api/com/com_api.py
 macrobond_data_api/com/com_client.py
 macrobond_data_api/com/com_types/__init__.py
 macrobond_data_api/com/com_types/connection.py
 macrobond_data_api/com/com_types/database.py
 macrobond_data_api/com/com_types/entity.py
 macrobond_data_api/com/com_types/metadata.py
@@ -60,14 +60,15 @@
 macrobond_data_api/common/types/search_result_long.py
 macrobond_data_api/common/types/series.py
 macrobond_data_api/common/types/series_entry.py
 macrobond_data_api/common/types/series_observation_history.py
 macrobond_data_api/common/types/series_with_vintages.py
 macrobond_data_api/common/types/start_or_end_point.py
 macrobond_data_api/common/types/unified_series.py
+macrobond_data_api/common/types/values_metadata.py
 macrobond_data_api/common/types/vintage_series.py
 macrobond_data_api/util/__init__.py
 macrobond_data_api/util/save_credential_to_keyring.py
 macrobond_data_api/web/__init__.py
 macrobond_data_api/web/_metadata.py
 macrobond_data_api/web/_metadata_directory.py
 macrobond_data_api/web/_split_in_to_chunks.py
```

### Comparing `macrobond-data-api-0.0.8/macrobond_data_api.egg-info/requires.txt` & `macrobond-data-api-0.0.9/macrobond_data_api.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/setup.cfg` & `macrobond-data-api-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.8/setup.py` & `macrobond-data-api-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 try:
     version = (
         subprocess.run(["git", "describe", "--tags"], stdout=subprocess.PIPE, check=True).stdout.decode("utf-8").strip()
     )
+    if version[0].lower() == "v":
+        version = version[1:]
     print("version is from git tag")
 except subprocess.CalledProcessError:
     if os.path.exists(version_info_path):
         with open(version_info_path, "r", encoding="utf-8") as f:
             about: dict = {}
             exec(f.read(), about)  # pylint: disable=exec-used
             version = about["__version__"]
```

