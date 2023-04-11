# Comparing `tmp/criteo-api-marketingsolutions-sdk-2023.1.0.230320.tar.gz` & `tmp/criteo-api-marketingsolutions-sdk-2023.1.0.230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.1.0.230320.tar", last modified: Mon Mar 20 15:37:55 2023, max compression
+gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.1.0.230411.tar", last modified: Tue Apr 11 12:51:35 2023, max compression
```

## Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320.tar` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411.tar`

### file list

```diff
@@ -1,145 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.474317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-20 15:37:55.474317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.454316 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-20 15:37:55.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-03-20 15:37:55.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:37:55.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 15:37:55.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 15:37:55.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.454316 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.454316 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33531 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66036 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/o_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.454316 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.470317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/access_token_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/o_auth_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.470317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.474317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-20 15:37:55.474317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:55.474317 criteo-api-marketingsolutions-sdk-2023.1.0.230320/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/test/test_gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-20 15:37:03.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230320/test/test_oauth_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.955249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 12:51:35.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-11 12:51:35.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:51:35.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 12:51:35.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 12:51:35.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.959249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.959249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33531 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66036 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.959249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:51:35.975249 criteo-api-marketingsolutions-sdk-2023.1.0.230411/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-11 12:50:41.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230411/test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320
+pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/README.md` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/README.md`

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
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320
+pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_01
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
@@ -59,15 +59,14 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 
 
 ## Documentation For Models
 
- - [AccessTokenModel](docs/AccessTokenModel.md)
  - [AdSetCategoryBid](docs/AdSetCategoryBid.md)
  - [AdSetCategoryBidListResponse](docs/AdSetCategoryBidListResponse.md)
  - [AdSetCategoryBidResource](docs/AdSetCategoryBidResource.md)
  - [AdSetDeliveryLimitations](docs/AdSetDeliveryLimitations.md)
  - [AdSetDisplayMultiplier](docs/AdSetDisplayMultiplier.md)
  - [AdSetDisplayMultiplierListResponse](docs/AdSetDisplayMultiplierListResponse.md)
  - [AdSetDisplayMultiplierResource](docs/AdSetDisplayMultiplierResource.md)
@@ -112,15 +111,14 @@
  - [NewAudienceAttributes](docs/NewAudienceAttributes.md)
  - [NewAudienceRequest](docs/NewAudienceRequest.md)
  - [NewAudienceResponse](docs/NewAudienceResponse.md)
  - [NillableAdSetTargetingRule](docs/NillableAdSetTargetingRule.md)
  - [NillableAdSetTargetingRuleValue](docs/NillableAdSetTargetingRuleValue.md)
  - [NillableDateTime](docs/NillableDateTime.md)
  - [NillableDecimal](docs/NillableDecimal.md)
- - [OAuthErrorModel](docs/OAuthErrorModel.md)
  - [PatchAdSet](docs/PatchAdSet.md)
  - [PatchAdSetBidding](docs/PatchAdSetBidding.md)
  - [PatchAdSetBudget](docs/PatchAdSetBudget.md)
  - [PatchAdSetCategoryBid](docs/PatchAdSetCategoryBid.md)
  - [PatchAdSetCategoryBidListRequest](docs/PatchAdSetCategoryBidListRequest.md)
  - [PatchAdSetCategoryBidResource](docs/PatchAdSetCategoryBidResource.md)
  - [PatchAdSetCategoryBidResultListResponse](docs/PatchAdSetCategoryBidResultListResponse.md)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320
+pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 criteo_api_marketingsolutions_v2023_01/rest.py
 criteo_api_marketingsolutions_v2023_01/api/__init__.py
 criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py
 criteo_api_marketingsolutions_v2023_01/api/analytics_api.py
 criteo_api_marketingsolutions_v2023_01/api/audience_api.py
 criteo_api_marketingsolutions_v2023_01/api/campaign_api.py
 criteo_api_marketingsolutions_v2023_01/api/gateway_api.py
-criteo_api_marketingsolutions_v2023_01/api/o_auth_api.py
 criteo_api_marketingsolutions_v2023_01/apis/__init__.py
 criteo_api_marketingsolutions_v2023_01/model/__init__.py
