# Comparing `tmp/credmark-1.0.3.tar.gz` & `tmp/credmark-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credmark-1.0.3.tar", max compression
+gzip compressed data, was "credmark-1.1.0.tar", max compression
```

## Comparing `credmark-1.0.3.tar` & `credmark-1.1.0.tar`

### file list

```diff
@@ -1,137 +1,148 @@
--rw-r--r--   0        0        0     3692 2023-03-28 06:37:36.035987 credmark-1.0.3/README.md
--rw-r--r--   0        0        0      160 2023-03-28 06:36:00.984958 credmark-1.0.3/credmark/__init__.py
--rw-r--r--   0        0        0     2898 2023-03-28 06:36:01.106155 credmark-1.0.3/credmark/client.py
--rw-r--r--   0        0        0        0 2023-03-28 06:35:58.814867 credmark-1.0.3/credmark/defi_api/__init__.py
--rw-r--r--   0        0        0     7279 2023-03-28 06:36:01.233344 credmark-1.0.3/credmark/defi_api/get_cached_model_results.py
--rw-r--r--   0        0        0     4097 2023-03-28 06:36:01.111375 credmark-1.0.3/credmark/defi_api/get_model_by_slug.py
--rw-r--r--   0        0        0     4428 2023-03-28 06:36:01.154227 credmark-1.0.3/credmark/defi_api/get_model_deployments_by_slug.py
--rw-r--r--   0        0        0     3911 2023-03-28 06:36:01.140699 credmark-1.0.3/credmark/defi_api/get_model_runtime_stats.py
--rw-r--r--   0        0        0     4117 2023-03-28 06:36:01.148019 credmark-1.0.3/credmark/defi_api/list_models.py
--rw-r--r--   0        0        0     4314 2023-03-28 06:36:01.144281 credmark-1.0.3/credmark/defi_api/run_model.py
--rw-r--r--   0        0        0      320 2023-03-28 06:35:58.753352 credmark-1.0.3/credmark/docs/CheckHealthResponse200.md
--rw-r--r--   0        0        0       79 2023-03-28 06:35:58.752036 credmark-1.0.3/credmark/docs/CheckHealthResponse200Details.md
--rw-r--r--   0        0        0      172 2023-03-28 06:35:58.751243 credmark-1.0.3/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
--rw-r--r--   0        0        0       33 2023-03-28 06:35:58.750390 credmark-1.0.3/credmark/docs/CheckHealthResponse200Error.md
--rw-r--r--   0        0        0      170 2023-03-28 06:35:58.749669 credmark-1.0.3/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-03-28 06:35:58.748810 credmark-1.0.3/credmark/docs/CheckHealthResponse200Info.md
--rw-r--r--   0        0        0      169 2023-03-28 06:35:58.748029 credmark-1.0.3/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
--rw-r--r--   0        0        0      320 2023-03-28 06:35:58.759600 credmark-1.0.3/credmark/docs/CheckHealthResponse503.md
--rw-r--r--   0        0        0      140 2023-03-28 06:35:58.758325 credmark-1.0.3/credmark/docs/CheckHealthResponse503Details.md
--rw-r--r--   0        0        0      172 2023-03-28 06:35:58.757542 credmark-1.0.3/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
--rw-r--r--   0        0        0      108 2023-03-28 06:35:58.756693 credmark-1.0.3/credmark/docs/CheckHealthResponse503Error.md
--rw-r--r--   0        0        0      170 2023-03-28 06:35:58.755782 credmark-1.0.3/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-03-28 06:35:58.754990 credmark-1.0.3/credmark/docs/CheckHealthResponse503Info.md
--rw-r--r--   0        0        0      169 2023-03-28 06:35:58.754253 credmark-1.0.3/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
--rw-r--r--   0        0        0     2390 2023-03-28 06:35:58.821772 credmark-1.0.3/credmark/docs/DeFiAPI.md
--rw-r--r--   0        0        0      390 2023-03-28 06:35:58.698759 credmark-1.0.3/credmark/docs/ModelCallStackEntry.md
--rw-r--r--   0        0        0      259 2023-03-28 06:35:58.650325 credmark-1.0.3/credmark/docs/ModelDeployment.md
--rw-r--r--   0        0        0      519 2023-03-28 06:35:58.649472 credmark-1.0.3/credmark/docs/ModelMetadata.md
--rw-r--r--   0        0        0      753 2023-03-28 06:35:58.703274 credmark-1.0.3/credmark/docs/ModelRunResponse.md
--rw-r--r--   0        0        0      637 2023-03-28 06:35:58.701422 credmark-1.0.3/credmark/docs/ModelRunResponseError.md
--rw-r--r--   0        0        0      418 2023-03-28 06:35:58.652484 credmark-1.0.3/credmark/docs/ModelRuntimeStatistics.md
--rw-r--r--   0        0        0      165 2023-03-28 06:35:58.675653 credmark-1.0.3/credmark/docs/ModelRuntimeStatsResponse.md
--rw-r--r--   0        0        0      485 2023-03-28 06:35:58.697673 credmark-1.0.3/credmark/docs/RunModelDto.md
--rw-r--r--   0        0        0     9741 2023-03-28 06:35:58.852148 credmark-1.0.3/credmark/docs/TokenAPI.md
--rw-r--r--   0        0        0      597 2023-03-28 06:35:58.717711 credmark-1.0.3/credmark/docs/TokenAbiResponse.md
--rw-r--r--   0        0        0      318 2023-03-28 06:35:58.723678 credmark-1.0.3/credmark/docs/TokenBalanceHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-03-28 06:35:58.725298 credmark-1.0.3/credmark/docs/TokenBalanceHistoricalResponse.md
--rw-r--r--   0        0        0      530 2023-03-28 06:35:58.722798 credmark-1.0.3/credmark/docs/TokenBalanceResponse.md
--rw-r--r--   0        0        0      371 2023-03-28 06:35:58.716025 credmark-1.0.3/credmark/docs/TokenCreationBlockResponse.md
--rw-r--r--   0        0        0      347 2023-03-28 06:35:58.709840 credmark-1.0.3/credmark/docs/TokenDecimalsResponse.md
--rw-r--r--   0        0        0      491 2023-03-28 06:35:58.706397 credmark-1.0.3/credmark/docs/TokenErrorResponse.md
--rw-r--r--   0        0        0      214 2023-03-28 06:35:58.743762 credmark-1.0.3/credmark/docs/TokenHolder.md
--rw-r--r--   0        0        0      357 2023-03-28 06:35:58.747148 credmark-1.0.3/credmark/docs/TokenHoldersCountResponse.md
--rw-r--r--   0        0        0      613 2023-03-28 06:35:58.745738 credmark-1.0.3/credmark/docs/TokenHoldersResponse.md
--rw-r--r--   0        0        0      341 2023-03-28 06:35:58.714965 credmark-1.0.3/credmark/docs/TokenLogoResponse.md
--rw-r--r--   0        0        0      399 2023-03-28 06:35:58.704819 credmark-1.0.3/credmark/docs/TokenMetadataResponse.md
--rw-r--r--   0        0        0      333 2023-03-28 06:35:58.707567 credmark-1.0.3/credmark/docs/TokenNameResponse.md
--rw-r--r--   0        0        0      379 2023-03-28 06:35:58.720007 credmark-1.0.3/credmark/docs/TokenPriceHistoricalItem.md
--rw-r--r--   0        0        0      582 2023-03-28 06:35:58.721469 credmark-1.0.3/credmark/docs/TokenPriceHistoricalResponse.md
--rw-r--r--   0        0        0      531 2023-03-28 06:35:58.719000 credmark-1.0.3/credmark/docs/TokenPriceResponse.md
--rw-r--r--   0        0        0      339 2023-03-28 06:35:58.708725 credmark-1.0.3/credmark/docs/TokenSymbolResponse.md
--rw-r--r--   0        0        0      284 2023-03-28 06:35:58.712103 credmark-1.0.3/credmark/docs/TokenTotalSupplyHistoricalItem.md
--rw-r--r--   0        0        0      581 2023-03-28 06:35:58.713823 credmark-1.0.3/credmark/docs/TokenTotalSupplyHistoricalResponse.md
--rw-r--r--   0        0        0      423 2023-03-28 06:35:58.711115 credmark-1.0.3/credmark/docs/TokenTotalSupplyResponse.md
--rw-r--r--   0        0        0      404 2023-03-28 06:35:58.728295 credmark-1.0.3/credmark/docs/TokenVolumeHistoricalItem.md
--rw-r--r--   0        0        0      565 2023-03-28 06:35:58.742778 credmark-1.0.3/credmark/docs/TokenVolumeHistoricalResponse.md
--rw-r--r--   0        0        0      537 2023-03-28 06:35:58.726613 credmark-1.0.3/credmark/docs/TokenVolumeResponse.md
--rw-r--r--   0        0        0     1244 2023-03-28 06:35:58.814669 credmark-1.0.3/credmark/docs/Utilities.md
--rw-r--r--   0        0        0      470 2023-03-28 06:36:01.010535 credmark-1.0.3/credmark/errors.py
--rw-r--r--   0        0        0     5146 2023-03-28 06:35:58.765966 credmark-1.0.3/credmark/models/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-28 06:36:01.208462 credmark-1.0.3/credmark/models/check_health_response_200.py
--rw-r--r--   0        0        0     2144 2023-03-28 06:36:01.095810 credmark-1.0.3/credmark/models/check_health_response_200_details.py
--rw-r--r--   0        0        0     1658 2023-03-28 06:36:01.121124 credmark-1.0.3/credmark/models/check_health_response_200_details_additional_property.py
--rw-r--r--   0        0        0     2061 2023-03-28 06:36:01.103666 credmark-1.0.3/credmark/models/check_health_response_200_error.py
--rw-r--r--   0        0        0     1648 2023-03-28 06:36:01.093229 credmark-1.0.3/credmark/models/check_health_response_200_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-03-28 06:36:01.200529 credmark-1.0.3/credmark/models/check_health_response_200_info.py
--rw-r--r--   0        0        0     1643 2023-03-28 06:36:01.169478 credmark-1.0.3/credmark/models/check_health_response_200_info_additional_property.py
--rw-r--r--   0        0        0     4364 2023-03-28 06:36:01.275004 credmark-1.0.3/credmark/models/check_health_response_503.py
--rw-r--r--   0        0        0     2205 2023-03-28 06:36:01.198973 credmark-1.0.3/credmark/models/check_health_response_503_details.py
--rw-r--r--   0        0        0     1658 2023-03-28 06:36:01.197371 credmark-1.0.3/credmark/models/check_health_response_503_details_additional_property.py
--rw-r--r--   0        0        0     2149 2023-03-28 06:36:01.184508 credmark-1.0.3/credmark/models/check_health_response_503_error.py
--rw-r--r--   0        0        0     1648 2023-03-28 06:36:01.192017 credmark-1.0.3/credmark/models/check_health_response_503_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-03-28 06:36:01.237395 credmark-1.0.3/credmark/models/check_health_response_503_info.py
--rw-r--r--   0        0        0     1643 2023-03-28 06:36:01.223380 credmark-1.0.3/credmark/models/check_health_response_503_info_additional_property.py
--rw-r--r--   0        0        0      165 2023-03-28 06:36:00.172628 credmark-1.0.3/credmark/models/get_cached_model_results_order.py
--rw-r--r--   0        0        0      166 2023-03-28 06:36:00.142979 credmark-1.0.3/credmark/models/get_token_price_align.py
--rw-r--r--   0        0        0      163 2023-03-28 06:36:00.097957 credmark-1.0.3/credmark/models/get_token_price_historical_src.py
--rw-r--r--   0        0        0      153 2023-03-28 06:36:00.177051 credmark-1.0.3/credmark/models/get_token_price_src.py
--rw-r--r--   0        0        0     2470 2023-03-28 06:36:01.259803 credmark-1.0.3/credmark/models/model_call_stack_entry.py
--rw-r--r--   0        0        0     1894 2023-03-28 06:36:01.253570 credmark-1.0.3/credmark/models/model_deployment.py
--rw-r--r--   0        0        0     3325 2023-03-28 06:36:01.313921 credmark-1.0.3/credmark/models/model_metadata.py
--rw-r--r--   0        0        0     4190 2023-03-28 06:36:01.341915 credmark-1.0.3/credmark/models/model_run_response.py
--rw-r--r--   0        0        0     3362 2023-03-28 06:36:01.304463 credmark-1.0.3/credmark/models/model_run_response_error.py
--rw-r--r--   0        0        0     2412 2023-03-28 06:36:01.294885 credmark-1.0.3/credmark/models/model_runtime_statistics.py
--rw-r--r--   0        0        0     2042 2023-03-28 06:36:01.281464 credmark-1.0.3/credmark/models/model_runtime_stats_response.py
--rw-r--r--   0        0        0     3294 2023-03-28 06:36:01.329832 credmark-1.0.3/credmark/models/run_model_dto.py
--rw-r--r--   0        0        0      204 2023-03-28 06:36:00.122506 credmark-1.0.3/credmark/models/run_model_dto_block_number_type_1.py
--rw-r--r--   0        0        0     5771 2023-03-28 06:36:01.340219 credmark-1.0.3/credmark/models/token_abi_response.py
--rw-r--r--   0        0        0     2319 2023-03-28 06:36:01.336069 credmark-1.0.3/credmark/models/token_balance_historical_item.py
--rw-r--r--   0        0        0     4365 2023-03-28 06:36:01.359676 credmark-1.0.3/credmark/models/token_balance_historical_response.py
--rw-r--r--   0        0        0     3378 2023-03-28 06:36:01.348262 credmark-1.0.3/credmark/models/token_balance_response.py
--rw-r--r--   0        0        0     2692 2023-03-28 06:36:01.344064 credmark-1.0.3/credmark/models/token_creation_block_response.py
--rw-r--r--   0        0        0     2587 2023-03-28 06:36:01.352234 credmark-1.0.3/credmark/models/token_decimals_response.py
--rw-r--r--   0        0        0     2779 2023-03-28 06:36:01.359698 credmark-1.0.3/credmark/models/token_error_response.py
--rw-r--r--   0        0        0     1836 2023-03-28 06:36:01.352676 credmark-1.0.3/credmark/models/token_holder.py
--rw-r--r--   0        0        0     2589 2023-03-28 06:36:01.390408 credmark-1.0.3/credmark/models/token_holders_count_response.py
--rw-r--r--   0        0        0     4074 2023-03-28 06:36:01.474894 credmark-1.0.3/credmark/models/token_holders_response.py
--rw-r--r--   0        0        0     2711 2023-03-28 06:36:01.409026 credmark-1.0.3/credmark/models/token_logo_response.py
--rw-r--r--   0        0        0     2951 2023-03-28 06:36:01.407150 credmark-1.0.3/credmark/models/token_metadata_response.py
--rw-r--r--   0        0        0     2527 2023-03-28 06:36:01.413455 credmark-1.0.3/credmark/models/token_name_response.py
--rw-r--r--   0        0        0     2551 2023-03-28 06:36:01.429835 credmark-1.0.3/credmark/models/token_price_historical_item.py
--rw-r--r--   0        0        0     4118 2023-03-28 06:36:01.499978 credmark-1.0.3/credmark/models/token_price_historical_response.py
--rw-r--r--   0        0        0     3387 2023-03-28 06:36:01.478940 credmark-1.0.3/credmark/models/token_price_response.py
--rw-r--r--   0        0        0     2553 2023-03-28 06:36:01.481414 credmark-1.0.3/credmark/models/token_symbol_response.py
--rw-r--r--   0        0        0     2168 2023-03-28 06:36:01.399288 credmark-1.0.3/credmark/models/token_total_supply_historical_item.py
--rw-r--r--   0        0        0     4072 2023-03-28 06:36:01.510965 credmark-1.0.3/credmark/models/token_total_supply_historical_response.py
--rw-r--r--   0        0        0     2881 2023-03-28 06:36:01.466976 credmark-1.0.3/credmark/models/token_total_supply_response.py
--rw-r--r--   0        0        0     2758 2023-03-28 06:36:01.496791 credmark-1.0.3/credmark/models/token_volume_historical_item.py
--rw-r--r--   0        0        0     4001 2023-03-28 06:36:01.567821 credmark-1.0.3/credmark/models/token_volume_historical_response.py
--rw-r--r--   0        0        0     3465 2023-03-28 06:36:01.527145 credmark-1.0.3/credmark/models/token_volume_response.py
--rw-r--r--   0        0        0       25 2023-03-28 06:35:58.620005 credmark-1.0.3/credmark/py.typed
--rw-r--r--   0        0        0        0 2023-03-28 06:35:58.821976 credmark-1.0.3/credmark/token_api/__init__.py
--rw-r--r--   0        0        0     6447 2023-03-28 06:36:01.649428 credmark-1.0.3/credmark/token_api/get_token_abi.py
--rw-r--r--   0        0        0     8285 2023-03-28 06:36:01.700407 credmark-1.0.3/credmark/token_api/get_token_balance.py
--rw-r--r--   0        0        0    11472 2023-03-28 06:36:01.765095 credmark-1.0.3/credmark/token_api/get_token_balance_historical.py
--rw-r--r--   0        0        0     6705 2023-03-28 06:36:01.693944 credmark-1.0.3/credmark/token_api/get_token_creation_block.py
--rw-r--r--   0        0        0     6557 2023-03-28 06:36:01.677277 credmark-1.0.3/credmark/token_api/get_token_decimals.py
--rw-r--r--   0        0        0     8853 2023-03-28 06:36:01.754375 credmark-1.0.3/credmark/token_api/get_token_holders.py
--rw-r--r--   0        0        0     6811 2023-03-28 06:36:01.687119 credmark-1.0.3/credmark/token_api/get_token_holders_count.py
--rw-r--r--   0        0        0     6469 2023-03-28 06:36:01.705349 credmark-1.0.3/credmark/token_api/get_token_logo.py
--rw-r--r--   0        0        0     6538 2023-03-28 06:36:01.690514 credmark-1.0.3/credmark/token_api/get_token_metadata.py
--rw-r--r--   0        0        0     6469 2023-03-28 06:36:01.730491 credmark-1.0.3/credmark/token_api/get_token_name.py
--rw-r--r--   0        0        0     9002 2023-03-28 06:36:01.796459 credmark-1.0.3/credmark/token_api/get_token_price.py
--rw-r--r--   0        0        0    11577 2023-03-28 06:36:01.810969 credmark-1.0.3/credmark/token_api/get_token_price_historical.py
--rw-r--r--   0        0        0     6513 2023-03-28 06:36:01.797534 credmark-1.0.3/credmark/token_api/get_token_symbol.py
--rw-r--r--   0        0        0     7229 2023-03-28 06:36:01.820103 credmark-1.0.3/credmark/token_api/get_token_total_supply.py
--rw-r--r--   0        0        0    10412 2023-03-28 06:36:01.844838 credmark-1.0.3/credmark/token_api/get_token_total_supply_historical.py
--rw-r--r--   0        0        0     8883 2023-03-28 06:36:01.840632 credmark-1.0.3/credmark/token_api/get_token_volume.py
--rw-r--r--   0        0        0    10488 2023-03-28 06:36:01.849607 credmark-1.0.3/credmark/token_api/get_token_volume_historical.py
--rw-r--r--   0        0        0      974 2023-03-28 06:36:01.741105 credmark-1.0.3/credmark/types.py
--rw-r--r--   0        0        0        0 2023-03-28 06:35:58.786256 credmark-1.0.3/credmark/utilities/__init__.py
--rw-r--r--   0        0        0     4154 2023-03-28 06:36:01.793233 credmark-1.0.3/credmark/utilities/check_health.py
--rw-r--r--   0        0        0     5888 2023-03-28 06:36:01.828442 credmark-1.0.3/credmark/utilities/get_daily_model_usage.py
--rw-r--r--   0        0        0     3766 2023-03-28 06:36:01.812035 credmark-1.0.3/credmark/utilities/get_top_models.py
--rw-r--r--   0        0        0     3744 2023-03-28 06:36:01.823394 credmark-1.0.3/credmark/utilities/get_total_model_usage.py
--rw-r--r--   0        0        0      853 2023-03-28 06:41:02.231551 credmark-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 credmark-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2942 2023-04-11 03:50:08.006270 credmark-1.1.0/README.md
+-rw-r--r--   0        0        0      110 2023-04-11 03:48:43.361532 credmark-1.1.0/credmark/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 03:48:40.841425 credmark-1.1.0/credmark/api/__init__.py
+-rw-r--r--   0        0        0     9809 2023-04-11 03:48:43.507216 credmark-1.1.0/credmark/api/defi_api/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-11 03:48:43.565142 credmark-1.1.0/credmark/api/defi_api/get_cached_model_results.py
+-rw-r--r--   0        0        0     4018 2023-04-11 03:48:43.474293 credmark-1.1.0/credmark/api/defi_api/get_model_by_slug.py
+-rw-r--r--   0        0        0     4355 2023-04-11 03:48:43.488715 credmark-1.1.0/credmark/api/defi_api/get_model_deployments_by_slug.py
+-rw-r--r--   0        0        0     3852 2023-04-11 03:48:43.477515 credmark-1.1.0/credmark/api/defi_api/get_model_runtime_stats.py
+-rw-r--r--   0        0        0     4064 2023-04-11 03:48:43.493711 credmark-1.1.0/credmark/api/defi_api/list_models.py
+-rw-r--r--   0        0        0     4251 2023-04-11 03:48:43.495256 credmark-1.1.0/credmark/api/defi_api/run_model.py
+-rw-r--r--   0        0        0    61221 2023-04-11 03:48:44.554649 credmark-1.1.0/credmark/api/token_api/__init__.py
+-rw-r--r--   0        0        0     6476 2023-04-11 03:48:43.593660 credmark-1.1.0/credmark/api/token_api/get_token_abi.py
+-rw-r--r--   0        0        0     8314 2023-04-11 03:48:43.766732 credmark-1.1.0/credmark/api/token_api/get_token_balance.py
+-rw-r--r--   0        0        0    11501 2023-04-11 03:48:43.853075 credmark-1.1.0/credmark/api/token_api/get_token_balance_historical.py
+-rw-r--r--   0        0        0     6734 2023-04-11 03:48:43.769696 credmark-1.1.0/credmark/api/token_api/get_token_creation_block.py
+-rw-r--r--   0        0        0     6586 2023-04-11 03:48:43.790323 credmark-1.1.0/credmark/api/token_api/get_token_decimals.py
+-rw-r--r--   0        0        0     8882 2023-04-11 03:48:43.872630 credmark-1.1.0/credmark/api/token_api/get_token_holders.py
+-rw-r--r--   0        0        0     6840 2023-04-11 03:48:43.817300 credmark-1.1.0/credmark/api/token_api/get_token_holders_count.py
+-rw-r--r--   0        0        0    10051 2023-04-11 03:48:43.877457 credmark-1.1.0/credmark/api/token_api/get_token_holders_count_historical.py
+-rw-r--r--   0        0        0    11573 2023-04-11 03:48:43.950121 credmark-1.1.0/credmark/api/token_api/get_token_holders_historical.py
+-rw-r--r--   0        0        0     6498 2023-04-11 03:48:43.836262 credmark-1.1.0/credmark/api/token_api/get_token_logo.py
+-rw-r--r--   0        0        0     6567 2023-04-11 03:48:43.893052 credmark-1.1.0/credmark/api/token_api/get_token_metadata.py
+-rw-r--r--   0        0        0     6498 2023-04-11 03:48:43.920809 credmark-1.1.0/credmark/api/token_api/get_token_name.py
+-rw-r--r--   0        0        0     9033 2023-04-11 03:48:44.037652 credmark-1.1.0/credmark/api/token_api/get_token_price.py
+-rw-r--r--   0        0        0    11607 2023-04-11 03:48:44.086836 credmark-1.1.0/credmark/api/token_api/get_token_price_historical.py
+-rw-r--r--   0        0        0     6542 2023-04-11 03:48:43.987606 credmark-1.1.0/credmark/api/token_api/get_token_symbol.py
+-rw-r--r--   0        0        0     7258 2023-04-11 03:48:44.025479 credmark-1.1.0/credmark/api/token_api/get_token_total_supply.py
+-rw-r--r--   0        0        0    10441 2023-04-11 03:48:44.163673 credmark-1.1.0/credmark/api/token_api/get_token_total_supply_historical.py
+-rw-r--r--   0        0        0     8912 2023-04-11 03:48:44.119242 credmark-1.1.0/credmark/api/token_api/get_token_volume.py
+-rw-r--r--   0        0        0    10517 2023-04-11 03:48:44.196668 credmark-1.1.0/credmark/api/token_api/get_token_volume_historical.py
+-rw-r--r--   0        0        0     5998 2023-04-11 03:48:43.992821 credmark-1.1.0/credmark/api/utilities/__init__.py
+-rw-r--r--   0        0        0     4182 2023-04-11 03:48:43.999926 credmark-1.1.0/credmark/api/utilities/check_health.py
+-rw-r--r--   0        0        0     5921 2023-04-11 03:48:44.149704 credmark-1.1.0/credmark/api/utilities/get_daily_model_usage.py
+-rw-r--r--   0        0        0     3712 2023-04-11 03:48:44.079720 credmark-1.1.0/credmark/api/utilities/get_top_models.py
+-rw-r--r--   0        0        0     3690 2023-04-11 03:48:44.145224 credmark-1.1.0/credmark/api/utilities/get_total_model_usage.py
+-rw-r--r--   0        0        0     2763 2023-04-11 03:48:44.115214 credmark-1.1.0/credmark/client.py
+-rw-r--r--   0        0        0      320 2023-04-11 03:48:40.826829 credmark-1.1.0/credmark/docs/CheckHealthResponse200.md
+-rw-r--r--   0        0        0       79 2023-04-11 03:48:40.825602 credmark-1.1.0/credmark/docs/CheckHealthResponse200Details.md
+-rw-r--r--   0        0        0      172 2023-04-11 03:48:40.824931 credmark-1.1.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0       33 2023-04-11 03:48:40.824198 credmark-1.1.0/credmark/docs/CheckHealthResponse200Error.md
+-rw-r--r--   0        0        0      170 2023-04-11 03:48:40.823491 credmark-1.1.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-04-11 03:48:40.822692 credmark-1.1.0/credmark/docs/CheckHealthResponse200Info.md
+-rw-r--r--   0        0        0      169 2023-04-11 03:48:40.821914 credmark-1.1.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
+-rw-r--r--   0        0        0      320 2023-04-11 03:48:40.832574 credmark-1.1.0/credmark/docs/CheckHealthResponse503.md
+-rw-r--r--   0        0        0      140 2023-04-11 03:48:40.831417 credmark-1.1.0/credmark/docs/CheckHealthResponse503Details.md
+-rw-r--r--   0        0        0      172 2023-04-11 03:48:40.830764 credmark-1.1.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0      108 2023-04-11 03:48:40.830089 credmark-1.1.0/credmark/docs/CheckHealthResponse503Error.md
+-rw-r--r--   0        0        0      170 2023-04-11 03:48:40.829438 credmark-1.1.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-04-11 03:48:40.828400 credmark-1.1.0/credmark/docs/CheckHealthResponse503Info.md
+-rw-r--r--   0        0        0      169 2023-04-11 03:48:40.827622 credmark-1.1.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
+-rw-r--r--   0        0        0     2390 2023-04-11 03:48:40.902832 credmark-1.1.0/credmark/docs/DefiApi.md
+-rw-r--r--   0        0        0      390 2023-04-11 03:48:40.773881 credmark-1.1.0/credmark/docs/ModelCallStackEntry.md
+-rw-r--r--   0        0        0      259 2023-04-11 03:48:40.716024 credmark-1.1.0/credmark/docs/ModelDeployment.md
+-rw-r--r--   0        0        0      519 2023-04-11 03:48:40.715002 credmark-1.1.0/credmark/docs/ModelMetadata.md
+-rw-r--r--   0        0        0      753 2023-04-11 03:48:40.778862 credmark-1.1.0/credmark/docs/ModelRunResponse.md
+-rw-r--r--   0        0        0      637 2023-04-11 03:48:40.776812 credmark-1.1.0/credmark/docs/ModelRunResponseError.md
+-rw-r--r--   0        0        0      418 2023-04-11 03:48:40.718689 credmark-1.1.0/credmark/docs/ModelRuntimeStatistics.md
+-rw-r--r--   0        0        0      165 2023-04-11 03:48:40.747025 credmark-1.1.0/credmark/docs/ModelRuntimeStatsResponse.md
+-rw-r--r--   0        0        0      485 2023-04-11 03:48:40.772657 credmark-1.1.0/credmark/docs/RunModelDto.md
+-rw-r--r--   0        0        0      597 2023-04-11 03:48:40.795189 credmark-1.1.0/credmark/docs/TokenAbiResponse.md
+-rw-r--r--   0        0        0    11323 2023-04-11 03:48:40.947456 credmark-1.1.0/credmark/docs/TokenApi.md
+-rw-r--r--   0        0        0      318 2023-04-11 03:48:40.803073 credmark-1.1.0/credmark/docs/TokenBalanceHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-04-11 03:48:40.805048 credmark-1.1.0/credmark/docs/TokenBalanceHistoricalResponse.md
+-rw-r--r--   0        0        0      530 2023-04-11 03:48:40.801986 credmark-1.1.0/credmark/docs/TokenBalanceResponse.md
+-rw-r--r--   0        0        0      371 2023-04-11 03:48:40.792994 credmark-1.1.0/credmark/docs/TokenCreationBlockResponse.md
+-rw-r--r--   0        0        0      347 2023-04-11 03:48:40.786060 credmark-1.1.0/credmark/docs/TokenDecimalsResponse.md
+-rw-r--r--   0        0        0      491 2023-04-11 03:48:40.781892 credmark-1.1.0/credmark/docs/TokenErrorResponse.md
+-rw-r--r--   0        0        0      518 2023-04-11 03:48:40.820845 credmark-1.1.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
+-rw-r--r--   0        0        0      214 2023-04-11 03:48:40.811281 credmark-1.1.0/credmark/docs/TokenHolder.md
+-rw-r--r--   0        0        0      283 2023-04-11 03:48:40.819193 credmark-1.1.0/credmark/docs/TokenHoldersCountHistoricalItem.md
+-rw-r--r--   0        0        0      357 2023-04-11 03:48:40.818232 credmark-1.1.0/credmark/docs/TokenHoldersCountResponse.md
+-rw-r--r--   0        0        0      336 2023-04-11 03:48:40.814990 credmark-1.1.0/credmark/docs/TokenHoldersHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-04-11 03:48:40.816948 credmark-1.1.0/credmark/docs/TokenHoldersHistoricalResponse.md
+-rw-r--r--   0        0        0      613 2023-04-11 03:48:40.813345 credmark-1.1.0/credmark/docs/TokenHoldersResponse.md
+-rw-r--r--   0        0        0      341 2023-04-11 03:48:40.791546 credmark-1.1.0/credmark/docs/TokenLogoResponse.md
+-rw-r--r--   0        0        0      399 2023-04-11 03:48:40.780314 credmark-1.1.0/credmark/docs/TokenMetadataResponse.md
+-rw-r--r--   0        0        0      333 2023-04-11 03:48:40.783219 credmark-1.1.0/credmark/docs/TokenNameResponse.md
+-rw-r--r--   0        0        0      379 2023-04-11 03:48:40.798118 credmark-1.1.0/credmark/docs/TokenPriceHistoricalItem.md
+-rw-r--r--   0        0        0      582 2023-04-11 03:48:40.800381 credmark-1.1.0/credmark/docs/TokenPriceHistoricalResponse.md
+-rw-r--r--   0        0        0      531 2023-04-11 03:48:40.796897 credmark-1.1.0/credmark/docs/TokenPriceResponse.md
+-rw-r--r--   0        0        0      339 2023-04-11 03:48:40.784850 credmark-1.1.0/credmark/docs/TokenSymbolResponse.md
+-rw-r--r--   0        0        0      284 2023-04-11 03:48:40.788368 credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
+-rw-r--r--   0        0        0      581 2023-04-11 03:48:40.790178 credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
+-rw-r--r--   0        0        0      423 2023-04-11 03:48:40.787418 credmark-1.1.0/credmark/docs/TokenTotalSupplyResponse.md
+-rw-r--r--   0        0        0      404 2023-04-11 03:48:40.808357 credmark-1.1.0/credmark/docs/TokenVolumeHistoricalItem.md
+-rw-r--r--   0        0        0      565 2023-04-11 03:48:40.810302 credmark-1.1.0/credmark/docs/TokenVolumeHistoricalResponse.md
+-rw-r--r--   0        0        0      537 2023-04-11 03:48:40.807133 credmark-1.1.0/credmark/docs/TokenVolumeResponse.md
+-rw-r--r--   0        0        0     1244 2023-04-11 03:48:40.894326 credmark-1.1.0/credmark/docs/Utilities.md
+-rw-r--r--   0        0        0      470 2023-04-11 03:48:44.014187 credmark-1.1.0/credmark/errors.py
+-rw-r--r--   0        0        0     5618 2023-04-11 03:48:40.837882 credmark-1.1.0/credmark/models/__init__.py
+-rw-r--r--   0        0        0     4203 2023-04-11 03:48:44.226307 credmark-1.1.0/credmark/models/check_health_response_200.py
+-rw-r--r--   0        0        0     2144 2023-04-11 03:48:44.168797 credmark-1.1.0/credmark/models/check_health_response_200_details.py
+-rw-r--r--   0        0        0     1658 2023-04-11 03:48:44.188389 credmark-1.1.0/credmark/models/check_health_response_200_details_additional_property.py
+-rw-r--r--   0        0        0     2061 2023-04-11 03:48:44.192642 credmark-1.1.0/credmark/models/check_health_response_200_error.py
+-rw-r--r--   0        0        0     1648 2023-04-11 03:48:44.157247 credmark-1.1.0/credmark/models/check_health_response_200_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-04-11 03:48:44.188178 credmark-1.1.0/credmark/models/check_health_response_200_info.py
+-rw-r--r--   0        0        0     1643 2023-04-11 03:48:44.210996 credmark-1.1.0/credmark/models/check_health_response_200_info_additional_property.py
+-rw-r--r--   0        0        0     4364 2023-04-11 03:48:44.282037 credmark-1.1.0/credmark/models/check_health_response_503.py
+-rw-r--r--   0        0        0     2205 2023-04-11 03:48:44.212103 credmark-1.1.0/credmark/models/check_health_response_503_details.py
+-rw-r--r--   0        0        0     1658 2023-04-11 03:48:44.218992 credmark-1.1.0/credmark/models/check_health_response_503_details_additional_property.py
+-rw-r--r--   0        0        0     2149 2023-04-11 03:48:44.225452 credmark-1.1.0/credmark/models/check_health_response_503_error.py
+-rw-r--r--   0        0        0     1648 2023-04-11 03:48:44.230259 credmark-1.1.0/credmark/models/check_health_response_503_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-04-11 03:48:44.244207 credmark-1.1.0/credmark/models/check_health_response_503_info.py
+-rw-r--r--   0        0        0     1643 2023-04-11 03:48:44.243058 credmark-1.1.0/credmark/models/check_health_response_503_info_additional_property.py
+-rw-r--r--   0        0        0      165 2023-04-11 03:48:42.483324 credmark-1.1.0/credmark/models/get_cached_model_results_order.py
+-rw-r--r--   0        0        0      166 2023-04-11 03:48:42.435579 credmark-1.1.0/credmark/models/get_token_price_align.py
+-rw-r--r--   0        0        0      163 2023-04-11 03:48:42.323444 credmark-1.1.0/credmark/models/get_token_price_historical_src.py
+-rw-r--r--   0        0        0      153 2023-04-11 03:48:42.490561 credmark-1.1.0/credmark/models/get_token_price_src.py
+-rw-r--r--   0        0        0     2470 2023-04-11 03:48:44.273396 credmark-1.1.0/credmark/models/model_call_stack_entry.py
+-rw-r--r--   0        0        0     1894 2023-04-11 03:48:44.265761 credmark-1.1.0/credmark/models/model_deployment.py
+-rw-r--r--   0        0        0     3325 2023-04-11 03:48:44.318835 credmark-1.1.0/credmark/models/model_metadata.py
+-rw-r--r--   0        0        0     4190 2023-04-11 03:48:44.335806 credmark-1.1.0/credmark/models/model_run_response.py
+-rw-r--r--   0        0        0     3362 2023-04-11 03:48:44.312579 credmark-1.1.0/credmark/models/model_run_response_error.py
+-rw-r--r--   0        0        0     2412 2023-04-11 03:48:44.299140 credmark-1.1.0/credmark/models/model_runtime_statistics.py
+-rw-r--r--   0        0        0     2042 2023-04-11 03:48:44.287431 credmark-1.1.0/credmark/models/model_runtime_stats_response.py
+-rw-r--r--   0        0        0     3294 2023-04-11 03:48:44.326929 credmark-1.1.0/credmark/models/run_model_dto.py
+-rw-r--r--   0        0        0      204 2023-04-11 03:48:42.381661 credmark-1.1.0/credmark/models/run_model_dto_block_number_type_1.py
+-rw-r--r--   0        0        0     5771 2023-04-11 03:48:44.340408 credmark-1.1.0/credmark/models/token_abi_response.py
+-rw-r--r--   0        0        0     2319 2023-04-11 03:48:44.311771 credmark-1.1.0/credmark/models/token_balance_historical_item.py
+-rw-r--r--   0        0        0     4365 2023-04-11 03:48:44.373211 credmark-1.1.0/credmark/models/token_balance_historical_response.py
+-rw-r--r--   0        0        0     3378 2023-04-11 03:48:44.364911 credmark-1.1.0/credmark/models/token_balance_response.py
+-rw-r--r--   0        0        0     2692 2023-04-11 03:48:44.358929 credmark-1.1.0/credmark/models/token_creation_block_response.py
+-rw-r--r--   0        0        0     2587 2023-04-11 03:48:44.363033 credmark-1.1.0/credmark/models/token_decimals_response.py
+-rw-r--r--   0        0        0     2779 2023-04-11 03:48:44.382210 credmark-1.1.0/credmark/models/token_error_response.py
+-rw-r--r--   0        0        0     3856 2023-04-11 03:48:44.408475 credmark-1.1.0/credmark/models/token_historical_holders_count_response.py
+-rw-r--r--   0        0        0     1836 2023-04-11 03:48:44.376935 credmark-1.1.0/credmark/models/token_holder.py
+-rw-r--r--   0        0        0     2104 2023-04-11 03:48:44.382363 credmark-1.1.0/credmark/models/token_holders_count_historical_item.py
+-rw-r--r--   0        0        0     2589 2023-04-11 03:48:44.394564 credmark-1.1.0/credmark/models/token_holders_count_response.py
+-rw-r--r--   0        0        0     2693 2023-04-11 03:48:44.413882 credmark-1.1.0/credmark/models/token_holders_historical_item.py
+-rw-r--r--   0        0        0     4365 2023-04-11 03:48:44.449993 credmark-1.1.0/credmark/models/token_holders_historical_response.py
+-rw-r--r--   0        0        0     4074 2023-04-11 03:48:44.473184 credmark-1.1.0/credmark/models/token_holders_response.py
+-rw-r--r--   0        0        0     2711 2023-04-11 03:48:44.448358 credmark-1.1.0/credmark/models/token_logo_response.py
+-rw-r--r--   0        0        0     2951 2023-04-11 03:48:44.447777 credmark-1.1.0/credmark/models/token_metadata_response.py
+-rw-r--r--   0        0        0     2527 2023-04-11 03:48:44.439384 credmark-1.1.0/credmark/models/token_name_response.py
+-rw-r--r--   0        0        0     2551 2023-04-11 03:48:44.464882 credmark-1.1.0/credmark/models/token_price_historical_item.py
+-rw-r--r--   0        0        0     4118 2023-04-11 03:48:44.486483 credmark-1.1.0/credmark/models/token_price_historical_response.py
+-rw-r--r--   0        0        0     3387 2023-04-11 03:48:44.472840 credmark-1.1.0/credmark/models/token_price_response.py
+-rw-r--r--   0        0        0     2553 2023-04-11 03:48:44.477369 credmark-1.1.0/credmark/models/token_symbol_response.py
+-rw-r--r--   0        0        0     2168 2023-04-11 03:48:44.479696 credmark-1.1.0/credmark/models/token_total_supply_historical_item.py
+-rw-r--r--   0        0        0     4072 2023-04-11 03:48:44.509065 credmark-1.1.0/credmark/models/token_total_supply_historical_response.py
+-rw-r--r--   0        0        0     2881 2023-04-11 03:48:44.507441 credmark-1.1.0/credmark/models/token_total_supply_response.py
+-rw-r--r--   0        0        0     2758 2023-04-11 03:48:44.509501 credmark-1.1.0/credmark/models/token_volume_historical_item.py
+-rw-r--r--   0        0        0     4001 2023-04-11 03:48:44.527795 credmark-1.1.0/credmark/models/token_volume_historical_response.py
+-rw-r--r--   0        0        0     3465 2023-04-11 03:48:44.522644 credmark-1.1.0/credmark/models/token_volume_response.py
+-rw-r--r--   0        0        0       25 2023-04-11 03:48:40.680579 credmark-1.1.0/credmark/py.typed
+-rw-r--r--   0        0        0      974 2023-04-11 03:48:44.491916 credmark-1.1.0/credmark/types.py
+-rw-r--r--   0        0        0      853 2023-04-11 03:49:15.755611 credmark-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 credmark-1.1.0/PKG-INFO
```

### Comparing `credmark-1.0.3/README.md` & `credmark-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,56 +8,48 @@
 
 ```bash
 pip install credmark
 ```
 
 ## Usage
 
