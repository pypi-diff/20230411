# Comparing `tmp/criteo-api-retailmedia-sdk-2023.1.0.230320.tar.gz` & `tmp/criteo-api-retailmedia-sdk-2023.1.0.230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-retailmedia-sdk-2023.1.0.230320.tar", last modified: Mon Mar 20 15:39:08 2023, max compression
+gzip compressed data, was "criteo-api-retailmedia-sdk-2023.1.0.230411.tar", last modified: Tue Apr 11 12:52:47 2023, max compression
```

## Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320.tar` & `criteo-api-retailmedia-sdk-2023.1.0.230411.tar`

### file list

```diff
@@ -1,202 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.511617 criteo-api-retailmedia-sdk-2023.1.0.230320/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-20 15:39:08.511617 criteo-api-retailmedia-sdk-2023.1.0.230320/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14403 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.479616 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-20 15:39:08.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-03-20 15:39:08.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:39:08.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 15:39:08.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-20 15:39:08.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.479616 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.479616 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23593 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   334272 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/o_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.479616 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.507617 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/access_token_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202207_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/customer_list_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/map_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/o_auth_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/section.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.507617 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18757 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.511617 criteo-api-retailmedia-sdk-2023.1.0.230320/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/examples/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/examples/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-20 15:39:08.511617 criteo-api-retailmedia-sdk-2023.1.0.230320/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:39:08.511617 criteo-api-retailmedia-sdk-2023.1.0.230320/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/test/test_gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-20 15:37:03.000000 criteo-api-retailmedia-sdk-2023.1.0.230320/test/test_oauth_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.393263 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-11 12:52:47.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-04-11 12:52:47.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:52:47.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 12:52:47.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 12:52:47.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.393263 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.397263 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23593 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334272 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.397263 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202207_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/customer_list_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/map_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/examples/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/examples/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:52:47.437265 criteo-api-retailmedia-sdk-2023.1.0.230411/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-11 12:50:41.000000 criteo-api-retailmedia-sdk-2023.1.0.230411/test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.1.0.230411/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.1.0.230320
+Version: 2023.1.0.230411
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.01.0.230320
+pip install criteo-api-retailmedia-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/README.md` & `criteo-api-retailmedia-sdk-2023.1.0.230411/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 More information: [https://developers.criteo.com/marketing-solutions/docs/python-api-client-library](https://developers.criteo.com/marketing-solutions/docs/python-api-client-library)
 
 [![](https://img.shields.io/pypi/pyversions/criteo-marketing.svg)](https://pypi.org/project/criteo-marketing-transition/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2023.01.0.230320
+- Package version: 2023.01.0.230411
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.01.0.230320
+pip install criteo-api-retailmedia-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_01
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
@@ -59,15 +59,14 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 
 
 ## Documentation For Models
 
- - [AccessTokenModel](docs/AccessTokenModel.md)
  - [AddToBasketIdsUpdateModel202110Request](docs/AddToBasketIdsUpdateModel202110Request.md)
  - [AddToBasketTarget202110Request](docs/AddToBasketTarget202110Request.md)
  - [AddToBasketTarget202110Response](docs/AddToBasketTarget202110Response.md)
  - [ApplicationSummaryModel](docs/ApplicationSummaryModel.md)
  - [ApplicationSummaryModelResource](docs/ApplicationSummaryModelResource.md)
  - [ApplicationSummaryModelResponse](docs/ApplicationSummaryModelResponse.md)
  - [Asset](docs/Asset.md)
@@ -169,15 +168,14 @@
  - [JsonApiSingleResponseOfLineItemBidMultipliers](docs/JsonApiSingleResponseOfLineItemBidMultipliers.md)
  - [KeywordTarget202110Request](docs/KeywordTarget202110Request.md)
  - [KeywordTarget202110Response](docs/KeywordTarget202110Response.md)
  - [LineItemBidMultipliers](docs/LineItemBidMultipliers.md)
  - [LineItemBidMultipliersRequest](docs/LineItemBidMultipliersRequest.md)
  - [LineItemBidMultipliersResponse](docs/LineItemBidMultipliersResponse.md)
  - [MapString](docs/MapString.md)
- - [OAuthErrorModel](docs/OAuthErrorModel.md)
  - [PageMetadata](docs/PageMetadata.md)
  - [PostCampaignV202301](docs/PostCampaignV202301.md)
  - [PreferredLineItem202110PagedListResponse](docs/PreferredLineItem202110PagedListResponse.md)
  - [PreferredLineItem202110Response](docs/PreferredLineItem202110Response.md)
  - [PreferredLineItemCreateModel202110Request](docs/PreferredLineItemCreateModel202110Request.md)
  - [PreferredLineItemUpdateModel202110Request](docs/PreferredLineItemUpdateModel202110Request.md)
  - [ProblemDetails](docs/ProblemDetails.md)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.1.0.230320
+Version: 2023.1.0.230411
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.01.0.230320
+pip install criteo-api-retailmedia-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 criteo_api_retailmedia_v2023_01/model_utils.py
 criteo_api_retailmedia_v2023_01/rest.py
 criteo_api_retailmedia_v2023_01/api/__init__.py
 criteo_api_retailmedia_v2023_01/api/analytics_api.py
 criteo_api_retailmedia_v2023_01/api/audience_api.py
 criteo_api_retailmedia_v2023_01/api/campaign_api.py
 criteo_api_retailmedia_v2023_01/api/gateway_api.py
-criteo_api_retailmedia_v2023_01/api/o_auth_api.py
 criteo_api_retailmedia_v2023_01/apis/__init__.py
 criteo_api_retailmedia_v2023_01/model/__init__.py
-criteo_api_retailmedia_v2023_01/model/access_token_model.py
 criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py
 criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py
 criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py
 criteo_api_retailmedia_v2023_01/model/application_summary_model.py
 criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py
 criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py
 criteo_api_retailmedia_v2023_01/model/asset.py
@@ -126,15 +124,14 @@
 criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py
 criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py
 criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py
 criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py
 criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py
 criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py
 criteo_api_retailmedia_v2023_01/model/map_string.py
-criteo_api_retailmedia_v2023_01/model/o_auth_error_model.py
 criteo_api_retailmedia_v2023_01/model/page_metadata.py
 criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py
 criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py
 criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py
 criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py
 criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py
 criteo_api_retailmedia_v2023_01/model/problem_details.py
@@ -184,9 +181,8 @@
 criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py
 criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py
 criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py
 criteo_api_retailmedia_v2023_01/models/__init__.py
 examples/__init__.py
 examples/portfolio.py
 examples/statistics.py
-test/test_gateway_api.py
-test/test_oauth_api.py
+test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/__init__.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Criteo publicly exposed API  # noqa: E501
 
     The version of the OpenAPI document: 2023-01
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.01.0.230320"
+__version__ = "2023.01.0.230411"
 
 # import ApiClient
 from criteo_api_retailmedia_v2023_01.api_client import ApiClient
 
 # import Configuration
 from criteo_api_retailmedia_v2023_01.configuration import Configuration
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/analytics_api.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/audience_api.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/campaign_api.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api/gateway_api.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/api_client.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2023.01.0.230320/python'
+        self.user_agent = 'OpenAPI-Generator/2023.01.0.230411/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/apis/__init__.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/apis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from criteo_api_retailmedia_v2023_01.api.analytics_api import AnalyticsApi
 from criteo_api_retailmedia_v2023_01.api.audience_api import AudienceApi
 from criteo_api_retailmedia_v2023_01.api.campaign_api import CampaignApi
 from criteo_api_retailmedia_v2023_01.api.gateway_api import GatewayApi
-from criteo_api_retailmedia_v2023_01.api.o_auth_api import OAuthApi
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/configuration.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2023-01\n"\
-               "SDK Package Version: 2023.01.0.230320".\
+               "SDK Package Version: 2023.01.0.230411".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/exceptions.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/access_token_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 
-class AccessTokenModel(ModelNormal):
+class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,41 +77,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'access_token': (str,),  # noqa: E501
-            'token_type': (str,),  # noqa: E501
-            'refresh_token': (str, none_type,),  # noqa: E501
-            'expires_in': (int,),  # noqa: E501
+            'application_id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'organization_id': (int,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'criteo_service': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'access_token': 'access_token',  # noqa: E501
-        'token_type': 'token_type',  # noqa: E501
-        'refresh_token': 'refresh_token',  # noqa: E501
-        'expires_in': 'expires_in',  # noqa: E501
+        'application_id': 'applicationId',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'organization_id': 'organizationId',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'criteo_service': 'criteoService',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AccessTokenModel - a model defined in OpenAPI
+        """ApplicationSummaryModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,18 +138,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            access_token (str): The access token issued by the authorization server.. [optional]  # noqa: E501
-            token_type (str): The type of the token issued.. [optional]  # noqa: E501
-            refresh_token (str, none_type): The refresh token issued by the authorization server.. [optional]  # noqa: E501
-            expires_in (int): The lifetime in seconds of the access token.For example, the value \"3600\" denotes that the access token will expire in one hour from the time the response was generated. If omitted, the authorization server SHOULD provide the expiration time via other means or document the default value.. [optional]  # noqa: E501
+            application_id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            organization_id (int): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            criteo_service (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AccessTokenModel - a model defined in OpenAPI
+        """ApplicationSummaryModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,18 +228,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            access_token (str): The access token issued by the authorization server.. [optional]  # noqa: E501
-            token_type (str): The type of the token issued.. [optional]  # noqa: E501
-            refresh_token (str, none_type): The refresh token issued by the authorization server.. [optional]  # noqa: E501
-            expires_in (int): The lifetime in seconds of the access token.For example, the value \"3600\" denotes that the access token will expire in one hour from the time the response was generated. If omitted, the authorization server SHOULD provide the expiration time via other means or document the default value.. [optional]  # noqa: E501
+            application_id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            organization_id (int): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            criteo_service (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202110 import ResourceOfCreative202110
+    globals()['ProblemDetails'] = ProblemDetails
+    globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
 
-class ApplicationSummaryModel(ModelNormal):
+
+class Creative202110ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,58 +68,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'application_id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'organization_id': (int,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'criteo_service': (str,),  # noqa: E501
+            'data': ([ResourceOfCreative202110],),  # noqa: E501
+            'warnings': ([ProblemDetails],),  # noqa: E501
+            'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'application_id': 'applicationId',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'organization_id': 'organizationId',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'criteo_service': 'criteoService',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'warnings': 'warnings',  # noqa: E501
+        'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
+        'warnings',  # noqa: E501
+        'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ApplicationSummaryModel - a model defined in OpenAPI
+        """Creative202110ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +144,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            application_id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            organization_id (int): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            criteo_service (str): [optional]  # noqa: E501
+            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            warnings ([ProblemDetails]): [optional]  # noqa: E501
+            errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ApplicationSummaryModel - a model defined in OpenAPI
+        """Creative202110ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,19 +232,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            application_id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            organization_id (int): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            criteo_service (str): [optional]  # noqa: E501
+            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            warnings ([ProblemDetails]): [optional]  # noqa: E501
+            errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset_resource.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/asset_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/asset_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/bad_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/category202204.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_option.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_option.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/color_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/color_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_error.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_problem.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/common_warning.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/common_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202207_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202110 import ResourceOfCreative202110
+    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202207 import ResourceOfCreative202207
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
+    globals()['ResourceOfCreative202207'] = ResourceOfCreative202207
 
 
-class Creative202110ListResponse(ModelNormal):
+class Creative202207Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([ResourceOfCreative202110],),  # noqa: E501
+            'data': (ResourceOfCreative202207,),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Creative202110ListResponse - a model defined in OpenAPI
+        """Creative202207Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            data (ResourceOfCreative202207): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Creative202110ListResponse - a model defined in OpenAPI
+        """Creative202207Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            data (ResourceOfCreative202207): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202207.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative202207_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202207 import ResourceOfCreative202207
+    from criteo_api_retailmedia_v2023_01.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfCreative202207'] = ResourceOfCreative202207
+    globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
-class Creative202207Response(ModelNormal):
+class TemplateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (ResourceOfCreative202207,),  # noqa: E501
+            'data': (ResourceOfTemplate,),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Creative202207Response - a model defined in OpenAPI
+        """TemplateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfCreative202207): [optional]  # noqa: E501
+            data (ResourceOfTemplate): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Creative202207Response - a model defined in OpenAPI
+        """TemplateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfCreative202207): [optional]  # noqa: E501
+            data (ResourceOfTemplate): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/customer_list_details.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/customer_list_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/error.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_account.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_balance202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_balance202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_brand.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_retailer.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/files_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/files_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/map_string.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/map_string.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/o_auth_error_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item import ExternalAuctionLineItem
+    globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
 
-class OAuthErrorModel(ModelNormal):
+
+class ResourceOfAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,54 +66,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'error': (str,),  # noqa: E501
-            'error_description': (str,),  # noqa: E501
-            'error_uri': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (ExternalAuctionLineItem,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'error': 'error',  # noqa: E501
-        'error_description': 'error_description',  # noqa: E501
-        'error_uri': 'error_uri',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """OAuthErrorModel - a model defined in OpenAPI
+        """ResourceOfAuctionLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (str): [optional]  # noqa: E501
-            error_description (str): [optional]  # noqa: E501
-            error_uri (str): [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """OAuthErrorModel - a model defined in OpenAPI
+        """ResourceOfAuctionLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (str): [optional]  # noqa: E501
-            error_description (str): [optional]  # noqa: E501
-            error_uri (str): [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/page_metadata.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/page_metadata.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/problem_details.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_status.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item import ExternalAuctionLineItem
-    globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
+    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+    globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
 
 
-class ResourceOfAuctionLineItem(ModelNormal):
+class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAuctionLineItem,),  # noqa: E501
+            'attributes': (ExternalAuctionLineItemUpdateModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItem - a model defined in OpenAPI
+        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItem - a model defined in OpenAPI
+        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
-    globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2023_01.model.external_common_line_item import ExternalCommonLineItem
+    globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
 
 
-class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
+class ResourceOfCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAuctionLineItemUpdateModel,),  # noqa: E501
+            'attributes': (ExternalCommonLineItem,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
+        """ResourceOfCommonLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
+            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
+        """ResourceOfCommonLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
+            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_common_line_item import ExternalCommonLineItem
-    globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
+    from criteo_api_retailmedia_v2023_01.model.template import Template
+    globals()['Template'] = Template
 
 
-class ResourceOfCommonLineItem(ModelNormal):
+class ResourceOfTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'attributes': (Template,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalCommonLineItem,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'attributes': 'attributes',  # noqa: E501
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfCommonLineItem - a model defined in OpenAPI
+        """ResourceOfTemplate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            attributes (Template): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfCommonLineItem - a model defined in OpenAPI
+        """ResourceOfTemplate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            attributes (Template): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/resource_of_template.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template import Template
-    globals()['Template'] = Template
+    from criteo_api_retailmedia_v2023_01.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+    globals()['ExternalStoreIdsUpdateModel202110'] = ExternalStoreIdsUpdateModel202110
 
 
-class ResourceOfTemplate(ModelNormal):
+class ValueTypeResourceOfStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (Template,),  # noqa: E501
-            'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': (ExternalStoreIdsUpdateModel202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfTemplate - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreIdsUpdateModel202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (Template): [optional]  # noqa: E501
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreIdsUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfTemplate - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreIdsUpdateModel202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (Template): [optional]  # noqa: E501
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreIdsUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/section.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/section.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_list_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_response.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_template import ResourceOfTemplate
-    globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfTemplate'] = ResourceOfTemplate
+    from criteo_api_retailmedia_v2023_01.model.external_store_target202110 import ExternalStoreTarget202110
+    globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
 
 
-class TemplateResponse(ModelNormal):
+class ValueTypeResourceOfStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,41 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (ResourceOfTemplate,),  # noqa: E501
-            'warnings': ([ProblemDetails],),  # noqa: E501
-            'errors': ([ProblemDetails],),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (ExternalStoreTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'warnings': 'warnings',  # noqa: E501
-        'errors': 'errors',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'warnings',  # noqa: E501
-        'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplateResponse - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfTemplate): [optional]  # noqa: E501
-            warnings ([ProblemDetails]): [optional]  # noqa: E501
-            errors ([ProblemDetails]): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -199,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplateResponse - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,17 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfTemplate): [optional]  # noqa: E501
-            warnings ([ProblemDetails]): [optional]  # noqa: E501
-            errors ([ProblemDetails]): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_variable.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_variable.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/template_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/template_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/text_variable_value.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/text_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/model_utils.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/models/__init__.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from criteo_api_retailmedia_v2023_01.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_retailmedia_v2023_01.model.access_token_model import AccessTokenModel
 from criteo_api_retailmedia_v2023_01.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
 from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
 from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
 from criteo_api_retailmedia_v2023_01.model.application_summary_model import ApplicationSummaryModel
 from criteo_api_retailmedia_v2023_01.model.application_summary_model_resource import ApplicationSummaryModelResource
 from criteo_api_retailmedia_v2023_01.model.application_summary_model_response import ApplicationSummaryModelResponse
 from criteo_api_retailmedia_v2023_01.model.asset import Asset
@@ -115,15 +114,14 @@
 from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
 from criteo_api_retailmedia_v2023_01.model.keyword_target202110_request import KeywordTarget202110Request
 from criteo_api_retailmedia_v2023_01.model.keyword_target202110_response import KeywordTarget202110Response
 from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers import LineItemBidMultipliers
 from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
 from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
 from criteo_api_retailmedia_v2023_01.model.map_string import MapString
-from criteo_api_retailmedia_v2023_01.model.o_auth_error_model import OAuthErrorModel
 from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
 from criteo_api_retailmedia_v2023_01.model.post_campaign_v202301 import PostCampaignV202301
 from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
 from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_response import PreferredLineItem202110Response
 from criteo_api_retailmedia_v2023_01.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
 from criteo_api_retailmedia_v2023_01.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
 from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/criteo_api_retailmedia_v2023_01/rest.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/criteo_api_retailmedia_v2023_01/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/examples/portfolio.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/examples/portfolio.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/examples/statistics.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/examples/statistics.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/setup.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
-VERSION = "2023.01.0.230320"
+VERSION = "2023.01.0.230411"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -21,17 +21,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.01.0.230320
+pip install criteo-api-retailmedia-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230320/test/test_gateway_api.py` & `criteo-api-retailmedia-sdk-2023.1.0.230411/test/test_gateway_api.py`

 * *Files identical despite different names*