-criteo_api_marketingsolutions_v2023_01/model/access_token_model.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py
 criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py
@@ -70,15 +68,14 @@
 criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py
 criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py
 criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py
 criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py
 criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py
 criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py
 criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py
-criteo_api_marketingsolutions_v2023_01/model/o_auth_error_model.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py
 criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py
@@ -127,9 +124,8 @@
 criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py
 criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py
 criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py
 criteo_api_marketingsolutions_v2023_01/models/__init__.py
 examples/__init__.py
 examples/portfolio.py
 examples/statistics.py
-test/test_gateway_api.py
-test/test_oauth_api.py
+test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Criteo publicly exposed API  # noqa: E501
 
     The version of the OpenAPI document: 2023-01
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.01.0.230320"
+__version__ = "2023.01.0.230411"
 
 # import ApiClient
 from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient
 
 # import Configuration
 from criteo_api_marketingsolutions_v2023_01.configuration import Configuration
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/audience_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/api_client.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/api_client.py`

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

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/apis/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/apis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 
 # Import APIs into API package:
 from criteo_api_marketingsolutions_v2023_01.api.advertiser_api import AdvertiserApi
 from criteo_api_marketingsolutions_v2023_01.api.analytics_api import AnalyticsApi
 from criteo_api_marketingsolutions_v2023_01.api.audience_api import AudienceApi
 from criteo_api_marketingsolutions_v2023_01.api.campaign_api import CampaignApi
 from criteo_api_marketingsolutions_v2023_01.api.gateway_api import GatewayApi
-from criteo_api_marketingsolutions_v2023_01.api.o_auth_api import OAuthApi
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/configuration.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/configuration.py`

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

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/exceptions.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/access_token_model.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
-class ApplicationSummaryModel(ModelNormal):
+class AudienceNameDescription(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,43 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'application_id': (int,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'organization_id': (int,),  # noqa: E501
             'description': (str,),  # noqa: E501
-            'criteo_service': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'application_id': 'applicationId',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'organization_id': 'organizationId',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'criteo_service': 'criteoService',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ApplicationSummaryModel - a model defined in OpenAPI
+        """AudienceNameDescription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +132,16 @@
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
+            name (str): The name to designate the audience by. [optional]  # noqa: E501
+            description (str): The description of the audience. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ApplicationSummaryModel - a model defined in OpenAPI
+        """AudienceNameDescription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,19 +219,16 @@
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
+            name (str): The name to designate the audience by. [optional]  # noqa: E501
+            description (str): The description of the audience. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_error.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
-class AudienceNameDescription(ModelNormal):
+class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'description': 'description',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AudienceNameDescription - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name to designate the audience by. [optional]  # noqa: E501
-            description (str): The description of the audience. [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AudienceNameDescription - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name to designate the audience by. [optional]  # noqa: E501
-            description (str): The description of the audience. [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/common_problem.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/error_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/error_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/o_auth_error_model.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
-class OAuthErrorModel(ModelNormal):
+class PortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,39 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'error': (str,),  # noqa: E501
-            'error_description': (str,),  # noqa: E501
-            'error_uri': (str,),  # noqa: E501
+            'advertiser_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'error': 'error',  # noqa: E501
-        'error_description': 'error_description',  # noqa: E501
-        'error_uri': 'error_uri',  # noqa: E501
+        'advertiser_name': 'advertiserName',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """OAuthErrorModel - a model defined in OpenAPI
+        """PortfolioMessage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +130,15 @@
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
+            advertiser_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """OAuthErrorModel - a model defined in OpenAPI
+        """PortfolioMessage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,17 +216,15 @@
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
+            advertiser_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
-class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
+class PatchResultCampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -92,22 +92,24 @@
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,15 +135,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,15 +222,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set import PatchAdSet
+    globals()['PatchAdSet'] = PatchAdSet
 
-class PatchResultCampaignReadResource(ModelNormal):
+
+class WriteModelPatchAdSet(ModelNormal):
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
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': (PatchAdSet,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
-        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +141,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +229,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2023_01.model.replace_audience import ReplaceAudience
+    globals()['ReplaceAudience'] = ReplaceAudience
 
-class PortfolioMessage(ModelNormal):
+
+class ReplaceAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,50 +66,55 @@
 
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
-            'advertiser_name': (str,),  # noqa: E501
+            'data': (ReplaceAudience,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'advertiser_name': 'advertiserName',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PortfolioMessage - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """ReplaceAudienceRequest - a model defined in OpenAPI
+
+        Args:
+            data (ReplaceAudience):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +139,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            advertiser_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -162,14 +170,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,16 +191,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PortfolioMessage - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """ReplaceAudienceRequest - a model defined in OpenAPI
+
+        Args:
+            data (ReplaceAudience):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +228,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            advertiser_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -246,14 +257,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/problem_details.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.replace_audience import ReplaceAudience
-    globals()['ReplaceAudience'] = ReplaceAudience
 
-
-class ReplaceAudienceRequest(ModelNormal):
+class TransparencyReportFile(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,55 +62,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
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
-        lazy_import()
         return {
-            'data': (ReplaceAudience,),  # noqa: E501
+            'file_name': (str,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'file_name': 'fileName',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """ReplaceAudienceRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, file_name, url, *args, **kwargs):  # noqa: E501
+        """TransparencyReportFile - a model defined in OpenAPI
 
         Args:
-            data (ReplaceAudience):
+            file_name (str):
+            url (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -170,15 +167,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.file_name = file_name
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,19 +189,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """ReplaceAudienceRequest - a model defined in OpenAPI
+    def __init__(self, file_name, url, *args, **kwargs):  # noqa: E501
+        """TransparencyReportFile - a model defined in OpenAPI
 
         Args:
-            data (ReplaceAudience):
+            file_name (str):
+            url (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,15 +256,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.file_name = file_name
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
 
 
 
-class TransparencyReportFile(ModelNormal):
+class WriteModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,41 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'file_name': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'file_name': 'fileName',  # noqa: E501
-        'url': 'url',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, file_name, url, *args, **kwargs):  # noqa: E501
-        """TransparencyReportFile - a model defined in OpenAPI
-
-        Args:
-            file_name (str):
-            url (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """WriteModelAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,14 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,16 +165,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.file_name = file_name
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,20 +185,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, file_name, url, *args, **kwargs):  # noqa: E501
-        """TransparencyReportFile - a model defined in OpenAPI
-
-        Args:
-            file_name (str):
-            url (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """WriteModelAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,14 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,16 +250,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.file_name = file_name
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/model_utils.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/models/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from criteo_api_marketingsolutions_v2023_01.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_marketingsolutions_v2023_01.model.access_token_model import AccessTokenModel
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid import AdSetCategoryBid
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_resource import AdSetCategoryBidResource
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier import AdSetDisplayMultiplier
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
 from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
@@ -58,15 +57,14 @@
 from criteo_api_marketingsolutions_v2023_01.model.new_audience_attributes import NewAudienceAttributes
 from criteo_api_marketingsolutions_v2023_01.model.new_audience_request import NewAudienceRequest
 from criteo_api_marketingsolutions_v2023_01.model.new_audience_response import NewAudienceResponse
 from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
 from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
 from criteo_api_marketingsolutions_v2023_01.model.nillable_date_time import NillableDateTime
 from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
-from criteo_api_marketingsolutions_v2023_01.model.o_auth_error_model import OAuthErrorModel
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set import PatchAdSet
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_bidding import PatchAdSetBidding
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_budget import PatchAdSetBudget
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
 from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/criteo_api_marketingsolutions_v2023_01/rest.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/criteo_api_marketingsolutions_v2023_01/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/portfolio.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/portfolio.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/examples/statistics.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/examples/statistics.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/setup.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
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
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320
+pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230320`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230411`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230320/test/test_gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.1.0.230411/test/test_gateway_api.py`

 * *Files identical despite different names*

