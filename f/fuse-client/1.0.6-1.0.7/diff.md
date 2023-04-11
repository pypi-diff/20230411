# Comparing `tmp/fuse-client-1.0.6.tar.gz` & `tmp/fuse-client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuse-client-1.0.6.tar", last modified: Tue Apr 11 09:43:37 2023, max compression
+gzip compressed data, was "fuse-client-1.0.7.tar", last modified: Tue Apr 11 10:09:13 2023, max compression
```

## Comparing `fuse-client-1.0.6.tar` & `fuse-client-1.0.7.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.268054 fuse-client-1.0.6/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.6/LICENSE
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 09:43:37.268137 fuse-client-1.0.6/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.6/README.md
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.244811 fuse-client-1.0.6/fuse-client/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      739 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.245021 fuse-client-1.0.6/fuse-client/api/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      212 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    91158 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    36894 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api_client.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.245196 fuse-client-1.0.6/fuse-client/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      452 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    21228 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/configuration.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5085 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/exceptions.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.256385 fuse-client-1.0.6/fuse-client/model/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      348 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    27574 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12061 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11690 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11513 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12371 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12132 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12167 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13358 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11510 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11929 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13654 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12128 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11360 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12294 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11715 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11350 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12404 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11587 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14438 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11530 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11616 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11687 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14204 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12931 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12630 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11913 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11124 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    19419 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14183 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11559 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13545 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14978 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11412 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    15583 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13181 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11708 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_addresses.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12117 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11797 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_emails.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11470 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_names.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_phone_numbers.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12712 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11967 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11598 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12323 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11714 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11940 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data_warnings.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11381 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11832 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13742 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12992 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11859 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12242 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_historical_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13394 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12094 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11336 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12724 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11318 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12579 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11933 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11334 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12049 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11312 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11645 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12391 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13137 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12694 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12065 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11293 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12451 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13477 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11313 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13115 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11267 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12271 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11448 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13344 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11333 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13168 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12017 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12370 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11603 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12286 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14669 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11153 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_response_removed.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    45053 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11097 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11963 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13317 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11759 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12227 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    81904 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model_utils.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.256489 fuse-client-1.0.6/fuse-client/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9568 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12686 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/rest.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.257003 fuse-client-1.0.6/fuse_client.egg-info/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10416 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/SOURCES.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/dependency_links.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       32 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/requires.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/top_level.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 09:43:37.268405 fuse-client-1.0.6/setup.cfg
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1068 2023-04-11 09:43:23.000000 fuse-client-1.0.6/setup.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.267956 fuse-client-1.0.6/test/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      771 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      742 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      843 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      844 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      865 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      836 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1147 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      728 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      714 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      999 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1006 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1465 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      871 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      899 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1480 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      913 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      956 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1114 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      941 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2156 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1199 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      993 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1259 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1247 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1586 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1081 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_addresses.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      878 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_emails.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      885 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_names.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_phone_numbers.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1054 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      842 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3752 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      874 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      975 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1047 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning_data_warnings.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      822 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      994 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1177 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1517 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      929 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1000 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_historical_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1037 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1040 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1323 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      942 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1251 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1165 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1130 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1169 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1143 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_response_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      970 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1022 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1064 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      921 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1108 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1580 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1049 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1518 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      992 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1214 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      721 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1111 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_response_removed.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      875 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      806 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      953 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      764 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.657669 fuse-client-1.0.7/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.7/LICENSE
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 10:09:13.657739 fuse-client-1.0.7/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.7/README.md
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632098 fuse-client-1.0.7/fuse_client/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      739 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632831 fuse-client-1.0.7/fuse_client/api/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      212 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    91158 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api/fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    36894 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api_client.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632991 fuse-client-1.0.7/fuse_client/apis/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      452 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/apis/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    21228 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/configuration.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5085 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/exceptions.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.645197 fuse-client-1.0.7/fuse_client/model/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      348 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    27574 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12061 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11690 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11513 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12371 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12132 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12167 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13358 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11510 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11929 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13654 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12128 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11360 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12294 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11715 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11350 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12404 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11587 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14438 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11530 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11616 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11687 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_teller.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14204 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12931 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12630 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11913 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_details_ach.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11124 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19419 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14183 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11559 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of_aprs.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13545 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14978 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11412 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    15583 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13181 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11708 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_addresses.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12117 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11797 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_emails.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11470 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_names.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_phone_numbers.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12712 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11967 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_institution_logo.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11598 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_error_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12323 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11714 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11940 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data_warnings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11381 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11832 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13742 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12992 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11859 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12242 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_historical_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13394 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12094 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11336 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12724 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11318 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12579 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11933 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11334 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12049 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11312 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11645 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12391 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13137 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12694 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12065 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11293 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12451 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13477 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11313 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13115 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11267 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12271 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11448 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13344 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11333 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13168 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12017 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12370 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11603 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12286 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14669 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11153 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_response_removed.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    45053 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11097 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/transaction_merchant.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11963 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13317 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11759 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12227 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    81904 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model_utils.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.645305 fuse-client-1.0.7/fuse_client/models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9568 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/models/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12686 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/rest.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632618 fuse-client-1.0.7/fuse_client.egg-info/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10416 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       32 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/requires.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/top_level.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 10:09:13.657983 fuse-client-1.0.7/setup.cfg
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1068 2023-04-11 10:09:06.000000 fuse-client-1.0.7/setup.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.657549 fuse-client-1.0.7/test/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      771 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      742 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      843 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      844 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      865 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      836 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1147 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      728 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      714 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      999 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1006 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1465 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      871 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      899 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_teller.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1480 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      913 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      956 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1114 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_details_ach.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      941 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2156 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1199 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      993 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of_aprs.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1259 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_security_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1247 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1586 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1081 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_addresses.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      878 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_emails.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      885 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_names.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_phone_numbers.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1054 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      842 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_institution_logo.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3752 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      874 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      975 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_error_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1047 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning_data_warnings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      822 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      994 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1177 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1517 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      929 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1000 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_historical_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1037 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1040 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1323 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      942 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1251 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1165 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1130 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1169 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1143 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_response_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      970 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1022 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1064 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      921 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1108 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1580 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1049 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1518 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      992 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_request_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1214 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      721 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1111 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_response_removed.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      875 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      806 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_transaction_merchant.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      953 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      764 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_type.py
```

### Comparing `fuse-client-1.0.6/LICENSE` & `fuse-client-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.6/README.md` & `fuse-client-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.6/fuse-client/__init__.py` & `fuse-client-1.0.7/fuse_client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 # import ApiClient
-from fuse-client.api_client import ApiClient
+from fuse_client.api_client import ApiClient
 
 # import Configuration
-from fuse-client.configuration import Configuration
+from fuse_client.configuration import Configuration
 
 # import exceptions
-from fuse-client.exceptions import OpenApiException
-from fuse-client.exceptions import ApiAttributeError
-from fuse-client.exceptions import ApiTypeError
-from fuse-client.exceptions import ApiValueError
-from fuse-client.exceptions import ApiKeyError
-from fuse-client.exceptions import ApiException
+from fuse_client.exceptions import OpenApiException
+from fuse_client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiTypeError
+from fuse_client.exceptions import ApiValueError
+from fuse_client.exceptions import ApiKeyError
+from fuse_client.exceptions import ApiException
```

### Comparing `fuse-client-1.0.6/fuse-client/api/fuse_api.py` & `fuse-client-1.0.7/fuse_client/api/fuse_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,58 +7,58 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.api_client import ApiClient, Endpoint as _Endpoint
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.api_client import ApiClient, Endpoint as _Endpoint
+from fuse_client.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fuse-client.model.create_asset_report_request import CreateAssetReportRequest
-from fuse-client.model.create_asset_report_response import CreateAssetReportResponse
-from fuse-client.model.create_link_token_request import CreateLinkTokenRequest
-from fuse-client.model.create_link_token_response import CreateLinkTokenResponse
-from fuse-client.model.create_session_request import CreateSessionRequest
-from fuse-client.model.create_session_response import CreateSessionResponse
-from fuse-client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
-from fuse-client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
-from fuse-client.model.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
-from fuse-client.model.get_asset_report_request import GetAssetReportRequest
-from fuse-client.model.get_asset_report_response import GetAssetReportResponse
-from fuse-client.model.get_entity_response import GetEntityResponse
-from fuse-client.model.get_financial_connection_response import GetFinancialConnectionResponse
-from fuse-client.model.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
-from fuse-client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
-from fuse-client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
-from fuse-client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
-from fuse-client.model.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
-from fuse-client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
-from fuse-client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
-from fuse-client.model.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
-from fuse-client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
-from fuse-client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
-from fuse-client.model.get_financial_institution_response import GetFinancialInstitutionResponse
-from fuse-client.model.get_investment_holdings_request import GetInvestmentHoldingsRequest
-from fuse-client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
-from fuse-client.model.get_investment_transactions_request import GetInvestmentTransactionsRequest
-from fuse-client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
-from fuse-client.model.get_liabilities_request import GetLiabilitiesRequest
-from fuse-client.model.get_liabilities_response import GetLiabilitiesResponse
-from fuse-client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
-from fuse-client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
-from fuse-client.model.refresh_asset_report_request import RefreshAssetReportRequest
-from fuse-client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
+from fuse_client.model.create_asset_report_request import CreateAssetReportRequest
+from fuse_client.model.create_asset_report_response import CreateAssetReportResponse
+from fuse_client.model.create_link_token_request import CreateLinkTokenRequest
+from fuse_client.model.create_link_token_response import CreateLinkTokenResponse
+from fuse_client.model.create_session_request import CreateSessionRequest
+from fuse_client.model.create_session_response import CreateSessionResponse
+from fuse_client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
+from fuse_client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
+from fuse_client.model.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
+from fuse_client.model.get_asset_report_request import GetAssetReportRequest
+from fuse_client.model.get_asset_report_response import GetAssetReportResponse
+from fuse_client.model.get_entity_response import GetEntityResponse
+from fuse_client.model.get_financial_connection_response import GetFinancialConnectionResponse
+from fuse_client.model.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
+from fuse_client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
+from fuse_client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
+from fuse_client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
+from fuse_client.model.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
+from fuse_client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
+from fuse_client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
+from fuse_client.model.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
+from fuse_client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
+from fuse_client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
+from fuse_client.model.get_financial_institution_response import GetFinancialInstitutionResponse
+from fuse_client.model.get_investment_holdings_request import GetInvestmentHoldingsRequest
+from fuse_client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
+from fuse_client.model.get_investment_transactions_request import GetInvestmentTransactionsRequest
+from fuse_client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
+from fuse_client.model.get_liabilities_request import GetLiabilitiesRequest
+from fuse_client.model.get_liabilities_response import GetLiabilitiesResponse
+from fuse_client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
+from fuse_client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
+from fuse_client.model.refresh_asset_report_request import RefreshAssetReportRequest
+from fuse_client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
 
 
 class FuseApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `fuse-client-1.0.6/fuse-client/api_client.py` & `fuse-client-1.0.7/fuse_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from fuse-client import rest
-from fuse-client.configuration import Configuration
-from fuse-client.exceptions import ApiTypeError, ApiValueError, ApiException
-from fuse-client.model_utils import (
+from fuse_client import rest
+from fuse_client.configuration import Configuration
+from fuse_client.exceptions import ApiTypeError, ApiValueError, ApiException
+from fuse_client.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.6/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.7/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `fuse-client-1.0.6/fuse-client/configuration.py` & `fuse-client-1.0.7/fuse_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from fuse-client.exceptions import ApiValueError
+from fuse_client.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -85,15 +85,15 @@
           cookieAuth:         # name for the security scheme
             type: apiKey
             in: cookie
             name: JSESSIONID  # cookie name
 
     You can programmatically set the cookie:
 
