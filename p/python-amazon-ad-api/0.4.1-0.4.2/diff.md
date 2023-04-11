# Comparing `tmp/python-amazon-ad-api-0.4.1.tar.gz` & `tmp/python-amazon-ad-api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-ad-api-0.4.1.tar", last modified: Fri Mar 31 03:49:58 2023, max compression
+gzip compressed data, was "python-amazon-ad-api-0.4.2.tar", last modified: Tue Apr 11 17:45:07 2023, max compression
```

## Comparing `python-amazon-ad-api-0.4.1.tar` & `python-amazon-ad-api-0.4.2.tar`

### file list

```diff
@@ -1,113 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.520012 python-amazon-ad-api-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-03-31 03:49:58.520012 python-amazon-ad-api-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.488011 python-amazon-ad-api-0.4.1/ad_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.496011 python-amazon-ad-api-0.4.1/ad_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/advertising_test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/brand_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/creative_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.496011 python-amazon-ad-api-0.4.1/ad_api/api/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/dsp/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/dsp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/dsp/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/dsp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/eligibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/manager_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.504011 python-amazon-ad-api-0.4.1/ad_api/api/sb/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/ad_groups_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/ads_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/brands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/campaigns_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/landing_page_asins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sb/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.508011 python-amazon-ad-api-0.4.1/ad_api/api/sd/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/creatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sd/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.512011 python-amazon-ad-api-0.4.1/ad_api/api/sp/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/budget_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/budget_rules_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/campaign_negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/campaigns_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/campaings_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/product_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/ranked_keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/sp/suggested_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/api/validation_configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.516012 python-amazon-ad-api-0.4.1/ad_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.520012 python-amazon-ad-api-0.4.1/ad_api/base/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/ad_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:49:58.520012 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-03-31 03:49:58.000000 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-31 03:49:58.000000 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 03:49:58.000000 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-31 03:49:58.000000 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 03:49:58.000000 python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-31 03:49:58.520012 python-amazon-ad-api-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-31 03:49:47.000000 python-amazon-ad-api-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.353552 python-amazon-ad-api-0.4.2/ad_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.353552 python-amazon-ad-api-0.4.2/ad_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/advertising_test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/brand_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/creative_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.357552 python-amazon-ad-api-0.4.2/ad_api/api/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/manager_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.361552 python-amazon-ad-api-0.4.2/ad_api/api/sb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ads_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/landing_page_asins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.361552 python-amazon-ad-api-0.4.2/ad_api/api/sd/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/creatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.369552 python-amazon-ad-api-0.4.2/ad_api/api/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_initial_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_consolidated_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaings_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ranked_keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/suggested_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/validation_configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.369552 python-amazon-ad-api-0.4.2/ad_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/ad_api/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/setup.py
```

### Comparing `python-amazon-ad-api-0.4.1/LICENSE` & `python-amazon-ad-api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/PKG-INFO` & `python-amazon-ad-api-0.4.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 
 # PYTHON-AMAZON-AD-API
 
 ![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
-[![Verified on Openbase](https://badges.openbase.com/python/verified/python-amazon-ad-api.svg?token=upNllBzLVJv/xZpn/LcPWzff0YEwlGXPszgv2vSJhgM=)](https://openbase.com/python/python-amazon-ad-api?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
 
 ## Amazon's Advertising API
 
 A python 3 wrapper to access Amazon's Advertising API with an easy-to-use interface.
 
 ### Install
 
@@ -228,15 +228,15 @@
     -H "Authorization: Bearer Your-Token \
     -H "Amazon-Advertising-API-ClientId: your-client-id" \
     --data '{"countryCode":"ES"}' \
      https://advertising-api-test.amazon.com/v2/profiles/register
 
 ```
 
-### Modules Available Common Resources
+### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
 * Billing
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
@@ -261,63 +261,79 @@
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
-### Modules Available Sponsored Products 2.0
-
-* Ad Groups
-* Bid Recommendations
-* Campaigns
-* Keywords
-* Negative Keywords
-* Product Ads
-* Suggested Keywords
-* Product Targeting
-* Negative Product Targeting
-* Campaign Negative Keywords
-* Reports
-* Snapshots
-
-### Modules Available Sponsored Products 3.0
+### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
+Warning: [PLANNED DEPRECATION 6/30/2023]
+There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-* Budget Rules
-* Campaign Optimization Rules
-* Ranked Keywords Recommendations
-* Product Targeting
-* Budget Recommendations
-* Budget Rules Recommendations
-* Product Recommendations
-* Campaigns V3
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
+* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
+
+### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
+
+
+* [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
+* [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords_v3.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Campaign Optimization](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_optimization_rules.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads_v3.html)
+* [Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting_v3.html)
+* [Campaign Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_targets.html)
+* [Budget recommendations and missed opportunities](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_recommendations.html)
+* [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
+* [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
+* [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
+* [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 
 
-### Modules Available Sponsored Brands
+### Modules Available Sponsored Brands 3.0
 
 * Campaigns
-* Campaigns V4
 * Ad Groups
-* Ad Groups V4
-* Ads Groups V4
 * Keywords
 * Negative Keywords
 * Product Targeting
 * Negative Product Targeting
 * Targeting Recommendations
 * Bid Recommendations
 * Stores
 * Landing Page Asins
 * Media
 * Brands
 * Moderation
 * Reports
 * Snapshots
 
+### Modules Available Sponsored Brands 4.0
+
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
+* [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
+
 ### Modules Available Sponsored Display
 
 * Campaigns
 * Ad Groups
 * Reports
 * Product Ads
 * Targets
@@ -372,12 +388,12 @@
 
 ### API NOTICE
 
 This API is based on the [API Client](https://github.com/saleweaver/rapid_rest_client) created by [@saleweaver](https://github.com/saleweaver) but adapted to amazon advertising authentication requeriments
 
 ### DISCLAIMER
 
-We are not affiliated with Amazon
+We are not affiliated with Amazon but they used our api :)
 
 ### LICENSE
 
 ![License](https://img.shields.io/badge/license-MIT-green)
```

### Comparing `python-amazon-ad-api-0.4.1/README.md` & `python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: python-amazon-ad-api
+Version: 0.4.2
+Summary: Python wrapper for the Amazon Advertising API
+Home-page: https://github.com/denisneuf/python-amazon-ad-api
+Author: Daniel Alvaro
+Author-email: info@leadtech.es
+License: MIT
+Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PYTHON-AMAZON-AD-API
 
 ![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
-[![Verified on Openbase](https://badges.openbase.com/python/verified/python-amazon-ad-api.svg?token=upNllBzLVJv/xZpn/LcPWzff0YEwlGXPszgv2vSJhgM=)](https://openbase.com/python/python-amazon-ad-api?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
 
 ## Amazon's Advertising API
 
 A python 3 wrapper to access Amazon's Advertising API with an easy-to-use interface.
 
 ### Install
 
@@ -213,15 +228,15 @@
     -H "Authorization: Bearer Your-Token \
     -H "Amazon-Advertising-API-ClientId: your-client-id" \
     --data '{"countryCode":"ES"}' \
      https://advertising-api-test.amazon.com/v2/profiles/register
 
 ```
 
-### Modules Available Common Resources
+### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
 * Billing
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
@@ -246,63 +261,79 @@
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
-### Modules Available Sponsored Products 2.0
+### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
-* Ad Groups
-* Bid Recommendations
-* Campaigns
-* Keywords
-* Negative Keywords
-* Product Ads
-* Suggested Keywords
-* Product Targeting
-* Negative Product Targeting
-* Campaign Negative Keywords
-* Reports
-* Snapshots
-
-### Modules Available Sponsored Products 3.0
+Warning: [PLANNED DEPRECATION 6/30/2023]
+There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-
-* Budget Rules
-* Campaign Optimization Rules
-* Ranked Keywords Recommendations
-* Product Targeting
-* Budget Recommendations
-* Budget Rules Recommendations
-* Product Recommendations
-* Campaigns V3
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
+* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
+
+### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
+
+
+* [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
+* [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords_v3.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Campaign Optimization](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_optimization_rules.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads_v3.html)
+* [Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting_v3.html)
+* [Campaign Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_targets.html)
+* [Budget recommendations and missed opportunities](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_recommendations.html)
+* [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
+* [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
+* [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
+* [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 
 
-### Modules Available Sponsored Brands
+### Modules Available Sponsored Brands 3.0
 
 * Campaigns
-* Campaigns V4
 * Ad Groups
-* Ad Groups V4
-* Ads Groups V4
 * Keywords
 * Negative Keywords
 * Product Targeting
 * Negative Product Targeting
 * Targeting Recommendations
 * Bid Recommendations
 * Stores
 * Landing Page Asins
 * Media
 * Brands
 * Moderation
 * Reports
 * Snapshots
 
+### Modules Available Sponsored Brands 4.0
+
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
+* [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
+
 ### Modules Available Sponsored Display
 
 * Campaigns
 * Ad Groups
 * Reports
 * Product Ads
 * Targets
@@ -357,12 +388,12 @@
 
 ### API NOTICE
 
 This API is based on the [API Client](https://github.com/saleweaver/rapid_rest_client) created by [@saleweaver](https://github.com/saleweaver) but adapted to amazon advertising authentication requeriments
 
 ### DISCLAIMER
 
-We are not affiliated with Amazon
+We are not affiliated with Amazon but they used our api :)
 
 ### LICENSE
 
 ![License](https://img.shields.io/badge/license-MIT-green)
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/__init__.py` & `python-amazon-ad-api-0.4.2/ad_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/advertising_test_account.py` & `python-amazon-ad-api-0.4.2/ad_api/api/advertising_test_account.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/attribution.py` & `python-amazon-ad-api-0.4.2/ad_api/api/attribution.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/audiences.py` & `python-amazon-ad-api-0.4.2/ad_api/api/audiences.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/billing.py` & `python-amazon-ad-api-0.4.2/ad_api/api/billing.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/brand_metrics.py` & `python-amazon-ad-api-0.4.2/ad_api/api/brand_metrics.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/creative_assets.py` & `python-amazon-ad-api-0.4.2/ad_api/api/creative_assets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/dsp/client.py` & `python-amazon-ad-api-0.4.2/ad_api/api/dsp/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/dsp/credential_provider.py` & `python-amazon-ad-api-0.4.2/ad_api/api/dsp/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/dsp/reports.py` & `python-amazon-ad-api-0.4.2/ad_api/api/dsp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/eligibility.py` & `python-amazon-ad-api-0.4.2/ad_api/api/eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/history.py` & `python-amazon-ad-api-0.4.2/ad_api/api/history.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/insights.py` & `python-amazon-ad-api-0.4.2/ad_api/api/insights.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/invoices.py` & `python-amazon-ad-api-0.4.2/ad_api/api/invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/localization.py` & `python-amazon-ad-api-0.4.2/ad_api/api/localization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/manager_accounts.py` & `python-amazon-ad-api-0.4.2/ad_api/api/manager_accounts.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/metadata.py` & `python-amazon-ad-api-0.4.2/ad_api/api/metadata.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/portfolios.py` & `python-amazon-ad-api-0.4.2/ad_api/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/profiles.py` & `python-amazon-ad-api-0.4.2/ad_api/api/profiles.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/reports.py` & `python-amazon-ad-api-0.4.2/ad_api/api/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/__init__.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/ad_groups.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/ad_groups_v4.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         """
 
         json_ressource = 'application/vnd.sbadgroupresource.v' + str(version) + "+json"
         headers = {
             'Accept': json_ressource
         }
 
-        return self._request(kwargs.pop('path'), params=kwargs, headers=headers)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False),
+                             params=kwargs, headers=headers)
 
     @sp_endpoint("/sb/v4/adGroups/delete", method="POST")
     def delete_ad_groups(self, version: int = 4, **kwargs) -> ApiResponse:
         """
         Delete Sponsored Brands ad groups.
 
         Request Body (optional) :
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/ads_v4.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/ads_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         """
 
         json_version = 'application/vnd.sbadresource.v' + str(version) + "+json"
         headers = {
             'Accept': json_version
         }
 
-        return self._request(kwargs.pop('path'), params=kwargs, headers=headers)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False),
+                             params=kwargs, headers=headers)
 
     @sp_endpoint('/sb/v4/ads/video', method='POST')
     def create_video_ads(self, version: int = 4,  **kwargs) -> ApiResponse:
 
         """
         Creates Sponsored Brand video ads.
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/bid_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/brands.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/brands.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/campaigns.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/campaigns_v4.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns_v4.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
         json_version = 'application/vnd.sbcampaignresource.v' + str(version) + "+json"
 
         headers = {
             "Accept": json_version,
         }
 
-        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs, headers=headers)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False),
+                             params=kwargs, headers=headers)
 
     @sp_endpoint('/sb/v4/campaigns', method='PUT')
     def edit_campaigns(self, version: int = 4, **kwargs) -> ApiResponse:
         """
         Update Sponsored Brand Campaigns
 
          Request body (required)
@@ -52,15 +53,16 @@
             ApiResponse
 
         """
 
         json_version = 'application/vnd.sbcampaignresource.v' + str(version) + "+json"
         headers = {"Accept": json_version}
 
-        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs, headers=headers)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False),
+                             params=kwargs, headers=headers)
 
     @sp_endpoint('/sb/v4/campaigns/delete', method='POST')
     @Utils.notsupported
     def delete_campaigns(self, version: int = 4, **kwargs) -> ApiResponse:
         """
         The operation is currently not supported subject to potential change.
         Deletes Sponsored Brands campaigns.
@@ -100,8 +102,9 @@
             ApiResponse
 
         """
 
         json_version = 'application/vnd.sbcampaignresource.v' + str(version) + "+json"
         headers = {"Accept": json_version}
 
-        return self._request(kwargs.pop('path'), params=kwargs, headers=headers)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False),
+                             params=kwargs, headers=headers)
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/landing_page_asins.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/landing_page_asins.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/media.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/media.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/moderation.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/moderation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/negative_keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/negative_product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/reports.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/snapshots.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/stores.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/stores.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sb/targeting_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sb/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/__init__.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/ad_groups.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/bid_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/campaigns.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/creatives.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/creatives.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/negative_product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/product_ads.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/reports.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/snapshots.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sd/targeting_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sd/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/ad_groups.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class AdGroups(Client):
 
     @sp_endpoint('/v2/sp/adGroups', method='POST')
+    @Utils.deprecated
     def create_ad_groups(self, **kwargs) -> ApiResponse:
         r"""
         create_ad_groups(self, \*\*kwargs) -> ApiResponse
 
         Creates one or more ad groups.
 
         body: | REQUIRED {'description': 'An array of ad groups.}'
@@ -21,14 +23,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups', method='PUT')
+    @Utils.deprecated
     def edit_ad_groups(self, **kwargs) -> ApiResponse:
         r"""
         edit_ad_group(self, \*\*kwargs) -> ApiResponse
 
         Updates one or more ad groups.
 
         body: | REQUIRED {'description': 'An array of ad groups.}'
@@ -42,14 +45,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups', method='GET')
+    @Utils.deprecated
     def list_ad_groups(self, **kwargs) -> ApiResponse:
         r"""
         list_ad_groups(self, \*\*kwargs) -> ApiResponse
 
         Gets an array of AdGroup objects for a requested set of Sponsored Display ad groups. Note that the AdGroup object is designed for performance, and includes a small set of commonly used fields to reduce size. If the extended set of fields is required, use the ad group operations that return the AdGroupResponseEx object.
 
             query **startIndex**:*integer* | Optional. Sets a cursor into the requested set of campaigns. Use in conjunction with the count parameter to control pagination of the returned array. 0-indexed record offset for the result set, defaults to 0.
@@ -70,14 +74,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'),  params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups/{}', method='GET')
+    @Utils.deprecated
     def get_ad_group(self, adGroupId, **kwargs) -> ApiResponse:
         r"""
 
         get_ad_group(self, adGroupId, \*\*kwargs) -> ApiResponse
 
         Gets an ad group specified by identifier.
 
@@ -87,14 +92,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), adGroupId), params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups/{}', method='DELETE')
+    @Utils.deprecated
     def delete_ad_group(self, adGroupId, **kwargs) -> ApiResponse:
         r"""
 
         delete_ad_group(self, adGroupId, \*\*kwargs) -> ApiResponse
 
         Sets the ad group status to archived. Archived entities cannot be made active again. See developer notes for more information.
 
@@ -104,14 +110,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), adGroupId), params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups/extended', method='GET')
+    @Utils.deprecated
     def list_ad_groups_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_ad_groups_extended(self, \*\*kwargs) -> ApiResponse
 
         Gets an array of AdGroup objects for a requested set of Sponsored Display ad groups. Note that the AdGroup object is designed for performance, and includes a small set of commonly used fields to reduce size. If the extended set of fields is required, use the ad group operations that return the AdGroupResponseEx object.
 
             query: **startIndex**:*integer* | Optional. Sets a cursor into the requested set of campaigns. Use in conjunction with the count parameter to control pagination of the returned array. 0-indexed record offset for the result set, defaults to 0.
@@ -130,14 +137,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'),  params=kwargs)
 
     @sp_endpoint('/v2/sp/adGroups/extended/{}', method='GET')
+    @Utils.deprecated
     def get_ad_group_extended(self, adGroupId, **kwargs) -> ApiResponse:
         r"""
 
         get_ad_group_extended(self, adGroupId, \*\*kwargs) -> ApiResponse
 
         Gets an ad group that has extended data fields.
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/bid_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/budget_rules_recommendations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_initial_recommendation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
 
-class BudgetRulesRecommendations(Client):
+class InitialBudgetRecommendation(Client):
+    @sp_endpoint('/sp/campaigns/initialbudgetrecommendation', method='POST')
+    def initial_campaign_budget_recommendation(self, **kwargs) -> ApiResponse:
+        json_version = 'application/vnd.spinitialbudgetrecommendation.v3+json'
 
-    @sp_endpoint('/sp/campaigns/budgetRules/recommendations', method='POST')
-    def list_campaigns_budget_rules_recommendations(self, **kwargs) -> ApiResponse:
-        contentType = 'application/vnd.spbudgetrulesrecommendation.v3+json'
-        headers = {'Content-Type': contentType}
-        return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs, headers=headers)
-        # return self._request(fill_query_params(kwargs.pop('path')), data=kwargs.pop('body'), params=kwargs)
+        headers = {
+            "Content-Type": json_version
+        }
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs, headers=headers)
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/campaign_negative_keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/campaigns.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Campaigns(account='default', marketplace: Marketplaces = Marketplaces.EU, credentials=None, debug=False)
 
     Amazon Ads API - Sponsored Products
 
     """
 
     @sp_endpoint('/v2/sp/campaigns', method='PUT')
+    @Utils.deprecated
     def edit_single_campaign_assistant(
             self,
             campaign_id: int,
             portfolio_id: int = None,
             campaign_name: str = None,
             po_number: str = None,
             account_manager: str = None,
@@ -140,14 +141,15 @@
             return ApiResponse(obj)
         else:
             required.update(optional)
             data_str = json.dumps([required])
             return self._request(kwargs.pop('path'), data=data_str, params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns', method='POST')
+    @Utils.deprecated
     def create_single_campaign_assistant(self,
                                          campaign_name: str,
                                          targeting_type: str,
                                          daily_budget: int,
                                          start_date: str,
                                          end_date: str = None,
                                          campaign_status: str = "enabled",
@@ -249,14 +251,15 @@
         if optional:
             required.update(optional)
 
         data_str = json.dumps([required])
         return self._request(kwargs.pop('path'), data=data_str, params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns', method='POST')
+    @Utils.deprecated
     def create_campaigns(self, **kwargs) -> ApiResponse:
         r"""
         create_campaigns(body: (dict, str, list)) -> ApiResponse
 
         Creates one or more campaigns.
 
         body: | REQUIRED {'description': 'An array of campaigns.}'
@@ -278,14 +281,15 @@
             ApiResponse
 
         """
         body = Utils.convert_body(kwargs.pop('body'))
         return self._request(kwargs.pop('path'), data=body, params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns', method='PUT')
+    @Utils.deprecated
     def edit_campaigns(self, **kwargs) -> ApiResponse:
         r"""
         edit_campaigns(body: (dict, str, list)) -> ApiResponse
 
         Updates one or more campaigns.
 
         body: | REQUIRED {'description': 'An array of campaigns.}'
@@ -333,14 +337,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns/{}', method='GET')
+    @Utils.deprecated
     def get_campaign(self, campaignId, **kwargs) -> ApiResponse:
         r"""
 
         get_campaign(campaignId: int) -> ApiResponse
 
         Gets a campaign specified by identifier.
 
@@ -350,14 +355,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), campaignId), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns/{}', method='DELETE')
+    @Utils.deprecated
     def delete_campaign(self, campaignId, **kwargs) -> ApiResponse:
         r"""
 
         delete_campaign(campaignId: int) -> ApiResponse
 
         Sets the campaign status to archived. Archived entities cannot be made active again. See developer notes for more information.
 
@@ -367,14 +373,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), campaignId), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns/extended', method='GET')
+    @Utils.deprecated
     def list_campaigns_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_campaigns_extended(**kwargs) -> ApiResponse
 
         Gets an array of campaigns with extended data fields.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -393,14 +400,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'),  params=kwargs)
 
     @sp_endpoint('/v2/sp/campaigns/extended/{}', method='GET')
+    @Utils.deprecated
     def get_campaign_extended(self, campaignId, **kwargs) -> ApiResponse:
         r"""
         get_campaign_extended(campaignId: int) -> ApiResponse
 
         Gets an array of campaigns with extended data fields.
 
             path **campaignId**:*number* | Required. The identifier of an existing campaign.
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class Keywords(Client):
 
     @sp_endpoint('/v2/sp/keywords/{}', method='GET')
+    @Utils.deprecated
     def get_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_keyword(self, keywordId, **kwargs) -> ApiResponse
 
         Gets a keyword specified by identifier.
 
@@ -17,14 +19,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords/{}', method='DELETE')
+    @Utils.deprecated
     def delete_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
         delete_keyword(self, keywordId, **kwargs) -> ApiResponse:
 
         Archives a keyword.
 
             path **keywordId**:*number* | Required. The identifier of an existing keyword.
@@ -33,14 +36,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords/extended/{}', method='GET')
+    @Utils.deprecated
     def get_keyword_extended(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_keyword_extended(self, keywordId, **kwargs) -> ApiResponse
 
         Gets a keyword with extended data fields.
 
@@ -51,14 +55,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords/extended', method='GET')
+    @Utils.deprecated
     def list_keywords_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_keywords_extended(self, **kwargs) -> ApiResponse
 
         Gets a list of keywords that have extended data fields.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -83,14 +88,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords', method='GET')
+    @Utils.deprecated
     def list_keywords(self, **kwargs) -> ApiResponse:
         r"""
         list_keywords(self, **kwargs) -> ApiResponse
 
         Gets a list of keywords.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -115,14 +121,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords', method='POST')
+    @Utils.deprecated
     def create_keywords(self, **kwargs) -> ApiResponse:
         r"""
         create_keywords(self, **kwargs) -> ApiResponse:
 
         Creates one or more keywords.
 
         body: | REQUIRED {'description': 'An array of keyword objects.}'
@@ -141,14 +148,15 @@
             ApiResponse
 
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/keywords', method='PUT')
+    @Utils.deprecated
     def edit_keywords(self, **kwargs) -> ApiResponse:
         r"""
         edit_keywords(self, **kwargs) -> ApiResponse:
 
         Updates one or more keywords.
 
         body: | REQUIRED {'description': 'An array of keyword objects.}'
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/negative_keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class NegativeKeywords(Client):
 
     @sp_endpoint('/v2/sp/negativeKeywords/{}', method='GET')
+    @Utils.deprecated
     def get_negative_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_negative_keyword(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Gets a campaign negative keyword specified by identifier.
 
@@ -17,14 +19,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords/{}', method='DELETE')
+    @Utils.deprecated
     def delete_negative_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         delete_negative_keyword(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Archives a campaign negative keyword.
 
@@ -35,14 +38,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords/extended/{}', method='GET')
+    @Utils.deprecated
     def get_negative_keyword_extended(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_negative_keyword_extended(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Gets a campaign negative keyword that has extended data fields.
 
@@ -52,14 +56,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords/extended', method='GET')
+    @Utils.deprecated
     def list_negative_keywords_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_negative_keywords_extended(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of negative keywords that have extended data fields.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -82,14 +87,15 @@
 
             ApiResponse
 
             """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords', method='GET')
+    @Utils.deprecated
     def list_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         list_negative_keywords(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of negative keyword objects.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -112,14 +118,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords', method='POST')
+    @Utils.deprecated
     def create_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         create_negative_keywords(self, \*\*kwargs) -> ApiResponse:
 
         Creates one or more campaign negative keywords.
 
         body: | REQUIRED {'description': 'An array of keyword objects.}'
@@ -134,14 +141,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeKeywords', method='PUT')
+    @Utils.deprecated
     def edit_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         edit_negative_keywords(self, \*\*kwargs) -> ApiResponse:
 
         Updates one or more campaign negative keywords.
 
         body: | REQUIRED {'description': 'An array of campaign negative keywords with updated values.'}
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/negative_product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class NegativeTargets(Client):
 
     @sp_endpoint('/v2/sp/negativeTargets', method='POST')
+    @Utils.deprecated
     def create_negative_targets(self, **kwargs) -> ApiResponse:
         r"""
         create_products_targets(self, \*\*kwargs) -> ApiResponse:
 
         Creates one or more targeting expressions.
 
         body: | REQUIRED {'description': 'An array of asins objects.}'
@@ -24,14 +26,15 @@
             ApiResponse
 
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets', method='PUT')
+    @Utils.deprecated
     def edit_negative_targets(self, **kwargs) -> ApiResponse:
         r"""
         edit_negative_targets(self, \*\*kwargs) -> ApiResponse:
 
         Updates one or more negative targeting clauses.
 
         body: | REQUIRED {'description': 'An array of asins objects.}'
@@ -49,14 +52,15 @@
             ApiResponse
 
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets', method='GET')
+    @Utils.deprecated
     def list_negative_targets(self, **kwargs) -> ApiResponse:
         r"""
         list_negative_targets(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of negative targeting clauses filtered by specified criteria.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -75,14 +79,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets/{}', method='GET')
+    @Utils.deprecated
     def get_negative_target(self, targetId, **kwargs) -> ApiResponse:
         r"""
 
         get_negative_targets(self, targetId, \*\*kwargs) -> ApiResponse
 
         Get a negative targeting clause specified by identifier.
 
@@ -92,14 +97,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), targetId), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets/{}', method='DELETE')
+    @Utils.deprecated
     def delete_negative_targets(self, targetId, **kwargs) -> ApiResponse:
         r"""
 
         delete_negative_targets(self, targetId, \*\*kwargs) -> ApiResponse
 
         Archives a negative targeting clause.
 
@@ -109,14 +115,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), targetId), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets/extended', method='GET')
+    @Utils.deprecated
     def list_negative_targets_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_negative_targets_extended(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of negative targeting clauses filtered by specified criteria.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -135,14 +142,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/negativeTargets/extended/{}', method='GET')
+    @Utils.deprecated
     def get_negative_target_extended(self, targetId, **kwargs) -> ApiResponse:
         r"""
 
         get_negative_target_extended(self, targetId, \*\*kwargs) -> ApiResponse
 
         Get a negative targeting clause specified by identifier.
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/product_ads.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class ProductAds(Client):
     @sp_endpoint('/v2/sp/productAds', method='GET')
+    @Utils.deprecated
     def list_product_ads(self, **kwargs) -> ApiResponse:
         r"""
         list_product_ads(self, \*\*kwargs) -> ApiResponse
 
         Gets an array of campaigns.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -24,14 +26,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'),  params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds/extended', method='GET')
+    @Utils.deprecated
     def list_product_ads_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_product_ads_extended_request(self, \*\*kwargs) -> ApiResponse
 
         Gets extended data for a list of product ads filtered by specified criteria.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -50,14 +53,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'),  params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds/{}', method='GET')
+    @Utils.deprecated
     def get_product_ad(self, adId, **kwargs) -> ApiResponse:
         r"""
 
         get_product_ad_request(self, adId, \*\*kwargs) -> ApiResponse
 
         Gets a product ad specified by identifier.
 
@@ -67,14 +71,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), adId), params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds/extended/{}', method='GET')
+    @Utils.deprecated
     def get_product_ad_extended(self, adId, **kwargs) -> ApiResponse:
         r"""
 
         get_product_ad_extended(self, adId, **kwargs) -> ApiResponse
 
         Gets extended data for a product ad specified by identifier.
 
@@ -84,14 +89,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), adId), params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds/{}', method='DELETE')
+    @Utils.deprecated
     def delete_product_ad(self, adId, **kwargs) -> ApiResponse:
         r"""
 
         delete_product_ad(self, adId, \*\*kwargs) -> ApiResponse
 
         Sets the state of a specified product ad to archived. Note that once the state is set to archived it cannot be changed.
 
@@ -101,14 +107,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), adId), params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds', method='PUT')
+    @Utils.deprecated
     def edit_product_ads(self, **kwargs) -> ApiResponse:
         r"""
         edit_product_ads(self, \*\*kwargs) -> ApiResponse
 
         Updates one or more product ads specified by identifier.
 
         body: | REQUIRED {'description': 'A list of product ad objects with updated values for the state field.}'
@@ -120,14 +127,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/productAds', method='POST')
+    @Utils.deprecated
     def create_product_ads(self, **kwargs) -> ApiResponse:
         r"""
         create_product_ads(self, \*\*kwargs) -> ApiResponse
 
         Creates one or more product ads.
 
         body: | REQUIRED {'description': 'A list of product ads for creation. Note that the SKU field is used by sellers and the ASIN field is used by vendors.'}
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/product_targeting.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
+
 
 class Targets(Client):
     """Amazon Advertising API - Sponsored Products - Product Targetting
 
     Use the Amazon Advertising API for Sponsored Products for campaign, ad group, keyword, negative keyword, and product
     ad management operations. For more information about Sponsored Products, see the Sponsored Products Support Center.
     For onboarding information, see the account setup topic.
@@ -18,14 +19,15 @@
     Doc: https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#/Product%20Targeting
     This specification is available for download from the `Advertising API Sponsored Products 3.0
     <https://dtrnk0o2zy01c.cloudfront.net/openapi/en-us/dest/SponsoredProducts_prod_3p.json>`_.
 
 
     """
     @sp_endpoint('/v2/sp/targets', method='POST')
+    @Utils.deprecated
     def create_products_targets(self, **kwargs) -> ApiResponse:
         r"""
         Creates one or more targeting expressions.
 
         body: | REQUIRED {'description': 'An array of asins objects.}'
 
             | '**campaignId**': *number*, {'description': 'The number or recommendations returned in a single page.'}
@@ -44,14 +46,15 @@
             ApiResponse
 
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets', method='PUT')
+    @Utils.deprecated
     def edit_products_targets(self, **kwargs) -> ApiResponse:
         r"""
         Updates one or more targeting clauses.
 
         body: | REQUIRED {'description': 'An array of asins objects.}'
 
             | '**targetId**': *number*, {'description': 'The target id.'}
@@ -69,14 +72,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets', method='GET')
+    @Utils.deprecated
     def list_products_targets(self, **kwargs) -> ApiResponse:
         r"""
         Gets a list of targeting clauses filtered by specified criteria.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
 
             query **count**:*integer* | Optional. Number of records to include in the paged response. Defaults to max page size.
@@ -93,42 +97,45 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/{}', method='GET')
+    @Utils.deprecated
     def get_products_target(self, targetId, **kwargs) -> ApiResponse:
         r"""
         Get a targeting clause specified by identifier.
 
             path **targetId**:*number* | Required. The target identifier.
 
         Returns:
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), targetId), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/{}', method='DELETE')
+    @Utils.deprecated
     def delete_products_target(self, targetId, **kwargs) -> ApiResponse:
         r"""
         Archives a targeting clause.
 
             path **targetId**:*number* | Required. The target identifier.
 
         Returns:
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), targetId), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/extended', method='GET')
+    @Utils.deprecated
     def list_products_targets_extended(self, **kwargs) -> ApiResponse:
         r"""
         Gets a list of targeting clauses filtered by specified criteria.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
 
             query **count**:*integer* | Optional. Number of records to include in the paged response. Defaults to max page size.
@@ -145,28 +152,30 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/extended/{}', method='GET')
+    @Utils.deprecated
     def get_products_target_extended(self, targetId, **kwargs) -> ApiResponse:
         r"""
         Get a targeting clause specified by identifier.
 
             path **targetId**:*number* | Required. The target identifier.
 
         Returns:
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), targetId), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/productRecommendations', method='POST')
+    @Utils.deprecated
     def get_products_targets_recommendations(self, **kwargs) -> ApiResponse:
         r"""
 
         Gets a list of recommended products for targeting.
 
         body: | REQUIRED {'description': 'An array of asins objects.}'
 
@@ -179,14 +188,15 @@
             ApiResponse
 
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/targets/brands', method='GET')
+    @Utils.deprecated
     def get_brand_targets(self, **kwargs) -> ApiResponse:
         r"""
         Gets a list of recommended products for targeting.
 
             path **keyword**:*string* | Optional Unique exclude categoryId. A keyword for which to get recommended brands.
             path **categoryId**:*number* | Optional Unique exclude keyword. Gets the top 50 brands for the specified category identifier.
```

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/reports.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/snapshots.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/sp/suggested_keywords.py` & `python-amazon-ad-api-0.4.2/ad_api/api/sp/suggested_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/api/validation_configurations.py` & `python-amazon-ad-api-0.4.2/ad_api/api/validation_configurations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/auth/access_token_client.py` & `python-amazon-ad-api-0.4.2/ad_api/auth/access_token_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/__init__.py` & `python-amazon-ad-api-0.4.2/ad_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/api_response.py` & `python-amazon-ad-api-0.4.2/ad_api/base/api_response.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/base_client.py` & `python-amazon-ad-api-0.4.2/ad_api/base/base_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/client.py` & `python-amazon-ad-api-0.4.2/ad_api/base/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/config.py` & `python-amazon-ad-api-0.4.2/ad_api/base/config.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/credential_provider.py` & `python-amazon-ad-api-0.4.2/ad_api/base/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/exceptions.py` & `python-amazon-ad-api-0.4.2/ad_api/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/helpers.py` & `python-amazon-ad-api-0.4.2/ad_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/marketplaces.py` & `python-amazon-ad-api-0.4.2/ad_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/ad_api/base/utils.py` & `python-amazon-ad-api-0.4.2/ad_api/base/utils.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/PKG-INFO` & `python-amazon-ad-api-0.4.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: python-amazon-ad-api
-Version: 0.4.1
-Summary: Python wrapper for the Amazon Advertising API
-Home-page: https://github.com/denisneuf/python-amazon-ad-api
-Author: Daniel Alvaro
-Author-email: info@leadtech.es
-License: MIT
-Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PYTHON-AMAZON-AD-API
 
 ![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
-[![Verified on Openbase](https://badges.openbase.com/python/verified/python-amazon-ad-api.svg?token=upNllBzLVJv/xZpn/LcPWzff0YEwlGXPszgv2vSJhgM=)](https://openbase.com/python/python-amazon-ad-api?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
 
 ## Amazon's Advertising API
 
 A python 3 wrapper to access Amazon's Advertising API with an easy-to-use interface.
 
 ### Install
 
@@ -228,15 +213,15 @@
     -H "Authorization: Bearer Your-Token \
     -H "Amazon-Advertising-API-ClientId: your-client-id" \
     --data '{"countryCode":"ES"}' \
      https://advertising-api-test.amazon.com/v2/profiles/register
 
 ```
 
-### Modules Available Common Resources
+### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
 * Billing
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
@@ -261,63 +246,79 @@
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
-### Modules Available Sponsored Products 2.0
+### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
-* Ad Groups
-* Bid Recommendations
-* Campaigns
-* Keywords
-* Negative Keywords
-* Product Ads
-* Suggested Keywords
-* Product Targeting
-* Negative Product Targeting
-* Campaign Negative Keywords
-* Reports
-* Snapshots
-
-### Modules Available Sponsored Products 3.0
+Warning: [PLANNED DEPRECATION 6/30/2023]
+There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-
-* Budget Rules
-* Campaign Optimization Rules
-* Ranked Keywords Recommendations
-* Product Targeting
-* Budget Recommendations
-* Budget Rules Recommendations
-* Product Recommendations
-* Campaigns V3
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
+* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
+
+### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
+
+
+* [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
+* [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords_v3.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
+* [Campaign Optimization](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_optimization_rules.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads_v3.html)
+* [Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting_v3.html)
+* [Campaign Negative Targeting Clauses](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_targets.html)
+* [Budget recommendations and missed opportunities](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_recommendations.html)
+* [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
+* [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
+* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
+* [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
+* [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 
 
-### Modules Available Sponsored Brands
+### Modules Available Sponsored Brands 3.0
 
 * Campaigns
-* Campaigns V4
 * Ad Groups
-* Ad Groups V4
-* Ads Groups V4
 * Keywords
 * Negative Keywords
 * Product Targeting
 * Negative Product Targeting
 * Targeting Recommendations
 * Bid Recommendations
 * Stores
 * Landing Page Asins
 * Media
 * Brands
 * Moderation
 * Reports
 * Snapshots
 
+### Modules Available Sponsored Brands 4.0
+
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
+* [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
+
 ### Modules Available Sponsored Display
 
 * Campaigns
 * Ad Groups
 * Reports
 * Product Ads
 * Targets
@@ -372,12 +373,12 @@
 
 ### API NOTICE
 
 This API is based on the [API Client](https://github.com/saleweaver/rapid_rest_client) created by [@saleweaver](https://github.com/saleweaver) but adapted to amazon advertising authentication requeriments
 
 ### DISCLAIMER
 
-We are not affiliated with Amazon
+We are not affiliated with Amazon but they used our api :)
 
 ### LICENSE
 
 ![License](https://img.shields.io/badge/license-MIT-green)
```

### Comparing `python-amazon-ad-api-0.4.1/python_amazon_ad_api.egg-info/SOURCES.txt` & `python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -58,28 +58,40 @@
 ad_api/api/sd/product_ads.py
 ad_api/api/sd/product_targeting.py
 ad_api/api/sd/reports.py
 ad_api/api/sd/snapshots.py
 ad_api/api/sd/targeting_recommendations.py
 ad_api/api/sp/__init__.py
 ad_api/api/sp/ad_groups.py
+ad_api/api/sp/ad_groups_v3.py
 ad_api/api/sp/bid_recommendations.py
+ad_api/api/sp/bid_recommendations_v3.py
+ad_api/api/sp/budget_initial_recommendation.py
 ad_api/api/sp/budget_recommendations.py
 ad_api/api/sp/budget_rules.py
 ad_api/api/sp/budget_rules_recommendations.py
+ad_api/api/sp/campaign_consolidated_recommendations.py
 ad_api/api/sp/campaign_negative_keywords.py
+ad_api/api/sp/campaign_negative_keywords_v3.py
+ad_api/api/sp/campaign_negative_targets.py
 ad_api/api/sp/campaigns.py
+ad_api/api/sp/campaigns_budget_usage.py
 ad_api/api/sp/campaigns_v3.py
 ad_api/api/sp/campaings_optimization.py
 ad_api/api/sp/keywords.py
+ad_api/api/sp/keywords_v3.py
 ad_api/api/sp/negative_keywords.py
+ad_api/api/sp/negative_keywords_v3.py
 ad_api/api/sp/negative_product_targeting.py
+ad_api/api/sp/negative_product_targeting_v3.py
 ad_api/api/sp/product_ads.py
+ad_api/api/sp/product_ads_v3.py
 ad_api/api/sp/product_recommendations.py
 ad_api/api/sp/product_targeting.py
+ad_api/api/sp/product_targeting_v3.py
 ad_api/api/sp/ranked_keywords_recommendations.py
 ad_api/api/sp/reports.py
 ad_api/api/sp/snapshots.py
 ad_api/api/sp/suggested_keywords.py
 ad_api/auth/__init__.py
 ad_api/auth/access_token_client.py
 ad_api/auth/access_token_response.py
```

### Comparing `python-amazon-ad-api-0.4.1/setup.cfg` & `python-amazon-ad-api-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-amazon-ad-api
-version = 0.4.1
+version = 0.4.2
 author = Daniel Alvaro
 author_email = denisneuf@hotmail.com
 description = Python wrapper for the Amazon Advertising API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/denisneuf/python-amazon-ad-api
 project_urls =
```

### Comparing `python-amazon-ad-api-0.4.1/setup.py` & `python-amazon-ad-api-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='python-amazon-ad-api',
-    version='0.4.1',
+    version='0.4.2',
     install_requires=[
         "requests>=2.27.1,<2.29.0",
         "six~=1.16.0",
         "cachetools>=5.0,<5.4",
         "pycryptodome>=3.13,<3.18",
         "python-dotenv>=0.19.2,<1.1.0",
         "pytz>=2021.3,<2024.0",
```