-First, create an authenticated client. In order to access the API, you will need a key. Information about getting a key is available in our [API setup guide](https://docs.credmark.com/api-how-to-guide/).
+First, create an instance of `Credmark` client. In order to access the API, you will need a key. Information about getting a key is available in our [API setup guide](https://docs.credmark.com/api-how-to-guide/).
 
 ```python
-from credmark import AuthenticatedClient
+from credmark import Credmark
 
-client = AuthenticatedClient(api_key="<Your API Key>")
+client = Credmark(api_key="<Your API Key>")
 ```
 
-Now call your endpoint and use your models:
+Now call your endpoint by tag and use your models:
 
 ```python
 from credmark.models import TokenMetadataResponse
-from credmark.token_api import get_token_metadata
-from credmark.types import Response
 
-metadata: TokenMetadataResponse = get_token_metadata.sync(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
-# or if you need more info (e.g. status_code)
-response: Response[TokenMetadataResponse] = get_token_metadata.sync(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
+metadata: TokenMetadataResponse = client.token_api.get_token_metadata(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 ```
 
 Or do the same thing with an async version:
 
 ```python
 from credmark.models import TokenMetadataResponse
-from credmark.token_api import get_token_metadata
-from credmark.types import Response
 
-metadata: TokenMetadataResponse = await get_token_metadata.asyncio(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
-response: Response[TokenMetadataResponse] = await get_token_metadata.asyncio_detailed(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
+metadata: TokenMetadataResponse = await client.token_api.get_token_metadata_async(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 ```
 
 ## Run a model
 
 You can run a model using DeFi API:
 
 ```python
 from credmark.defi_api import run_model
 from credmark.models import RunModelDto
 
 async def run_model_example():
-    price_data = await run_model.asyncio(
-        client=client,
+    price_data = await client.defi_api.run_model_async(
         json_body=RunModelDto(
             chain_id=1, 
             block_number="latest", 
             slug="price.quote", 
             input={"base": {"symbol": "AAVE"}}
         ),
     )
@@ -75,37 +67,35 @@
 - [Token API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/TokenAPI.md)
 - [DeFi API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/DeFiAPI.md)
 - [Utilities API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/Utilities.md)
 
 ## Things to know
 
 1. Every path/method combo has four functions:
-    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
-    2. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
-    3. `asyncio`: Like `sync` but async instead of blocking
-    4. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
+    1. default: Blocking request that returns parsed data (if successful) or `None`
+    2. `async`: Like default but async instead of blocking
 
 2. All path/query params, and bodies become method arguments.
 
 ## Advanced Usage
 
 By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
 
 ```python
-client = AuthenticatedClient(
+client = Credmark(
     base_url="https://internal_api.example.com", 
     api_key="SuperSecretToken",
     verify_ssl="/path/to/certificate_bundle.pem",
 )
 ```
 
 You can also disable certificate validation altogether, but beware that **this is a security risk**.
 
 ```python
-client = AuthenticatedClient(
+client = Credmark(
     base_url="https://internal_api.example.com", 
     api_key="SuperSecretToken", 
     verify_ssl=False
 )
 ```
 
-There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info.
+There are more settings on the generated `Credmark` class which let you control more runtime behavior, check out the docstring on that class for more info.
```

### Comparing `credmark-1.0.3/credmark/client.py` & `credmark-1.1.0/credmark/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import ssl
 from typing import Dict, Union
 
-import attr
+from .api.defi_api import DefiApi
+from .api.token_api import TokenApi
+from .api.utilities import Utilities
 
 
-@attr.s(auto_attribs=True)
-class Client:
+class Credmark:
     """A class for keeping track of data related to the API
 
     Attributes:
         base_url: The base URL for the API, all requests are made to a relative path to this URL
         cookies: A dictionary of cookies to be sent with every request
         headers: A dictionary of headers to be sent with every request
         timeout: The maximum amount of a time in seconds a request can take. API functions will raise
@@ -18,50 +19,50 @@
         verify_ssl: Whether or not to verify the SSL certificate of the API server. This should be True in production,
             but can be set to False for testing purposes.
         raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
             status code that was not documented in the source OpenAPI document.
         follow_redirects: Whether or not to follow redirects. Default value is False.
     """
 
-    base_url: str = "https://gateway.credmark.com"
-    cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    timeout: float = attr.ib(5.0, kw_only=True)
-    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
-    raise_on_unexpected_status: bool = attr.ib(False, kw_only=True)
-    follow_redirects: bool = attr.ib(False, kw_only=True)
+    def __init__(
+        self,
+        base_url: str = "https://gateway.credmark.com",
+        cookies: Union[Dict[str, str], None] = None,
+        headers: Union[Dict[str, str], None] = None,
+        timeout: float = 5.0,
+        verify_ssl: Union[str, bool, ssl.SSLContext] = True,
+        raise_on_unexpected_status: bool = False,
+        follow_redirects: bool = False,
+        api_key: Union[str, None] = os.getenv("CREDMARK_API_KEY"),
+        prefix: str = "Bearer",
+        auth_header_name: str = "Authorization",
+    ):
+        cookies = cookies if cookies is not None else {}
+        headers = headers if headers is not None else {}
+
+        self.base_url = base_url
+        self.cookies = cookies
+        self.headers = headers
+        self.timeout = timeout
+        self.verify_ssl = verify_ssl
+        self.raise_on_unexpected_status = raise_on_unexpected_status
+        self.follow_redirects = follow_redirects
+        self.api_key = api_key
+        self.prefix = prefix
+        self.auth_header_name = auth_header_name
+
+        self.utilities = Utilities(client=self)
+        self.defi_api = DefiApi(client=self)
+        self.token_api = TokenApi(client=self)
 
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in all endpoints"""
-        return {**self.headers}
-
-    def with_headers(self, headers: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional headers"""
-        return attr.evolve(self, headers={**self.headers, **headers})
+        if not self.api_key:
+            return {**self.headers}
+        auth_header_value = f"{self.prefix} {self.api_key}" if self.prefix else self.api_key
+        return {self.auth_header_name: auth_header_value, **self.headers}
 
     def get_cookies(self) -> Dict[str, str]:
         return {**self.cookies}
 
-    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional cookies"""
-        return attr.evolve(self, cookies={**self.cookies, **cookies})
-
     def get_timeout(self) -> float:
         return self.timeout
-
-    def with_timeout(self, timeout: float) -> "Client":
-        """Get a new client matching this one with a new timeout (in seconds)"""
-        return attr.evolve(self, timeout=timeout)
-
-
-@attr.s(auto_attribs=True)
-class AuthenticatedClient(Client):
-    """A Client which has been authenticated for use on secured endpoints"""
-
-    api_key: str = os.getenv("CREDMARK_API_KEY")
-    prefix: str = "Bearer"
-    auth_header_name: str = "Authorization"
-
-    def get_headers(self) -> Dict[str, str]:
-        """Get headers to be used in authenticated endpoints"""
-        auth_header_value = f"{self.prefix} {self.api_key}" if self.prefix else self.api_key
-        return {self.auth_header_name: auth_header_value, **self.headers}
```

### Comparing `credmark-1.0.3/credmark/defi_api/get_cached_model_results.py` & `credmark-1.1.0/credmark/api/defi_api/get_cached_model_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.get_cached_model_results_order import GetCachedModelResultsOrder
-from ..models.model_runtime_stats_response import ModelRuntimeStatsResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.get_cached_model_results_order import GetCachedModelResultsOrder
+from ...models.model_runtime_stats_response import ModelRuntimeStatsResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/model/results".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -48,42 +52,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ModelRuntimeStatsResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[ModelRuntimeStatsResponse]:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
@@ -116,20 +120,20 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[ModelRuntimeStatsResponse]:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
@@ -155,20 +159,20 @@
         limit=limit,
         offset=offset,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[ModelRuntimeStatsResponse]:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
@@ -199,20 +203,20 @@
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[ModelRuntimeStatsResponse]:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
```

### Comparing `credmark-1.0.3/credmark/defi_api/get_model_by_slug.py` & `credmark-1.1.0/credmark/api/defi_api/get_model_by_slug.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.model_metadata import ModelMetadata
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict
 
-def _get_kwargs(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.model_metadata import ModelMetadata
+from ...types import Response
+
+
+def _get_kwargs(slug: str, client: "Credmark") -> Dict[str, Any]:
     url = "{}/v1/models/{slug}".format(client.base_url, slug=slug)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
@@ -25,39 +25,35 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ModelMetadata]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelMetadata]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ModelMetadata.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ModelMetadata]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelMetadata]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[ModelMetadata]:
+def sync_detailed(slug: str, client: "Credmark") -> Response[ModelMetadata]:
     """Get model metadata by slug
 
      Returns the metadata for the specified model.
 
     Args:
         slug (str):
 
@@ -78,19 +74,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[ModelMetadata]:
+def sync(slug: str, client: "Credmark") -> Optional[ModelMetadata]:
     """Get model metadata by slug
 
      Returns the metadata for the specified model.
 
     Args:
         slug (str):
 
@@ -104,19 +96,15 @@
 
     return sync_detailed(
         slug=slug,
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[ModelMetadata]:
+async def asyncio_detailed(slug: str, client: "Credmark") -> Response[ModelMetadata]:
     """Get model metadata by slug
 
      Returns the metadata for the specified model.
 
     Args:
         slug (str):
 
@@ -135,19 +123,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[ModelMetadata]:
+async def asyncio(slug: str, client: "Credmark") -> Optional[ModelMetadata]:
     """Get model metadata by slug
 
      Returns the metadata for the specified model.
 
     Args:
         slug (str):
```

### Comparing `credmark-1.0.3/credmark/defi_api/get_model_deployments_by_slug.py` & `credmark-1.1.0/credmark/api/defi_api/get_model_deployments_by_slug.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.model_deployment import ModelDeployment
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict, List
 
-def _get_kwargs(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.model_deployment import ModelDeployment
+from ...types import Response
+
+
+def _get_kwargs(slug: str, client: "Credmark") -> Dict[str, Any]:
     url = "{}/v1/models/{slug}/deployments".format(client.base_url, slug=slug)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
@@ -25,15 +25,15 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["ModelDeployment"]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List["ModelDeployment"]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = ModelDeployment.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
@@ -41,28 +41,24 @@
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List["ModelDeployment"]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List["ModelDeployment"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[List["ModelDeployment"]]:
+def sync_detailed(slug: str, client: "Credmark") -> Response[List["ModelDeployment"]]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
@@ -83,19 +79,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List["ModelDeployment"]]:
+def sync(slug: str, client: "Credmark") -> Optional[List["ModelDeployment"]]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
@@ -109,19 +101,15 @@
 
     return sync_detailed(
         slug=slug,
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[List["ModelDeployment"]]:
+async def asyncio_detailed(slug: str, client: "Credmark") -> Response[List["ModelDeployment"]]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
@@ -140,19 +128,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    slug: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List["ModelDeployment"]]:
+async def asyncio(slug: str, client: "Credmark") -> Optional[List["ModelDeployment"]]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
```

### Comparing `credmark-1.0.3/credmark/defi_api/get_model_runtime_stats.py` & `credmark-1.1.0/credmark/api/defi_api/get_model_runtime_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.model_runtime_stats_response import ModelRuntimeStatsResponse
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict
 
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.model_runtime_stats_response import ModelRuntimeStatsResponse
+from ...types import Response
+
+
+def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
     url = "{}/v1/model/runtime-stats".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
@@ -24,38 +25,35 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ModelRuntimeStatsResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[ModelRuntimeStatsResponse]:
+def sync_detailed(client: "Credmark") -> Response[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -72,18 +70,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[ModelRuntimeStatsResponse]:
+def sync(client: "Credmark") -> Optional[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -93,18 +88,15 @@
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[ModelRuntimeStatsResponse]:
+async def asyncio_detailed(client: "Credmark") -> Response[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -119,18 +111,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[ModelRuntimeStatsResponse]:
+async def asyncio(client: "Credmark") -> Optional[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `credmark-1.0.3/credmark/defi_api/list_models.py` & `credmark-1.1.0/credmark/api/defi_api/list_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.model_metadata import ModelMetadata
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict, List
 
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.model_metadata import ModelMetadata
+from ...types import Response
+
+
+def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
     url = "{}/v1/models".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
@@ -24,15 +25,15 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["ModelMetadata"]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List["ModelMetadata"]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = ModelMetadata.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
@@ -40,27 +41,24 @@
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List["ModelMetadata"]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List["ModelMetadata"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[List["ModelMetadata"]]:
+def sync_detailed(client: "Credmark") -> Response[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -77,18 +75,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List["ModelMetadata"]]:
+def sync(client: "Credmark") -> Optional[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -98,18 +93,15 @@
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[List["ModelMetadata"]]:
+async def asyncio_detailed(client: "Credmark") -> Response[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -124,18 +116,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List["ModelMetadata"]]:
+async def asyncio(client: "Credmark") -> Optional[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `credmark-1.0.3/credmark/defi_api/run_model.py` & `credmark-1.1.0/credmark/api/defi_api/run_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.model_run_response import ModelRunResponse
-from ..models.run_model_dto import RunModelDto
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict
 
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: RunModelDto,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.model_run_response import ModelRunResponse
+from ...models.run_model_dto import RunModelDto
+from ...types import Response
+
+
+def _get_kwargs(*, json_body: RunModelDto, client: "Credmark") -> Dict[str, Any]:
     url = "{}/v1/model/run".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
@@ -29,39 +29,35 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ModelRunResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRunResponse]:
     if response.status_code == HTTPStatus.CREATED:
         response_201 = ModelRunResponse.from_dict(response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ModelRunResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRunResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: RunModelDto,
-) -> Response[ModelRunResponse]:
+def sync_detailed(*, json_body: RunModelDto, client: "Credmark") -> Response[ModelRunResponse]:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
@@ -82,19 +78,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: RunModelDto,
-) -> Optional[ModelRunResponse]:
+def sync(*, json_body: RunModelDto, client: "Credmark") -> Optional[ModelRunResponse]:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
@@ -108,19 +100,15 @@
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: RunModelDto,
-) -> Response[ModelRunResponse]:
+async def asyncio_detailed(*, json_body: RunModelDto, client: "Credmark") -> Response[ModelRunResponse]:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
@@ -139,19 +127,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: RunModelDto,
-) -> Optional[ModelRunResponse]:
+async def asyncio(*, json_body: RunModelDto, client: "Credmark") -> Optional[ModelRunResponse]:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
```

### Comparing `credmark-1.0.3/credmark/docs/DeFiAPI.md` & `credmark-1.1.0/credmark/docs/DefiApi.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/ModelMetadata.md` & `credmark-1.1.0/credmark/docs/ModelMetadata.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/ModelRunResponse.md` & `credmark-1.1.0/credmark/docs/ModelRunResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/ModelRunResponseError.md` & `credmark-1.1.0/credmark/docs/ModelRunResponseError.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenAPI.md` & `credmark-1.1.0/credmark/docs/TokenApi.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 [**get_token_price**](#get_token_price) | GET /v1/tokens/{chainId}/{tokenAddress}/price | Returns price data for a token.
 [**get_token_price_historical**](#get_token_price_historical) | GET /v1/tokens/{chainId}/{tokenAddress}/price/historical | Returns historical price data for a token.
 [**get_token_balance**](#get_token_balance) | GET /v1/tokens/{chainId}/{tokenAddress}/balance | Returns token balance for an account.
 [**get_token_balance_historical**](#get_token_balance_historical) | GET /v1/tokens/{chainId}/{tokenAddress}/balance/historical | Returns historical token balance for an account.
 [**get_token_volume**](#get_token_volume) | GET /v1/tokens/{chainId}/{tokenAddress}/volume | Returns traded volume for a token over a period of blocks or time.
 [**get_token_volume_historical**](#get_token_volume_historical) | GET /v1/tokens/{chainId}/{tokenAddress}/volume/historical | Returns traded volume for a token over a period of blocks or time divided by intervals.
 [**get_token_holders**](#get_token_holders) | GET /v1/tokens/{chainId}/{tokenAddress}/holders | Returns holders of a token at a block or time.
+[**get_token_holders_historical**](#get_token_holders_historical) | GET /v1/tokens/{chainId}/{tokenAddress}/holders/historical | Returns historical holders of a token at a block or time.
 [**get_token_holders_count**](#get_token_holders_count) | GET /v1/tokens/{chainId}/{tokenAddress}/holders/count | Returns total number of holders of a token at a block or time.
+[**get_token_holders_count_historical**](#get_token_holders_count_historical) | GET /v1/tokens/{chainId}/{tokenAddress}/holders/count/historical | Returns historical total number of holders of a token at a block or time.
 
 
 # **get_token_metadata**
 
 Get token metadata
 
  Returns metadata for a token.
@@ -126,21 +128,21 @@
 
 
 ### Parameters:
 Name | Type | Description
 ------------ | ------------- | -------------
 chain_id | float | None
 token_address | str | None
-scaled | bool | None
 start_block_number | float | None
 end_block_number | float | None
 block_interval | float | None
 start_timestamp | float | None
 end_timestamp | float | None
 time_interval | float | None
+scaled | bool | None
 
 
 ### Response Type
 Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]
 
 # **get_token_logo**
 
@@ -229,22 +231,22 @@
 
 
 ### Parameters:
 Name | Type | Description
 ------------ | ------------- | -------------
 chain_id | float | None
 token_address | str | None
-quote_address | str | None
-src | GetTokenPriceHistoricalSrc | None
 start_block_number | float | None
 end_block_number | float | None
 block_interval | float | None
 start_timestamp | float | None
 end_timestamp | float | None
 time_interval | float | None
+quote_address | str | None
+src | GetTokenPriceHistoricalSrc | None
 
 
 ### Response Type
 Union[TokenErrorResponse, TokenPriceHistoricalResponse]
 
 # **get_token_balance**
 
@@ -276,23 +278,23 @@
 
 
 ### Parameters:
 Name | Type | Description
 ------------ | ------------- | -------------
 chain_id | float | None
 token_address | str | None
-account_address | str | None
-quote_address | str | None
-scaled | bool | None
 start_block_number | float | None
 end_block_number | float | None
 block_interval | float | None
 start_timestamp | float | None
 end_timestamp | float | None
 time_interval | float | None
+account_address | str | None
+quote_address | str | None
+scaled | bool | None
 
 
 ### Response Type
 Union[TokenBalanceHistoricalResponse, TokenErrorResponse]
 
 # **get_token_volume**
 
@@ -359,14 +361,40 @@
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
 Union[TokenErrorResponse, TokenHoldersResponse]
 
+# **get_token_holders_historical**
+
+Get token historical holders
+
+ Returns historical holders of a token at a block or time.
+
+
+### Parameters:
+Name | Type | Description
+------------ | ------------- | -------------
+chain_id | float | None
+token_address | str | None
+start_block_number | float | None
+end_block_number | float | None
+block_interval | float | None
+start_timestamp | float | None
+end_timestamp | float | None
+time_interval | float | None
+page_size | float | None
+quote_address | str | None
+scaled | bool | None
+
+
+### Response Type
+Union[TokenErrorResponse, TokenHoldersHistoricalResponse]
+
 # **get_token_holders_count**
 
 Get total number of token holders
 
  Returns total number of holders of a token at a block or time.
 
 
@@ -378,7 +406,30 @@
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
 Union[TokenErrorResponse, TokenHoldersCountResponse]
 
+# **get_token_holders_count_historical**
+
+Get historical total number of token holders
+
+ Returns historical total number of holders of a token at a block or time.
+
+
+### Parameters:
+Name | Type | Description
+------------ | ------------- | -------------
+chain_id | float | None
+token_address | str | None
+start_block_number | float | None
+end_block_number | float | None
+block_interval | float | None
+start_timestamp | float | None
+end_timestamp | float | None
+time_interval | float | None
+
+
+### Response Type
+Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]
+
```

### Comparing `credmark-1.0.3/credmark/docs/TokenAbiResponse.md` & `credmark-1.1.0/credmark/docs/TokenAbiResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenBalanceHistoricalResponse.md` & `credmark-1.1.0/credmark/docs/TokenBalanceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenBalanceResponse.md` & `credmark-1.1.0/credmark/docs/TokenBalanceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenHoldersResponse.md` & `credmark-1.1.0/credmark/docs/TokenHoldersResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenPriceHistoricalResponse.md` & `credmark-1.1.0/credmark/docs/TokenPriceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenPriceResponse.md` & `credmark-1.1.0/credmark/docs/TokenPriceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenTotalSupplyHistoricalResponse.md` & `credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenVolumeHistoricalResponse.md` & `credmark-1.1.0/credmark/docs/TokenVolumeHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/TokenVolumeResponse.md` & `credmark-1.1.0/credmark/docs/TokenVolumeResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/docs/Utilities.md` & `credmark-1.1.0/credmark/docs/Utilities.md`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/__init__.py` & `credmark-1.1.0/credmark/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,20 @@
 from .token_abi_response import TokenAbiResponse
 from .token_balance_historical_item import TokenBalanceHistoricalItem
 from .token_balance_historical_response import TokenBalanceHistoricalResponse
 from .token_balance_response import TokenBalanceResponse
 from .token_creation_block_response import TokenCreationBlockResponse
 from .token_decimals_response import TokenDecimalsResponse
 from .token_error_response import TokenErrorResponse
+from .token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
 from .token_holder import TokenHolder
+from .token_holders_count_historical_item import TokenHoldersCountHistoricalItem
 from .token_holders_count_response import TokenHoldersCountResponse
+from .token_holders_historical_item import TokenHoldersHistoricalItem
+from .token_holders_historical_response import TokenHoldersHistoricalResponse
 from .token_holders_response import TokenHoldersResponse
 from .token_logo_response import TokenLogoResponse
 from .token_metadata_response import TokenMetadataResponse
 from .token_name_response import TokenNameResponse
 from .token_price_historical_item import TokenPriceHistoricalItem
 from .token_price_historical_response import TokenPriceHistoricalResponse
 from .token_price_response import TokenPriceResponse
@@ -82,16 +86,20 @@
     "TokenAbiResponse",
     "TokenBalanceHistoricalItem",
     "TokenBalanceHistoricalResponse",
     "TokenBalanceResponse",
     "TokenCreationBlockResponse",
     "TokenDecimalsResponse",
     "TokenErrorResponse",
+    "TokenHistoricalHoldersCountResponse",
     "TokenHolder",
+    "TokenHoldersCountHistoricalItem",
     "TokenHoldersCountResponse",
+    "TokenHoldersHistoricalItem",
+    "TokenHoldersHistoricalResponse",
     "TokenHoldersResponse",
     "TokenLogoResponse",
     "TokenMetadataResponse",
     "TokenNameResponse",
     "TokenPriceHistoricalItem",
     "TokenPriceHistoricalResponse",
     "TokenPriceResponse",
```

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200.py` & `credmark-1.1.0/credmark/models/check_health_response_200.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_details.py` & `credmark-1.1.0/credmark/models/check_health_response_200_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_details_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_200_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_error.py` & `credmark-1.1.0/credmark/models/check_health_response_200_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_error_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_200_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_info.py` & `credmark-1.1.0/credmark/models/check_health_response_200_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_200_info_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_200_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503.py` & `credmark-1.1.0/credmark/models/check_health_response_503.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_details.py` & `credmark-1.1.0/credmark/models/check_health_response_503_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_details_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_503_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_error.py` & `credmark-1.1.0/credmark/models/check_health_response_503_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_error_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_503_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_info.py` & `credmark-1.1.0/credmark/models/check_health_response_503_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/check_health_response_503_info_additional_property.py` & `credmark-1.1.0/credmark/models/check_health_response_503_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_call_stack_entry.py` & `credmark-1.1.0/credmark/models/model_call_stack_entry.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_deployment.py` & `credmark-1.1.0/credmark/models/model_deployment.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_metadata.py` & `credmark-1.1.0/credmark/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_run_response.py` & `credmark-1.1.0/credmark/models/model_run_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_run_response_error.py` & `credmark-1.1.0/credmark/models/model_run_response_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_runtime_statistics.py` & `credmark-1.1.0/credmark/models/model_runtime_statistics.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/model_runtime_stats_response.py` & `credmark-1.1.0/credmark/models/model_runtime_stats_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/run_model_dto.py` & `credmark-1.1.0/credmark/models/run_model_dto.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_abi_response.py` & `credmark-1.1.0/credmark/models/token_abi_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_balance_historical_item.py` & `credmark-1.1.0/credmark/models/token_balance_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_balance_historical_response.py` & `credmark-1.1.0/credmark/models/token_balance_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_balance_response.py` & `credmark-1.1.0/credmark/models/token_balance_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_creation_block_response.py` & `credmark-1.1.0/credmark/models/token_creation_block_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_decimals_response.py` & `credmark-1.1.0/credmark/models/token_decimals_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_error_response.py` & `credmark-1.1.0/credmark/models/token_error_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_holder.py` & `credmark-1.1.0/credmark/models/token_holder.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_holders_count_response.py` & `credmark-1.1.0/credmark/models/token_holders_count_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TokenHoldersCountResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        count (float): Total number of holders Example: 10.
+        count (float): Total number of holders Example: 42.
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
     count: float
```

### Comparing `credmark-1.0.3/credmark/models/token_holders_response.py` & `credmark-1.1.0/credmark/models/token_holders_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_logo_response.py` & `credmark-1.1.0/credmark/models/token_logo_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_metadata_response.py` & `credmark-1.1.0/credmark/models/token_metadata_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_name_response.py` & `credmark-1.1.0/credmark/models/token_name_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_price_historical_item.py` & `credmark-1.1.0/credmark/models/token_price_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_price_historical_response.py` & `credmark-1.1.0/credmark/models/token_price_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_price_response.py` & `credmark-1.1.0/credmark/models/token_price_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_symbol_response.py` & `credmark-1.1.0/credmark/models/token_symbol_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_total_supply_historical_item.py` & `credmark-1.1.0/credmark/models/token_total_supply_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_total_supply_historical_response.py` & `credmark-1.1.0/credmark/models/token_total_supply_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_total_supply_response.py` & `credmark-1.1.0/credmark/models/token_total_supply_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_volume_historical_item.py` & `credmark-1.1.0/credmark/models/token_volume_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_volume_historical_response.py` & `credmark-1.1.0/credmark/models/token_volume_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/models/token_volume_response.py` & `credmark-1.1.0/credmark/models/token_volume_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/token_api/get_token_abi.py` & `credmark-1.1.0/credmark/api/token_api/get_token_abi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_abi_response import TokenAbiResponse
-from ..models.token_error_response import TokenErrorResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_abi_response import TokenAbiResponse
+from ...models.token_error_response import TokenErrorResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/abi".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -40,15 +44,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenAbiResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -57,31 +61,31 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
@@ -113,17 +117,17 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
@@ -148,17 +152,17 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
@@ -188,17 +192,17 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_balance.py` & `credmark-1.1.0/credmark/api/token_api/get_token_balance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_balance_response import TokenBalanceResponse
-from ..models.token_error_response import TokenErrorResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_balance_response import TokenBalanceResponse
+from ...models.token_error_response import TokenErrorResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/balance".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -49,15 +53,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenBalanceResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -66,34 +70,34 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
@@ -131,20 +135,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
@@ -175,20 +179,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
@@ -224,20 +228,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_balance_historical.py` & `credmark-1.1.0/credmark/api/token_api/get_token_balance_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_balance_historical_response import TokenBalanceHistoricalResponse
-from ..models.token_error_response import TokenErrorResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_balance_historical_response import TokenBalanceHistoricalResponse
+from ...models.token_error_response import TokenErrorResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    account_address: str,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/balance/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["accountAddress"] = account_address
-
-    params["quoteAddress"] = quote_address
-
-    params["scaled"] = scaled
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
     params["blockInterval"] = block_interval
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
     params["timeInterval"] = time_interval
 
+    params["accountAddress"] = account_address
+
+    params["quoteAddress"] = quote_address
+
+    params["scaled"] = scaled
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenBalanceHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -78,253 +82,253 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    account_address: str,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        account_address (str):
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        account_address=account_address,
+        quote_address=quote_address,
+        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    account_address: str,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        account_address (str):
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        account_address=account_address,
+        quote_address=quote_address,
+        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    account_address: str,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        account_address (str):
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        account_address=account_address,
+        quote_address=quote_address,
+        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    account_address: str,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        account_address (str):
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            account_address=account_address,
-            quote_address=quote_address,
-            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             time_interval=time_interval,
+            account_address=account_address,
+            quote_address=quote_address,
+            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_creation_block.py` & `credmark-1.1.0/credmark/api/token_api/get_token_creation_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_creation_block_response import TokenCreationBlockResponse
-from ..models.token_error_response import TokenErrorResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_creation_block_response import TokenCreationBlockResponse
+from ...models.token_error_response import TokenErrorResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/creation-block".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -40,15 +44,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenCreationBlockResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -57,31 +61,31 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     """Get token creation block
 
      Returns creation block number of a token.
 
     Args:
         chain_id (float):
@@ -113,17 +117,17 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     """Get token creation block
 
      Returns creation block number of a token.
 
     Args:
         chain_id (float):
@@ -148,17 +152,17 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     """Get token creation block
 
      Returns creation block number of a token.
 
     Args:
         chain_id (float):
@@ -188,17 +192,17 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
     """Get token creation block
 
      Returns creation block number of a token.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_decimals.py` & `credmark-1.1.0/credmark/api/token_api/get_token_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_decimals_response import TokenDecimalsResponse
-from ..models.token_error_response import TokenErrorResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_name_response import TokenNameResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/decimals".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -40,65 +44,65 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenDecimalsResponse.from_dict(response.json())
+        response_200 = TokenNameResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
-    """Get token decimals
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
+    """Get token name
 
-     Returns decimals of a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[Union[TokenErrorResponse, TokenNameResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -113,34 +117,34 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
-    """Get token decimals
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+    """Get token name
 
-     Returns decimals of a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[Union[TokenErrorResponse, TokenNameResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -148,34 +152,34 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
-    """Get token decimals
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
+    """Get token name
 
-     Returns decimals of a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[Union[TokenErrorResponse, TokenNameResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -188,34 +192,34 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
-    """Get token decimals
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+    """Get token name
 
-     Returns decimals of a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[Union[TokenErrorResponse, TokenNameResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_holders.py` & `credmark-1.1.0/credmark/api/token_api/get_token_holders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_holders_response import TokenHoldersResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_holders_response import TokenHoldersResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -52,15 +56,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenHoldersResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -69,35 +73,35 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
@@ -137,21 +141,21 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
@@ -184,21 +188,21 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
@@ -236,21 +240,21 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_holders_count.py` & `credmark-1.1.0/credmark/api/token_api/get_token_total_supply.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,244 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_holders_count_response import TokenHoldersCountResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_total_supply_response import TokenTotalSupplyResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/total-supply".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["blockNumber"] = block_number
 
     params["timestamp"] = timestamp
 
+    params["scaled"] = scaled
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenHoldersCountResponse.from_dict(response.json())
+        response_200 = TokenTotalSupplyResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
-    """Get total number of token holders
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    """Get token's total supply
 
-     Returns total number of holders of a token at a block or time.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
-    """Get total number of token holders
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    """Get token's total supply
 
-     Returns total number of holders of a token at a block or time.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
-    """Get total number of token holders
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    """Get token's total supply
 
-     Returns total number of holders of a token at a block or time.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
-    """Get total number of token holders
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    """Get token's total supply
 
-     Returns total number of holders of a token at a block or time.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
             block_number=block_number,
             timestamp=timestamp,
+            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_logo.py` & `credmark-1.1.0/credmark/api/token_api/get_token_symbol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_logo_response import TokenLogoResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_symbol_response import TokenSymbolResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/logo".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/symbol".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -40,65 +44,65 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenLogoResponse.from_dict(response.json())
+        response_200 = TokenSymbolResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    """Get token symbol
 
-     Returns logo of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -113,34 +117,34 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    """Get token symbol
 
-     Returns logo of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -148,34 +152,34 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    """Get token symbol
 
-     Returns logo of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -188,34 +192,34 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    """Get token symbol
 
-     Returns logo of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_metadata.py` & `credmark-1.1.0/credmark/api/token_api/get_token_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_metadata_response import TokenMetadataResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_metadata_response import TokenMetadataResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}".format(client.base_url, chainId=chain_id, tokenAddress=token_address)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -38,15 +42,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenMetadataResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -55,31 +59,31 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
     """Get token metadata
 
      Returns metadata for a token.
 
     Args:
         chain_id (float):
@@ -111,17 +115,17 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
     """Get token metadata
 
      Returns metadata for a token.
 
     Args:
         chain_id (float):
@@ -146,17 +150,17 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
     """Get token metadata
 
      Returns metadata for a token.
 
     Args:
         chain_id (float):
@@ -186,17 +190,17 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
     """Get token metadata
 
      Returns metadata for a token.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_name.py` & `credmark-1.1.0/credmark/api/token_api/get_token_decimals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_name_response import TokenNameResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_decimals_response import TokenDecimalsResponse
+from ...models.token_error_response import TokenErrorResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/decimals".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -40,65 +44,65 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenNameResponse.from_dict(response.json())
+        response_200 = TokenDecimalsResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+    client: "Credmark",
+) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    """Get token decimals
 
-     Returns name of a token.
+     Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -113,34 +117,34 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+    client: "Credmark",
+) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    """Get token decimals
 
-     Returns name of a token.
+     Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -148,34 +152,34 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+    client: "Credmark",
+) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    """Get token decimals
 
-     Returns name of a token.
+     Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -188,34 +192,34 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+    client: "Credmark",
+) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    """Get token decimals
 
-     Returns name of a token.
+     Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_price.py` & `credmark-1.1.0/credmark/api/token_api/get_token_price.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.get_token_price_align import GetTokenPriceAlign
-from ..models.get_token_price_src import GetTokenPriceSrc
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_price_response import TokenPriceResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.get_token_price_align import GetTokenPriceAlign
+from ...models.get_token_price_src import GetTokenPriceSrc
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_price_response import TokenPriceResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/price".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -59,15 +63,15 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenPriceResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -76,34 +80,34 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
@@ -141,20 +145,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
@@ -185,20 +189,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
@@ -234,20 +238,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_price_historical.py` & `credmark-1.1.0/credmark/api/token_api/get_token_price_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.get_token_price_historical_src import GetTokenPriceHistoricalSrc
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_price_historical_response import TokenPriceHistoricalResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.get_token_price_historical_src import GetTokenPriceHistoricalSrc
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_price_historical_response import TokenPriceHistoricalResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    quote_address: Union[Unset, None, str] = UNSET,
-    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    quote_address: Union[Unset, None, str] = UNSET,
+    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/tokens/{chainId}/{tokenAddress}/price/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["quoteAddress"] = quote_address
-
-    json_src: Union[Unset, None, str] = UNSET
-    if not isinstance(src, Unset):
-        json_src = src.value if src else None
-
-    params["src"] = json_src
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
     params["blockInterval"] = block_interval
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
     params["timeInterval"] = time_interval
 
+    params["quoteAddress"] = quote_address
+
+    json_src: Union[Unset, None, str] = UNSET
+    if not isinstance(src, Unset):
+        json_src = src.value if src else None
+
+    params["src"] = json_src
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenPriceHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
@@ -80,245 +84,245 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    quote_address: Union[Unset, None, str] = UNSET,
-    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    quote_address: Union[Unset, None, str] = UNSET,
+    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        quote_address (Union[Unset, None, str]):
-        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-            GetTokenPriceHistoricalSrc.DEX.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        quote_address (Union[Unset, None, str]):
+        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
+            GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        quote_address=quote_address,
-        src=src,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        quote_address=quote_address,
+        src=src,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    quote_address: Union[Unset, None, str] = UNSET,
-    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    quote_address: Union[Unset, None, str] = UNSET,
+    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        quote_address (Union[Unset, None, str]):
-        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-            GetTokenPriceHistoricalSrc.DEX.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        quote_address (Union[Unset, None, str]):
+        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
+            GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        quote_address=quote_address,
-        src=src,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        quote_address=quote_address,
+        src=src,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    quote_address: Union[Unset, None, str] = UNSET,
-    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    quote_address: Union[Unset, None, str] = UNSET,
+    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
+    client: "Credmark",
 ) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        quote_address (Union[Unset, None, str]):
-        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-            GetTokenPriceHistoricalSrc.DEX.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        quote_address (Union[Unset, None, str]):
+        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
+            GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        quote_address=quote_address,
-        src=src,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        quote_address=quote_address,
+        src=src,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    quote_address: Union[Unset, None, str] = UNSET,
-    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    quote_address: Union[Unset, None, str] = UNSET,
+    src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
+    client: "Credmark",
 ) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        quote_address (Union[Unset, None, str]):
-        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-            GetTokenPriceHistoricalSrc.DEX.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        quote_address (Union[Unset, None, str]):
+        src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
+            GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            quote_address=quote_address,
-            src=src,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             time_interval=time_interval,
+            quote_address=quote_address,
+            src=src,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_symbol.py` & `credmark-1.1.0/credmark/api/token_api/get_token_holders_count.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_symbol_response import TokenSymbolResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_holders_count_response import TokenHoldersCountResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/symbol".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -40,65 +44,65 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenSymbolResponse.from_dict(response.json())
+        response_200 = TokenHoldersCountResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    """Get total number of token holders
 
-     Returns symbol of a token.
+     Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -113,34 +117,34 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    """Get total number of token holders
 
-     Returns symbol of a token.
+     Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -148,34 +152,34 @@
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    """Get total number of token holders
 
-     Returns symbol of a token.
+     Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -188,34 +192,34 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    """Get total number of token holders
 
-     Returns symbol of a token.
+     Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_total_supply.py` & `credmark-1.1.0/credmark/api/token_api/get_token_volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_total_supply_response import TokenTotalSupplyResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_volume_response import TokenVolumeResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
+    start_block_number: Union[Unset, None, float] = UNSET,
+    end_block_number: Union[Unset, None, float] = UNSET,
+    start_timestamp: Union[Unset, None, float] = UNSET,
+    end_timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/total-supply".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["blockNumber"] = block_number
+    params["scaled"] = scaled
 
-    params["timestamp"] = timestamp
+    params["startBlockNumber"] = start_block_number
 
-    params["scaled"] = scaled
+    params["endBlockNumber"] = end_block_number
+
+    params["startTimestamp"] = start_timestamp
+
+    params["endTimestamp"] = end_timestamp
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
@@ -43,198 +53,222 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenTotalSupplyResponse.from_dict(response.json())
+        response_200 = TokenVolumeResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
-    """Get token's total supply
+    start_block_number: Union[Unset, None, float] = UNSET,
+    end_block_number: Union[Unset, None, float] = UNSET,
+    start_timestamp: Union[Unset, None, float] = UNSET,
+    end_timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    """Get token volume
 
-     Returns total supply of a token.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
+        start_block_number (Union[Unset, None, float]):
+        end_block_number (Union[Unset, None, float]):
+        start_timestamp (Union[Unset, None, float]):
+        end_timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
         scaled=scaled,
+        start_block_number=start_block_number,
+        end_block_number=end_block_number,
+        start_timestamp=start_timestamp,
+        end_timestamp=end_timestamp,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
-    """Get token's total supply
+    start_block_number: Union[Unset, None, float] = UNSET,
+    end_block_number: Union[Unset, None, float] = UNSET,
+    start_timestamp: Union[Unset, None, float] = UNSET,
+    end_timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    """Get token volume
 
-     Returns total supply of a token.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
+        start_block_number (Union[Unset, None, float]):
+        end_block_number (Union[Unset, None, float]):
+        start_timestamp (Union[Unset, None, float]):
+        end_timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
         scaled=scaled,
+        start_block_number=start_block_number,
+        end_block_number=end_block_number,
+        start_timestamp=start_timestamp,
+        end_timestamp=end_timestamp,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
-    """Get token's total supply
+    start_block_number: Union[Unset, None, float] = UNSET,
+    end_block_number: Union[Unset, None, float] = UNSET,
+    start_timestamp: Union[Unset, None, float] = UNSET,
+    end_timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    """Get token volume
 
-     Returns total supply of a token.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
+        start_block_number (Union[Unset, None, float]):
+        end_block_number (Union[Unset, None, float]):
+        start_timestamp (Union[Unset, None, float]):
+        end_timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
         scaled=scaled,
+        start_block_number=start_block_number,
+        end_block_number=end_block_number,
+        start_timestamp=start_timestamp,
+        end_timestamp=end_timestamp,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
-    """Get token's total supply
+    start_block_number: Union[Unset, None, float] = UNSET,
+    end_block_number: Union[Unset, None, float] = UNSET,
+    start_timestamp: Union[Unset, None, float] = UNSET,
+    end_timestamp: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    """Get token volume
 
-     Returns total supply of a token.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
+        start_block_number (Union[Unset, None, float]):
+        end_block_number (Union[Unset, None, float]):
+        start_timestamp (Union[Unset, None, float]):
+        end_timestamp (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            block_number=block_number,
-            timestamp=timestamp,
             scaled=scaled,
+            start_block_number=start_block_number,
+            end_block_number=end_block_number,
+            start_timestamp=start_timestamp,
+            end_timestamp=end_timestamp,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_total_supply_historical.py` & `credmark-1.1.0/credmark/api/token_api/get_token_holders_historical.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,300 +1,334 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_total_supply_historical_response import TokenTotalSupplyHistoricalResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_holders_historical_response import TokenHoldersHistoricalResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    page_size: float = 100.0,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/total-supply/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["scaled"] = scaled
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
     params["blockInterval"] = block_interval
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
     params["timeInterval"] = time_interval
 
+    params["pageSize"] = page_size
+
+    params["quoteAddress"] = quote_address
+
+    params["scaled"] = scaled
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenTotalSupplyHistoricalResponse.from_dict(response.json())
+        response_200 = TokenHoldersHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
-    """Get historical total supply
+    page_size: float = 100.0,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    """Get token historical holders
 
-     Returns historical total supply for a token.
+     Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        page_size (float):  Default: 100.0.
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        page_size=page_size,
+        quote_address=quote_address,
+        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
-    """Get historical total supply
+    page_size: float = 100.0,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    """Get token historical holders
 
-     Returns historical total supply for a token.
+     Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        page_size (float):  Default: 100.0.
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        page_size=page_size,
+        quote_address=quote_address,
+        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
-    """Get historical total supply
+    page_size: float = 100.0,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    """Get token historical holders
 
-     Returns historical total supply for a token.
+     Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        page_size (float):  Default: 100.0.
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
+        page_size=page_size,
+        quote_address=quote_address,
+        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
-    """Get historical total supply
+    page_size: float = 100.0,
+    quote_address: Union[Unset, None, str] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    """Get token historical holders
 
-     Returns historical total supply for a token.
+     Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
+        page_size (float):  Default: 100.0.
+        quote_address (Union[Unset, None, str]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             time_interval=time_interval,
+            page_size=page_size,
+            quote_address=quote_address,
+            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_volume.py` & `credmark-1.1.0/credmark/api/token_api/get_token_total_supply_historical.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,270 +1,304 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_volume_response import TokenVolumeResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_total_supply_historical_response import TokenTotalSupplyHistoricalResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/total-supply/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["scaled"] = scaled
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
+    params["blockInterval"] = block_interval
+
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
+    params["timeInterval"] = time_interval
+
+    params["scaled"] = scaled
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenVolumeResponse.from_dict(response.json())
+        response_200 = TokenTotalSupplyHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+    time_interval: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    """Get historical total supply
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
+        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+    time_interval: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    """Get historical total supply
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
+        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+    time_interval: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    """Get historical total supply
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
+        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+    time_interval: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    """Get historical total supply
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
+            block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
+            time_interval=time_interval,
+            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/token_api/get_token_volume_historical.py` & `credmark-1.1.0/credmark/api/token_api/get_token_holders_count_historical.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..models.token_error_response import TokenErrorResponse
-from ..models.token_volume_historical_response import TokenVolumeHistoricalResponse
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import Dict, Optional, Union
+
+from ... import errors
+from ...models.token_error_response import TokenErrorResponse
+from ...models.token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["scaled"] = scaled
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
+    params["blockInterval"] = block_interval
+
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
-    params["blockInterval"] = block_interval
-
     params["timeInterval"] = time_interval
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
@@ -55,87 +56,84 @@
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenVolumeHistoricalResponse.from_dict(response.json())
+        response_200 = TokenHistoricalHoldersCountResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+    *, client: "Credmark", response: httpx.Response
+) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
         time_interval=time_interval,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
@@ -143,158 +141,149 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
         time_interval=time_interval,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+    client: "Credmark",
+) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
         time_interval=time_interval,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    client: AuthenticatedClient,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+    client: "Credmark",
+) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
+            block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
-            block_interval=block_interval,
             time_interval=time_interval,
         )
     ).parsed
```

### Comparing `credmark-1.0.3/credmark/types.py` & `credmark-1.1.0/credmark/types.py`

 * *Files identical despite different names*

### Comparing `credmark-1.0.3/credmark/utilities/check_health.py` & `credmark-1.1.0/credmark/api/utilities/check_health.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 
-from .. import errors
-from ..client import Client
-from ..models.check_health_response_200 import CheckHealthResponse200
-from ..models.check_health_response_503 import CheckHealthResponse503
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import Dict
 
-def _get_kwargs(
-    *,
-    client: Client,
-) -> Dict[str, Any]:
+from ... import errors
+from ...models.check_health_response_200 import CheckHealthResponse200
+from ...models.check_health_response_503 import CheckHealthResponse503
+from ...types import Response
+
+
+def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
     url = "{}/health".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
@@ -26,15 +27,15 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = CheckHealthResponse200.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.SERVICE_UNAVAILABLE:
         response_503 = CheckHealthResponse503.from_dict(response.json())
@@ -43,28 +44,25 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Client, response: httpx.Response
+    *, client: "Credmark", response: httpx.Response
 ) -> Response[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    *,
-    client: Client,
-) -> Response[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+def sync_detailed(client: "Credmark") -> Response[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     """Healthcheck status
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
@@ -79,18 +77,15 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: Client,
-) -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+def sync(client: "Credmark") -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     """Healthcheck status
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
@@ -98,18 +93,15 @@
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    *,
-    client: Client,
-) -> Response[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+async def asyncio_detailed(client: "Credmark") -> Response[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     """Healthcheck status
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
@@ -122,18 +114,15 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    *,
-    client: Client,
-) -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+async def asyncio(client: "Credmark") -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
     """Healthcheck status
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
```

### Comparing `credmark-1.0.3/credmark/utilities/get_daily_model_usage.py` & `credmark-1.1.0/credmark/api/utilities/get_daily_model_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..types import UNSET, Response, Unset
+if TYPE_CHECKING:
+    from ...client import Credmark
+
+from typing import List, Optional, Union, cast
+
+from ... import errors
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
+    client: "Credmark",
 ) -> Dict[str, Any]:
     url = "{}/v1/usage/requests".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -36,40 +40,40 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(List[Dict[str, Any]], response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List[Dict[str, Any]]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List[Dict[str, Any]]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
+    client: "Credmark",
 ) -> Response[List[Dict[str, Any]]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
@@ -97,18 +101,18 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
+    client: "Credmark",
 ) -> Optional[List[Dict[str, Any]]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
@@ -129,18 +133,18 @@
         group_by=group_by,
         requester=requester,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
+    client: "Credmark",
 ) -> Response[List[Dict[str, Any]]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
@@ -166,18 +170,18 @@
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
+    client: "Credmark",
 ) -> Optional[List[Dict[str, Any]]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
```

### Comparing `credmark-1.0.3/credmark/utilities/get_top_models.py` & `credmark-1.1.0/credmark/api/utilities/get_total_model_usage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
 
 import httpx
 
-from .. import errors
-from ..client import AuthenticatedClient, Client
-from ..types import Response
+if TYPE_CHECKING:
+    from ...client import Credmark
 
+from typing import List, cast
 
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
-    url = "{}/v1/usage/top".format(client.base_url)
+from ... import errors
+from ...types import Response
+
+
+def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
+    url = "{}/v1/usage/total".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(List[Dict[str, Any]], response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List[Dict[str, Any]]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List[Dict[str, Any]]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[List[Dict[str, Any]]]:
-    """Top Used Models
+def sync_detailed(client: "Credmark") -> Response[List[Dict[str, Any]]]:
+    """Total Model Usage
 
-     Returns a list of the top used models.
+     Returns a count of model runs.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
@@ -71,42 +69,36 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List[Dict[str, Any]]]:
-    """Top Used Models
+def sync(client: "Credmark") -> Optional[List[Dict[str, Any]]]:
+    """Total Model Usage
 
-     Returns a list of the top used models.
+     Returns a count of model runs.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-) -> Response[List[Dict[str, Any]]]:
-    """Top Used Models
+async def asyncio_detailed(client: "Credmark") -> Response[List[Dict[str, Any]]]:
+    """Total Model Usage
 
-     Returns a list of the top used models.
+     Returns a count of model runs.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
@@ -118,21 +110,18 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-) -> Optional[List[Dict[str, Any]]]:
-    """Top Used Models
+async def asyncio(client: "Credmark") -> Optional[List[Dict[str, Any]]]:
+    """Total Model Usage
 
-     Returns a list of the top used models.
+     Returns a count of model runs.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
```

### Comparing `credmark-1.0.3/pyproject.toml` & `credmark-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "credmark"
-version = "1.0.3"
+version = "1.1.0"
 description = "A client library for accessing Credmark Gateway"
 license = "MIT"
 
 authors = [
   "Credmark <info@credmark.com>",
 ]
```

### Comparing `credmark-1.0.3/PKG-INFO` & `credmark-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credmark
-Version: 1.0.3
+Version: 1.1.0
 Summary: A client library for accessing Credmark Gateway
 Home-page: https://credmark.com
 License: MIT
 Author: Credmark
 Author-email: info@credmark.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -31,56 +31,48 @@
 
 ```bash
 pip install credmark
 ```
 
 ## Usage
 
-First, create an authenticated client. In order to access the API, you will need a key. Information about getting a key is available in our [API setup guide](https://docs.credmark.com/api-how-to-guide/).
+First, create an instance of `Credmark` client. In order to access the API, you will need a key. Information about getting a key is available in our [API setup guide](https://docs.credmark.com/api-how-to-guide/).
 
 ```python
-from credmark import AuthenticatedClient
+from credmark import Credmark
 
-client = AuthenticatedClient(api_key="<Your API Key>")
+client = Credmark(api_key="<Your API Key>")
 ```
 
-Now call your endpoint and use your models:
+Now call your endpoint by tag and use your models:
 
 ```python
 from credmark.models import TokenMetadataResponse
-from credmark.token_api import get_token_metadata
-from credmark.types import Response
 
-metadata: TokenMetadataResponse = get_token_metadata.sync(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
-# or if you need more info (e.g. status_code)
-response: Response[TokenMetadataResponse] = get_token_metadata.sync(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
+metadata: TokenMetadataResponse = client.token_api.get_token_metadata(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 ```
 
 Or do the same thing with an async version:
 
 ```python
 from credmark.models import TokenMetadataResponse
-from credmark.token_api import get_token_metadata
-from credmark.types import Response
 
-metadata: TokenMetadataResponse = await get_token_metadata.asyncio(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
-response: Response[TokenMetadataResponse] = await get_token_metadata.asyncio_detailed(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9", client=client)
+metadata: TokenMetadataResponse = await client.token_api.get_token_metadata_async(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 ```
 
 ## Run a model
 
 You can run a model using DeFi API:
 
 ```python
 from credmark.defi_api import run_model
 from credmark.models import RunModelDto
 
 async def run_model_example():
-    price_data = await run_model.asyncio(
-        client=client,
+    price_data = await client.defi_api.run_model_async(
         json_body=RunModelDto(
             chain_id=1, 
             block_number="latest", 
             slug="price.quote", 
             input={"base": {"symbol": "AAVE"}}
         ),
     )
@@ -98,38 +90,36 @@
 - [Token API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/TokenAPI.md)
 - [DeFi API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/DeFiAPI.md)
 - [Utilities API](https://github.com/credmark/credmark-sdk-py/blob/main/credmark/docs/Utilities.md)
 
 ## Things to know
 
 1. Every path/method combo has four functions:
-    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
-    2. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
-    3. `asyncio`: Like `sync` but async instead of blocking
-    4. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
+    1. default: Blocking request that returns parsed data (if successful) or `None`
+    2. `async`: Like default but async instead of blocking
 
 2. All path/query params, and bodies become method arguments.
 
 ## Advanced Usage
 
 By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
 
 ```python
-client = AuthenticatedClient(
+client = Credmark(
     base_url="https://internal_api.example.com", 
     api_key="SuperSecretToken",
     verify_ssl="/path/to/certificate_bundle.pem",
 )
 ```
 
 You can also disable certificate validation altogether, but beware that **this is a security risk**.
 
 ```python
-client = AuthenticatedClient(
+client = Credmark(
     base_url="https://internal_api.example.com", 
     api_key="SuperSecretToken", 
     verify_ssl=False
 )
 ```
 
-There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info.
+There are more settings on the generated `Credmark` class which let you control more runtime behavior, check out the docstring on that class for more info.
```