-conf = fuse-client.Configuration(
+conf = fuse_client.Configuration(
     api_key={'cookieAuth': 'abc123'}
     api_key_prefix={'cookieAuth': 'JSESSIONID'}
 )
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
@@ -148,15 +148,15 @@
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("fuse-client")
+        self.logger["package_logger"] = logging.getLogger("fuse_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -519,15 +519,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.6".\
+               "SDK Package Version: 1.0.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fuse-client-1.0.6/fuse-client/exceptions.py` & `fuse-client-1.0.7/fuse_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.6/fuse-client/model/account_subtype.py` & `fuse-client-1.0.7/fuse_client/model/account_subtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class AccountSubtype(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/account_type.py` & `fuse-client-1.0.7/fuse_client/model/account_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class AccountType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/aggregator.py` & `fuse-client-1.0.7/fuse_client/model/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class Aggregator(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/country_code.py` & `fuse-client-1.0.7/fuse_client/model/country_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CountryCode(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_asset_report_request.py` & `fuse-client-1.0.7/fuse_client/model/create_asset_report_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateAssetReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_asset_report_response.py` & `fuse-client-1.0.7/fuse_client/model/create_asset_report_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateAssetReportResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_entity_request.py` & `fuse-client-1.0.7/fuse_client/model/create_entity_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
+    from fuse_client.model.aggregator import Aggregator
     globals()['Aggregator'] = Aggregator
 
 
 class CreateEntityRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_entity_response.py` & `fuse-client-1.0.7/fuse_client/model/create_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
+    from fuse_client.model.aggregator import Aggregator
     globals()['Aggregator'] = Aggregator
 
 
 class CreateEntityResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_link_token_request.py` & `fuse-client-1.0.7/fuse_client/model/create_link_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
-    from fuse-client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
-    from fuse-client.model.entity import Entity
+    from fuse_client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
+    from fuse_client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
+    from fuse_client.model.entity import Entity
     globals()['CreateLinkTokenRequestMx'] = CreateLinkTokenRequestMx
     globals()['CreateLinkTokenRequestPlaid'] = CreateLinkTokenRequestPlaid
     globals()['Entity'] = Entity
 
 
 class CreateLinkTokenRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_link_token_request_mx.py` & `fuse-client-1.0.7/fuse_client/model/create_link_token_request_mx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateLinkTokenRequestMx(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_link_token_request_plaid.py` & `fuse-client-1.0.7/fuse_client/model/create_link_token_request_plaid.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateLinkTokenRequestPlaid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_link_token_response.py` & `fuse-client-1.0.7/fuse_client/model/create_link_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateLinkTokenResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_session_request.py` & `fuse-client-1.0.7/fuse_client/model/create_session_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
-    from fuse-client.model.country_code import CountryCode
-    from fuse-client.model.entity import Entity
-    from fuse-client.model.product import Product
+    from fuse_client.model.aggregator import Aggregator
+    from fuse_client.model.country_code import CountryCode
+    from fuse_client.model.entity import Entity
+    from fuse_client.model.product import Product
     globals()['Aggregator'] = Aggregator
     globals()['CountryCode'] = CountryCode
     globals()['Entity'] = Entity
     globals()['Product'] = Product
 
 
 class CreateSessionRequest(ModelNormal):
```

### Comparing `fuse-client-1.0.6/fuse-client/model/create_session_response.py` & `fuse-client-1.0.7/fuse_client/model/create_session_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class CreateSessionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/currency.py` & `fuse-client-1.0.7/fuse_client/model/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class Currency(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/delete_financial_connection_response.py` & `fuse-client-1.0.7/fuse_client/model/delete_financial_connection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class DeleteFinancialConnectionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/entity.py` & `fuse-client-1.0.7/fuse_client/model/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class Entity(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class ExchangeFinancialConnectionsPublicTokenRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_response.py` & `fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class ExchangeFinancialConnectionsPublicTokenResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connection_data.py` & `fuse-client-1.0.7/fuse_client/model/financial_connection_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connection_details.py` & `fuse-client-1.0.7/fuse_client/model/financial_connection_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
-    from fuse-client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
-    from fuse-client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
-    from fuse-client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
+    from fuse_client.model.aggregator import Aggregator
+    from fuse_client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
+    from fuse_client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
+    from fuse_client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
     globals()['Aggregator'] = Aggregator
     globals()['FinancialConnectionDetailsMx'] = FinancialConnectionDetailsMx
     globals()['FinancialConnectionDetailsPlaid'] = FinancialConnectionDetailsPlaid
     globals()['FinancialConnectionDetailsTeller'] = FinancialConnectionDetailsTeller
 
 
 class FinancialConnectionDetails(ModelNormal):
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connection_details_mx.py` & `fuse-client-1.0.7/fuse_client/model/financial_connection_details_mx.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionDetailsMx(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connection_details_plaid.py` & `fuse-client-1.0.7/fuse_client/model/financial_connection_details_plaid.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionDetailsPlaid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connection_details_teller.py` & `fuse-client-1.0.7/fuse_client/model/financial_connection_details_teller.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionDetailsTeller(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.account_subtype import AccountSubtype
-    from fuse-client.model.account_type import AccountType
-    from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-    from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+    from fuse_client.model.account_subtype import AccountSubtype
+    from fuse_client.model.account_type import AccountType
+    from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+    from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
     globals()['AccountSubtype'] = AccountSubtype
     globals()['AccountType'] = AccountType
     globals()['FinancialConnectionsAccountCachedBalance'] = FinancialConnectionsAccountCachedBalance
     globals()['FinancialConnectionsAccountInstitution'] = FinancialConnectionsAccountInstitution
 
 
 class FinancialConnectionsAccount(ModelNormal):
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_balance.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsAccountBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_cached_balance.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_cached_balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsAccountCachedBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_details.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
+    from fuse_client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
     globals()['FinancialConnectionsAccountDetailsAch'] = FinancialConnectionsAccountDetailsAch
 
 
 class FinancialConnectionsAccountDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_details_ach.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_details_ach.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsAccountDetailsAch(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_institution.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsAccountInstitution(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.account_subtype import AccountSubtype
-    from fuse-client.model.account_type import AccountType
-    from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-    from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-    from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
-    from fuse-client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
-    from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+    from fuse_client.model.account_subtype import AccountSubtype
+    from fuse_client.model.account_type import AccountType
+    from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+    from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+    from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+    from fuse_client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
+    from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
     globals()['AccountSubtype'] = AccountSubtype
     globals()['AccountType'] = AccountType
     globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
     globals()['FinancialConnectionsAccountCachedBalance'] = FinancialConnectionsAccountCachedBalance
     globals()['FinancialConnectionsAccountInstitution'] = FinancialConnectionsAccountInstitution
     globals()['FinancialConnectionsAccountLiabilityAllOf'] = FinancialConnectionsAccountLiabilityAllOf
     globals()['FinancialConnectionsAccountLiabilityAllOfAprs'] = FinancialConnectionsAccountLiabilityAllOfAprs
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+    from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
     globals()['FinancialConnectionsAccountLiabilityAllOfAprs'] = FinancialConnectionsAccountLiabilityAllOfAprs
 
 
 class FinancialConnectionsAccountLiabilityAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of_aprs.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of_aprs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsAccountLiabilityAllOfAprs(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_holding.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_holding.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+    from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
     globals()['FinancialConnectionsInvestmentSecurity'] = FinancialConnectionsInvestmentSecurity
 
 
 class FinancialConnectionsHolding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.currency import Currency
-    from fuse-client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
+    from fuse_client.model.currency import Currency
+    from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
     globals()['Currency'] = Currency
     globals()['FinancialConnectionsInvestmentSecurityExchange'] = FinancialConnectionsInvestmentSecurityExchange
 
 
 class FinancialConnectionsInvestmentSecurity(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security_exchange.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsInvestmentSecurityExchange(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_investment_transaction.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_investment_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.currency import Currency
-    from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+    from fuse_client.model.currency import Currency
+    from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
     globals()['Currency'] = Currency
     globals()['FinancialConnectionsInvestmentSecurity'] = FinancialConnectionsInvestmentSecurity
 
 
 class FinancialConnectionsInvestmentTransaction(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
-    from fuse-client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
-    from fuse-client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
-    from fuse-client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
+    from fuse_client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
+    from fuse_client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
+    from fuse_client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
+    from fuse_client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
     globals()['FinancialConnectionsOwnerAddresses'] = FinancialConnectionsOwnerAddresses
     globals()['FinancialConnectionsOwnerEmails'] = FinancialConnectionsOwnerEmails
     globals()['FinancialConnectionsOwnerNames'] = FinancialConnectionsOwnerNames
     globals()['FinancialConnectionsOwnerPhoneNumbers'] = FinancialConnectionsOwnerPhoneNumbers
 
 
 class FinancialConnectionsOwner(ModelNormal):
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner_addresses.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner_addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
+    from fuse_client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
     globals()['FinancialConnectionsOwnerData'] = FinancialConnectionsOwnerData
 
 
 class FinancialConnectionsOwnerAddresses(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner_data.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsOwnerData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner_emails.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner_emails.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsOwnerEmails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner_names.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsOwnerNames(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_connections_owner_phone_numbers.py` & `fuse-client-1.0.7/fuse_client/model/financial_connections_owner_phone_numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialConnectionsOwnerPhoneNumbers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_institution.py` & `fuse-client-1.0.7/fuse_client/model/financial_institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.country_code import CountryCode
-    from fuse-client.model.financial_institution_logo import FinancialInstitutionLogo
+    from fuse_client.model.country_code import CountryCode
+    from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
     globals()['CountryCode'] = CountryCode
     globals()['FinancialInstitutionLogo'] = FinancialInstitutionLogo
 
 
 class FinancialInstitution(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/financial_institution_logo.py` & `fuse-client-1.0.7/fuse_client/model/financial_institution_logo.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FinancialInstitutionLogo(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/fuse_api_error.py` & `fuse-client-1.0.7/fuse_client/model/fuse_api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.fuse_api_error_data import FuseApiErrorData
+    from fuse_client.model.fuse_api_error_data import FuseApiErrorData
     globals()['FuseApiErrorData'] = FuseApiErrorData
 
 
 class FuseApiError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/fuse_api_error_data.py` & `fuse-client-1.0.7/fuse_client/model/fuse_api_error_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
-    from fuse-client.model.fuse_api_error import FuseApiError
+    from fuse_client.model.aggregator import Aggregator
+    from fuse_client.model.fuse_api_error import FuseApiError
     globals()['Aggregator'] = Aggregator
     globals()['FuseApiError'] = FuseApiError
 
 
 class FuseApiErrorData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/fuse_api_warning.py` & `fuse-client-1.0.7/fuse_client/model/fuse_api_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.fuse_api_warning_data import FuseApiWarningData
+    from fuse_client.model.fuse_api_warning_data import FuseApiWarningData
     globals()['FuseApiWarningData'] = FuseApiWarningData
 
 
 class FuseApiWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data.py` & `fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
-    from fuse-client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
+    from fuse_client.model.aggregator import Aggregator
+    from fuse_client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
     globals()['Aggregator'] = Aggregator
     globals()['FuseApiWarningDataWarnings'] = FuseApiWarningDataWarnings
 
 
 class FuseApiWarningData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data_warnings.py` & `fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data_warnings.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class FuseApiWarningDataWarnings(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_request.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetAssetReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_response.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.get_asset_report_response_report import GetAssetReportResponseReport
+    from fuse_client.model.get_asset_report_response_report import GetAssetReportResponseReport
     globals()['GetAssetReportResponseReport'] = GetAssetReportResponseReport
 
 
 class GetAssetReportResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.fuse_api_warning import FuseApiWarning
-    from fuse-client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
+    from fuse_client.model.fuse_api_warning import FuseApiWarning
+    from fuse_client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
     globals()['FuseApiWarning'] = FuseApiWarning
     globals()['GetAssetReportResponseReportAccounts'] = GetAssetReportResponseReportAccounts
 
 
 class GetAssetReportResponseReport(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_accounts.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
-    from fuse-client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
-    from fuse-client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
+    from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
+    from fuse_client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
+    from fuse_client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
     globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
     globals()['GetAssetReportResponseReportBalances'] = GetAssetReportResponseReportBalances
     globals()['GetAssetReportResponseReportHistoricalBalances'] = GetAssetReportResponseReportHistoricalBalances
 
 
 class GetAssetReportResponseReportAccounts(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_balances.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_balances.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetAssetReportResponseReportBalances(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_historical_balances.py` & `fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_historical_balances.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetAssetReportResponseReportHistoricalBalances(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_entity_response.py` & `fuse-client-1.0.7/fuse_client/model/get_entity_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
-    from fuse-client.model.financial_connection_details import FinancialConnectionDetails
+    from fuse_client.model.aggregator import Aggregator
+    from fuse_client.model.financial_connection_details import FinancialConnectionDetails
     globals()['Aggregator'] = Aggregator
     globals()['FinancialConnectionDetails'] = FinancialConnectionDetails
 
 
 class GetEntityResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connection_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connection_details import FinancialConnectionDetails
+    from fuse_client.model.financial_connection_details import FinancialConnectionDetails
     globals()['FinancialConnectionDetails'] = FinancialConnectionDetails
 
 
 class GetFinancialConnectionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_request.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetFinancialConnectionsAccountDetailsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connection_data import FinancialConnectionData
-    from fuse-client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
+    from fuse_client.model.financial_connection_data import FinancialConnectionData
+    from fuse_client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
     globals()['FinancialConnectionData'] = FinancialConnectionData
     globals()['FinancialConnectionsAccountDetails'] = FinancialConnectionsAccountDetails
 
 
 class GetFinancialConnectionsAccountDetailsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_request.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetFinancialConnectionsAccountsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connection_data import FinancialConnectionData
-    from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+    from fuse_client.model.financial_connection_data import FinancialConnectionData
+    from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
     globals()['FinancialConnectionData'] = FinancialConnectionData
     globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
 
 
 class GetFinancialConnectionsAccountsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
+    from fuse_client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
     globals()['GetFinancialConnectionsBalanceRequestOptions'] = GetFinancialConnectionsBalanceRequestOptions
 
 
 class GetFinancialConnectionsBalanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request_options.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetFinancialConnectionsBalanceRequestOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+    from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
     globals()['FinancialConnectionsAccountBalance'] = FinancialConnectionsAccountBalance
 
 
 class GetFinancialConnectionsBalanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_request.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetFinancialConnectionsOwnersRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
+    from fuse_client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
     globals()['GetFinancialConnectionsOwnersResponseAccounts'] = GetFinancialConnectionsOwnersResponseAccounts
 
 
 class GetFinancialConnectionsOwnersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response_accounts.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
+    from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
     globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
 
 
 class GetFinancialConnectionsOwnersResponseAccounts(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_request.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetFinancialConnectionsTransactionsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.transaction import Transaction
+    from fuse_client.model.transaction import Transaction
     globals()['Transaction'] = Transaction
 
 
 class GetFinancialConnectionsTransactionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_financial_institution_response.py` & `fuse-client-1.0.7/fuse_client/model/get_financial_institution_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_institution import FinancialInstitution
+    from fuse_client.model.financial_institution import FinancialInstitution
     globals()['FinancialInstitution'] = FinancialInstitution
 
 
 class GetFinancialInstitutionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
+    from fuse_client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
     globals()['GetInvestmentHoldingsRequestOptions'] = GetInvestmentHoldingsRequestOptions
 
 
 class GetInvestmentHoldingsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request_options.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetInvestmentHoldingsRequestOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_holdings_response.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_holdings_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-    from fuse-client.model.financial_connections_holding import FinancialConnectionsHolding
+    from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+    from fuse_client.model.financial_connections_holding import FinancialConnectionsHolding
     globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
     globals()['FinancialConnectionsHolding'] = FinancialConnectionsHolding
 
 
 class GetInvestmentHoldingsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
+    from fuse_client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
     globals()['GetInvestmentTransactionsRequestOptions'] = GetInvestmentTransactionsRequestOptions
 
 
 class GetInvestmentTransactionsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request_options.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetInvestmentTransactionsRequestOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_investment_transactions_response.py` & `fuse-client-1.0.7/fuse_client/model/get_investment_transactions_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-    from fuse-client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
+    from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+    from fuse_client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
     globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
     globals()['FinancialConnectionsInvestmentTransaction'] = FinancialConnectionsInvestmentTransaction
 
 
 class GetInvestmentTransactionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_liabilities_request.py` & `fuse-client-1.0.7/fuse_client/model/get_liabilities_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class GetLiabilitiesRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/get_liabilities_response.py` & `fuse-client-1.0.7/fuse_client/model/get_liabilities_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
+    from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
     globals()['FinancialConnectionsAccountLiability'] = FinancialConnectionsAccountLiability
 
 
 class GetLiabilitiesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
-    from fuse-client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
+    from fuse_client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
+    from fuse_client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
     globals()['MigrateFinancialConnectionsAggregatorConnectionDataMx'] = MigrateFinancialConnectionsAggregatorConnectionDataMx
     globals()['MigrateFinancialConnectionsAggregatorConnectionDataPlaid'] = MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 
 
 class MigrateFinancialConnectionsAggregatorConnectionData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_mx.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_mx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class MigrateFinancialConnectionsAggregatorConnectionDataMx(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_plaid.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_plaid.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class MigrateFinancialConnectionsAggregatorConnectionDataPlaid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-    from fuse-client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
-    from fuse-client.model.product import Product
+    from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+    from fuse_client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
+    from fuse_client.model.product import Product
     globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
     globals()['MigrateFinancialConnectionsTokenRequestEntity'] = MigrateFinancialConnectionsTokenRequestEntity
     globals()['Product'] = Product
 
 
 class MigrateFinancialConnectionsTokenRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request_entity.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class MigrateFinancialConnectionsTokenRequestEntity(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_response.py` & `fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+    from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
     globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
 
 
 class MigrateFinancialConnectionsTokenResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/product.py` & `fuse-client-1.0.7/fuse_client/model/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class Product(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/refresh_asset_report_request.py` & `fuse-client-1.0.7/fuse_client/model/refresh_asset_report_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class RefreshAssetReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/sync_financial_connections_data_response.py` & `fuse-client-1.0.7/fuse_client/model/sync_financial_connections_data_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class SyncFinancialConnectionsDataResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/sync_transactions_request.py` & `fuse-client-1.0.7/fuse_client/model/sync_transactions_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class SyncTransactionsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/sync_transactions_response.py` & `fuse-client-1.0.7/fuse_client/model/sync_transactions_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
-    from fuse-client.model.transaction import Transaction
+    from fuse_client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
+    from fuse_client.model.transaction import Transaction
     globals()['SyncTransactionsResponseRemoved'] = SyncTransactionsResponseRemoved
     globals()['Transaction'] = Transaction
 
 
 class SyncTransactionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/sync_transactions_response_removed.py` & `fuse-client-1.0.7/fuse_client/model/sync_transactions_response_removed.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class SyncTransactionsResponseRemoved(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/transaction.py` & `fuse-client-1.0.7/fuse_client/model/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.transaction_merchant import TransactionMerchant
+    from fuse_client.model.transaction_merchant import TransactionMerchant
     globals()['TransactionMerchant'] = TransactionMerchant
 
 
 class Transaction(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/transaction_merchant.py` & `fuse-client-1.0.7/fuse_client/model/transaction_merchant.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class TransactionMerchant(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/update_entity_request.py` & `fuse-client-1.0.7/fuse_client/model/update_entity_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
+    from fuse_client.model.aggregator import Aggregator
     globals()['Aggregator'] = Aggregator
 
 
 class UpdateEntityRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/update_entity_response.py` & `fuse-client-1.0.7/fuse_client/model/update_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.aggregator import Aggregator
+    from fuse_client.model.aggregator import Aggregator
     globals()['Aggregator'] = Aggregator
 
 
 class UpdateEntityResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/webhook_event.py` & `fuse-client-1.0.7/fuse_client/model/webhook_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fuse-client.model.webhook_source import WebhookSource
-    from fuse-client.model.webhook_type import WebhookType
+    from fuse_client.model.webhook_source import WebhookSource
+    from fuse_client.model.webhook_type import WebhookType
     globals()['WebhookSource'] = WebhookSource
     globals()['WebhookType'] = WebhookType
 
 
 class WebhookEvent(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/webhook_source.py` & `fuse-client-1.0.7/fuse_client/model/webhook_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class WebhookSource(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model/webhook_type.py` & `fuse-client-1.0.7/fuse_client/model/webhook_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from fuse-client.model_utils import (  # noqa: F401
+from fuse_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from fuse-client.exceptions import ApiAttributeError
+from fuse_client.exceptions import ApiAttributeError
 
 
 
 class WebhookType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `fuse-client-1.0.6/fuse-client/model_utils.py` & `fuse-client-1.0.7/fuse_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import pprint
 import re
 import tempfile
 
 from dateutil.parser import parse
 
-from fuse-client.exceptions import (
+from fuse_client.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `fuse-client-1.0.6/fuse-client/rest.py` & `fuse-client-1.0.7/fuse_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 import re
 import ssl
 from urllib.parse import urlencode
 
 import urllib3
 
-from fuse-client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from fuse_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `fuse-client-1.0.6/fuse_client.egg-info/SOURCES.txt` & `fuse-client-1.0.7/fuse_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-fuse-client/__init__.py
-fuse-client/api_client.py
-fuse-client/configuration.py
-fuse-client/exceptions.py
-fuse-client/model_utils.py
-fuse-client/rest.py
-fuse-client/api/__init__.py
-fuse-client/api/fuse_api.py
-fuse-client/apis/__init__.py
-fuse-client/model/__init__.py
-fuse-client/model/account_subtype.py
-fuse-client/model/account_type.py
-fuse-client/model/aggregator.py
-fuse-client/model/country_code.py
-fuse-client/model/create_asset_report_request.py
-fuse-client/model/create_asset_report_response.py
-fuse-client/model/create_entity_request.py
-fuse-client/model/create_entity_response.py
-fuse-client/model/create_link_token_request.py
-fuse-client/model/create_link_token_request_mx.py
-fuse-client/model/create_link_token_request_plaid.py
-fuse-client/model/create_link_token_response.py
-fuse-client/model/create_session_request.py
-fuse-client/model/create_session_response.py
-fuse-client/model/currency.py
-fuse-client/model/delete_financial_connection_response.py
-fuse-client/model/entity.py
-fuse-client/model/exchange_financial_connections_public_token_request.py
-fuse-client/model/exchange_financial_connections_public_token_response.py
-fuse-client/model/financial_connection_data.py
-fuse-client/model/financial_connection_details.py
-fuse-client/model/financial_connection_details_mx.py
-fuse-client/model/financial_connection_details_plaid.py
-fuse-client/model/financial_connection_details_teller.py
-fuse-client/model/financial_connections_account.py
-fuse-client/model/financial_connections_account_balance.py
-fuse-client/model/financial_connections_account_cached_balance.py
-fuse-client/model/financial_connections_account_details.py
-fuse-client/model/financial_connections_account_details_ach.py
-fuse-client/model/financial_connections_account_institution.py
-fuse-client/model/financial_connections_account_liability.py
-fuse-client/model/financial_connections_account_liability_all_of.py
-fuse-client/model/financial_connections_account_liability_all_of_aprs.py
-fuse-client/model/financial_connections_holding.py
-fuse-client/model/financial_connections_investment_security.py
-fuse-client/model/financial_connections_investment_security_exchange.py
-fuse-client/model/financial_connections_investment_transaction.py
-fuse-client/model/financial_connections_owner.py
-fuse-client/model/financial_connections_owner_addresses.py
-fuse-client/model/financial_connections_owner_data.py
-fuse-client/model/financial_connections_owner_emails.py
-fuse-client/model/financial_connections_owner_names.py
-fuse-client/model/financial_connections_owner_phone_numbers.py
-fuse-client/model/financial_institution.py
-fuse-client/model/financial_institution_logo.py
-fuse-client/model/fuse_api_error.py
-fuse-client/model/fuse_api_error_data.py
-fuse-client/model/fuse_api_warning.py
-fuse-client/model/fuse_api_warning_data.py
-fuse-client/model/fuse_api_warning_data_warnings.py
-fuse-client/model/get_asset_report_request.py
-fuse-client/model/get_asset_report_response.py
-fuse-client/model/get_asset_report_response_report.py
-fuse-client/model/get_asset_report_response_report_accounts.py
-fuse-client/model/get_asset_report_response_report_balances.py
-fuse-client/model/get_asset_report_response_report_historical_balances.py
-fuse-client/model/get_entity_response.py
-fuse-client/model/get_financial_connection_response.py
-fuse-client/model/get_financial_connections_account_details_request.py
-fuse-client/model/get_financial_connections_account_details_response.py
-fuse-client/model/get_financial_connections_accounts_request.py
-fuse-client/model/get_financial_connections_accounts_response.py
-fuse-client/model/get_financial_connections_balance_request.py
-fuse-client/model/get_financial_connections_balance_request_options.py
-fuse-client/model/get_financial_connections_balance_response.py
-fuse-client/model/get_financial_connections_owners_request.py
-fuse-client/model/get_financial_connections_owners_response.py
-fuse-client/model/get_financial_connections_owners_response_accounts.py
-fuse-client/model/get_financial_connections_transactions_request.py
-fuse-client/model/get_financial_connections_transactions_response.py
-fuse-client/model/get_financial_institution_response.py
-fuse-client/model/get_investment_holdings_request.py
-fuse-client/model/get_investment_holdings_request_options.py
-fuse-client/model/get_investment_holdings_response.py
-fuse-client/model/get_investment_transactions_request.py
-fuse-client/model/get_investment_transactions_request_options.py
-fuse-client/model/get_investment_transactions_response.py
-fuse-client/model/get_liabilities_request.py
-fuse-client/model/get_liabilities_response.py
-fuse-client/model/migrate_financial_connections_aggregator_connection_data.py
-fuse-client/model/migrate_financial_connections_aggregator_connection_data_mx.py
-fuse-client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
-fuse-client/model/migrate_financial_connections_token_request.py
-fuse-client/model/migrate_financial_connections_token_request_entity.py
-fuse-client/model/migrate_financial_connections_token_response.py
-fuse-client/model/product.py
-fuse-client/model/refresh_asset_report_request.py
-fuse-client/model/sync_financial_connections_data_response.py
-fuse-client/model/sync_transactions_request.py
-fuse-client/model/sync_transactions_response.py
-fuse-client/model/sync_transactions_response_removed.py
-fuse-client/model/transaction.py
-fuse-client/model/transaction_merchant.py
-fuse-client/model/update_entity_request.py
-fuse-client/model/update_entity_response.py
-fuse-client/model/webhook_event.py
-fuse-client/model/webhook_source.py
-fuse-client/model/webhook_type.py
-fuse-client/models/__init__.py
+fuse_client/__init__.py
+fuse_client/api_client.py
+fuse_client/configuration.py
+fuse_client/exceptions.py
+fuse_client/model_utils.py
+fuse_client/rest.py
 fuse_client.egg-info/PKG-INFO
 fuse_client.egg-info/SOURCES.txt
 fuse_client.egg-info/dependency_links.txt
 fuse_client.egg-info/requires.txt
 fuse_client.egg-info/top_level.txt
+fuse_client/api/__init__.py
+fuse_client/api/fuse_api.py
+fuse_client/apis/__init__.py
+fuse_client/model/__init__.py
+fuse_client/model/account_subtype.py
+fuse_client/model/account_type.py
+fuse_client/model/aggregator.py
+fuse_client/model/country_code.py
+fuse_client/model/create_asset_report_request.py
+fuse_client/model/create_asset_report_response.py
+fuse_client/model/create_entity_request.py
+fuse_client/model/create_entity_response.py
+fuse_client/model/create_link_token_request.py
+fuse_client/model/create_link_token_request_mx.py
+fuse_client/model/create_link_token_request_plaid.py
+fuse_client/model/create_link_token_response.py
+fuse_client/model/create_session_request.py
+fuse_client/model/create_session_response.py
+fuse_client/model/currency.py
+fuse_client/model/delete_financial_connection_response.py
+fuse_client/model/entity.py
+fuse_client/model/exchange_financial_connections_public_token_request.py
+fuse_client/model/exchange_financial_connections_public_token_response.py
+fuse_client/model/financial_connection_data.py
+fuse_client/model/financial_connection_details.py
+fuse_client/model/financial_connection_details_mx.py
+fuse_client/model/financial_connection_details_plaid.py
+fuse_client/model/financial_connection_details_teller.py
+fuse_client/model/financial_connections_account.py
+fuse_client/model/financial_connections_account_balance.py
+fuse_client/model/financial_connections_account_cached_balance.py
+fuse_client/model/financial_connections_account_details.py
+fuse_client/model/financial_connections_account_details_ach.py
+fuse_client/model/financial_connections_account_institution.py
+fuse_client/model/financial_connections_account_liability.py
+fuse_client/model/financial_connections_account_liability_all_of.py
+fuse_client/model/financial_connections_account_liability_all_of_aprs.py
+fuse_client/model/financial_connections_holding.py
+fuse_client/model/financial_connections_investment_security.py
+fuse_client/model/financial_connections_investment_security_exchange.py
+fuse_client/model/financial_connections_investment_transaction.py
+fuse_client/model/financial_connections_owner.py
+fuse_client/model/financial_connections_owner_addresses.py
+fuse_client/model/financial_connections_owner_data.py
+fuse_client/model/financial_connections_owner_emails.py
+fuse_client/model/financial_connections_owner_names.py
+fuse_client/model/financial_connections_owner_phone_numbers.py
+fuse_client/model/financial_institution.py
+fuse_client/model/financial_institution_logo.py
+fuse_client/model/fuse_api_error.py
+fuse_client/model/fuse_api_error_data.py
+fuse_client/model/fuse_api_warning.py
+fuse_client/model/fuse_api_warning_data.py
+fuse_client/model/fuse_api_warning_data_warnings.py
+fuse_client/model/get_asset_report_request.py
+fuse_client/model/get_asset_report_response.py
+fuse_client/model/get_asset_report_response_report.py
+fuse_client/model/get_asset_report_response_report_accounts.py
+fuse_client/model/get_asset_report_response_report_balances.py
+fuse_client/model/get_asset_report_response_report_historical_balances.py
+fuse_client/model/get_entity_response.py
+fuse_client/model/get_financial_connection_response.py
+fuse_client/model/get_financial_connections_account_details_request.py
+fuse_client/model/get_financial_connections_account_details_response.py
+fuse_client/model/get_financial_connections_accounts_request.py
+fuse_client/model/get_financial_connections_accounts_response.py
+fuse_client/model/get_financial_connections_balance_request.py
+fuse_client/model/get_financial_connections_balance_request_options.py
+fuse_client/model/get_financial_connections_balance_response.py
+fuse_client/model/get_financial_connections_owners_request.py
+fuse_client/model/get_financial_connections_owners_response.py
+fuse_client/model/get_financial_connections_owners_response_accounts.py
+fuse_client/model/get_financial_connections_transactions_request.py
+fuse_client/model/get_financial_connections_transactions_response.py
+fuse_client/model/get_financial_institution_response.py
+fuse_client/model/get_investment_holdings_request.py
+fuse_client/model/get_investment_holdings_request_options.py
+fuse_client/model/get_investment_holdings_response.py
+fuse_client/model/get_investment_transactions_request.py
+fuse_client/model/get_investment_transactions_request_options.py
+fuse_client/model/get_investment_transactions_response.py
+fuse_client/model/get_liabilities_request.py
+fuse_client/model/get_liabilities_response.py
+fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
+fuse_client/model/migrate_financial_connections_aggregator_connection_data_mx.py
+fuse_client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
+fuse_client/model/migrate_financial_connections_token_request.py
+fuse_client/model/migrate_financial_connections_token_request_entity.py
+fuse_client/model/migrate_financial_connections_token_response.py
+fuse_client/model/product.py
+fuse_client/model/refresh_asset_report_request.py
+fuse_client/model/sync_financial_connections_data_response.py
+fuse_client/model/sync_transactions_request.py
+fuse_client/model/sync_transactions_response.py
+fuse_client/model/sync_transactions_response_removed.py
+fuse_client/model/transaction.py
+fuse_client/model/transaction_merchant.py
+fuse_client/model/update_entity_request.py
+fuse_client/model/update_entity_response.py
+fuse_client/model/webhook_event.py
+fuse_client/model/webhook_source.py
+fuse_client/model/webhook_type.py
+fuse_client/models/__init__.py
 test/test_account_subtype.py
 test/test_account_type.py
 test/test_aggregator.py
 test/test_country_code.py
 test/test_create_asset_report_request.py
 test/test_create_asset_report_response.py
 test/test_create_entity_request.py
```

### Comparing `fuse-client-1.0.6/setup.py` & `fuse-client-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "fuse-client"
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fuse-client-1.0.6/test/test_account_subtype.py` & `fuse-client-1.0.7/test/test_account_subtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.account_subtype import AccountSubtype
+import fuse_client
+from fuse_client.model.account_subtype import AccountSubtype
 
 
 class TestAccountSubtype(unittest.TestCase):
     """AccountSubtype unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_account_type.py` & `fuse-client-1.0.7/test/test_webhook_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.account_type import AccountType
+import fuse_client
+from fuse_client.model.webhook_type import WebhookType
 
 
-class TestAccountType(unittest.TestCase):
-    """AccountType unit test stubs"""
+class TestWebhookType(unittest.TestCase):
+    """WebhookType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountType(self):
-        """Test AccountType"""
+    def testWebhookType(self):
+        """Test WebhookType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = AccountType()  # noqa: E501
+        # model = WebhookType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_aggregator.py` & `fuse-client-1.0.7/test/test_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
 
 
 class TestAggregator(unittest.TestCase):
     """Aggregator unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_country_code.py` & `fuse-client-1.0.7/test/test_country_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.country_code import CountryCode
+import fuse_client
+from fuse_client.model.country_code import CountryCode
 
 
 class TestCountryCode(unittest.TestCase):
     """CountryCode unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_asset_report_request.py` & `fuse-client-1.0.7/test/test_create_asset_report_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_asset_report_request import CreateAssetReportRequest
+import fuse_client
+from fuse_client.model.create_asset_report_request import CreateAssetReportRequest
 
 
 class TestCreateAssetReportRequest(unittest.TestCase):
     """CreateAssetReportRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_asset_report_response.py` & `fuse-client-1.0.7/test/test_create_asset_report_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_asset_report_response import CreateAssetReportResponse
+import fuse_client
+from fuse_client.model.create_asset_report_response import CreateAssetReportResponse
 
 
 class TestCreateAssetReportResponse(unittest.TestCase):
     """CreateAssetReportResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_entity_request.py` & `fuse-client-1.0.7/test/test_create_entity_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
 globals()['Aggregator'] = Aggregator
-from fuse-client.model.create_entity_request import CreateEntityRequest
+from fuse_client.model.create_entity_request import CreateEntityRequest
 
 
 class TestCreateEntityRequest(unittest.TestCase):
     """CreateEntityRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_entity_response.py` & `fuse-client-1.0.7/test/test_create_entity_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
 globals()['Aggregator'] = Aggregator
-from fuse-client.model.create_entity_response import CreateEntityResponse
+from fuse_client.model.create_entity_response import CreateEntityResponse
 
 
 class TestCreateEntityResponse(unittest.TestCase):
     """CreateEntityResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_link_token_request.py` & `fuse-client-1.0.7/test/test_create_link_token_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
-from fuse-client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
-from fuse-client.model.entity import Entity
+import fuse_client
+from fuse_client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
+from fuse_client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
+from fuse_client.model.entity import Entity
 globals()['CreateLinkTokenRequestMx'] = CreateLinkTokenRequestMx
 globals()['CreateLinkTokenRequestPlaid'] = CreateLinkTokenRequestPlaid
 globals()['Entity'] = Entity
-from fuse-client.model.create_link_token_request import CreateLinkTokenRequest
+from fuse_client.model.create_link_token_request import CreateLinkTokenRequest
 
 
 class TestCreateLinkTokenRequest(unittest.TestCase):
     """CreateLinkTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_link_token_request_mx.py` & `fuse-client-1.0.7/test/test_create_link_token_request_mx.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
+import fuse_client
+from fuse_client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
 
 
 class TestCreateLinkTokenRequestMx(unittest.TestCase):
     """CreateLinkTokenRequestMx unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_link_token_request_plaid.py` & `fuse-client-1.0.7/test/test_create_link_token_request_plaid.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
+import fuse_client
+from fuse_client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
 
 
 class TestCreateLinkTokenRequestPlaid(unittest.TestCase):
     """CreateLinkTokenRequestPlaid unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_link_token_response.py` & `fuse-client-1.0.7/test/test_create_link_token_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_link_token_response import CreateLinkTokenResponse
+import fuse_client
+from fuse_client.model.create_link_token_response import CreateLinkTokenResponse
 
 
 class TestCreateLinkTokenResponse(unittest.TestCase):
     """CreateLinkTokenResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_session_request.py` & `fuse-client-1.0.7/test/test_create_session_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
-from fuse-client.model.country_code import CountryCode
-from fuse-client.model.entity import Entity
-from fuse-client.model.product import Product
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+from fuse_client.model.country_code import CountryCode
+from fuse_client.model.entity import Entity
+from fuse_client.model.product import Product
 globals()['Aggregator'] = Aggregator
 globals()['CountryCode'] = CountryCode
 globals()['Entity'] = Entity
 globals()['Product'] = Product
-from fuse-client.model.create_session_request import CreateSessionRequest
+from fuse_client.model.create_session_request import CreateSessionRequest
 
 
 class TestCreateSessionRequest(unittest.TestCase):
     """CreateSessionRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_create_session_response.py` & `fuse-client-1.0.7/test/test_create_session_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.create_session_response import CreateSessionResponse
+import fuse_client
+from fuse_client.model.create_session_response import CreateSessionResponse
 
 
 class TestCreateSessionResponse(unittest.TestCase):
     """CreateSessionResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_currency.py` & `fuse-client-1.0.7/test/test_currency.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.currency import Currency
+import fuse_client
+from fuse_client.model.currency import Currency
 
 
 class TestCurrency(unittest.TestCase):
     """Currency unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_delete_financial_connection_response.py` & `fuse-client-1.0.7/test/test_delete_financial_connection_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
+import fuse_client
+from fuse_client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
 
 
 class TestDeleteFinancialConnectionResponse(unittest.TestCase):
     """DeleteFinancialConnectionResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_entity.py` & `fuse-client-1.0.7/test/test_financial_connections_owner_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.entity import Entity
+import fuse_client
+from fuse_client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
 
 
-class TestEntity(unittest.TestCase):
-    """Entity unit test stubs"""
+class TestFinancialConnectionsOwnerData(unittest.TestCase):
+    """FinancialConnectionsOwnerData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEntity(self):
-        """Test Entity"""
+    def testFinancialConnectionsOwnerData(self):
+        """Test FinancialConnectionsOwnerData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Entity()  # noqa: E501
+        # model = FinancialConnectionsOwnerData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
+import fuse_client
+from fuse_client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
 
 
 class TestExchangeFinancialConnectionsPublicTokenRequest(unittest.TestCase):
     """ExchangeFinancialConnectionsPublicTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_response.py` & `fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
+import fuse_client
+from fuse_client.model.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
 
 
 class TestExchangeFinancialConnectionsPublicTokenResponse(unittest.TestCase):
     """ExchangeFinancialConnectionsPublicTokenResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connection_data.py` & `fuse-client-1.0.7/test/test_financial_connection_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_data import FinancialConnectionData
+import fuse_client
+from fuse_client.model.financial_connection_data import FinancialConnectionData
 
 
 class TestFinancialConnectionData(unittest.TestCase):
     """FinancialConnectionData unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connection_details.py` & `fuse-client-1.0.7/test/test_financial_connection_details.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
-from fuse-client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
-from fuse-client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
-from fuse-client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+from fuse_client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
+from fuse_client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
+from fuse_client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
 globals()['Aggregator'] = Aggregator
 globals()['FinancialConnectionDetailsMx'] = FinancialConnectionDetailsMx
 globals()['FinancialConnectionDetailsPlaid'] = FinancialConnectionDetailsPlaid
 globals()['FinancialConnectionDetailsTeller'] = FinancialConnectionDetailsTeller
-from fuse-client.model.financial_connection_details import FinancialConnectionDetails
+from fuse_client.model.financial_connection_details import FinancialConnectionDetails
 
 
 class TestFinancialConnectionDetails(unittest.TestCase):
     """FinancialConnectionDetails unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connection_details_mx.py` & `fuse-client-1.0.7/test/test_financial_connection_details_mx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
+import fuse_client
+from fuse_client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
 
 
 class TestFinancialConnectionDetailsMx(unittest.TestCase):
     """FinancialConnectionDetailsMx unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connection_details_plaid.py` & `fuse-client-1.0.7/test/test_financial_connection_details_plaid.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
+import fuse_client
+from fuse_client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
 
 
 class TestFinancialConnectionDetailsPlaid(unittest.TestCase):
     """FinancialConnectionDetailsPlaid unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connection_details_teller.py` & `fuse-client-1.0.7/test/test_financial_connection_details_teller.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
+import fuse_client
+from fuse_client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
 
 
 class TestFinancialConnectionDetailsTeller(unittest.TestCase):
     """FinancialConnectionDetailsTeller unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account.py` & `fuse-client-1.0.7/test/test_financial_connections_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.account_subtype import AccountSubtype
-from fuse-client.model.account_type import AccountType
-from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+import fuse_client
+from fuse_client.model.account_subtype import AccountSubtype
+from fuse_client.model.account_type import AccountType
+from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
 globals()['AccountSubtype'] = AccountSubtype
 globals()['AccountType'] = AccountType
 globals()['FinancialConnectionsAccountCachedBalance'] = FinancialConnectionsAccountCachedBalance
 globals()['FinancialConnectionsAccountInstitution'] = FinancialConnectionsAccountInstitution
-from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
 
 
 class TestFinancialConnectionsAccount(unittest.TestCase):
     """FinancialConnectionsAccount unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_balance.py` & `fuse-client-1.0.7/test/test_financial_connections_account_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+import fuse_client
+from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
 
 
 class TestFinancialConnectionsAccountBalance(unittest.TestCase):
     """FinancialConnectionsAccountBalance unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_cached_balance.py` & `fuse-client-1.0.7/test/test_financial_connections_account_cached_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+import fuse_client
+from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
 
 
 class TestFinancialConnectionsAccountCachedBalance(unittest.TestCase):
     """FinancialConnectionsAccountCachedBalance unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_details.py` & `fuse-client-1.0.7/test/test_financial_connections_account_details_ach.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
-globals()['FinancialConnectionsAccountDetailsAch'] = FinancialConnectionsAccountDetailsAch
-from fuse-client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
+import fuse_client
+from fuse_client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
 
 
-class TestFinancialConnectionsAccountDetails(unittest.TestCase):
-    """FinancialConnectionsAccountDetails unit test stubs"""
+class TestFinancialConnectionsAccountDetailsAch(unittest.TestCase):
+    """FinancialConnectionsAccountDetailsAch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionsAccountDetails(self):
-        """Test FinancialConnectionsAccountDetails"""
+    def testFinancialConnectionsAccountDetailsAch(self):
+        """Test FinancialConnectionsAccountDetailsAch"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountDetails()  # noqa: E501
+        # model = FinancialConnectionsAccountDetailsAch()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_details_ach.py` & `fuse-client-1.0.7/test/test_get_financial_connections_account_details_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
+import fuse_client
+from fuse_client.model.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
 
 
-class TestFinancialConnectionsAccountDetailsAch(unittest.TestCase):
-    """FinancialConnectionsAccountDetailsAch unit test stubs"""
+class TestGetFinancialConnectionsAccountDetailsRequest(unittest.TestCase):
+    """GetFinancialConnectionsAccountDetailsRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionsAccountDetailsAch(self):
-        """Test FinancialConnectionsAccountDetailsAch"""
+    def testGetFinancialConnectionsAccountDetailsRequest(self):
+        """Test GetFinancialConnectionsAccountDetailsRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountDetailsAch()  # noqa: E501
+        # model = GetFinancialConnectionsAccountDetailsRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_institution.py` & `fuse-client-1.0.7/test/test_financial_connections_account_institution.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+import fuse_client
+from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
 
 
 class TestFinancialConnectionsAccountInstitution(unittest.TestCase):
     """FinancialConnectionsAccountInstitution unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_liability.py` & `fuse-client-1.0.7/test/test_financial_connections_account_liability.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.account_subtype import AccountSubtype
-from fuse-client.model.account_type import AccountType
-from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
-from fuse-client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
-from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+import fuse_client
+from fuse_client.model.account_subtype import AccountSubtype
+from fuse_client.model.account_type import AccountType
+from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+from fuse_client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
+from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 globals()['AccountSubtype'] = AccountSubtype
 globals()['AccountType'] = AccountType
 globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
 globals()['FinancialConnectionsAccountCachedBalance'] = FinancialConnectionsAccountCachedBalance
 globals()['FinancialConnectionsAccountInstitution'] = FinancialConnectionsAccountInstitution
 globals()['FinancialConnectionsAccountLiabilityAllOf'] = FinancialConnectionsAccountLiabilityAllOf
 globals()['FinancialConnectionsAccountLiabilityAllOfAprs'] = FinancialConnectionsAccountLiabilityAllOfAprs
-from fuse-client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
+from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
 
 
 class TestFinancialConnectionsAccountLiability(unittest.TestCase):
     """FinancialConnectionsAccountLiability unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of.py` & `fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+import fuse_client
+from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 globals()['FinancialConnectionsAccountLiabilityAllOfAprs'] = FinancialConnectionsAccountLiabilityAllOfAprs
-from fuse-client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
+from fuse_client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
 
 
 class TestFinancialConnectionsAccountLiabilityAllOf(unittest.TestCase):
     """FinancialConnectionsAccountLiabilityAllOf unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of_aprs.py` & `fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of_aprs.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+import fuse_client
+from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 
 
 class TestFinancialConnectionsAccountLiabilityAllOfAprs(unittest.TestCase):
     """FinancialConnectionsAccountLiabilityAllOfAprs unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_holding.py` & `fuse-client-1.0.7/test/test_financial_connections_holding.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+import fuse_client
+from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 globals()['FinancialConnectionsInvestmentSecurity'] = FinancialConnectionsInvestmentSecurity
-from fuse-client.model.financial_connections_holding import FinancialConnectionsHolding
+from fuse_client.model.financial_connections_holding import FinancialConnectionsHolding
 
 
 class TestFinancialConnectionsHolding(unittest.TestCase):
     """FinancialConnectionsHolding unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_investment_security.py` & `fuse-client-1.0.7/test/test_financial_connections_investment_security.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.currency import Currency
-from fuse-client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
+import fuse_client
+from fuse_client.model.currency import Currency
+from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
 globals()['Currency'] = Currency
 globals()['FinancialConnectionsInvestmentSecurityExchange'] = FinancialConnectionsInvestmentSecurityExchange
-from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 
 
 class TestFinancialConnectionsInvestmentSecurity(unittest.TestCase):
     """FinancialConnectionsInvestmentSecurity unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_investment_security_exchange.py` & `fuse-client-1.0.7/test/test_financial_connections_investment_security_exchange.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
+import fuse_client
+from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
 
 
 class TestFinancialConnectionsInvestmentSecurityExchange(unittest.TestCase):
     """FinancialConnectionsInvestmentSecurityExchange unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_investment_transaction.py` & `fuse-client-1.0.7/test/test_financial_connections_investment_transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.currency import Currency
-from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+import fuse_client
+from fuse_client.model.currency import Currency
+from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 globals()['Currency'] = Currency
 globals()['FinancialConnectionsInvestmentSecurity'] = FinancialConnectionsInvestmentSecurity
-from fuse-client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
+from fuse_client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
 
 
 class TestFinancialConnectionsInvestmentTransaction(unittest.TestCase):
     """FinancialConnectionsInvestmentTransaction unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner.py` & `fuse-client-1.0.7/test/test_financial_connections_owner.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
-from fuse-client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
-from fuse-client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
-from fuse-client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
+import fuse_client
+from fuse_client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
+from fuse_client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
+from fuse_client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
+from fuse_client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
 globals()['FinancialConnectionsOwnerAddresses'] = FinancialConnectionsOwnerAddresses
 globals()['FinancialConnectionsOwnerEmails'] = FinancialConnectionsOwnerEmails
 globals()['FinancialConnectionsOwnerNames'] = FinancialConnectionsOwnerNames
 globals()['FinancialConnectionsOwnerPhoneNumbers'] = FinancialConnectionsOwnerPhoneNumbers
-from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
+from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
 
 
 class TestFinancialConnectionsOwner(unittest.TestCase):
     """FinancialConnectionsOwner unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner_addresses.py` & `fuse-client-1.0.7/test/test_financial_connections_owner_addresses.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
+import fuse_client
+from fuse_client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
 globals()['FinancialConnectionsOwnerData'] = FinancialConnectionsOwnerData
-from fuse-client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
+from fuse_client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
 
 
 class TestFinancialConnectionsOwnerAddresses(unittest.TestCase):
     """FinancialConnectionsOwnerAddresses unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner_data.py` & `fuse-client-1.0.7/test/test_get_financial_connections_accounts_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
+import fuse_client
+from fuse_client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
 
 
-class TestFinancialConnectionsOwnerData(unittest.TestCase):
-    """FinancialConnectionsOwnerData unit test stubs"""
+class TestGetFinancialConnectionsAccountsRequest(unittest.TestCase):
+    """GetFinancialConnectionsAccountsRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionsOwnerData(self):
-        """Test FinancialConnectionsOwnerData"""
+    def testGetFinancialConnectionsAccountsRequest(self):
+        """Test GetFinancialConnectionsAccountsRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsOwnerData()  # noqa: E501
+        # model = GetFinancialConnectionsAccountsRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner_emails.py` & `fuse-client-1.0.7/test/test_financial_connections_owner_emails.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
+import fuse_client
+from fuse_client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
 
 
 class TestFinancialConnectionsOwnerEmails(unittest.TestCase):
     """FinancialConnectionsOwnerEmails unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner_names.py` & `fuse-client-1.0.7/test/test_financial_connections_owner_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
+import fuse_client
+from fuse_client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
 
 
 class TestFinancialConnectionsOwnerNames(unittest.TestCase):
     """FinancialConnectionsOwnerNames unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_connections_owner_phone_numbers.py` & `fuse-client-1.0.7/test/test_financial_connections_owner_phone_numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
+import fuse_client
+from fuse_client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
 
 
 class TestFinancialConnectionsOwnerPhoneNumbers(unittest.TestCase):
     """FinancialConnectionsOwnerPhoneNumbers unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_institution.py` & `fuse-client-1.0.7/test/test_financial_institution.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.country_code import CountryCode
-from fuse-client.model.financial_institution_logo import FinancialInstitutionLogo
+import fuse_client
+from fuse_client.model.country_code import CountryCode
+from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
 globals()['CountryCode'] = CountryCode
 globals()['FinancialInstitutionLogo'] = FinancialInstitutionLogo
-from fuse-client.model.financial_institution import FinancialInstitution
+from fuse_client.model.financial_institution import FinancialInstitution
 
 
 class TestFinancialInstitution(unittest.TestCase):
     """FinancialInstitution unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_financial_institution_logo.py` & `fuse-client-1.0.7/test/test_financial_institution_logo.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_institution_logo import FinancialInstitutionLogo
+import fuse_client
+from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
 
 
 class TestFinancialInstitutionLogo(unittest.TestCase):
     """FinancialInstitutionLogo unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api.py` & `fuse-client-1.0.7/test/test_fuse_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
-import fuse-client
-from fuse-client.api.fuse_api import FuseApi  # noqa: E501
+import fuse_client
+from fuse_client.api.fuse_api import FuseApi  # noqa: E501
 
 
 class TestFuseApi(unittest.TestCase):
     """FuseApi unit test stubs"""
 
     def setUp(self):
         self.api = FuseApi()  # noqa: E501
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api_error.py` & `fuse-client-1.0.7/test/test_fuse_api_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.fuse_api_error_data import FuseApiErrorData
+import fuse_client
+from fuse_client.model.fuse_api_error_data import FuseApiErrorData
 globals()['FuseApiErrorData'] = FuseApiErrorData
-from fuse-client.model.fuse_api_error import FuseApiError
+from fuse_client.model.fuse_api_error import FuseApiError
 
 
 class TestFuseApiError(unittest.TestCase):
     """FuseApiError unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api_error_data.py` & `fuse-client-1.0.7/test/test_entity.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,33 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
-from fuse-client.model.fuse_api_error import FuseApiError
-globals()['Aggregator'] = Aggregator
-globals()['FuseApiError'] = FuseApiError
-from fuse-client.model.fuse_api_error_data import FuseApiErrorData
+import fuse_client
+from fuse_client.model.entity import Entity
 
 
-class TestFuseApiErrorData(unittest.TestCase):
-    """FuseApiErrorData unit test stubs"""
+class TestEntity(unittest.TestCase):
+    """Entity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFuseApiErrorData(self):
-        """Test FuseApiErrorData"""
+    def testEntity(self):
+        """Test Entity"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = FuseApiErrorData()  # noqa: E501
+        # model = Entity()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api_warning.py` & `fuse-client-1.0.7/test/test_fuse_api_warning.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.fuse_api_warning_data import FuseApiWarningData
+import fuse_client
+from fuse_client.model.fuse_api_warning_data import FuseApiWarningData
 globals()['FuseApiWarningData'] = FuseApiWarningData
-from fuse-client.model.fuse_api_warning import FuseApiWarning
+from fuse_client.model.fuse_api_warning import FuseApiWarning
 
 
 class TestFuseApiWarning(unittest.TestCase):
     """FuseApiWarning unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api_warning_data.py` & `fuse-client-1.0.7/test/test_fuse_api_warning_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
-from fuse-client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+from fuse_client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
 globals()['Aggregator'] = Aggregator
 globals()['FuseApiWarningDataWarnings'] = FuseApiWarningDataWarnings
-from fuse-client.model.fuse_api_warning_data import FuseApiWarningData
+from fuse_client.model.fuse_api_warning_data import FuseApiWarningData
 
 
 class TestFuseApiWarningData(unittest.TestCase):
     """FuseApiWarningData unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_fuse_api_warning_data_warnings.py` & `fuse-client-1.0.7/test/test_fuse_api_warning_data_warnings.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
+import fuse_client
+from fuse_client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
 
 
 class TestFuseApiWarningDataWarnings(unittest.TestCase):
     """FuseApiWarningDataWarnings unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_request.py` & `fuse-client-1.0.7/test/test_get_asset_report_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_asset_report_request import GetAssetReportRequest
+import fuse_client
+from fuse_client.model.get_asset_report_request import GetAssetReportRequest
 
 
 class TestGetAssetReportRequest(unittest.TestCase):
     """GetAssetReportRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_response.py` & `fuse-client-1.0.7/test/test_refresh_asset_report_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_asset_report_response_report import GetAssetReportResponseReport
-globals()['GetAssetReportResponseReport'] = GetAssetReportResponseReport
-from fuse-client.model.get_asset_report_response import GetAssetReportResponse
+import fuse_client
+from fuse_client.model.refresh_asset_report_request import RefreshAssetReportRequest
 
 
-class TestGetAssetReportResponse(unittest.TestCase):
-    """GetAssetReportResponse unit test stubs"""
+class TestRefreshAssetReportRequest(unittest.TestCase):
+    """RefreshAssetReportRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetAssetReportResponse(self):
-        """Test GetAssetReportResponse"""
+    def testRefreshAssetReportRequest(self):
+        """Test RefreshAssetReportRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetAssetReportResponse()  # noqa: E501
+        # model = RefreshAssetReportRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_response_report.py` & `fuse-client-1.0.7/test/test_get_asset_report_response_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.fuse_api_warning import FuseApiWarning
-from fuse-client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
+import fuse_client
+from fuse_client.model.fuse_api_warning import FuseApiWarning
+from fuse_client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
 globals()['FuseApiWarning'] = FuseApiWarning
 globals()['GetAssetReportResponseReportAccounts'] = GetAssetReportResponseReportAccounts
-from fuse-client.model.get_asset_report_response_report import GetAssetReportResponseReport
+from fuse_client.model.get_asset_report_response_report import GetAssetReportResponseReport
 
 
 class TestGetAssetReportResponseReport(unittest.TestCase):
     """GetAssetReportResponseReport unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_response_report_accounts.py` & `fuse-client-1.0.7/test/test_get_asset_report_response_report_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
-from fuse-client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
-from fuse-client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
+import fuse_client
+from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
+from fuse_client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
+from fuse_client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
 globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
 globals()['GetAssetReportResponseReportBalances'] = GetAssetReportResponseReportBalances
 globals()['GetAssetReportResponseReportHistoricalBalances'] = GetAssetReportResponseReportHistoricalBalances
-from fuse-client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
+from fuse_client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
 
 
 class TestGetAssetReportResponseReportAccounts(unittest.TestCase):
     """GetAssetReportResponseReportAccounts unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_response_report_balances.py` & `fuse-client-1.0.7/test/test_get_asset_report_response_report_balances.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
+import fuse_client
+from fuse_client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
 
 
 class TestGetAssetReportResponseReportBalances(unittest.TestCase):
     """GetAssetReportResponseReportBalances unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_asset_report_response_report_historical_balances.py` & `fuse-client-1.0.7/test/test_get_asset_report_response_report_historical_balances.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
+import fuse_client
+from fuse_client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
 
 
 class TestGetAssetReportResponseReportHistoricalBalances(unittest.TestCase):
     """GetAssetReportResponseReportHistoricalBalances unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_entity_response.py` & `fuse-client-1.0.7/test/test_get_liabilities_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,33 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.aggregator import Aggregator
-from fuse-client.model.financial_connection_details import FinancialConnectionDetails
-globals()['Aggregator'] = Aggregator
-globals()['FinancialConnectionDetails'] = FinancialConnectionDetails
-from fuse-client.model.get_entity_response import GetEntityResponse
+import fuse_client
+from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
+globals()['FinancialConnectionsAccountLiability'] = FinancialConnectionsAccountLiability
+from fuse_client.model.get_liabilities_response import GetLiabilitiesResponse
 
 
-class TestGetEntityResponse(unittest.TestCase):
-    """GetEntityResponse unit test stubs"""
+class TestGetLiabilitiesResponse(unittest.TestCase):
+    """GetLiabilitiesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetEntityResponse(self):
-        """Test GetEntityResponse"""
+    def testGetLiabilitiesResponse(self):
+        """Test GetLiabilitiesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetEntityResponse()  # noqa: E501
+        # model = GetLiabilitiesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connection_response.py` & `fuse-client-1.0.7/test/test_get_financial_connection_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_details import FinancialConnectionDetails
+import fuse_client
+from fuse_client.model.financial_connection_details import FinancialConnectionDetails
 globals()['FinancialConnectionDetails'] = FinancialConnectionDetails
-from fuse-client.model.get_financial_connection_response import GetFinancialConnectionResponse
+from fuse_client.model.get_financial_connection_response import GetFinancialConnectionResponse
 
 
 class TestGetFinancialConnectionResponse(unittest.TestCase):
     """GetFinancialConnectionResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_account_details_request.py` & `fuse-client-1.0.7/test/test_financial_connections_account_details.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
+import fuse_client
+from fuse_client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
+globals()['FinancialConnectionsAccountDetailsAch'] = FinancialConnectionsAccountDetailsAch
+from fuse_client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
 
 
-class TestGetFinancialConnectionsAccountDetailsRequest(unittest.TestCase):
-    """GetFinancialConnectionsAccountDetailsRequest unit test stubs"""
+class TestFinancialConnectionsAccountDetails(unittest.TestCase):
+    """FinancialConnectionsAccountDetails unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetFinancialConnectionsAccountDetailsRequest(self):
-        """Test GetFinancialConnectionsAccountDetailsRequest"""
+    def testFinancialConnectionsAccountDetails(self):
+        """Test FinancialConnectionsAccountDetails"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsAccountDetailsRequest()  # noqa: E501
+        # model = FinancialConnectionsAccountDetails()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_account_details_response.py` & `fuse-client-1.0.7/test/test_get_financial_connections_account_details_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_data import FinancialConnectionData
-from fuse-client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
+import fuse_client
+from fuse_client.model.financial_connection_data import FinancialConnectionData
+from fuse_client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
 globals()['FinancialConnectionData'] = FinancialConnectionData
 globals()['FinancialConnectionsAccountDetails'] = FinancialConnectionsAccountDetails
-from fuse-client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
+from fuse_client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
 
 
 class TestGetFinancialConnectionsAccountDetailsResponse(unittest.TestCase):
     """GetFinancialConnectionsAccountDetailsResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_accounts_request.py` & `fuse-client-1.0.7/test/test_get_financial_connections_owners_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
+import fuse_client
+from fuse_client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
 
 
-class TestGetFinancialConnectionsAccountsRequest(unittest.TestCase):
-    """GetFinancialConnectionsAccountsRequest unit test stubs"""
+class TestGetFinancialConnectionsOwnersRequest(unittest.TestCase):
+    """GetFinancialConnectionsOwnersRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetFinancialConnectionsAccountsRequest(self):
-        """Test GetFinancialConnectionsAccountsRequest"""
+    def testGetFinancialConnectionsOwnersRequest(self):
+        """Test GetFinancialConnectionsOwnersRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsAccountsRequest()  # noqa: E501
+        # model = GetFinancialConnectionsOwnersRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_accounts_response.py` & `fuse-client-1.0.7/test/test_get_financial_connections_accounts_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connection_data import FinancialConnectionData
-from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+import fuse_client
+from fuse_client.model.financial_connection_data import FinancialConnectionData
+from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
 globals()['FinancialConnectionData'] = FinancialConnectionData
 globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
-from fuse-client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
+from fuse_client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
 
 
 class TestGetFinancialConnectionsAccountsResponse(unittest.TestCase):
     """GetFinancialConnectionsAccountsResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_balance_request.py` & `fuse-client-1.0.7/test/test_get_financial_connections_balance_request_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
-globals()['GetFinancialConnectionsBalanceRequestOptions'] = GetFinancialConnectionsBalanceRequestOptions
-from fuse-client.model.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
+import fuse_client
+from fuse_client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
 
 
-class TestGetFinancialConnectionsBalanceRequest(unittest.TestCase):
-    """GetFinancialConnectionsBalanceRequest unit test stubs"""
+class TestGetFinancialConnectionsBalanceRequestOptions(unittest.TestCase):
+    """GetFinancialConnectionsBalanceRequestOptions unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetFinancialConnectionsBalanceRequest(self):
-        """Test GetFinancialConnectionsBalanceRequest"""
+    def testGetFinancialConnectionsBalanceRequestOptions(self):
+        """Test GetFinancialConnectionsBalanceRequestOptions"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsBalanceRequest()  # noqa: E501
+        # model = GetFinancialConnectionsBalanceRequestOptions()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_balance_request_options.py` & `fuse-client-1.0.7/test/test_get_liabilities_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
+import fuse_client
+from fuse_client.model.get_liabilities_request import GetLiabilitiesRequest
 
 
-class TestGetFinancialConnectionsBalanceRequestOptions(unittest.TestCase):
-    """GetFinancialConnectionsBalanceRequestOptions unit test stubs"""
+class TestGetLiabilitiesRequest(unittest.TestCase):
+    """GetLiabilitiesRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetFinancialConnectionsBalanceRequestOptions(self):
-        """Test GetFinancialConnectionsBalanceRequestOptions"""
+    def testGetLiabilitiesRequest(self):
+        """Test GetLiabilitiesRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsBalanceRequestOptions()  # noqa: E501
+        # model = GetLiabilitiesRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_balance_response.py` & `fuse-client-1.0.7/test/test_get_financial_connections_balance_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+import fuse_client
+from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
 globals()['FinancialConnectionsAccountBalance'] = FinancialConnectionsAccountBalance
-from fuse-client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
+from fuse_client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
 
 
 class TestGetFinancialConnectionsBalanceResponse(unittest.TestCase):
     """GetFinancialConnectionsBalanceResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_owners_request.py` & `fuse-client-1.0.7/test/test_get_financial_connections_owners_response_accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
+import fuse_client
+from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
+globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
+from fuse_client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
 
 
-class TestGetFinancialConnectionsOwnersRequest(unittest.TestCase):
-    """GetFinancialConnectionsOwnersRequest unit test stubs"""
+class TestGetFinancialConnectionsOwnersResponseAccounts(unittest.TestCase):
+    """GetFinancialConnectionsOwnersResponseAccounts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetFinancialConnectionsOwnersRequest(self):
-        """Test GetFinancialConnectionsOwnersRequest"""
+    def testGetFinancialConnectionsOwnersResponseAccounts(self):
+        """Test GetFinancialConnectionsOwnersResponseAccounts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsOwnersRequest()  # noqa: E501
+        # model = GetFinancialConnectionsOwnersResponseAccounts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_owners_response.py` & `fuse-client-1.0.7/test/test_get_financial_connections_owners_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
+import fuse_client
+from fuse_client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
 globals()['GetFinancialConnectionsOwnersResponseAccounts'] = GetFinancialConnectionsOwnersResponseAccounts
-from fuse-client.model.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
+from fuse_client.model.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
 
 
 class TestGetFinancialConnectionsOwnersResponse(unittest.TestCase):
     """GetFinancialConnectionsOwnersResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_transactions_request.py` & `fuse-client-1.0.7/test/test_get_financial_connections_transactions_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
+import fuse_client
+from fuse_client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
 
 
 class TestGetFinancialConnectionsTransactionsRequest(unittest.TestCase):
     """GetFinancialConnectionsTransactionsRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_connections_transactions_response.py` & `fuse-client-1.0.7/test/test_get_financial_connections_transactions_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.transaction import Transaction
+import fuse_client
+from fuse_client.model.transaction import Transaction
 globals()['Transaction'] = Transaction
-from fuse-client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
+from fuse_client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
 
 
 class TestGetFinancialConnectionsTransactionsResponse(unittest.TestCase):
     """GetFinancialConnectionsTransactionsResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_financial_institution_response.py` & `fuse-client-1.0.7/test/test_get_financial_institution_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_institution import FinancialInstitution
+import fuse_client
+from fuse_client.model.financial_institution import FinancialInstitution
 globals()['FinancialInstitution'] = FinancialInstitution
-from fuse-client.model.get_financial_institution_response import GetFinancialInstitutionResponse
+from fuse_client.model.get_financial_institution_response import GetFinancialInstitutionResponse
 
 
 class TestGetFinancialInstitutionResponse(unittest.TestCase):
     """GetFinancialInstitutionResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_holdings_request.py` & `fuse-client-1.0.7/test/test_get_investment_holdings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
+import fuse_client
+from fuse_client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 globals()['GetInvestmentHoldingsRequestOptions'] = GetInvestmentHoldingsRequestOptions
-from fuse-client.model.get_investment_holdings_request import GetInvestmentHoldingsRequest
+from fuse_client.model.get_investment_holdings_request import GetInvestmentHoldingsRequest
 
 
 class TestGetInvestmentHoldingsRequest(unittest.TestCase):
     """GetInvestmentHoldingsRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_holdings_request_options.py` & `fuse-client-1.0.7/test/test_get_investment_holdings_request_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
+import fuse_client
+from fuse_client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 
 
 class TestGetInvestmentHoldingsRequestOptions(unittest.TestCase):
     """GetInvestmentHoldingsRequestOptions unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_holdings_response.py` & `fuse-client-1.0.7/test/test_get_investment_transactions_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,33 +7,33 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-from fuse-client.model.financial_connections_holding import FinancialConnectionsHolding
+import fuse_client
+from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
 globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
-globals()['FinancialConnectionsHolding'] = FinancialConnectionsHolding
-from fuse-client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
+globals()['FinancialConnectionsInvestmentTransaction'] = FinancialConnectionsInvestmentTransaction
+from fuse_client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
 
 
-class TestGetInvestmentHoldingsResponse(unittest.TestCase):
-    """GetInvestmentHoldingsResponse unit test stubs"""
+class TestGetInvestmentTransactionsResponse(unittest.TestCase):
+    """GetInvestmentTransactionsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetInvestmentHoldingsResponse(self):
-        """Test GetInvestmentHoldingsResponse"""
+    def testGetInvestmentTransactionsResponse(self):
+        """Test GetInvestmentTransactionsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetInvestmentHoldingsResponse()  # noqa: E501
+        # model = GetInvestmentTransactionsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_transactions_request.py` & `fuse-client-1.0.7/test/test_get_investment_transactions_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
+import fuse_client
+from fuse_client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
 globals()['GetInvestmentTransactionsRequestOptions'] = GetInvestmentTransactionsRequestOptions
-from fuse-client.model.get_investment_transactions_request import GetInvestmentTransactionsRequest
+from fuse_client.model.get_investment_transactions_request import GetInvestmentTransactionsRequest
 
 
 class TestGetInvestmentTransactionsRequest(unittest.TestCase):
     """GetInvestmentTransactionsRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_transactions_request_options.py` & `fuse-client-1.0.7/test/test_get_investment_transactions_request_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
+import fuse_client
+from fuse_client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
 
 
 class TestGetInvestmentTransactionsRequestOptions(unittest.TestCase):
     """GetInvestmentTransactionsRequestOptions unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_get_investment_transactions_response.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_mx.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,33 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
-from fuse-client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
-globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
-globals()['FinancialConnectionsInvestmentTransaction'] = FinancialConnectionsInvestmentTransaction
-from fuse-client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
+import fuse_client
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
 
 
-class TestGetInvestmentTransactionsResponse(unittest.TestCase):
-    """GetInvestmentTransactionsResponse unit test stubs"""
+class TestMigrateFinancialConnectionsAggregatorConnectionDataMx(unittest.TestCase):
+    """MigrateFinancialConnectionsAggregatorConnectionDataMx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetInvestmentTransactionsResponse(self):
-        """Test GetInvestmentTransactionsResponse"""
+    def testMigrateFinancialConnectionsAggregatorConnectionDataMx(self):
+        """Test MigrateFinancialConnectionsAggregatorConnectionDataMx"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetInvestmentTransactionsResponse()  # noqa: E501
+        # model = MigrateFinancialConnectionsAggregatorConnectionDataMx()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_liabilities_request.py` & `fuse-client-1.0.7/test/test_transaction_merchant.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.get_liabilities_request import GetLiabilitiesRequest
+import fuse_client
+from fuse_client.model.transaction_merchant import TransactionMerchant
 
 
-class TestGetLiabilitiesRequest(unittest.TestCase):
-    """GetLiabilitiesRequest unit test stubs"""
+class TestTransactionMerchant(unittest.TestCase):
+    """TransactionMerchant unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetLiabilitiesRequest(self):
-        """Test GetLiabilitiesRequest"""
+    def testTransactionMerchant(self):
+        """Test TransactionMerchant"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetLiabilitiesRequest()  # noqa: E501
+        # model = TransactionMerchant()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_get_liabilities_response.py` & `fuse-client-1.0.7/test/test_update_entity_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
-globals()['FinancialConnectionsAccountLiability'] = FinancialConnectionsAccountLiability
-from fuse-client.model.get_liabilities_response import GetLiabilitiesResponse
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+globals()['Aggregator'] = Aggregator
+from fuse_client.model.update_entity_response import UpdateEntityResponse
 
 
-class TestGetLiabilitiesResponse(unittest.TestCase):
-    """GetLiabilitiesResponse unit test stubs"""
+class TestUpdateEntityResponse(unittest.TestCase):
+    """UpdateEntityResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetLiabilitiesResponse(self):
-        """Test GetLiabilitiesResponse"""
+    def testUpdateEntityResponse(self):
+        """Test UpdateEntityResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GetLiabilitiesResponse()  # noqa: E501
+        # model = UpdateEntityResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
+import fuse_client
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 globals()['MigrateFinancialConnectionsAggregatorConnectionDataMx'] = MigrateFinancialConnectionsAggregatorConnectionDataMx
 globals()['MigrateFinancialConnectionsAggregatorConnectionDataPlaid'] = MigrateFinancialConnectionsAggregatorConnectionDataPlaid
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
 
 
 class TestMigrateFinancialConnectionsAggregatorConnectionData(unittest.TestCase):
     """MigrateFinancialConnectionsAggregatorConnectionData unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_mx.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
+import fuse_client
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 
 
-class TestMigrateFinancialConnectionsAggregatorConnectionDataMx(unittest.TestCase):
-    """MigrateFinancialConnectionsAggregatorConnectionDataMx unit test stubs"""
+class TestMigrateFinancialConnectionsAggregatorConnectionDataPlaid(unittest.TestCase):
+    """MigrateFinancialConnectionsAggregatorConnectionDataPlaid unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMigrateFinancialConnectionsAggregatorConnectionDataMx(self):
-        """Test MigrateFinancialConnectionsAggregatorConnectionDataMx"""
+    def testMigrateFinancialConnectionsAggregatorConnectionDataPlaid(self):
+        """Test MigrateFinancialConnectionsAggregatorConnectionDataPlaid"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MigrateFinancialConnectionsAggregatorConnectionDataMx()  # noqa: E501
+        # model = MigrateFinancialConnectionsAggregatorConnectionDataPlaid()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_token_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
+import fuse_client
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
 
 
-class TestMigrateFinancialConnectionsAggregatorConnectionDataPlaid(unittest.TestCase):
-    """MigrateFinancialConnectionsAggregatorConnectionDataPlaid unit test stubs"""
+class TestMigrateFinancialConnectionsTokenResponse(unittest.TestCase):
+    """MigrateFinancialConnectionsTokenResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMigrateFinancialConnectionsAggregatorConnectionDataPlaid(self):
-        """Test MigrateFinancialConnectionsAggregatorConnectionDataPlaid"""
+    def testMigrateFinancialConnectionsTokenResponse(self):
+        """Test MigrateFinancialConnectionsTokenResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MigrateFinancialConnectionsAggregatorConnectionDataPlaid()  # noqa: E501
+        # model = MigrateFinancialConnectionsTokenResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_token_request.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_token_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-from fuse-client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
-from fuse-client.model.product import Product
+import fuse_client
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
+from fuse_client.model.product import Product
 globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
 globals()['MigrateFinancialConnectionsTokenRequestEntity'] = MigrateFinancialConnectionsTokenRequestEntity
 globals()['Product'] = Product
-from fuse-client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
+from fuse_client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
 
 
 class TestMigrateFinancialConnectionsTokenRequest(unittest.TestCase):
     """MigrateFinancialConnectionsTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_token_request_entity.py` & `fuse-client-1.0.7/test/test_migrate_financial_connections_token_request_entity.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
+import fuse_client
+from fuse_client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
 
 
 class TestMigrateFinancialConnectionsTokenRequestEntity(unittest.TestCase):
     """MigrateFinancialConnectionsTokenRequestEntity unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_migrate_financial_connections_token_response.py` & `fuse-client-1.0.7/test/test_get_investment_holdings_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,31 +7,33 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
-from fuse-client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
+import fuse_client
+from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.model.financial_connections_holding import FinancialConnectionsHolding
+globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
+globals()['FinancialConnectionsHolding'] = FinancialConnectionsHolding
+from fuse_client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
 
 
-class TestMigrateFinancialConnectionsTokenResponse(unittest.TestCase):
-    """MigrateFinancialConnectionsTokenResponse unit test stubs"""
+class TestGetInvestmentHoldingsResponse(unittest.TestCase):
+    """GetInvestmentHoldingsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMigrateFinancialConnectionsTokenResponse(self):
-        """Test MigrateFinancialConnectionsTokenResponse"""
+    def testGetInvestmentHoldingsResponse(self):
+        """Test GetInvestmentHoldingsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MigrateFinancialConnectionsTokenResponse()  # noqa: E501
+        # model = GetInvestmentHoldingsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_product.py` & `fuse-client-1.0.7/test/test_product.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.product import Product
+import fuse_client
+from fuse_client.model.product import Product
 
 
 class TestProduct(unittest.TestCase):
     """Product unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_refresh_asset_report_request.py` & `fuse-client-1.0.7/test/test_account_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.refresh_asset_report_request import RefreshAssetReportRequest
+import fuse_client
+from fuse_client.model.account_type import AccountType
 
 
-class TestRefreshAssetReportRequest(unittest.TestCase):
-    """RefreshAssetReportRequest unit test stubs"""
+class TestAccountType(unittest.TestCase):
+    """AccountType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRefreshAssetReportRequest(self):
-        """Test RefreshAssetReportRequest"""
+    def testAccountType(self):
+        """Test AccountType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = RefreshAssetReportRequest()  # noqa: E501
+        # model = AccountType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_sync_financial_connections_data_response.py` & `fuse-client-1.0.7/test/test_sync_financial_connections_data_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
+import fuse_client
+from fuse_client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
 
 
 class TestSyncFinancialConnectionsDataResponse(unittest.TestCase):
     """SyncFinancialConnectionsDataResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_sync_transactions_request.py` & `fuse-client-1.0.7/test/test_sync_transactions_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.sync_transactions_request import SyncTransactionsRequest
+import fuse_client
+from fuse_client.model.sync_transactions_request import SyncTransactionsRequest
 
 
 class TestSyncTransactionsRequest(unittest.TestCase):
     """SyncTransactionsRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_sync_transactions_response.py` & `fuse-client-1.0.7/test/test_sync_transactions_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
-from fuse-client.model.transaction import Transaction
+import fuse_client
+from fuse_client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
+from fuse_client.model.transaction import Transaction
 globals()['SyncTransactionsResponseRemoved'] = SyncTransactionsResponseRemoved
 globals()['Transaction'] = Transaction
-from fuse-client.model.sync_transactions_response import SyncTransactionsResponse
+from fuse_client.model.sync_transactions_response import SyncTransactionsResponse
 
 
 class TestSyncTransactionsResponse(unittest.TestCase):
     """SyncTransactionsResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_sync_transactions_response_removed.py` & `fuse-client-1.0.7/test/test_sync_transactions_response_removed.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
+import fuse_client
+from fuse_client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
 
 
 class TestSyncTransactionsResponseRemoved(unittest.TestCase):
     """SyncTransactionsResponseRemoved unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_transaction.py` & `fuse-client-1.0.7/test/test_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.transaction_merchant import TransactionMerchant
+import fuse_client
+from fuse_client.model.transaction_merchant import TransactionMerchant
 globals()['TransactionMerchant'] = TransactionMerchant
-from fuse-client.model.transaction import Transaction
+from fuse_client.model.transaction import Transaction
 
 
 class TestTransaction(unittest.TestCase):
     """Transaction unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_transaction_merchant.py` & `fuse-client-1.0.7/test/test_update_entity_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,29 +7,31 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.transaction_merchant import TransactionMerchant
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+globals()['Aggregator'] = Aggregator
+from fuse_client.model.update_entity_request import UpdateEntityRequest
 
 
-class TestTransactionMerchant(unittest.TestCase):
-    """TransactionMerchant unit test stubs"""
+class TestUpdateEntityRequest(unittest.TestCase):
+    """UpdateEntityRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransactionMerchant(self):
-        """Test TransactionMerchant"""
+    def testUpdateEntityRequest(self):
+        """Test UpdateEntityRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TransactionMerchant()  # noqa: E501
+        # model = UpdateEntityRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.6/test/test_webhook_event.py` & `fuse-client-1.0.7/test/test_webhook_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.webhook_source import WebhookSource
-from fuse-client.model.webhook_type import WebhookType
+import fuse_client
+from fuse_client.model.webhook_source import WebhookSource
+from fuse_client.model.webhook_type import WebhookType
 globals()['WebhookSource'] = WebhookSource
 globals()['WebhookType'] = WebhookType
-from fuse-client.model.webhook_event import WebhookEvent
+from fuse_client.model.webhook_event import WebhookEvent
 
 
 class TestWebhookEvent(unittest.TestCase):
     """WebhookEvent unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_webhook_source.py` & `fuse-client-1.0.7/test/test_webhook_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.webhook_source import WebhookSource
+import fuse_client
+from fuse_client.model.webhook_source import WebhookSource
 
 
 class TestWebhookSource(unittest.TestCase):
     """WebhookSource unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `fuse-client-1.0.6/test/test_webhook_type.py` & `fuse-client-1.0.7/test/test_fuse_api_error_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,33 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
-import fuse-client
-from fuse-client.model.webhook_type import WebhookType
+import fuse_client
+from fuse_client.model.aggregator import Aggregator
+from fuse_client.model.fuse_api_error import FuseApiError
+globals()['Aggregator'] = Aggregator
+globals()['FuseApiError'] = FuseApiError
+from fuse_client.model.fuse_api_error_data import FuseApiErrorData
 
 
-class TestWebhookType(unittest.TestCase):
-    """WebhookType unit test stubs"""
+class TestFuseApiErrorData(unittest.TestCase):
+    """FuseApiErrorData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebhookType(self):
-        """Test WebhookType"""
+    def testFuseApiErrorData(self):
+        """Test FuseApiErrorData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WebhookType()  # noqa: E501
+        # model = FuseApiErrorData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

