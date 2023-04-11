# Comparing `tmp/fuse-client-1.0.7.tar.gz` & `tmp/fuse-client-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuse-client-1.0.7.tar", last modified: Tue Apr 11 10:09:13 2023, max compression
+gzip compressed data, was "fuse-client-1.0.8.tar", last modified: Tue Apr 11 12:12:53 2023, max compression
```

## Comparing `fuse-client-1.0.7.tar` & `fuse-client-1.0.8.tar`

### file list

```diff
@@ -1,226 +1,311 @@
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.657669 fuse-client-1.0.7/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.7/LICENSE
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 10:09:13.657739 fuse-client-1.0.7/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.7/README.md
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632098 fuse-client-1.0.7/fuse_client/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      739 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632831 fuse-client-1.0.7/fuse_client/api/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      212 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    91158 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    36894 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/api_client.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632991 fuse-client-1.0.7/fuse_client/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      452 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    21228 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/configuration.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5085 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/exceptions.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.645197 fuse-client-1.0.7/fuse_client/model/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      348 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    27574 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12061 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11690 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11513 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12371 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12132 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12167 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13358 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11510 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11929 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13654 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12128 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11360 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12294 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11715 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11350 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12404 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11587 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14438 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11530 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11616 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11687 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14204 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12931 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12630 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11913 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11124 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    19419 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14183 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11559 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13545 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14978 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11412 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    15583 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13181 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11708 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_addresses.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12117 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11797 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_emails.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11470 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_names.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_connections_owner_phone_numbers.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12712 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11967 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11598 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12323 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11714 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11940 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/fuse_api_warning_data_warnings.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11381 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11832 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13742 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12992 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11859 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12242 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_asset_report_response_report_historical_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13394 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12094 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11336 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12724 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11318 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12579 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11933 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11334 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12049 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11312 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11645 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12391 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_owners_response_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13137 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12694 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12065 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11293 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12451 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13477 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11313 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13115 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11267 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12271 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11448 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13344 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11333 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13168 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12017 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12370 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11603 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12286 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14669 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11153 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/sync_transactions_response_removed.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    45053 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11097 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11963 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    13317 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11759 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12227 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    81904 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/model_utils.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.645305 fuse-client-1.0.7/fuse_client/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9568 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12686 2023-04-11 10:09:06.000000 fuse-client-1.0.7/fuse_client/rest.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.632618 fuse-client-1.0.7/fuse_client.egg-info/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10416 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/SOURCES.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/dependency_links.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       32 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/requires.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-11 10:09:13.000000 fuse-client-1.0.7/fuse_client.egg-info/top_level.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 10:09:13.657983 fuse-client-1.0.7/setup.cfg
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1068 2023-04-11 10:09:06.000000 fuse-client-1.0.7/setup.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 10:09:13.657549 fuse-client-1.0.7/test/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      771 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      742 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      843 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      844 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      865 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      836 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1147 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      728 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      714 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      999 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1006 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1465 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      871 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      899 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1480 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      913 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      956 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1114 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      941 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2156 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1199 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      993 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1259 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1247 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1586 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1081 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_addresses.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      878 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_emails.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      885 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_names.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_connections_owner_phone_numbers.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1054 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      842 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3752 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      874 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      975 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1047 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_fuse_api_warning_data_warnings.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      822 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      994 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1177 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1517 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      929 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1000 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_asset_report_response_report_historical_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1037 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1040 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1323 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      942 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1251 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1165 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1130 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1169 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1143 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_owners_response_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      970 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1022 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1064 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      921 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1108 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1580 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1049 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1518 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      992 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1214 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      721 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1111 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_sync_transactions_response_removed.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      875 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      806 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      953 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      764 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 10:09:06.000000 fuse-client-1.0.7/test/test_webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327831 fuse-client-1.0.8/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.8/LICENSE
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:12:53.327918 fuse-client-1.0.8/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.8/README.md
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.285382 fuse-client-1.0.8/fuse_client/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      755 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    58516 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/api_client.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.286831 fuse-client-1.0.8/fuse_client/apis/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      214 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5677 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/path_to_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.289858 fuse-client-1.0.8/fuse_client/apis/paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      238 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      113 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      126 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report_create.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      128 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report_refresh.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      121 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_entities_entity_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      163 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_accounts_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      173 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_financial_connection_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      200 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_financial_connection_id_to_delete.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      181 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_institutions_institution_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      171 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_investments_holdings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      179 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_investments_transactions.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      154 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_liabilities.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      146 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_migrate.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      144 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_owners.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      172 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_public_token_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      140 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_sync.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      156 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_transactions.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      109 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_link_token.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      104 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_session.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      296 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tag_to_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.290106 fuse-client-1.0.8/fuse_client/apis/tags/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      302 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tags/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2958 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tags/fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    20767 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/configuration.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4542 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/exceptions.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303387 fuse-client-1.0.8/fuse_client/model/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    20979 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1731 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1316 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1065 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4096 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3792 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5853 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10013 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3128 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8645 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3744 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2909 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3960 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3365 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2577 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3988 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3064 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    16866 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8918 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5102 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4394 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     7342 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14140 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5892 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9498 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10325 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    31683 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11085 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    15913 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    17374 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    33113 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8247 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3437 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2630 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5197 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5016 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6638 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4222 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2614 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9445 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5285 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4863 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3402 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6620 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5739 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9233 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     7099 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2584 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4186 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8943 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8395 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5129 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1669 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4432 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3049 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10548 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)   164458 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5400 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6464 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1425 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1673 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303516 fuse-client-1.0.8/fuse_client/models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6216 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/models/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303648 fuse-client-1.0.8/fuse_client/paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1863 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304012 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      311 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304322 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      325 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11981 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304607 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      327 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11999 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304926 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      323 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.305340 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12002 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.305808 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      363 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12151 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306281 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11994 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306658 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      377 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9986 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306994 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      397 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10107 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/delete.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.307370 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      385 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9935 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.307985 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      371 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308283 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      379 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308569 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      353 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11951 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308898 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12259 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309370 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      343 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11966 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309649 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      373 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12475 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309963 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      339 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12200 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310335 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      355 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12090 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310620 fuse-client-1.0.8/fuse_client/paths/v1_link_token/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      307 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_link_token/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11939 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_link_token/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310883 fuse-client-1.0.8/fuse_client/paths/v1_session/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      301 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_session/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11881 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_session/post.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10567 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/rest.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    97672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/schemas.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.286416 fuse-client-1.0.8/fuse_client.egg-info/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14209 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      118 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/requires.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       17 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/top_level.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 12:12:53.328200 fuse-client-1.0.8/setup.cfg
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 12:12:22.000000 fuse-client-1.0.8/setup.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.281176 fuse-client-1.0.8/test/
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321352 fuse-client-1.0.8/test/test_models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      581 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      564 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      623 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      619 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      556 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      548 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      713 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      717 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      630 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      671 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      679 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      691 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      626 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      605 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      574 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      582 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      611 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      594 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      647 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      705 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      709 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      696 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      700 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      651 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      639 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      643 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      655 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      614 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      733 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      552 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      622 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      568 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321545 fuse-client-1.0.8/test/test_paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1995 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321833 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      772 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322113 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      791 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322444 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      794 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322799 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.323288 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.323656 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324013 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324308 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324634 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324930 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      924 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325221 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325505 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      922 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325744 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      873 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325990 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      872 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326300 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326571 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      859 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326819 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      868 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327074 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      877 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327376 fuse-client-1.0.8/test/test_paths/test_v1_link_token/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_link_token/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      766 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_link_token/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327660 fuse-client-1.0.8/test/test_paths/test_v1_session/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_session/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      759 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_session/test_post.py
```

### Comparing `fuse-client-1.0.7/LICENSE` & `fuse-client-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.7/README.md` & `fuse-client-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.7/fuse_client/__init__.py` & `fuse-client-1.0.8/fuse_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+# coding: utf-8
+
 # flake8: noqa
 
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 # import ApiClient
 from fuse_client.api_client import ApiClient
 
 # import Configuration
 from fuse_client.configuration import Configuration
```

### Comparing `fuse-client-1.0.7/fuse_client/configuration.py` & `fuse-client-1.0.8/fuse_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
 from fuse_client.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
 }
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
@@ -69,16 +71,14 @@
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
 
     :Example:
 
     API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -96,24 +96,26 @@
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
-    def __init__(self, host=None,
-                 api_key=None, api_key_prefix=None,
-                 access_token=None,
-                 username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
-                 server_index=None, server_variables=None,
-                 server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
-                 ):
+    def __init__(
+        self,
+        host=None,
+        api_key=None,
+        api_key_prefix=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+    ):
         """Constructor
         """
         self._base_path = "https://sandbox-api.letsfuse.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -123,35 +125,27 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
             self.api_key_prefix = api_key_prefix
         """dict to store API prefix (e.g. Bearer)
         """
         self.refresh_api_key_hook = None
         """function hook to refresh API key if expired
         """
-        self.username = username
-        """Username for HTTP basic authentication
-        """
-        self.password = password
-        """Password for HTTP basic authentication
-        """
-        self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("fuse_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
@@ -171,15 +165,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -400,134 +394,134 @@
                 'type': 'api_key',
                 'in': 'header',
                 'key': 'Fuse-Client-Id',
                 'value': self.get_api_key_with_prefix(
                     'fuseClientId',
                 ),
             }
-        if 'mxApiKey' in self.api_key:
-            auth['mxApiKey'] = {
+        if 'plaidClientId' in self.api_key:
+            auth['plaidClientId'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Mx-Api-Key',
+                'key': 'Plaid-Client-Id',
                 'value': self.get_api_key_with_prefix(
-                    'mxApiKey',
+                    'plaidClientId',
                 ),
             }
-        if 'mxClientId' in self.api_key:
-            auth['mxClientId'] = {
+        if 'plaidSecret' in self.api_key:
+            auth['plaidSecret'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Mx-Client-Id',
+                'key': 'Plaid-Secret',
                 'value': self.get_api_key_with_prefix(
-                    'mxClientId',
+                    'plaidSecret',
                 ),
             }
-        if 'plaidClientId' in self.api_key:
-            auth['plaidClientId'] = {
+        if 'tellerApplicationId' in self.api_key:
+            auth['tellerApplicationId'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Plaid-Client-Id',
+                'key': 'Teller-Application-Id',
                 'value': self.get_api_key_with_prefix(
-                    'plaidClientId',
+                    'tellerApplicationId',
                 ),
             }
-        if 'plaidSecret' in self.api_key:
-            auth['plaidSecret'] = {
+        if 'tellerCertificate' in self.api_key:
+            auth['tellerCertificate'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Plaid-Secret',
+                'key': 'Teller-Certificate',
                 'value': self.get_api_key_with_prefix(
-                    'plaidSecret',
+                    'tellerCertificate',
                 ),
             }
-        if 'proxyUrlKey' in self.api_key:
-            auth['proxyUrlKey'] = {
+        if 'tellerPrivateKey' in self.api_key:
+            auth['tellerPrivateKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Proxy-Url',
+                'key': 'Teller-Private-Key',
                 'value': self.get_api_key_with_prefix(
-                    'proxyUrlKey',
+                    'tellerPrivateKey',
                 ),
             }
-        if 'snaptradeClientId' in self.api_key:
-            auth['snaptradeClientId'] = {
+        if 'tellerTokenSigningKey' in self.api_key:
+            auth['tellerTokenSigningKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Snaptrade-Client-Id',
+                'key': 'Teller-Token-Signing-Key',
                 'value': self.get_api_key_with_prefix(
-                    'snaptradeClientId',
+                    'tellerTokenSigningKey',
                 ),
             }
-        if 'snaptradeConsumerKey' in self.api_key:
-            auth['snaptradeConsumerKey'] = {
+        if 'tellerSigningSecret' in self.api_key:
+            auth['tellerSigningSecret'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Snaptrade-Consumer-Id',
+                'key': 'Teller-Signing-Secret',
                 'value': self.get_api_key_with_prefix(
-                    'snaptradeConsumerKey',
+                    'tellerSigningSecret',
                 ),
             }
-        if 'tellerApplicationId' in self.api_key:
-            auth['tellerApplicationId'] = {
+        if 'mxClientId' in self.api_key:
+            auth['mxClientId'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Teller-Application-Id',
+                'key': 'Mx-Client-Id',
                 'value': self.get_api_key_with_prefix(
-                    'tellerApplicationId',
+                    'mxClientId',
                 ),
             }
-        if 'tellerCertificate' in self.api_key:
-            auth['tellerCertificate'] = {
+        if 'mxApiKey' in self.api_key:
+            auth['mxApiKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Teller-Certificate',
+                'key': 'Mx-Api-Key',
                 'value': self.get_api_key_with_prefix(
-                    'tellerCertificate',
+                    'mxApiKey',
                 ),
             }
-        if 'tellerPrivateKey' in self.api_key:
-            auth['tellerPrivateKey'] = {
+        if 'snaptradeClientId' in self.api_key:
+            auth['snaptradeClientId'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Teller-Private-Key',
+                'key': 'Snaptrade-Client-Id',
                 'value': self.get_api_key_with_prefix(
-                    'tellerPrivateKey',
+                    'snaptradeClientId',
                 ),
             }
-        if 'tellerSigningSecret' in self.api_key:
-            auth['tellerSigningSecret'] = {
+        if 'snaptradeConsumerKey' in self.api_key:
+            auth['snaptradeConsumerKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Teller-Signing-Secret',
+                'key': 'Snaptrade-Consumer-Id',
                 'value': self.get_api_key_with_prefix(
-                    'tellerSigningSecret',
+                    'snaptradeConsumerKey',
                 ),
             }
-        if 'tellerTokenSigningKey' in self.api_key:
-            auth['tellerTokenSigningKey'] = {
+        if 'proxyUrlKey' in self.api_key:
+            auth['proxyUrlKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'Teller-Token-Signing-Key',
+                'key': 'Proxy-Url',
                 'value': self.get_api_key_with_prefix(
-                    'tellerTokenSigningKey',
+                    'proxyUrlKey',
                 ),
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.7".\
+               "SDK Package Version: 1.0.8".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fuse-client-1.0.7/fuse_client/exceptions.py` & `fuse-client-1.0.8/fuse_client/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
+import dataclasses
+import typing
 
+from urllib3._collections import HTTPHeaderDict
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -92,27 +97,34 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-class ApiException(OpenApiException):
+T = typing.TypeVar("T")
+
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
+@dataclasses.dataclass
+class ApiException(OpenApiException, typing.Generic[T]):
+    status: int
+    reason: str
+    api_response: typing.Optional[T] = None
+
+    @property
+    def body(self) -> typing.Union[str, bytes, None]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.data
+
+    @property
+    def headers(self) -> typing.Optional[HTTPHeaderDict]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
@@ -120,38 +132,14 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `fuse-client-1.0.7/fuse_client/model_utils.py` & `fuse-client-1.0.8/fuse_client/schemas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,2033 +1,2475 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from datetime import date, datetime  # noqa: F401
-from copy import deepcopy
-import inspect
+from collections import defaultdict
+from datetime import date, datetime, timedelta  # noqa: F401
+import functools
+import decimal
 import io
-import os
-import pprint
 import re
-import tempfile
+import types
+import typing
+import uuid
 
-from dateutil.parser import parse
+from dateutil.parser.isoparser import isoparser, _takes_ascii
+import frozendict
 
 from fuse_client.exceptions import (
-    ApiKeyError,
-    ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
+from fuse_client.configuration import (
+    Configuration,
+)
+
+
+class Unset(object):
+    """
+    An instance of this class is set as the default value for object type(dict) properties that are optional
+    When a property has an unset value, that property will not be assigned in the dict
+    """
+    pass
+
+unset = Unset()
 
 none_type = type(None)
 file_type = io.IOBase
 
 
-def convert_js_args_to_python_args(fn):
-    from functools import wraps
-    @wraps(fn)
-    def wrapped_init(_self, *args, **kwargs):
-        """
-        An attribute named `self` received from the api will conflicts with the reserved `self`
-        parameter of a class method. During generation, `self` attributes are mapped
-        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
-        """
-        spec_property_naming = kwargs.get('_spec_property_naming', False)
-        if spec_property_naming:
-            kwargs = change_keys_js_to_python(kwargs, _self if isinstance(_self, type) else _self.__class__)
-        return fn(_self, *args, **kwargs)
-    return wrapped_init
-
-
-class cached_property(object):
-    # this caches the result of the function call for fn with no inputs
-    # use this as a decorator on function methods that you want converted
-    # into cached properties
-    result_key = '_results'
-
-    def __init__(self, fn):
-        self._fn = fn
-
-    def __get__(self, instance, cls=None):
-        if self.result_key in vars(self):
-            return vars(self)[self.result_key]
-        else:
-            result = self._fn()
-            setattr(self, self.result_key, result)
-            return result
-
-
-PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
-
-def allows_single_value_input(cls):
-    """
-    This function returns True if the input composed schema model or any
-    descendant model allows a value only input
-    This is true for cases where oneOf contains items like:
-    oneOf:
-      - float
-      - NumberWithValidation
-      - StringEnum
-      - ArrayModel
-      - null
-    TODO: lru_cache this
-    """
-    if (
-        issubclass(cls, ModelSimple) or
-        cls in PRIMITIVE_TYPES
-    ):
-        return True
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return False
-        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
-    return False
+class FileIO(io.FileIO):
+    """
+    A class for storing files
+    Note: this class is not immutable
+    """
 
-def composed_model_input_classes(cls):
+    def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader]):
+        if isinstance(_arg, (io.FileIO, io.BufferedReader)):
+            if _arg.closed:
+                raise ApiValueError('Invalid file state; file is closed and must be open')
+            _arg.close()
+            inst = super(FileIO, cls).__new__(cls, _arg.name)
+            super(FileIO, inst).__init__(_arg.name)
+            return inst
+        raise ApiValueError('FileIO must be passed _arg which contains the open file')
+
+    def __init__(self, _arg: typing.Union[io.FileIO, io.BufferedReader]):
+        pass
+
+
+def update(d: dict, u: dict):
     """
-    This function returns a list of the possible models that can be accepted as
-    inputs.
-    TODO: lru_cache this
-    """
-    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
-        return [cls]
-    elif issubclass(cls, ModelNormal):
-        if cls.discriminator is None:
-            return [cls]
-        else:
-            return get_discriminated_classes(cls)
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return []
-        if cls.discriminator is None:
-            input_classes = []
-            for c in cls._composed_schemas['oneOf']:
-                input_classes.extend(composed_model_input_classes(c))
-            return input_classes
+    Adds u to d
+    Where each dict is defaultdict(set)
+    """
+    if not u:
+        return d
+    for k, v in u.items():
+        if k not in d:
+            d[k] = v
         else:
-            return get_discriminated_classes(cls)
-    return []
+            d[k] = d[k] | v
 
 
-class OpenApiModel(object):
-    """The base class for all OpenAPIModels"""
+class ValidationMetadata(frozendict.frozendict):
+    """
+    A class storing metadata that is needed to validate OpenApi Schema payloads
+    """
+    def __new__(
+        cls,
+        path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+        from_server: bool = False,
+        configuration: typing.Optional[Configuration] = None,
+        seen_classes: typing.FrozenSet[typing.Type] = frozenset(),
+        validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]] = frozendict.frozendict()
+    ):
+        """
+        Args:
+            path_to_item: the path to the current data being instantiated.
+                For {'a': [1]} if the code is handling, 1, then the path is ('args[0]', 'a', 0)
+                This changes from location to location
+            from_server: whether or not this data came form the server
+                True when receiving server data
+                False when instantiating model with client side data not form the server
+                This does not change from location to location
+            configuration: the Configuration instance to use
+                This is needed because in Configuration:
+                - one can disable validation checking
+                This does not change from location to location
+            seen_classes: when deserializing data that matches multiple schemas, this is used to store
+                the schemas that have been traversed. This is used to stop processing when a cycle is seen.
+                This changes from location to location
+            validated_path_to_schemas: stores the already validated schema classes for a given path location
+                This does not change from location to location
+        """
+        return super().__new__(
+            cls,
+            path_to_item=path_to_item,
+            from_server=from_server,
+            configuration=configuration,
+            seen_classes=seen_classes,
+            validated_path_to_schemas=validated_path_to_schemas
+        )
 
-    def set_attribute(self, name, value):
-        # this is only used to set properties on self
-
-        path_to_item = []
-        if self._path_to_item:
-            path_to_item.extend(self._path_to_item)
-        path_to_item.append(name)
-
-        if name in self.openapi_types:
-            required_types_mixed = self.openapi_types[name]
-        elif self.additional_properties_type is None:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                path_to_item
-            )
-        elif self.additional_properties_type is not None:
-            required_types_mixed = self.additional_properties_type
-
-        if get_simple_class(name) != str:
-            error_msg = type_error_message(
-                var_name=name,
-                var_value=name,
-                valid_classes=(str,),
-                key_type=True
-            )
-            raise ApiTypeError(
-                error_msg,
-                path_to_item=path_to_item,
-                valid_classes=(str,),
-                key_type=True
-            )
+    def validation_ran_earlier(self, cls: type) -> bool:
+        validated_schemas = self.validated_path_to_schemas.get(self.path_to_item, set())
+        validation_ran_earlier = validated_schemas and cls in validated_schemas
+        if validation_ran_earlier:
+            return True
+        if cls in self.seen_classes:
+            return True
+        return False
+
+    @property
+    def path_to_item(self) -> typing.Tuple[typing.Union[str, int], ...]:
+        return self.get('path_to_item')
+
+    @property
+    def from_server(self) -> bool:
+        return self.get('from_server')
+
+    @property
+    def configuration(self) -> typing.Optional[Configuration]:
+        return self.get('configuration')
+
+    @property
+    def seen_classes(self) -> typing.FrozenSet[typing.Type]:
+        return self.get('seen_classes')
+
+    @property
+    def validated_path_to_schemas(self) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]]:
+        return self.get('validated_path_to_schemas')
+
+
+def add_deeper_validated_schemas(validation_metadata: ValidationMetadata, path_to_schemas: dict):
+    # this is called if validation_ran_earlier and current and deeper locations need to be added
+    current_path_to_item = validation_metadata.path_to_item
+    other_path_to_schemas = {}
+    for path_to_item, schemas in validation_metadata.validated_path_to_schemas.items():
+        if len(path_to_item) < len(current_path_to_item):
+            continue
+        path_begins_with_current_path = path_to_item[:len(current_path_to_item)] == current_path_to_item
+        if path_begins_with_current_path:
+            other_path_to_schemas[path_to_item] = schemas
+    update(path_to_schemas, other_path_to_schemas)
 
-        if self._check_type:
-            value = validate_and_convert_types(
-                value, required_types_mixed, path_to_item, self._spec_property_naming,
-                self._check_type, configuration=self._configuration)
-        if (name,) in self.allowed_values:
-            check_allowed_values(
-                self.allowed_values,
-                (name,),
-                value
-            )
-        if (name,) in self.validations:
-            check_validations(
-                self.validations,
-                (name,),
-                value,
-                self._configuration
-            )
-        self.__dict__['_data_store'][name] = value
+
+class Singleton:
+    """
+    Enums and singletons are the same
+    The same instance is returned for a given key of (cls, _arg)
+    """
+    _instances = {}
+
+    def __new__(cls, _arg: typing.Any, **kwargs):
+        """
+        cls base classes: BoolClass, NoneClass, str, decimal.Decimal
+        The 3rd key is used in the tuple below for a corner case where an enum contains integer 1
+        However 1.0  can also be ingested into that enum schema because 1.0 == 1 and
+        Decimal('1.0') == Decimal('1')
+        But if we omitted the 3rd value in the key, then Decimal('1.0') would be stored as Decimal('1')
+        and json serializing that instance would be '1' rather than the expected '1.0'
+        Adding the 3rd value, the str of _arg ensures that 1.0 -> Decimal('1.0') which is serialized as 1.0
+        """
+        key = (cls, _arg, str(_arg))
+        if key not in cls._instances:
+            if isinstance(_arg, (none_type, bool, BoolClass, NoneClass)):
+                inst = super().__new__(cls)
+                cls._instances[key] = inst
+            else:
+                cls._instances[key] = super().__new__(cls, _arg)
+        return cls._instances[key]
 
     def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
+        if isinstance(self, NoneClass):
+            return f'<{self.__class__.__name__}: None>'
+        elif isinstance(self, BoolClass):
+            if bool(self):
+                return f'<{self.__class__.__name__}: True>'
+            return f'<{self.__class__.__name__}: False>'
+        return f'<{self.__class__.__name__}: {super().__repr__()}>'
 
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        return not self == other
-
-    def __setattr__(self, attr, value):
-        """set the value of an attribute using dot notation: `instance.attr = val`"""
-        self[attr] = value
-
-    def __getattr__(self, attr):
-        """get the value of an attribute using dot notation: `instance.attr`"""
-        return self.__getitem__(attr)
-
-    def __copy__(self):
-        cls = self.__class__
-        if self.get("_spec_property_naming", False):
-            return cls._new_from_openapi_data(**self.__dict__)
-        else:
-            return new_cls.__new__(cls, **self.__dict__)
 
-    def __deepcopy__(self, memo):
-        cls = self.__class__
+class classproperty:
 
-        if self.get("_spec_property_naming", False):
-            new_inst = cls._new_from_openapi_data()
-        else:
-            new_inst = cls.__new__(cls)
+    def __init__(self, fget):
+        self.fget = fget
 
-        for k, v in self.__dict__.items():
-            setattr(new_inst, k, deepcopy(v, memo))
-        return new_inst
+    def __get__(self, owner_self, owner_cls):
+        return self.fget(owner_cls)
 
 
-    def __new__(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
+class NoneClass(Singleton):
+    @classproperty
+    def NONE(cls):
+        return cls(None)
 
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-                    cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = super(OpenApiModel, cls).__new__(cls)
-            self_inst.__init__(*args, **kwargs)
-
-        if kwargs.get("_spec_property_naming", False):
-            # when true, implies new is from deserialization
-            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        else:
-            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
-            new_inst.__init__(*args, **kwargs)
+    def __bool__(self) -> bool:
+        return False
 
-        return new_inst
 
+class BoolClass(Singleton):
+    @classproperty
+    def TRUE(cls):
+        return cls(True)
+
+    @classproperty
+    def FALSE(cls):
+        return cls(False)
+
+    @functools.lru_cache()
+    def __bool__(self) -> bool:
+        for key, instance in self._instances.items():
+            if self is instance:
+                return bool(key[1])
+        raise ValueError('Unable to find the boolean value of this instance')
+
+
+class MetaOapgTyped:
+    exclusive_maximum: typing.Union[int, float]
+    inclusive_maximum: typing.Union[int, float]
+    exclusive_minimum: typing.Union[int, float]
+    inclusive_minimum: typing.Union[int, float]
+    max_items: int
+    min_items: int
+    discriminator: typing.Dict[str, typing.Dict[str, typing.Type['Schema']]]
+
+
+    class properties:
+        # to hold object properties
+        pass
+
+    additional_properties: typing.Optional[typing.Type['Schema']]
+    max_properties: int
+    min_properties: int
+    all_of: typing.List[typing.Type['Schema']]
+    one_of: typing.List[typing.Type['Schema']]
+    any_of: typing.List[typing.Type['Schema']]
+    not_schema: typing.Type['Schema']
+    max_length: int
+    min_length: int
+    items: typing.Type['Schema']
+
+
+class Schema:
+    """
+    the base class of all swagger/openapi schemas/models
+    """
+    __inheritable_primitive_types_set = {decimal.Decimal, str, tuple, frozendict.frozendict, FileIO, bytes, BoolClass, NoneClass}
+    _types: typing.Set[typing.Type]
+    MetaOapg = MetaOapgTyped
+
+    @staticmethod
+    def __get_valid_classes_phrase(input_classes):
+        """Returns a string phrase describing what types are allowed"""
+        all_classes = list(input_classes)
+        all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
+        all_class_names = [cls.__name__ for cls in all_classes]
+        if len(all_class_names) == 1:
+            return "is {0}".format(all_class_names[0])
+        return "is one of [{0}]".format(", ".join(all_class_names))
+
+    @staticmethod
+    def _get_class_oapg(item_cls: typing.Union[types.FunctionType, staticmethod, typing.Type['Schema']]) -> typing.Type['Schema']:
+        if isinstance(item_cls, types.FunctionType):
+            # referenced schema
+            return item_cls()
+        elif isinstance(item_cls, staticmethod):
+            # referenced schema
+            return item_cls.__func__()
+        return item_cls
 
     @classmethod
-    @convert_js_args_to_python_args
-    def _new_from_openapi_data(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
+    def __type_error_message(
+        cls, var_value=None, var_name=None, valid_classes=None, key_type=None
+    ):
+        """
+        Keyword Args:
+            var_value (any): the variable which has the type_error
+            var_name (str): the name of the variable which has the typ error
+            valid_classes (tuple): the accepted classes for current_item's
+                                      value
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a tuple
+        """
+        key_or_value = "value"
+        if key_type:
+            key_or_value = "key"
+        valid_classes_phrase = cls.__get_valid_classes_phrase(valid_classes)
+        msg = "Invalid type. Required {1} type {2} and " "passed type was {3}".format(
+            var_name,
+            key_or_value,
+            valid_classes_phrase,
+            type(var_value).__name__,
+        )
+        return msg
+
+    @classmethod
+    def __get_type_error(cls, var_value, path_to_item, valid_classes, key_type=False):
+        error_msg = cls.__type_error_message(
+            var_name=path_to_item[-1],
+            var_value=var_value,
+            valid_classes=valid_classes,
+            key_type=key_type,
+        )
+        return ApiTypeError(
+            error_msg,
+            path_to_item=path_to_item,
+            valid_classes=valid_classes,
+            key_type=key_type,
+        )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        Schema _validate_oapg
+        All keyword validation except for type checking was done in calling stack frames
+        If those validations passed, the validated classes are collected in path_to_schemas
+
+        Returns:
+            path_to_schemas: a map of path to schemas
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        base_class = type(arg)
+        if base_class not in cls._types:
+            raise cls.__get_type_error(
+                arg,
+                validation_metadata.path_to_item,
+                cls._types,
+                key_type=False,
             )
 
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-                    cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = cls._from_openapi_data(*args, **kwargs)
+        path_to_schemas = {validation_metadata.path_to_item: set()}
+        path_to_schemas[validation_metadata.path_to_item].add(cls)
+        path_to_schemas[validation_metadata.path_to_item].add(base_class)
+        return path_to_schemas
+
+    @staticmethod
+    def _process_schema_classes_oapg(
+        schema_classes: typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]
+    ):
+        """
+        Processes and mutates schema_classes
+        If a SomeSchema is a subclass of DictSchema then remove DictSchema because it is already included
+        """
+        if len(schema_classes) < 2:
+            return
+        if len(schema_classes) > 2 and UnsetAnyTypeSchema in schema_classes:
+            schema_classes.remove(UnsetAnyTypeSchema)
+        x_schema = schema_type_classes & schema_classes
+        if not x_schema:
+            return
+        x_schema = x_schema.pop()
+        if any(c is not x_schema and issubclass(c, x_schema) for c in schema_classes):
+            # needed to not have a mro error in get_new_class
+            schema_classes.remove(x_schema)
+
+    @classmethod
+    def __get_new_cls(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]:
+        """
+        Make a new dynamic class and return an instance of that class
+        We are making an instance of cls, but instead of making cls
+        make a new class, new_cls
+        which includes dynamic bases including cls
+        return an instance of that new class
+
+        Dict property + List Item Assignment Use cases:
+        1. value is NOT an instance of the required schema class
+            the value is validated by _validate_oapg
+            _validate_oapg returns a key value pair
+            where the key is the path to the item, and the value will be the required manufactured class
+            made out of the matching schemas
+        2. value is an instance of the correct schema type
+            the value is NOT validated by _validate_oapg, _validate_oapg only checks that the instance is of the correct schema type
+            for this value, _validate_oapg does NOT return an entry for it in _path_to_schemas
+            and in list/dict _get_items_oapg,_get_properties_oapg the value will be directly assigned
+            because value is of the correct type, and validation was run earlier when the instance was created
+        """
+        _path_to_schemas = {}
+        if validation_metadata.validation_ran_earlier(cls):
+            add_deeper_validated_schemas(validation_metadata, _path_to_schemas)
+        else:
+            other_path_to_schemas = cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            update(_path_to_schemas, other_path_to_schemas)
+        # loop through it make a new class for each entry
+        # do not modify the returned result because it is cached and we would be modifying the cached value
+        path_to_schemas = {}
+        for path, schema_classes in _path_to_schemas.items():
+            """
+            Use cases
+            1. N number of schema classes + enum + type != bool/None, classes in path_to_schemas: tuple/frozendict.frozendict/str/Decimal/bytes/FileIo
+                needs Singleton added
+            2. N number of schema classes + enum + type == bool/None, classes in path_to_schemas: BoolClass/NoneClass
+                Singleton already added
+            3. N number of schema classes, classes in path_to_schemas: BoolClass/NoneClass/tuple/frozendict.frozendict/str/Decimal/bytes/FileIo
+            """
+            cls._process_schema_classes_oapg(schema_classes)
+            enum_schema = any(
+                issubclass(this_cls, EnumBase) for this_cls in schema_classes)
+            inheritable_primitive_type = schema_classes.intersection(cls.__inheritable_primitive_types_set)
+            chosen_schema_classes = schema_classes - inheritable_primitive_type
+            suffix = tuple(inheritable_primitive_type)
+            if enum_schema and suffix[0] not in {NoneClass, BoolClass}:
+                suffix = (Singleton,) + suffix
+
+            used_classes = tuple(sorted(chosen_schema_classes, key=lambda a_cls: a_cls.__name__)) + suffix
+            mfg_cls = get_new_class(class_name='DynamicSchema', bases=used_classes)
+            path_to_schemas[path] = mfg_cls
+
+        return path_to_schemas
 
+    @classmethod
+    def _get_new_instance_without_conversion_oapg(
+        cls,
+        arg: typing.Any,
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        # We have a Dynamic class and we are making an instance of it
+        if issubclass(cls, frozendict.frozendict) and issubclass(cls, DictBase):
+            properties = cls._get_properties_oapg(arg, path_to_item, path_to_schemas)
+            return super(Schema, cls).__new__(cls, properties)
+        elif issubclass(cls, tuple) and issubclass(cls, ListBase):
+            items = cls._get_items_oapg(arg, path_to_item, path_to_schemas)
+            return super(Schema, cls).__new__(cls, items)
+        """
+        str = openapi str, date, and datetime
+        decimal.Decimal = openapi int and float
+        FileIO = openapi binary type and the user inputs a file
+        bytes = openapi binary type and the user inputs bytes
+        """
+        return super(Schema, cls).__new__(cls, arg)
 
-        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+    @classmethod
+    def from_openapi_data_oapg(
+        cls,
+        arg: typing.Union[
+            str,
+            date,
+            datetime,
+            int,
+            float,
+            decimal.Decimal,
+            bool,
+            None,
+            'Schema',
+            dict,
+            frozendict.frozendict,
+            tuple,
+            list,
+            io.FileIO,
+            io.BufferedReader,
+            bytes
+        ],
+        _configuration: typing.Optional[Configuration]
+    ):
+        """
+        Schema from_openapi_data_oapg
+        """
+        from_server = True
+        validated_path_to_schemas = {}
+        arg = cast_to_allowed_types(arg, from_server, validated_path_to_schemas)
+        validation_metadata = ValidationMetadata(
+            from_server=from_server, configuration=_configuration, validated_path_to_schemas=validated_path_to_schemas)
+        path_to_schemas = cls.__get_new_cls(arg, validation_metadata)
+        new_cls = path_to_schemas[validation_metadata.path_to_item]
+        new_inst = new_cls._get_new_instance_without_conversion_oapg(
+            arg,
+            validation_metadata.path_to_item,
+            path_to_schemas
+        )
         return new_inst
 
+    @staticmethod
+    def __get_input_dict(*args, **kwargs) -> frozendict.frozendict:
+        input_dict = {}
+        if args and isinstance(args[0], (dict, frozendict.frozendict)):
+            input_dict.update(args[0])
+        if kwargs:
+            input_dict.update(kwargs)
+        return frozendict.frozendict(input_dict)
+
+    @staticmethod
+    def __remove_unsets(kwargs):
+        return {key: val for key, val in kwargs.items() if val is not unset}
 
-class ModelSimple(OpenApiModel):
-    """the parent class of models whose type != object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
+    def __new__(cls, *_args: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'], _configuration: typing.Optional[Configuration] = None, **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset]):
+        """
+        Schema __new__
 
-        self.set_attribute(name, value)
+        Args:
+            _args (int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): the value
+            kwargs (str, int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): dict values
+            _configuration: contains the Configuration that enables json schema validation keywords
+                like minItems, minLength etc
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
+        Note: double underscores are used here because pycharm thinks that these variables
+        are instance properties if they are named normally :(
+        """
+        __kwargs = cls.__remove_unsets(kwargs)
+        if not _args and not __kwargs:
+            raise TypeError(
+                'No input given. args or kwargs must be given.'
+            )
+        if not __kwargs and _args and not isinstance(_args[0], dict):
+            __arg = _args[0]
+        else:
+            __arg = cls.__get_input_dict(*_args, **__kwargs)
+        __from_server = False
+        __validated_path_to_schemas = {}
+        __arg = cast_to_allowed_types(
+            __arg, __from_server, __validated_path_to_schemas)
+        __validation_metadata = ValidationMetadata(
+            configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
+        __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
+        __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
+        return __new_cls._get_new_instance_without_conversion_oapg(
+            __arg,
+            __validation_metadata.path_to_item,
+            __path_to_schemas
         )
 
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return str(self.value)
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
+    def __init__(
+        self,
+        *_args: typing.Union[
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'],
+        _configuration: typing.Optional[Configuration] = None,
+        **kwargs: typing.Union[
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset
+        ]
+    ):
+        """
+        this is needed to fix 'Unexpected argument' warning in pycharm
+        this code does nothing because all Schema instances are immutable
+        this means that all input data is passed into and used in new, and after the new instance is made
+        no new attributes are assigned and init is not used
+        """
+        pass
 
-        this_val = self._data_store['value']
-        that_val = other._data_store['value']
-        types = set()
-        types.add(this_val.__class__)
-        types.add(that_val.__class__)
-        vals_equal = this_val == that_val
-        return vals_equal
-
-
-class ModelNormal(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
+"""
+import itertools
+data_types = ('None', 'FrozenDict', 'Tuple', 'Str', 'Decimal', 'Bool')
+type_to_cls = {
+    'None': 'NoneClass',
+    'FrozenDict': 'frozendict.frozendict',
+    'Tuple': 'tuple',
+    'Str': 'str',
+    'Decimal': 'decimal.Decimal',
+    'Bool': 'BoolClass'
+}
+cls_tuples = [v for v in itertools.combinations(data_types, 5)]
+typed_classes = [f"class {''.join(cls_tuple)}Mixin({', '.join(type_to_cls[typ] for typ in cls_tuple)}):\n    pass" for cls_tuple in cls_tuples]
+for cls in typed_classes:
+    print(cls)
+object_classes = [f"{''.join(cls_tuple)}Mixin = object" for cls_tuple in cls_tuples]
+for cls in object_classes:
+    print(cls)
+"""
+if typing.TYPE_CHECKING:
+    # qty 1
+    NoneMixin = NoneClass
+    FrozenDictMixin = frozendict.frozendict
+    TupleMixin = tuple
+    StrMixin = str
+    DecimalMixin = decimal.Decimal
+    BoolMixin = BoolClass
+    BytesMixin = bytes
+    FileMixin = FileIO
+    # qty 2
+    class BinaryMixin(bytes, FileIO):
+        pass
+    class NoneFrozenDictMixin(NoneClass, frozendict.frozendict):
+        pass
+    class NoneTupleMixin(NoneClass, tuple):
+        pass
+    class NoneStrMixin(NoneClass, str):
+        pass
+    class NoneDecimalMixin(NoneClass, decimal.Decimal):
+        pass
+    class NoneBoolMixin(NoneClass, BoolClass):
+        pass
+    class FrozenDictTupleMixin(frozendict.frozendict, tuple):
+        pass
+    class FrozenDictStrMixin(frozendict.frozendict, str):
+        pass
+    class FrozenDictDecimalMixin(frozendict.frozendict, decimal.Decimal):
+        pass
+    class FrozenDictBoolMixin(frozendict.frozendict, BoolClass):
+        pass
+    class TupleStrMixin(tuple, str):
+        pass
+    class TupleDecimalMixin(tuple, decimal.Decimal):
+        pass
+    class TupleBoolMixin(tuple, BoolClass):
+        pass
+    class StrDecimalMixin(str, decimal.Decimal):
+        pass
+    class StrBoolMixin(str, BoolClass):
+        pass
+    class DecimalBoolMixin(decimal.Decimal, BoolClass):
+        pass
+    # qty 3
+    class NoneFrozenDictTupleMixin(NoneClass, frozendict.frozendict, tuple):
+        pass
+    class NoneFrozenDictStrMixin(NoneClass, frozendict.frozendict, str):
+        pass
+    class NoneFrozenDictDecimalMixin(NoneClass, frozendict.frozendict, decimal.Decimal):
+        pass
+    class NoneFrozenDictBoolMixin(NoneClass, frozendict.frozendict, BoolClass):
+        pass
+    class NoneTupleStrMixin(NoneClass, tuple, str):
+        pass
+    class NoneTupleDecimalMixin(NoneClass, tuple, decimal.Decimal):
+        pass
+    class NoneTupleBoolMixin(NoneClass, tuple, BoolClass):
+        pass
+    class NoneStrDecimalMixin(NoneClass, str, decimal.Decimal):
+        pass
+    class NoneStrBoolMixin(NoneClass, str, BoolClass):
+        pass
+    class NoneDecimalBoolMixin(NoneClass, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrMixin(frozendict.frozendict, tuple, str):
+        pass
+    class FrozenDictTupleDecimalMixin(frozendict.frozendict, tuple, decimal.Decimal):
+        pass
+    class FrozenDictTupleBoolMixin(frozendict.frozendict, tuple, BoolClass):
+        pass
+    class FrozenDictStrDecimalMixin(frozendict.frozendict, str, decimal.Decimal):
+        pass
+    class FrozenDictStrBoolMixin(frozendict.frozendict, str, BoolClass):
+        pass
+    class FrozenDictDecimalBoolMixin(frozendict.frozendict, decimal.Decimal, BoolClass):
+        pass
+    class TupleStrDecimalMixin(tuple, str, decimal.Decimal):
+        pass
+    class TupleStrBoolMixin(tuple, str, BoolClass):
+        pass
+    class TupleDecimalBoolMixin(tuple, decimal.Decimal, BoolClass):
+        pass
+    class StrDecimalBoolMixin(str, decimal.Decimal, BoolClass):
+        pass
+    # qty 4
+    class NoneFrozenDictTupleStrMixin(NoneClass, frozendict.frozendict, tuple, str):
+        pass
+    class NoneFrozenDictTupleDecimalMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal):
+        pass
+    class NoneFrozenDictTupleBoolMixin(NoneClass, frozendict.frozendict, tuple, BoolClass):
+        pass
+    class NoneFrozenDictStrDecimalMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal):
+        pass
+    class NoneFrozenDictStrBoolMixin(NoneClass, frozendict.frozendict, str, BoolClass):
+        pass
+    class NoneFrozenDictDecimalBoolMixin(NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass):
+        pass
+    class NoneTupleStrDecimalMixin(NoneClass, tuple, str, decimal.Decimal):
+        pass
+    class NoneTupleStrBoolMixin(NoneClass, tuple, str, BoolClass):
+        pass
+    class NoneTupleDecimalBoolMixin(NoneClass, tuple, decimal.Decimal, BoolClass):
+        pass
+    class NoneStrDecimalBoolMixin(NoneClass, str, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrDecimalMixin(frozendict.frozendict, tuple, str, decimal.Decimal):
+        pass
+    class FrozenDictTupleStrBoolMixin(frozendict.frozendict, tuple, str, BoolClass):
+        pass
+    class FrozenDictTupleDecimalBoolMixin(frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictStrDecimalBoolMixin(frozendict.frozendict, str, decimal.Decimal, BoolClass):
+        pass
+    class TupleStrDecimalBoolMixin(tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 5
+    class NoneFrozenDictTupleStrDecimalMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal):
+        pass
+    class NoneFrozenDictTupleStrBoolMixin(NoneClass, frozendict.frozendict, tuple, str, BoolClass):
+        pass
+    class NoneFrozenDictTupleDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
+        pass
+    class NoneFrozenDictStrDecimalBoolMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass):
+        pass
+    class NoneTupleStrDecimalBoolMixin(NoneClass, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrDecimalBoolMixin(frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 6
+    class NoneFrozenDictTupleStrDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 8
+    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes):
+        pass
+else:
+    # qty 1
+    class NoneMixin:
+        _types = {NoneClass}
+    class FrozenDictMixin:
+        _types = {frozendict.frozendict}
+    class TupleMixin:
+        _types = {tuple}
+    class StrMixin:
+        _types = {str}
+    class DecimalMixin:
+        _types = {decimal.Decimal}
+    class BoolMixin:
+        _types = {BoolClass}
+    class BytesMixin:
+        _types = {bytes}
+    class FileMixin:
+        _types = {FileIO}
+    # qty 2
+    class BinaryMixin:
+        _types = {bytes, FileIO}
+    class NoneFrozenDictMixin:
+        _types = {NoneClass, frozendict.frozendict}
+    class NoneTupleMixin:
+        _types = {NoneClass, tuple}
+    class NoneStrMixin:
+        _types = {NoneClass, str}
+    class NoneDecimalMixin:
+        _types = {NoneClass, decimal.Decimal}
+    class NoneBoolMixin:
+        _types = {NoneClass, BoolClass}
+    class FrozenDictTupleMixin:
+        _types = {frozendict.frozendict, tuple}
+    class FrozenDictStrMixin:
+        _types = {frozendict.frozendict, str}
+    class FrozenDictDecimalMixin:
+        _types = {frozendict.frozendict, decimal.Decimal}
+    class FrozenDictBoolMixin:
+        _types = {frozendict.frozendict, BoolClass}
+    class TupleStrMixin:
+        _types = {tuple, str}
+    class TupleDecimalMixin:
+        _types = {tuple, decimal.Decimal}
+    class TupleBoolMixin:
+        _types = {tuple, BoolClass}
+    class StrDecimalMixin:
+        _types = {str, decimal.Decimal}
+    class StrBoolMixin:
+        _types = {str, BoolClass}
+    class DecimalBoolMixin:
+        _types = {decimal.Decimal, BoolClass}
+    # qty 3
+    class NoneFrozenDictTupleMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple}
+    class NoneFrozenDictStrMixin:
+        _types = {NoneClass, frozendict.frozendict, str}
+    class NoneFrozenDictDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, decimal.Decimal}
+    class NoneFrozenDictBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, BoolClass}
+    class NoneTupleStrMixin:
+        _types = {NoneClass, tuple, str}
+    class NoneTupleDecimalMixin:
+        _types = {NoneClass, tuple, decimal.Decimal}
+    class NoneTupleBoolMixin:
+        _types = {NoneClass, tuple, BoolClass}
+    class NoneStrDecimalMixin:
+        _types = {NoneClass, str, decimal.Decimal}
+    class NoneStrBoolMixin:
+        _types = {NoneClass, str, BoolClass}
+    class NoneDecimalBoolMixin:
+        _types = {NoneClass, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrMixin:
+        _types = {frozendict.frozendict, tuple, str}
+    class FrozenDictTupleDecimalMixin:
+        _types = {frozendict.frozendict, tuple, decimal.Decimal}
+    class FrozenDictTupleBoolMixin:
+        _types = {frozendict.frozendict, tuple, BoolClass}
+    class FrozenDictStrDecimalMixin:
+        _types = {frozendict.frozendict, str, decimal.Decimal}
+    class FrozenDictStrBoolMixin:
+        _types = {frozendict.frozendict, str, BoolClass}
+    class FrozenDictDecimalBoolMixin:
+        _types = {frozendict.frozendict, decimal.Decimal, BoolClass}
+    class TupleStrDecimalMixin:
+        _types = {tuple, str, decimal.Decimal}
+    class TupleStrBoolMixin:
+        _types = {tuple, str, BoolClass}
+    class TupleDecimalBoolMixin:
+        _types = {tuple, decimal.Decimal, BoolClass}
+    class StrDecimalBoolMixin:
+        _types = {str, decimal.Decimal, BoolClass}
+    # qty 4
+    class NoneFrozenDictTupleStrMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str}
+    class NoneFrozenDictTupleDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal}
+    class NoneFrozenDictTupleBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, BoolClass}
+    class NoneFrozenDictStrDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal}
+    class NoneFrozenDictStrBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, str, BoolClass}
+    class NoneFrozenDictDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass}
+    class NoneTupleStrDecimalMixin:
+        _types = {NoneClass, tuple, str, decimal.Decimal}
+    class NoneTupleStrBoolMixin:
+        _types = {NoneClass, tuple, str, BoolClass}
+    class NoneTupleDecimalBoolMixin:
+        _types = {NoneClass, tuple, decimal.Decimal, BoolClass}
+    class NoneStrDecimalBoolMixin:
+        _types = {NoneClass, str, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrDecimalMixin:
+        _types = {frozendict.frozendict, tuple, str, decimal.Decimal}
+    class FrozenDictTupleStrBoolMixin:
+        _types = {frozendict.frozendict, tuple, str, BoolClass}
+    class FrozenDictTupleDecimalBoolMixin:
+        _types = {frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
+    class FrozenDictStrDecimalBoolMixin:
+        _types = {frozendict.frozendict, str, decimal.Decimal, BoolClass}
+    class TupleStrDecimalBoolMixin:
+        _types = {tuple, str, decimal.Decimal, BoolClass}
+    # qty 5
+    class NoneFrozenDictTupleStrDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal}
+    class NoneFrozenDictTupleStrBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, BoolClass}
+    class NoneFrozenDictTupleDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
+    class NoneFrozenDictStrDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass}
+    class NoneTupleStrDecimalBoolMixin:
+        _types = {NoneClass, tuple, str, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrDecimalBoolMixin:
+        _types = {frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
+    # qty 6
+    class NoneFrozenDictTupleStrDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
+    # qty 8
+    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes}
+
+
+class ValidatorBase:
+    @staticmethod
+    def _is_json_validation_enabled_oapg(schema_keyword, configuration=None):
+        """Returns true if JSON schema validation is enabled for the specified
+        validation keyword. This can be used to skip JSON schema structural validation
+        as requested in the configuration.
+        Note: the suffix _oapg stands for openapi python (experimental) generator and
+        it has been added to prevent collisions with other methods and properties
+
+        Args:
+            schema_keyword (string): the name of a JSON schema validation keyword.
+            configuration (Configuration): the configuration class.
+        """
 
-        self.set_attribute(name, value)
+        return (configuration is None or
+            not hasattr(configuration, '_disabled_client_side_validations') or
+            schema_keyword not in configuration._disabled_client_side_validations)
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
+    @staticmethod
+    def _raise_validation_error_message_oapg(value, constraint_msg, constraint_value, path_to_item, additional_txt=""):
+        raise ApiValueError(
+            "Invalid value `{value}`, {constraint_msg} `{constraint_value}`{additional_txt} at {path_to_item}".format(
+                value=value,
+                constraint_msg=constraint_msg,
+                constraint_value=constraint_value,
+                additional_txt=additional_txt,
+                path_to_item=path_to_item,
+            )
         )
 
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
+
+class EnumBase:
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        EnumBase _validate_oapg
+        Validates that arg is in the enum's allowed values
+        """
+        try:
+            cls.MetaOapg.enum_value_to_name[arg]
+        except KeyError:
+            raise ApiValueError("Invalid value {} passed in to {}, allowed_values={}".format(arg, cls, cls.MetaOapg.enum_value_to_name.keys()))
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class BoolBase:
+    def is_true_oapg(self) -> bool:
+        """
+        A replacement for x is True
+        True if the instance is a BoolClass True Singleton
+        """
+        if not issubclass(self.__class__, BoolClass):
             return False
+        return bool(self)
 
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+    def is_false_oapg(self) -> bool:
+        """
+        A replacement for x is False
+        True if the instance is a BoolClass False Singleton
+        """
+        if not issubclass(self.__class__, BoolClass):
             return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-class ModelComposed(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi and have oneOf/allOf/anyOf
-
-    When one sets a property we use var_name_to_model_instances to store the value in
-    the correct class instances + run any type checking + validation code.
-    When one gets a property we use var_name_to_model_instances to get the value
-    from the correct class instances.
-    This allows multiple composed schemas to contain the same property with additive
-    constraints on the value.
-
-    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
-    key (str): allOf/oneOf/anyOf
-    value (list): the classes in the XOf definition.
-        Note: none_type can be included when the openapi document version >= 3.1.0
-    _composed_instances (list): stores a list of instances of the composed schemas
-    defined in _composed_schemas. When properties are accessed in the self instance,
-    they are returned from the self._data_store or the data stores in the instances
-    in self._composed_schemas
-    _var_name_to_model_instances (dict): maps between a variable name on self and
-    the composed instances (self included) which contain that data
-    key (str): property name
-    value (list): list of class instances, self or instances in _composed_instances
-    which contain the value that the key is referring to.
-    """
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
+        return bool(self) is False
+
+
+class NoneBase:
+    def is_none_oapg(self) -> bool:
+        """
+        A replacement for x is None
+        True if the instance is a NoneClass None Singleton
+        """
+        if issubclass(self.__class__, NoneClass):
+            return True
+        return False
+
+
+class StrBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
+
+    @property
+    def as_str_oapg(self) -> str:
+        return self
+
+    @property
+    def as_date_oapg(self) -> date:
+        raise Exception('not implemented')
+
+    @property
+    def as_datetime_oapg(self) -> datetime:
+        raise Exception('not implemented')
+
+    @property
+    def as_decimal_oapg(self) -> decimal.Decimal:
+        raise Exception('not implemented')
+
+    @property
+    def as_uuid_oapg(self) -> uuid.UUID:
+        raise Exception('not implemented')
+
+    @classmethod
+    def __check_str_validations(
+        cls,
+        arg: str,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
             return
+        if (cls._is_json_validation_enabled_oapg('maxLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_length') and
+                len(arg) > cls.MetaOapg.max_length):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="length must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_length,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_length') and
+                len(arg) < cls.MetaOapg.min_length):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="length must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_length,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('pattern', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'regex')):
+            for regex_dict in cls.MetaOapg.regex:
+                flags = regex_dict.get('flags', 0)
+                if not re.search(regex_dict['pattern'], arg, flags=flags):
+                    if flags != 0:
+                        # Don't print the regex flags if the flags are not
+                        # specified in the OAS document.
+                        cls._raise_validation_error_message_oapg(
+                            value=arg,
+                            constraint_msg="must match regular expression",
+                            constraint_value=regex_dict['pattern'],
+                            path_to_item=validation_metadata.path_to_item,
+                            additional_txt=" with flags=`{}`".format(flags)
+                        )
+                    cls._raise_validation_error_message_oapg(
+                        value=arg,
+                        constraint_msg="must match regular expression",
+                        constraint_value=regex_dict['pattern'],
+                        path_to_item=validation_metadata.path_to_item
+                    )
 
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
-        Use cases:
-        1. additional_properties_type is None (additionalProperties == False in spec)
-            Check for property presence in self.openapi_types
-            if not present then throw an error
-            if present set in self, set attribute
-            always set on composed schemas
-        2.  additional_properties_type exists
-            set attribute on self
-            always set on composed schemas
+        StrBase _validate_oapg
+        Validates that validations pass
         """
-        if self.additional_properties_type is None:
-            """
-            For an attribute to exist on a composed schema it must:
-            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
-            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
-
-            schema_requirements:
-            For an attribute to exist on a schema it must:
-            - be present in properties at the schema OR
-            - have additionalProperties unset (defaults additionalProperties = any type) OR
-            - have additionalProperties set
-            """
-            if name not in self.openapi_types:
-                raise ApiAttributeError(
-                    "{0} has no attribute '{1}'".format(
-                        type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
+        if isinstance(arg, str):
+            cls.__check_str_validations(arg, validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class UUIDBase:
+    @property
+    @functools.lru_cache()
+    def as_uuid_oapg(self) -> uuid.UUID:
+        return uuid.UUID(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                uuid.UUID(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Invalid value '{}' for type UUID at {}".format(arg, validation_metadata.path_to_item)
                 )
-        # attribute must be set on self and composed instances
-        self.set_attribute(name, value)
-        for model_instance in self._composed_instances:
-            setattr(model_instance, name, value)
-        if name not in self._var_name_to_model_instances:
-            # we assigned an additional property
-            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
-        return None
 
-    __unset_attribute_value__ = object()
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: typing.Optional[ValidationMetadata] = None,
+    ):
+        """
+        UUIDBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        # get the attribute from the correct instance
-        model_instances = self._var_name_to_model_instances.get(name)
-        values = []
-        # A composed model stores self and child (oneof/anyOf/allOf) models under
-        # self._var_name_to_model_instances.
-        # Any property must exist in self and all model instances
-        # The value stored in all model instances must be the same
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    v = model_instance._data_store[name]
-                    if v not in values:
-                        values.append(v)
-        len_values = len(values)
-        if len_values == 0:
-            return default
-        elif len_values == 1:
-            return values[0]
-        elif len_values > 1:
-            raise ApiValueError(
-                "Values stored for property {0} in {1} differ when looking "
-                "at self and self's composed instances. All values must be "
-                "the same".format(name, type(self).__name__),
-                [e for e in [self._path_to_item, name] if e]
-            )
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        value = self.get(name, self.__unset_attribute_value__)
-        if value is self.__unset_attribute_value__:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-            )
-        return value
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        model_instances = self._var_name_to_model_instances.get(
-            name, self._additional_properties_model_instances)
-
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    return True
 
-        return False
+class CustomIsoparser(isoparser):
 
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
+    @_takes_ascii
+    def parse_isodatetime(self, dt_str):
+        components, pos = self._parse_isodate(dt_str)
+        if len(dt_str) > pos:
+            if self._sep is None or dt_str[pos:pos + 1] == self._sep:
+                components += self._parse_isotime(dt_str[pos + 1:])
+            else:
+                raise ValueError('String contains unknown ISO components')
 
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-COERCION_INDEX_BY_TYPE = {
-    ModelComposed: 0,
-    ModelNormal: 1,
-    ModelSimple: 2,
-    none_type: 3,    # The type of 'None'.
-    list: 4,
-    dict: 5,
-    float: 6,
-    int: 7,
-    bool: 8,
-    datetime: 9,
-    date: 10,
-    str: 11,
-    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
-}
+        if len(components) > 3 and components[3] == 24:
+            components[3] = 0
+            return datetime(*components) + timedelta(days=1)
 
-# these are used to limit what type conversions we try to do
-# when we have a valid type already and we want to try converting
-# to another type
-UPCONVERSION_TYPE_PAIRS = (
-    (str, datetime),
-    (str, date),
-    (int, float),             # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
-    (list, ModelComposed),
-    (dict, ModelComposed),
-    (str, ModelComposed),
-    (int, ModelComposed),
-    (float, ModelComposed),
-    (list, ModelComposed),
-    (list, ModelNormal),
-    (dict, ModelNormal),
-    (str, ModelSimple),
-    (int, ModelSimple),
-    (float, ModelSimple),
-    (list, ModelSimple),
-)
+        if len(components) <= 3:
+            raise ValueError('Value is not a datetime')
 
-COERCIBLE_TYPE_PAIRS = {
-    False: (  # client instantiation of a model with client data
-        # (dict, ModelComposed),
-        # (list, ModelComposed),
-        # (dict, ModelNormal),
-        # (list, ModelNormal),
-        # (str, ModelSimple),
-        # (int, ModelSimple),
-        # (float, ModelSimple),
-        # (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        # (str, datetime),
-        # (str, date),
-        # (int, str),
-        # (float, str),
-    ),
-    True: (  # server -> client data
-        (dict, ModelComposed),
-        (list, ModelComposed),
-        (dict, ModelNormal),
-        (list, ModelNormal),
-        (str, ModelSimple),
-        (int, ModelSimple),
-        (float, ModelSimple),
-        (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        (str, datetime),
-        (str, date),
-        # (int, str),
-        # (float, str),
-        (str, file_type)
-    ),
-}
+        return datetime(*components)
 
+    @_takes_ascii
+    def parse_isodate(self, datestr):
+        components, pos = self._parse_isodate(datestr)
 
-def get_simple_class(input_value):
-    """Returns an input_value's simple class that we will use for type checking
-    Python2:
-    float and int will return int, where int is the python3 int backport
-    str and unicode will return str, where str is the python3 str backport
-    Note: float and int ARE both instances of int backport
-    Note: str_py2 and unicode_py2 are NOT both instances of str backport
+        if len(datestr) > pos:
+            raise ValueError('String contains invalid time components')
 
-    Args:
-        input_value (class/class_instance): the item for which we will return
-                                            the simple class
+        if len(components) > 3:
+            raise ValueError('String contains invalid time components')
+
+        return date(*components)
+
+
+DEFAULT_ISOPARSER = CustomIsoparser()
+
+
+class DateBase:
+    @property
+    @functools.lru_cache()
+    def as_date_oapg(self) -> date:
+        return DEFAULT_ISOPARSER.parse_isodate(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                DEFAULT_ISOPARSER.parse_isodate(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Value does not conform to the required ISO-8601 date format. "
+                    "Invalid value '{}' for type date at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: typing.Optional[ValidationMetadata] = None,
+    ):
+        """
+        DateBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class DateTimeBase:
+    @property
+    @functools.lru_cache()
+    def as_datetime_oapg(self) -> datetime:
+        return DEFAULT_ISOPARSER.parse_isodatetime(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                DEFAULT_ISOPARSER.parse_isodatetime(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Value does not conform to the required ISO-8601 datetime format. "
+                    "Invalid value '{}' for type datetime at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DateTimeBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class DecimalBase:
+    """
+    A class for storing decimals that are sent over the wire as strings
+    These schemas must remain based on StrBase rather than NumberBase
+    because picking base classes must be deterministic
     """
-    if isinstance(input_value, type):
-        # input_value is a class
-        return input_value
-    elif isinstance(input_value, tuple):
-        return tuple
-    elif isinstance(input_value, list):
-        return list
-    elif isinstance(input_value, dict):
-        return dict
-    elif isinstance(input_value, none_type):
-        return none_type
-    elif isinstance(input_value, file_type):
-        return file_type
-    elif isinstance(input_value, bool):
-        # this must be higher than the int check because
-        # isinstance(True, int) == True
-        return bool
-    elif isinstance(input_value, int):
-        return int
-    elif isinstance(input_value, datetime):
-        # this must be higher than the date check because
-        # isinstance(datetime_instance, date) == True
-        return datetime
-    elif isinstance(input_value, date):
-        return date
-    elif isinstance(input_value, str):
-        return str
-    return type(input_value)
 
+    @property
+    @functools.lru_cache()
+    def as_decimal_oapg(self) -> decimal.Decimal:
+        return decimal.Decimal(self)
 
-def check_allowed_values(allowed_values, input_variable_path, input_values):
-    """Raises an exception if the input_values are not allowed
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                decimal.Decimal(arg)
+                return True
+            except decimal.InvalidOperation:
+                raise ApiValueError(
+                    "Value cannot be converted to a decimal. "
+                    "Invalid value '{}' for type decimal at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-    Args:
-        allowed_values (dict): the allowed_values dict
-        input_variable_path (tuple): the path to the input variable
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking to see if they are in allowed_values
-    """
-    these_allowed_values = list(allowed_values[input_variable_path].values())
-    if (isinstance(input_values, list)
-            and not set(input_values).issubset(
-                set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values) - set(these_allowed_values))),
-        raise ApiValueError(
-            "Invalid values for `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (isinstance(input_values, dict)
-            and not set(
-                input_values.keys()).issubset(set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values.keys()) - set(these_allowed_values)))
-        raise ApiValueError(
-            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DecimalBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class NumberBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
+
+    @property
+    def as_int_oapg(self) -> int:
+        try:
+            return self._as_int
+        except AttributeError:
+            """
+            Note: for some numbers like 9.0 they could be represented as an
+            integer but our code chooses to store them as
+            >>> Decimal('9.0').as_tuple()
+            DecimalTuple(sign=0, digits=(9, 0), exponent=-1)
+            so we can tell that the value came from a float and convert it back to a float
+            during later serialization
+            """
+            if self.as_tuple().exponent < 0:
+                # this could be represented as an integer but should be represented as a float
+                # because that's what it was serialized from
+                raise ApiValueError(f'{self} is not an integer')
+            self._as_int = int(self)
+            return self._as_int
+
+    @property
+    def as_float_oapg(self) -> float:
+        try:
+            return self._as_float
+        except AttributeError:
+            if self.as_tuple().exponent >= 0:
+                raise ApiValueError(f'{self} is not a float')
+            self._as_float = float(self)
+            return self._as_float
+
+    @classmethod
+    def __check_numeric_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if cls._is_json_validation_enabled_oapg('multipleOf',
+                                      validation_metadata.configuration) and hasattr(cls.MetaOapg, 'multiple_of'):
+            multiple_of_value = cls.MetaOapg.multiple_of
+            if (not (float(arg) / multiple_of_value).is_integer()):
+                # Note 'multipleOf' will be as good as the floating point arithmetic.
+                cls._raise_validation_error_message_oapg(
+                    value=arg,
+                    constraint_msg="value must be a multiple of",
+                    constraint_value=multiple_of_value,
+                    path_to_item=validation_metadata.path_to_item
+                )
+
+        checking_max_or_min_values = any(
+            hasattr(cls.MetaOapg, validation_key) for validation_key in {
+                'exclusive_maximum',
+                'inclusive_maximum',
+                'exclusive_minimum',
+                'inclusive_minimum',
+            }
         )
-    elif (not isinstance(input_values, (list, dict))
-            and input_values not in these_allowed_values):
-        raise ApiValueError(
-            "Invalid value for `%s` (%s), must be one of %s" %
-            (
-                input_variable_path[0],
-                input_values,
-                these_allowed_values
+        if not checking_max_or_min_values:
+            return
+
+        if (cls._is_json_validation_enabled_oapg('exclusiveMaximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_maximum') and
+                arg >= cls.MetaOapg.exclusive_maximum):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="must be a value less than",
+                constraint_value=cls.MetaOapg.exclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('maximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_maximum') and
+                arg > cls.MetaOapg.inclusive_maximum):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="must be a value less than or equal to",
+                constraint_value=cls.MetaOapg.inclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('exclusiveMinimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_minimum') and
+                arg <= cls.MetaOapg.exclusive_minimum):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="must be a value greater than",
+                constraint_value=cls.MetaOapg.exclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_minimum') and
+                arg < cls.MetaOapg.inclusive_minimum):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="must be a value greater than or equal to",
+                constraint_value=cls.MetaOapg.inclusive_minimum,
+                path_to_item=validation_metadata.path_to_item
             )
-        )
 
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        NumberBase _validate_oapg
+        Validates that validations pass
+        """
+        if isinstance(arg, decimal.Decimal):
+            cls.__check_numeric_validations(arg, validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-def is_json_validation_enabled(schema_keyword, configuration=None):
-    """Returns true if JSON schema validation is enabled for the specified
-    validation keyword. This can be used to skip JSON schema structural validation
-    as requested in the configuration.
 
-    Args:
-        schema_keyword (string): the name of a JSON schema validation keyword.
-        configuration (Configuration): the configuration class.
-    """
+class ListBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
 
-    return (configuration is None or
-        not hasattr(configuration, '_disabled_client_side_validations') or
-        schema_keyword not in configuration._disabled_client_side_validations)
+    @classmethod
+    def __validate_items(cls, list_items, validation_metadata: ValidationMetadata):
+        """
+        Ensures that:
+        - values passed in for items are valid
+        Exceptions will be raised if:
+        - invalid arguments were passed in
 
+        Args:
+            list_items: the input list of items
 
-def check_validations(
-        validations, input_variable_path, input_values,
-        configuration=None):
-    """Raises an exception if the input_values are invalid
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
 
-    Args:
-        validations (dict): the validation dictionary.
-        input_variable_path (tuple): the path to the input variable.
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking.
-        configuration (Configuration): the configuration class.
-    """
-
-    if input_values is None:
-        return
-
-    current_validations = validations[input_variable_path]
-    if (is_json_validation_enabled('multipleOf', configuration) and
-            'multiple_of' in current_validations and
-            isinstance(input_values, (int, float)) and
-            not (float(input_values) / current_validations['multiple_of']).is_integer()):
-        # Note 'multipleOf' will be as good as the floating point arithmetic.
-        raise ApiValueError(
-            "Invalid value for `%s`, value must be a multiple of "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['multiple_of']
+        # if we have definitions for an items schema, use it
+        # otherwise accept anything
+        item_cls = getattr(cls.MetaOapg, 'items', UnsetAnyTypeSchema)
+        item_cls = cls._get_class_oapg(item_cls)
+        path_to_schemas = {}
+        for i, value in enumerate(list_items):
+            item_validation_metadata = ValidationMetadata(
+                from_server=validation_metadata.from_server,
+                configuration=validation_metadata.configuration,
+                path_to_item=validation_metadata.path_to_item+(i,),
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
+            if item_validation_metadata.validation_ran_earlier(item_cls):
+                add_deeper_validated_schemas(item_validation_metadata, path_to_schemas)
+                continue
+            other_path_to_schemas = item_cls._validate_oapg(
+                value, validation_metadata=item_validation_metadata)
+            update(path_to_schemas, other_path_to_schemas)
+        return path_to_schemas
+
+    @classmethod
+    def __check_tuple_validations(
+            cls, arg,
+            validation_metadata: ValidationMetadata):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if (cls._is_json_validation_enabled_oapg('maxItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_items') and
+                len(arg) > cls.MetaOapg.max_items):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="number of items must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_items,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_items') and
+                len(arg) < cls.MetaOapg.min_items):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="number of items must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_items,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('uniqueItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'unique_items') and cls.MetaOapg.unique_items and arg):
+            unique_items = set(arg)
+            if len(arg) > len(unique_items):
+                cls._raise_validation_error_message_oapg(
+                    value=arg,
+                    constraint_msg="duplicate items were found, and the tuple must not contain duplicates because",
+                    constraint_value='unique_items==True',
+                    path_to_item=validation_metadata.path_to_item
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        ListBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        if isinstance(arg, tuple):
+            cls.__check_tuple_validations(arg, validation_metadata)
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+        if not isinstance(arg, tuple):
+            return _path_to_schemas
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
+        other_path_to_schemas = cls.__validate_items(arg, validation_metadata=updated_vm)
+        update(_path_to_schemas, other_path_to_schemas)
+        return _path_to_schemas
 
-    if (is_json_validation_enabled('maxLength', configuration) and
-            'max_length' in current_validations and
-            len(input_values) > current_validations['max_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['max_length']
+    @classmethod
+    def _get_items_oapg(
+        cls: 'Schema',
+        arg: typing.List[typing.Any],
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        '''
+        ListBase _get_items_oapg
+        '''
+        cast_items = []
+
+        for i, value in enumerate(arg):
+            item_path_to_item = path_to_item + (i,)
+            item_cls = path_to_schemas[item_path_to_item]
+            new_value = item_cls._get_new_instance_without_conversion_oapg(
+                value,
+                item_path_to_item,
+                path_to_schemas
             )
-        )
+            cast_items.append(new_value)
 
-    if (is_json_validation_enabled('minLength', configuration) and
-            'min_length' in current_validations and
-            len(input_values) < current_validations['min_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be greater than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['min_length']
+        return cast_items
+
+
+class Discriminable:
+    MetaOapg: MetaOapgTyped
+
+    @classmethod
+    def _ensure_discriminator_value_present_oapg(cls, disc_property_name: str, validation_metadata: ValidationMetadata, *args):
+        if not args or args and disc_property_name not in args[0]:
+            # The input data does not contain the discriminator property
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '{}' is missing at path: {}".format(disc_property_name, validation_metadata.path_to_item)
             )
-        )
 
-    if (is_json_validation_enabled('maxItems', configuration) and
-            'max_items' in current_validations and
-            len(input_values) > current_validations['max_items']):
-        raise ApiValueError(
-            "Invalid value for `%s`, number of items must be less than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['max_items']
+    @classmethod
+    def get_discriminated_class_oapg(cls, disc_property_name: str, disc_payload_value: str):
+        """
+        Used in schemas with discriminators
+        """
+        if not hasattr(cls.MetaOapg, 'discriminator'):
+            return None
+        disc = cls.MetaOapg.discriminator()
+        if disc_property_name not in disc:
+            return None
+        discriminated_cls = disc[disc_property_name].get(disc_payload_value)
+        if discriminated_cls is not None:
+            return discriminated_cls
+        if not hasattr(cls, 'MetaOapg'):
+            return None
+        elif not (
+            hasattr(cls.MetaOapg, 'all_of') or
+            hasattr(cls.MetaOapg, 'one_of') or
+            hasattr(cls.MetaOapg, 'any_of')
+        ):
+            return None
+        # TODO stop traveling if a cycle is hit
+        if hasattr(cls.MetaOapg, 'all_of'):
+            for allof_cls in cls.MetaOapg.all_of():
+                discriminated_cls = allof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        if hasattr(cls.MetaOapg, 'one_of'):
+            for oneof_cls in cls.MetaOapg.one_of():
+                discriminated_cls = oneof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        if hasattr(cls.MetaOapg, 'any_of'):
+            for anyof_cls in cls.MetaOapg.any_of():
+                discriminated_cls = anyof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        return None
+
+
+class DictBase(Discriminable, ValidatorBase):
+
+    @classmethod
+    def __validate_arg_presence(cls, arg):
+        """
+        Ensures that:
+        - all required arguments are passed in
+        - the input variable names are valid
+            - present in properties or
+            - accepted because additionalProperties exists
+        Exceptions will be raised if:
+        - invalid arguments were passed in
+            - a var_name is invalid if additional_properties == NotAnyTypeSchema
+            and var_name not in properties.__annotations__
+        - required properties were not passed in
+
+        Args:
+            arg: the input dict
+
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
+        seen_required_properties = set()
+        invalid_arguments = []
+        required_property_names = getattr(cls.MetaOapg, 'required', set())
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
+        for property_name in arg:
+            if property_name in required_property_names:
+                seen_required_properties.add(property_name)
+            elif property_name in property_annotations:
+                continue
+            elif additional_properties is not NotAnyTypeSchema:
+                continue
+            else:
+                invalid_arguments.append(property_name)
+        missing_required_arguments = list(required_property_names - seen_required_properties)
+        if missing_required_arguments:
+            missing_required_arguments.sort()
+            raise ApiTypeError(
+                "{} is missing {} required argument{}: {}".format(
+                    cls.__name__,
+                    len(missing_required_arguments),
+                    "s" if len(missing_required_arguments) > 1 else "",
+                    missing_required_arguments
+                )
             )
-        )
+        if invalid_arguments:
+            invalid_arguments.sort()
+            raise ApiTypeError(
+                "{} was passed {} invalid argument{}: {}".format(
+                    cls.__name__,
+                    len(invalid_arguments),
+                    "s" if len(invalid_arguments) > 1 else "",
+                    invalid_arguments
+                )
+            )
+
+    @classmethod
+    def __validate_args(cls, arg, validation_metadata: ValidationMetadata):
+        """
+        Ensures that:
+        - values passed in for properties are valid
+        Exceptions will be raised if:
+        - invalid arguments were passed in
 
-    if (is_json_validation_enabled('minItems', configuration) and
-            'min_items' in current_validations and
-            len(input_values) < current_validations['min_items']):
-        raise ValueError(
-            "Invalid value for `%s`, number of items must be greater than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['min_items']
+        Args:
+            arg: the input dict
+
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
+        path_to_schemas = {}
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
+        for property_name, value in arg.items():
+            path_to_item = validation_metadata.path_to_item+(property_name,)
+            if property_name in property_annotations:
+                schema = property_annotations[property_name]
+            elif additional_properties is not NotAnyTypeSchema:
+                if additional_properties is UnsetAnyTypeSchema:
+                    """
+                    If additionalProperties is unset and this path_to_item does not yet have
+                    any validations on it, validate it.
+                    If it already has validations on it, skip this validation.
+                    """
+                    if path_to_item in path_to_schemas:
+                        continue
+                schema = additional_properties
+            else:
+                raise ApiTypeError('Unable to find schema for value={} in class={} at path_to_item={}'.format(
+                    value, cls, validation_metadata.path_to_item+(property_name,)
+                ))
+            schema = cls._get_class_oapg(schema)
+            arg_validation_metadata = ValidationMetadata(
+                from_server=validation_metadata.from_server,
+                configuration=validation_metadata.configuration,
+                path_to_item=path_to_item,
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
-        )
+            if arg_validation_metadata.validation_ran_earlier(schema):
+                add_deeper_validated_schemas(arg_validation_metadata, path_to_schemas)
+                continue
+            other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
+            update(path_to_schemas, other_path_to_schemas)
+        return path_to_schemas
 
-    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
-             'inclusive_minimum')
-    if (any(item in current_validations for item in items)):
-        if isinstance(input_values, list):
-            max_val = max(input_values)
-            min_val = min(input_values)
-        elif isinstance(input_values, dict):
-            max_val = max(input_values.values())
-            min_val = min(input_values.values())
-        else:
-            max_val = input_values
-            min_val = input_values
+    @classmethod
+    def __check_dict_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if (cls._is_json_validation_enabled_oapg('maxProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_properties') and
+                len(arg) > cls.MetaOapg.max_properties):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="number of properties must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_properties,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_properties') and
+                len(arg) < cls.MetaOapg.min_properties):
+            cls._raise_validation_error_message_oapg(
+                value=arg,
+                constraint_msg="number of properties must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_properties,
+                path_to_item=validation_metadata.path_to_item
+            )
 
-    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
-            'exclusive_maximum' in current_validations and
-            max_val >= current_validations['exclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than `%s`" % (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DictBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        if isinstance(arg, frozendict.frozendict):
+            cls.__check_dict_validations(arg, validation_metadata)
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+        if not isinstance(arg, frozendict.frozendict):
+            return _path_to_schemas
+        cls.__validate_arg_presence(arg)
+        other_path_to_schemas = cls.__validate_args(arg, validation_metadata=validation_metadata)
+        update(_path_to_schemas, other_path_to_schemas)
+        try:
+            discriminator = cls.MetaOapg.discriminator()
+        except AttributeError:
+            return _path_to_schemas
+        # discriminator exists
+        disc_prop_name = list(discriminator.keys())[0]
+        cls._ensure_discriminator_value_present_oapg(disc_prop_name, validation_metadata, arg)
+        discriminated_cls = cls.get_discriminated_class_oapg(
+            disc_property_name=disc_prop_name, disc_payload_value=arg[disc_prop_name])
+        if discriminated_cls is None:
+            raise ApiValueError(
+                "Invalid discriminator value was passed in to {}.{} Only the values {} are allowed at {}".format(
+                    cls.__name__,
+                    disc_prop_name,
+                    list(discriminator[disc_prop_name].keys()),
+                    validation_metadata.path_to_item + (disc_prop_name,)
+                )
             )
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
+        if updated_vm.validation_ran_earlier(discriminated_cls):
+            add_deeper_validated_schemas(updated_vm, _path_to_schemas)
+            return _path_to_schemas
+        other_path_to_schemas = discriminated_cls._validate_oapg(arg, validation_metadata=updated_vm)
+        update(_path_to_schemas, other_path_to_schemas)
+        return _path_to_schemas
 
-    if (is_json_validation_enabled('maximum', configuration) and
-            'inclusive_maximum' in current_validations and
-            max_val > current_validations['inclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_maximum']
+    @classmethod
+    def _get_properties_oapg(
+        cls,
+        arg: typing.Dict[str, typing.Any],
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        """
+        DictBase _get_properties_oapg, this is how properties are set
+        These values already passed validation
+        """
+        dict_items = {}
+
+        for property_name_js, value in arg.items():
+            property_path_to_item = path_to_item + (property_name_js,)
+            property_cls = path_to_schemas[property_path_to_item]
+            new_value = property_cls._get_new_instance_without_conversion_oapg(
+                value,
+                property_path_to_item,
+                path_to_schemas
             )
-        )
+            dict_items[property_name_js] = new_value
 
-    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
-            'exclusive_minimum' in current_validations and
-            min_val <= current_validations['exclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than `%s`" %
-            (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
+        return dict_items
+
+    def __setattr__(self, name: str, value: typing.Any):
+        if not isinstance(self, FileIO):
+            raise AttributeError('property setting not supported on immutable instances')
+
+    def __getattr__(self, name: str):
+        """
+        for instance.name access
+        Properties are only type hinted for required properties
+        so that hasattr(instance, 'optionalProp') is False when that key is not present
+        """
+        if not isinstance(self, frozendict.frozendict):
+            return super().__getattr__(name)
+        if name not in self.__class__.__annotations__:
+            raise AttributeError(f"{self} has no attribute '{name}'")
+        try:
+            value = self[name]
+            return value
+        except KeyError as ex:
+            raise AttributeError(str(ex))
+
+    def __getitem__(self, name: str):
+        """
+        dict_instance[name] accessor
+        key errors thrown
+        """
+        if not isinstance(self, frozendict.frozendict):
+            return super().__getattr__(name)
+        return super().__getitem__(name)
+
+    def get_item_oapg(self, name: str) -> typing.Union['AnyTypeSchema', Unset]:
+        # dict_instance[name] accessor
+        if not isinstance(self, frozendict.frozendict):
+            raise NotImplementedError()
+        try:
+            return super().__getitem__(name)
+        except KeyError:
+            return unset
+
+
+def cast_to_allowed_types(
+    arg: typing.Union[str, date, datetime, uuid.UUID, decimal.Decimal, int, float, None, dict, frozendict.frozendict, list, tuple, bytes, Schema, io.FileIO, io.BufferedReader],
+    from_server: bool,
+    validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]],
+    path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+) -> typing.Union[frozendict.frozendict, tuple, decimal.Decimal, str, bytes, BoolClass, NoneClass, FileIO]:
+    """
+    Casts the input payload arg into the allowed types
+    The input validated_path_to_schemas is mutated by running this function
+
+    When from_server is False then
+    - date/datetime is cast to str
+    - int/float is cast to Decimal
+
+    If a Schema instance is passed in it is converted back to a primitive instance because
+    One may need to validate that data to the original Schema class AND additional different classes
+    those additional classes will need to be added to the new manufactured class for that payload
+    If the code didn't do this and kept the payload as a Schema instance it would fail to validate to other
+    Schema classes and the code wouldn't be able to mfg a new class that includes all valid schemas
+    TODO: store the validated schema classes in validation_metadata
+
+    Args:
+        arg: the payload
+        from_server: whether this payload came from the server or not
+        validated_path_to_schemas: a dict that stores the validated classes at any path location in the payload
+    """
+    if isinstance(arg, Schema):
+        # store the already run validations
+        schema_classes = set()
+        for cls in arg.__class__.__bases__:
+            if cls is Singleton:
+                # Skip Singleton
+                continue
+            schema_classes.add(cls)
+        validated_path_to_schemas[path_to_item] = schema_classes
+
+    type_error = ApiTypeError(f"Invalid type. Required value type is str and passed type was {type(arg)} at {path_to_item}")
+    if isinstance(arg, str):
+        return str(arg)
+    elif isinstance(arg, (dict, frozendict.frozendict)):
+        return frozendict.frozendict({key: cast_to_allowed_types(val, from_server, validated_path_to_schemas, path_to_item + (key,)) for key, val in arg.items()})
+    elif isinstance(arg, (bool, BoolClass)):
+        """
+        this check must come before isinstance(arg, (int, float))
+        because isinstance(True, int) is True
+        """
+        if arg:
+            return BoolClass.TRUE
+        return BoolClass.FALSE
+    elif isinstance(arg, int):
+        return decimal.Decimal(arg)
+    elif isinstance(arg, float):
+        decimal_from_float = decimal.Decimal(arg)
+        if decimal_from_float.as_integer_ratio()[1] == 1:
+            # 9.0 -> Decimal('9.0')
+            # 3.4028234663852886e+38 -> Decimal('340282346638528859811704183484516925440.0')
+            return decimal.Decimal(str(decimal_from_float)+'.0')
+        return decimal_from_float
+    elif isinstance(arg, (tuple, list)):
+        return tuple([cast_to_allowed_types(item, from_server, validated_path_to_schemas, path_to_item + (i,)) for i, item in enumerate(arg)])
+    elif isinstance(arg, (none_type, NoneClass)):
+        return NoneClass.NONE
+    elif isinstance(arg, (date, datetime)):
+        if not from_server:
+            return arg.isoformat()
+        raise type_error
+    elif isinstance(arg, uuid.UUID):
+        if not from_server:
+            return str(arg)
+        raise type_error
+    elif isinstance(arg, decimal.Decimal):
+        return decimal.Decimal(arg)
+    elif isinstance(arg, bytes):
+        return bytes(arg)
+    elif isinstance(arg, (io.FileIO, io.BufferedReader)):
+        return FileIO(arg)
+    raise ValueError('Invalid type passed in got input={} type={}'.format(arg, type(arg)))
+
+
+class ComposedBase(Discriminable):
+
+    @classmethod
+    def __get_allof_classes(cls, arg, validation_metadata: ValidationMetadata):
+        path_to_schemas = defaultdict(set)
+        for allof_cls in cls.MetaOapg.all_of():
+            if validation_metadata.validation_ran_earlier(allof_cls):
+                add_deeper_validated_schemas(validation_metadata, path_to_schemas)
+                continue
+            other_path_to_schemas = allof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            update(path_to_schemas, other_path_to_schemas)
+        return path_to_schemas
+
+    @classmethod
+    def __get_oneof_class(
+        cls,
+        arg,
+        discriminated_cls,
+        validation_metadata: ValidationMetadata,
+    ):
+        oneof_classes = []
+        path_to_schemas = defaultdict(set)
+        for oneof_cls in cls.MetaOapg.one_of():
+            if oneof_cls in path_to_schemas[validation_metadata.path_to_item]:
+                oneof_classes.append(oneof_cls)
+                continue
+            if validation_metadata.validation_ran_earlier(oneof_cls):
+                oneof_classes.append(oneof_cls)
+                add_deeper_validated_schemas(validation_metadata, path_to_schemas)
+                continue
+            try:
+                path_to_schemas = oneof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            except (ApiValueError, ApiTypeError) as ex:
+                if discriminated_cls is not None and oneof_cls is discriminated_cls:
+                    raise ex
+                continue
+            oneof_classes.append(oneof_cls)
+        if not oneof_classes:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of {}. None "
+                "of the oneOf schemas matched the input data.".format(cls)
             )
-        )
+        elif len(oneof_classes) > 1:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of {}. Multiple "
+                "oneOf schemas {} matched the inputs, but a max of one is allowed.".format(cls, oneof_classes)
+            )
+        # exactly one class matches
+        return path_to_schemas
 
-    if (is_json_validation_enabled('minimum', configuration) and
-            'inclusive_minimum' in current_validations and
-            min_val < current_validations['inclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than or equal "
-            "to `%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_minimum']
+    @classmethod
+    def __get_anyof_classes(
+        cls,
+        arg,
+        discriminated_cls,
+        validation_metadata: ValidationMetadata
+    ):
+        anyof_classes = []
+        path_to_schemas = defaultdict(set)
+        for anyof_cls in cls.MetaOapg.any_of():
+            if validation_metadata.validation_ran_earlier(anyof_cls):
+                anyof_classes.append(anyof_cls)
+                add_deeper_validated_schemas(validation_metadata, path_to_schemas)
+                continue
+
+            try:
+                other_path_to_schemas = anyof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            except (ApiValueError, ApiTypeError) as ex:
+                if discriminated_cls is not None and anyof_cls is discriminated_cls:
+                    raise ex
+                continue
+            anyof_classes.append(anyof_cls)
+            update(path_to_schemas, other_path_to_schemas)
+        if not anyof_classes:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of {}. None "
+                "of the anyOf schemas matched the input data.".format(cls)
             )
+        return path_to_schemas
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        ComposedBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        # validation checking on types, validations, and enums
+        path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
-    flags = current_validations.get('regex', {}).get('flags', 0)
-    if (is_json_validation_enabled('pattern', configuration) and
-            'regex' in current_validations and
-            not re.search(current_validations['regex']['pattern'],
-                          input_values, flags=flags)):
-        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
-                    input_variable_path[0],
-                    current_validations['regex']['pattern']
+
+        # process composed schema
+        discriminator = None
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'discriminator'):
+            discriminator = cls.MetaOapg.discriminator()
+        discriminated_cls = None
+        if discriminator and arg and isinstance(arg, frozendict.frozendict):
+            disc_property_name = list(discriminator.keys())[0]
+            cls._ensure_discriminator_value_present_oapg(disc_property_name, updated_vm, arg)
+            # get discriminated_cls by looking at the dict in the current class
+            discriminated_cls = cls.get_discriminated_class_oapg(
+                disc_property_name=disc_property_name, disc_payload_value=arg[disc_property_name])
+            if discriminated_cls is None:
+                raise ApiValueError(
+                    "Invalid discriminator value '{}' was passed in to {}.{} Only the values {} are allowed at {}".format(
+                        arg[disc_property_name],
+                        cls.__name__,
+                        disc_property_name,
+                        list(discriminator[disc_property_name].keys()),
+                        updated_vm.path_to_item + (disc_property_name,)
+                    )
                 )
-        if flags != 0:
-            # Don't print the regex flags if the flags are not
-            # specified in the OAS document.
-            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
-        raise ApiValueError(err_msg)
 
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'all_of'):
+            other_path_to_schemas = cls.__get_allof_classes(arg, validation_metadata=updated_vm)
+            update(path_to_schemas, other_path_to_schemas)
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'one_of'):
+            other_path_to_schemas = cls.__get_oneof_class(
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
+            )
+            update(path_to_schemas, other_path_to_schemas)
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'any_of'):
+            other_path_to_schemas = cls.__get_anyof_classes(
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
+            )
+            update(path_to_schemas, other_path_to_schemas)
+        not_cls = None
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'not_schema'):
+            not_cls = cls.MetaOapg.not_schema
+            not_cls = cls._get_class_oapg(not_cls)
+        if not_cls:
+            other_path_to_schemas = None
+            not_exception = ApiValueError(
+                "Invalid value '{}' was passed in to {}. Value is invalid because it is disallowed by {}".format(
+                    arg,
+                    cls.__name__,
+                    not_cls.__name__,
+                )
+            )
+            if updated_vm.validation_ran_earlier(not_cls):
+                raise not_exception
 
-def order_response_types(required_types):
-    """Returns the required types sorted in coercion order
+            try:
+                other_path_to_schemas = not_cls._validate_oapg(arg, validation_metadata=updated_vm)
+            except (ApiValueError, ApiTypeError):
+                pass
+            if other_path_to_schemas:
+                raise not_exception
 
-    Args:
-        required_types (list/tuple): collection of classes or instance of
-            list or dict with class information inside it.
+        if discriminated_cls is not None and not updated_vm.validation_ran_earlier(discriminated_cls):
+            # TODO use an exception from this package here
+            add_deeper_validated_schemas(updated_vm, path_to_schemas)
+            assert discriminated_cls in path_to_schemas[updated_vm.path_to_item]
+        return path_to_schemas
+
+
+# DictBase, ListBase, NumberBase, StrBase, BoolBase, NoneBase
+class ComposedSchema(
+    ComposedBase,
+    DictBase,
+    ListBase,
+    NumberBase,
+    StrBase,
+    BoolBase,
+    NoneBase,
+    Schema,
+    NoneFrozenDictTupleStrDecimalBoolMixin
+):
+    @classmethod
+    def from_openapi_data_oapg(cls, *args: typing.Any, _configuration: typing.Optional[Configuration] = None, **kwargs):
+        if not args:
+            if not kwargs:
+                raise ApiTypeError('{} is missing required input data in args or kwargs'.format(cls.__name__))
+            args = (kwargs, )
+        return super().from_openapi_data_oapg(args[0], _configuration=_configuration)
 
-    Returns:
-        (list): coercion order sorted collection of classes or instance
-            of list or dict with class information inside it.
-    """
-
-    def index_getter(class_or_instance):
-        if isinstance(class_or_instance, list):
-            return COERCION_INDEX_BY_TYPE[list]
-        elif isinstance(class_or_instance, dict):
-            return COERCION_INDEX_BY_TYPE[dict]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelComposed)):
-            return COERCION_INDEX_BY_TYPE[ModelComposed]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelNormal)):
-            return COERCION_INDEX_BY_TYPE[ModelNormal]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelSimple)):
-            return COERCION_INDEX_BY_TYPE[ModelSimple]
-        elif class_or_instance in COERCION_INDEX_BY_TYPE:
-            return COERCION_INDEX_BY_TYPE[class_or_instance]
-        raise ApiValueError("Unsupported type: %s" % class_or_instance)
-
-    sorted_types = sorted(
-        required_types,
-        key=lambda class_or_instance: index_getter(class_or_instance)
-    )
-    return sorted_types
-
-
-def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
-                       must_convert=True):
-    """Only keeps the type conversions that are possible
 
-    Args:
-        required_types_classes (tuple): tuple of classes that are required
-                          these should be ordered by COERCION_INDEX_BY_TYPE
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        current_item (any): the current item (input data) to be converted
-
-    Keyword Args:
-        must_convert (bool): if True the item to convert is of the wrong
-                          type and we want a big list of coercibles
-                          if False, we want a limited list of coercibles
-
-    Returns:
-        (list): the remaining coercible required types, classes only
-    """
-    current_type_simple = get_simple_class(current_item)
-
-    results_classes = []
-    for required_type_class in required_types_classes:
-        # convert our models to OpenApiModel
-        required_type_class_simplified = required_type_class
-        if isinstance(required_type_class_simplified, type):
-            if issubclass(required_type_class_simplified, ModelComposed):
-                required_type_class_simplified = ModelComposed
-            elif issubclass(required_type_class_simplified, ModelNormal):
-                required_type_class_simplified = ModelNormal
-            elif issubclass(required_type_class_simplified, ModelSimple):
-                required_type_class_simplified = ModelSimple
+class ListSchema(
+    ListBase,
+    Schema,
+    TupleMixin
+):
 
-        if required_type_class_simplified == current_type_simple:
-            # don't consider converting to one's own class
-            continue
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.List[typing.Any], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-        class_pair = (current_type_simple, required_type_class_simplified)
-        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
-            results_classes.append(required_type_class)
-        elif class_pair in UPCONVERSION_TYPE_PAIRS:
-            results_classes.append(required_type_class)
-    return results_classes
-
-def get_discriminated_classes(cls):
-    """
-    Returns all the classes that a discriminator converts to
-    TODO: lru_cache this
-    """
-    possible_classes = []
-    key = list(cls.discriminator.keys())[0]
-    if is_type_nullable(cls):
-        possible_classes.append(cls)
-    for discr_cls in cls.discriminator[key].values():
-        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
-            possible_classes.extend(get_discriminated_classes(discr_cls))
-        else:
-            possible_classes.append(discr_cls)
-    return possible_classes
+    def __new__(cls, _arg: typing.Union[typing.List[typing.Any], typing.Tuple[typing.Any]], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
 
-def get_possible_classes(cls, from_server_context):
-    # TODO: lru_cache this
-    possible_classes = [cls]
-    if from_server_context:
-        return possible_classes
-    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-        possible_classes = []
-        possible_classes.extend(get_discriminated_classes(cls))
-    elif issubclass(cls, ModelComposed):
-        possible_classes.extend(composed_model_input_classes(cls))
-    return possible_classes
-
-
-def get_required_type_classes(required_types_mixed, spec_property_naming):
-    """Converts the tuple required_types into a tuple and a dict described
-    below
+class NoneSchema(
+    NoneBase,
+    Schema,
+    NoneMixin
+):
 
-    Args:
-        required_types_mixed (tuple/list): will contain either classes or
-            instance of list or dict
-        spec_property_naming (bool): if True these values came from the
-            server, and we use the data types in our endpoints.
-            If False, we are client side and we need to include
-            oneOf and discriminator classes inside the data types in our endpoints
-
-    Returns:
-        (valid_classes, dict_valid_class_to_child_types_mixed):
-            valid_classes (tuple): the valid classes that the current item
-                                   should be
-            dict_valid_class_to_child_types_mixed (dict):
-                valid_class (class): this is the key
-                child_types_mixed (list/dict/tuple): describes the valid child
-                    types
-    """
-    valid_classes = []
-    child_req_types_by_current_type = {}
-    for required_type in required_types_mixed:
-        if isinstance(required_type, list):
-            valid_classes.append(list)
-            child_req_types_by_current_type[list] = required_type
-        elif isinstance(required_type, tuple):
-            valid_classes.append(tuple)
-            child_req_types_by_current_type[tuple] = required_type
-        elif isinstance(required_type, dict):
-            valid_classes.append(dict)
-            child_req_types_by_current_type[dict] = required_type[str]
-        else:
-            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
-    return tuple(valid_classes), child_req_types_by_current_type
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: None, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
+    def __new__(cls, _arg: None, **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
-def change_keys_js_to_python(input_dict, model_class):
+
+class NumberSchema(
+    NumberBase,
+    Schema,
+    DecimalMixin
+):
+    """
+    This is used for type: number with no format
+    Both integers AND floats are accepted
     """
-    Converts from javascript_key keys in the input_dict to python_keys in
-    the output dict using the mapping in model_class.
-    If the input_dict contains a key which does not declared in the model_class,
-    the key is added to the output dict as is. The assumption is the model_class
-    may have undeclared properties (additionalProperties attribute in the OAS
-    document).
-    """
-
-    if getattr(model_class, 'attribute_map', None) is None:
-        return input_dict
-    output_dict = {}
-    reversed_attr_map = {value: key for key, value in
-                         model_class.attribute_map.items()}
-    for javascript_key, value in input_dict.items():
-        python_key = reversed_attr_map.get(javascript_key)
-        if python_key is None:
-            # if the key is unknown, it is in error or it is an
-            # additionalProperties variable
-            python_key = javascript_key
-        output_dict[python_key] = value
-    return output_dict
-
-
-def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
-    error_msg = type_error_message(
-        var_name=path_to_item[-1],
-        var_value=var_value,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-    return ApiTypeError(
-        error_msg,
-        path_to_item=path_to_item,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-
-
-def deserialize_primitive(data, klass, path_to_item):
-    """Deserializes string to primitive type.
-
-    :param data: str/int/float
-    :param klass: str/class the class to convert to
-
-    :return: int, float, str, bool, date, datetime
-    """
-    additional_message = ""
-    try:
-        if klass in {datetime, date}:
-            additional_message = (
-                "If you need your parameter to have a fallback "
-                "string value, please set its type as `type: {}` in your "
-                "spec. That allows the value to be any type. "
-            )
-            if klass == datetime:
-                if len(data) < 8:
-                    raise ValueError("This is not a datetime")
-                # The string should be in iso8601 datetime format.
-                parsed_datetime = parse(data)
-                date_only = (
-                    parsed_datetime.hour == 0 and
-                    parsed_datetime.minute == 0 and
-                    parsed_datetime.second == 0 and
-                    parsed_datetime.tzinfo is None and
-                    8 <= len(data) <= 10
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.Union[int, float], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+    def __new__(cls, _arg: typing.Union[decimal.Decimal, int, float], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
+
+
+class IntBase:
+    @property
+    def as_int_oapg(self) -> int:
+        try:
+            return self._as_int
+        except AttributeError:
+            self._as_int = int(self)
+            return self._as_int
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+
+            denominator = arg.as_integer_ratio()[-1]
+            if denominator != 1:
+                raise ApiValueError(
+                    "Invalid value '{}' for type integer at {}".format(arg, validation_metadata.path_to_item)
                 )
-                if date_only:
-                    raise ValueError("This is a date, not a datetime")
-                return parsed_datetime
-            elif klass == date:
-                if len(data) < 8:
-                    raise ValueError("This is not a date")
-                return parse(data).date()
-        else:
-            converted_value = klass(data)
-            if isinstance(data, str) and klass == float:
-                if str(converted_value) != data:
-                    # '7' -> 7.0 -> '7.0' != '7'
-                    raise ValueError('This is not a float')
-            return converted_value
-    except (OverflowError, ValueError) as ex:
-        # parse can raise OverflowError
-        raise ApiValueError(
-            "{0}Failed to parse {1} as {2}".format(
-                additional_message, repr(data), klass.__name__
-            ),
-            path_to_item=path_to_item
-        ) from ex
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        IntBase _validate_oapg
+        TODO what about types = (int, number) -> IntBase, NumberBase? We could drop int and keep number only
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
-def get_discriminator_class(model_class,
-                            discr_name,
-                            discr_value, cls_visited):
-    """Returns the child class specified by the discriminator.
+class IntSchema(IntBase, NumberSchema):
 
-    Args:
-        model_class (OpenApiModel): the model class.
-        discr_name (string): the name of the discriminator property.
-        discr_value (any): the discriminator value.
-        cls_visited (list): list of model classes that have been visited.
-            Used to determine the discriminator class without
-            visiting circular references indefinitely.
-
-    Returns:
-        used_model_class (class/None): the chosen child class that will be used
-            to deserialize the data, for example dog.Dog.
-            If a class is not found, None is returned.
-    """
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: int, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    if model_class in cls_visited:
-        # The class has already been visited and no suitable class was found.
-        return None
-    cls_visited.append(model_class)
-    used_model_class = None
-    if discr_name in model_class.discriminator:
-        class_name_to_discr_class = model_class.discriminator[discr_name]
-        used_model_class = class_name_to_discr_class.get(discr_value)
-    if used_model_class is None:
-        # We didn't find a discriminated class in class_name_to_discr_class.
-        # So look in the ancestor or descendant discriminators
-        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
-        # or ancestor (allOf).
-        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
-        #   hierarchy, the discriminator mappings may be defined at any level
-        #   in the hierarchy.
-        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
-        #   if we try to make BasquePig from mammal, we need to travel through
-        #   the oneOf descendant discriminators to find BasquePig
-        descendant_classes =  model_class._composed_schemas.get('oneOf', ()) + \
-            model_class._composed_schemas.get('anyOf', ())
-        ancestor_classes = model_class._composed_schemas.get('allOf', ())
-        possible_classes = descendant_classes + ancestor_classes
-        for cls in possible_classes:
-            # Check if the schema has inherited discriminators.
-            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-                used_model_class = get_discriminator_class(
-                                    cls, discr_name, discr_value, cls_visited)
-                if used_model_class is not None:
-                    return used_model_class
-    return used_model_class
-
-
-def deserialize_model(model_data, model_class, path_to_item, check_type,
-                      configuration, spec_property_naming):
-    """Deserializes model_data to model instance.
+    def __new__(cls, _arg: typing.Union[decimal.Decimal, int], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
-    Args:
-        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
-        model_class (OpenApiModel): the model class
-        path_to_item (list): path to the model in the received data
-        check_type (bool): whether to check the data tupe for the values in
-            the model
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-
-    Returns:
-        model instance
-
-    Raise:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-
-    kw_args = dict(_check_type=check_type,
-                   _path_to_item=path_to_item,
-                   _configuration=configuration,
-                   _spec_property_naming=spec_property_naming)
-
-    if issubclass(model_class, ModelSimple):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-    elif isinstance(model_data, list):
-        return model_class._new_from_openapi_data(*model_data, **kw_args)
-    if isinstance(model_data, dict):
-        kw_args.update(model_data)
-        return model_class._new_from_openapi_data(**kw_args)
-    elif isinstance(model_data, PRIMITIVE_TYPES):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
 
+class Int32Base:
+    __inclusive_minimum = decimal.Decimal(-2147483648)
+    __inclusive_maximum = decimal.Decimal(2147483647)
 
-def deserialize_file(response_data, configuration, content_disposition=None):
-    """Deserializes body to file
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type int32 at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-    Saves response body into a file in a temporary folder,
-    using the filename from the `Content-Disposition` header if provided.
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Int32Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-    Args:
-        param response_data (str):  the file data to write
-        configuration (Configuration): the instance to use to convert files
 
-    Keyword Args:
-        content_disposition (str):  the value of the Content-Disposition
-            header
-
-    Returns:
-        (file_type): the deserialized file which is open
-            The user is responsible for closing and reading the file
-    """
-    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
-    os.close(fd)
-    os.remove(path)
-
-    if content_disposition:
-        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                             content_disposition).group(1)
-        path = os.path.join(os.path.dirname(path), filename)
-
-    with open(path, "wb") as f:
-        if isinstance(response_data, str):
-            # change str to bytes so we can write it
-            response_data = response_data.encode('utf-8')
-        f.write(response_data)
-
-    f = open(path, "rb")
-    return f
-
-
-def attempt_convert_item(input_value, valid_classes, path_to_item,
-                         configuration, spec_property_naming, key_type=False,
-                         must_convert=False, check_type=True):
-    """
-    Args:
-        input_value (any): the data to convert
-        valid_classes (any): the classes that are valid
-        path_to_item (list): the path to the item to convert
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        key_type (bool): if True we need to convert a key type (not supported)
-        must_convert (bool): if True we must convert
-        check_type (bool): if True we check the type or the returned data in
-            ModelComposed/ModelNormal/ModelSimple instances
-
-    Returns:
-        instance (any) the fixed item
-
-    Raises:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-    valid_classes_ordered = order_response_types(valid_classes)
-    valid_classes_coercible = remove_uncoercible(
-        valid_classes_ordered, input_value, spec_property_naming)
-    if not valid_classes_coercible or key_type:
-        # we do not handle keytype errors, json will take care
-        # of this for us
-        if configuration is None or not configuration.discard_unknown_keys:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=key_type)
-    for valid_class in valid_classes_coercible:
-        try:
-            if issubclass(valid_class, OpenApiModel):
-                return deserialize_model(input_value, valid_class,
-                                         path_to_item, check_type,
-                                         configuration, spec_property_naming)
-            elif valid_class == file_type:
-                return deserialize_file(input_value, configuration)
-            return deserialize_primitive(input_value, valid_class,
-                                         path_to_item)
-        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
-            if must_convert:
-                raise conversion_exc
-            # if we have conversion errors when must_convert == False
-            # we ignore the exception and move on to the next class
-            continue
-    # we were unable to convert, must_convert == False
-    return input_value
+class Int32Schema(
+    Int32Base,
+    IntSchema
+):
+    pass
 
 
-def is_type_nullable(input_type):
-    """
-    Returns true if None is an allowed value for the specified input_type.
+class Int64Base:
+    __inclusive_minimum = decimal.Decimal(-9223372036854775808)
+    __inclusive_maximum = decimal.Decimal(9223372036854775807)
 
-    A type is nullable if at least one of the following conditions is true:
-    1. The OAS 'nullable' attribute has been specified,
-    1. The type is the 'null' type,
-    1. The type is a anyOf/oneOf composed schema, and a child schema is
-       the 'null' type.
-    Args:
-        input_type (type): the class of the input_value that we are
-            checking
-    Returns:
-        bool
-    """
-    if input_type is none_type:
-        return True
-    if issubclass(input_type, OpenApiModel) and input_type._nullable:
-        return True
-    if issubclass(input_type, ModelComposed):
-        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
-        for t in input_type._composed_schemas.get('oneOf', ()):
-            if is_type_nullable(t): return True
-        for t in input_type._composed_schemas.get('anyOf', ()):
-            if is_type_nullable(t): return True
-    return False
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type int64 at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Int64Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class Int64Schema(
+    Int64Base,
+    IntSchema
+):
+    pass
+
+
+class Float32Base:
+    __inclusive_minimum = decimal.Decimal(-3.4028234663852886e+38)
+    __inclusive_maximum = decimal.Decimal(3.4028234663852886e+38)
 
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type float at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Float32Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class Float32Schema(
+    Float32Base,
+    NumberSchema
+):
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+
+class Float64Base:
+    __inclusive_minimum = decimal.Decimal(-1.7976931348623157E+308)
+    __inclusive_maximum = decimal.Decimal(1.7976931348623157E+308)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type double at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-def is_valid_type(input_class_simple, valid_classes):
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Float64Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+class Float64Schema(
+    Float64Base,
+    NumberSchema
+):
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
+        # todo check format
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+
+class StrSchema(
+    StrBase,
+    Schema,
+    StrMixin
+):
+    """
+    date + datetime string types must inherit from this class
+    That is because one can validate a str payload as both:
+    - type: string (format unset)
+    - type: string, format: date
     """
-    Args:
-        input_class_simple (class): the class of the input_value that we are
-            checking
-        valid_classes (tuple): the valid classes that the current item
-            should be
-    Returns:
-        bool
-    """
-    if issubclass(input_class_simple, OpenApiModel) and \
-        valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
-        return True
-    valid_type = input_class_simple in valid_classes
-    if not valid_type and (
-            issubclass(input_class_simple, OpenApiModel) or
-            input_class_simple is none_type):
-        for valid_class in valid_classes:
-            if input_class_simple is none_type and is_type_nullable(valid_class):
-                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
-                return True
-            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
-                continue
-            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
-            discriminator_classes = (
-                valid_class.discriminator[discr_propertyname_py].values()
-            )
-            valid_type = is_valid_type(input_class_simple, discriminator_classes)
-            if valid_type:
-                return True
-    return valid_type
 
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: str, _configuration: typing.Optional[Configuration] = None) -> 'StrSchema':
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
-                               spec_property_naming, _check_type, configuration=None):
-    """Raises a TypeError is there is a problem, otherwise returns value
+    def __new__(cls, _arg: typing.Union[str, date, datetime, uuid.UUID], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
-    Args:
-        input_value (any): the data to validate/convert
-        required_types_mixed (list/dict/tuple): A list of
-            valid classes, or a list tuples of valid classes, or a dict where
-            the value is a tuple of value classes
-        path_to_item: (list) the path to the data being validated
-            this stores a list of keys or indices to get to the data being
-            validated
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        _check_type: (boolean) if true, type will be checked and conversion
-            will be attempted.
-        configuration: (Configuration): the configuration class to use
-            when converting file_type items.
-            If passed, conversion will be attempted when possible
-            If not passed, no conversions will be attempted and
-            exceptions will be raised
-
-    Returns:
-        the correctly typed value
-
-    Raises:
-        ApiTypeError
-    """
-    results = get_required_type_classes(required_types_mixed, spec_property_naming)
-    valid_classes, child_req_types_by_current_type = results
-
-    input_class_simple = get_simple_class(input_value)
-    valid_type = is_valid_type(input_class_simple, valid_classes)
-    if not valid_type:
-        if configuration:
-            # if input_value is not valid_type try to convert it
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=True,
-                check_type=_check_type
-            )
-            return converted_instance
-        else:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=False)
 
-    # input_value's type is in valid_classes
-    if len(valid_classes) > 1 and configuration:
-        # there are valid classes which are not the current class
-        valid_classes_coercible = remove_uncoercible(
-            valid_classes, input_value, spec_property_naming, must_convert=False)
-        if valid_classes_coercible:
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes_coercible,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=False,
-                check_type=_check_type
-            )
-            return converted_instance
+class UUIDSchema(UUIDBase, StrSchema):
 
-    if child_req_types_by_current_type == {}:
-        # all types are of the required types and there are no more inner
-        # variables left to look at
-        return input_value
-    inner_required_types = child_req_types_by_current_type.get(
-        type(input_value)
-    )
-    if inner_required_types is None:
-        # for this type, there are not more inner variables left to look at
-        return input_value
-    if isinstance(input_value, list):
-        if input_value == []:
-            # allow an empty list
-            return input_value
-        for index, inner_value in enumerate(input_value):
-            inner_path = list(path_to_item)
-            inner_path.append(index)
-            input_value[index] = validate_and_convert_types(
-                inner_value,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    elif isinstance(input_value, dict):
-        if input_value == {}:
-            # allow an empty dict
-            return input_value
-        for inner_key, inner_val in input_value.items():
-            inner_path = list(path_to_item)
-            inner_path.append(inner_key)
-            if get_simple_class(inner_key) != str:
-                raise get_type_error(inner_key, inner_path, valid_classes,
-                                     key_type=True)
-            input_value[inner_key] = validate_and_convert_types(
-                inner_val,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    return input_value
+    def __new__(cls, _arg: typing.Union[str, uuid.UUID], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
 
-def model_to_dict(model_instance, serialize=True):
-    """Returns the model properties as a dict
+class DateSchema(DateBase, StrSchema):
 
-    Args:
-        model_instance (one of your model instances): the model instance that
-            will be converted to a dict.
+    def __new__(cls, _arg: typing.Union[str, date], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
 
-    Keyword Args:
-        serialize (bool): if True, the keys in the dict will be values from
-            attribute_map
-    """
-    result = {}
-
-    model_instances = [model_instance]
-    if model_instance._composed_schemas:
-        model_instances.extend(model_instance._composed_instances)
-    seen_json_attribute_names = set()
-    used_fallback_python_attribute_names = set()
-    py_to_json_map = {}
-    for model_instance in model_instances:
-        for attr, value in model_instance._data_store.items():
-            if serialize:
-                # we use get here because additional property key names do not
-                # exist in attribute_map
-                try:
-                    attr = model_instance.attribute_map[attr]
-                    py_to_json_map.update(model_instance.attribute_map)
-                    seen_json_attribute_names.add(attr)
-                except KeyError:
-                    used_fallback_python_attribute_names.add(attr)
-            if isinstance(value, list):
-               if not value:
-                   # empty list or None
-                   result[attr] = value
-               else:
-                   res = []
-                   for v in value:
-                       if isinstance(v, PRIMITIVE_TYPES) or v is None:
-                           res.append(v)
-                       elif isinstance(v, ModelSimple):
-                           res.append(v.value)
-                       else:
-                           res.append(model_to_dict(v, serialize=serialize))
-                   result[attr] = res
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0],
-                                  model_to_dict(item[1], serialize=serialize))
-                    if hasattr(item[1], '_data_store') else item,
-                    value.items()
-                ))
-            elif isinstance(value, ModelSimple):
-                result[attr] = value.value
-            elif hasattr(value, '_data_store'):
-                result[attr] = model_to_dict(value, serialize=serialize)
-            else:
-                result[attr] = value
-    if serialize:
-        for python_key in used_fallback_python_attribute_names:
-            json_key = py_to_json_map.get(python_key)
-            if json_key is None:
-                continue
-            if python_key == json_key:
-                continue
-            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
-            if json_key_assigned_no_need_for_python_key:
-                del result[python_key]
-
-    return result
-
-
-def type_error_message(var_value=None, var_name=None, valid_classes=None,
-                       key_type=None):
-    """
-    Keyword Args:
-        var_value (any): the variable which has the type_error
-        var_name (str): the name of the variable which has the typ error
-        valid_classes (tuple): the accepted classes for current_item's
-                                  value
-        key_type (bool): False if our value is a value in a dict
-                         True if it is a key in a dict
-                         False if our item is an item in a list
-    """
-    key_or_value = 'value'
-    if key_type:
-        key_or_value = 'key'
-    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
-    msg = (
-        "Invalid type for variable '{0}'. Required {1} type {2} and "
-        "passed type was {3}".format(
-            var_name,
-            key_or_value,
-            valid_classes_phrase,
-            type(var_value).__name__,
-        )
-    )
-    return msg
 
+class DateTimeSchema(DateTimeBase, StrSchema):
 
-def get_valid_classes_phrase(input_classes):
-    """Returns a string phrase describing what types are allowed
+    def __new__(cls, _arg: typing.Union[str, datetime], **kwargs: Configuration):
+        return super().__new__(cls, _arg, **kwargs)
+
+
+class DecimalSchema(DecimalBase, StrSchema):
+
+    def __new__(cls, _arg: str, **kwargs: Configuration):
+        """
+        Note: Decimals may not be passed in because cast_to_allowed_types is only invoked once for payloads
+        which can be simple (str) or complex (dicts or lists with nested values)
+        Because casting is only done once and recursively casts all values prior to validation then for a potential
+        client side Decimal input if Decimal was accepted as an input in DecimalSchema then one would not know
+        if one was using it for a StrSchema (where it should be cast to str) or one is using it for NumberSchema
+        where it should stay as Decimal.
+        """
+        return super().__new__(cls, _arg, **kwargs)
+
+
+class BytesSchema(
+    Schema,
+    BytesMixin
+):
+    """
+    this class will subclass bytes and is immutable
     """
-    all_classes = list(input_classes)
-    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
-    all_class_names = [cls.__name__ for cls in all_classes]
-    if len(all_class_names) == 1:
-        return 'is {0}'.format(all_class_names[0])
-    return "is one of [{0}]".format(", ".join(all_class_names))
+    def __new__(cls, _arg: bytes, **kwargs: Configuration):
+        return super(Schema, cls).__new__(cls, _arg)
 
 
-def get_allof_instances(self, model_args, constant_args):
+class FileSchema(
+    Schema,
+    FileMixin
+):
     """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            used to make instances
-        constant_args (dict):
-            metadata arguments:
-            _check_type
-            _path_to_item
-            _spec_property_naming
-            _configuration
-            _visited_composed_classes
+    This class is NOT immutable
+    Dynamic classes are built using it for example when AnyType allows in binary data
+    Al other schema classes ARE immutable
+    If one wanted to make this immutable one could make this a DictSchema with required properties:
+    - data = BytesSchema (which would be an immutable bytes based schema)
+    - file_name = StrSchema
+    and cast_to_allowed_types would convert bytes and file instances into dicts containing data + file_name
+    The downside would be that data would be stored in memory which one may not want to do for very large files
+
+    The developer is responsible for closing this file and deleting it
 
-    Returns
-        composed_instances (list)
+    This class was kept as mutable:
+    - to allow file reading and writing to disk
+    - to be able to preserve file name info
     """
-    composed_instances = []
-    for allof_class in self._composed_schemas['allOf']:
 
-        try:
-            if constant_args.get('_spec_property_naming'):
-                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                allof_instance = allof_class(**model_args, **constant_args)
-            composed_instances.append(allof_instance)
-        except Exception as ex:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of '%s'. The "
-                "input data was invalid for the allOf schema '%s' in the composed "
-                "schema '%s'. Error=%s" % (
-                    allof_class.__name__,
-                    allof_class.__name__,
-                    self.__class__.__name__,
-                    str(ex)
-                )
-            ) from ex
-    return composed_instances
+    def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader], **kwargs: Configuration):
+        return super(Schema, cls).__new__(cls, _arg)
 
 
-def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
-    """
-    Find the oneOf schema that matches the input data (e.g. payload).
-    If exactly one schema matches the input data, an instance of that schema
-    is returned.
-    If zero or more than one schema match the input data, an exception is raised.
-    In OAS 3.x, the payload MUST, by validation, match exactly one of the
-    schemas described by oneOf.
+class BinaryBase:
+    pass
 
-    Args:
-        cls: the class we are handling
-        model_kwargs (dict): var_name to var_value
-            The input data, e.g. the payload that must match a oneOf schema
-            in the OpenAPI document.
-        constant_kwargs (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Kwargs:
-        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
-            the value to assign to a primitive class or ModelSimple class
-            Notes:
-            - this is only passed in when oneOf includes types which are not object
-            - None is used to suppress handling of model_arg, nullable models are handled in __new__
 
-    Returns
-        oneof_instance (instance)
-    """
-    if len(cls._composed_schemas['oneOf']) == 0:
-        return None
+class BinarySchema(
+    ComposedBase,
+    BinaryBase,
+    Schema,
+    BinaryMixin
+):
+    class MetaOapg:
+        @staticmethod
+        def one_of():
+            return [
+                BytesSchema,
+                FileSchema,
+            ]
 
-    oneof_instances = []
-    # Iterate over each oneOf schema and determine if the input data
-    # matches the oneOf schemas.
-    for oneof_class in cls._composed_schemas['oneOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if oneof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
+    def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader, bytes], **kwargs: Configuration):
+        return super().__new__(cls, _arg)
 
-        single_value_input = allows_single_value_input(oneof_class)
 
-        try:
-            if not single_value_input:
-                if constant_kwargs.get('_spec_property_naming'):
-                    oneof_instance = oneof_class._from_openapi_data(**model_kwargs, **constant_kwargs)
-                else:
-                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
-            else:
-                if issubclass(oneof_class, ModelSimple):
-                    if constant_kwargs.get('_spec_property_naming'):
-                        oneof_instance = oneof_class._from_openapi_data(model_arg, **constant_kwargs)
-                    else:
-                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
-                elif oneof_class in PRIMITIVE_TYPES:
-                    oneof_instance = validate_and_convert_types(
-                        model_arg,
-                        (oneof_class,),
-                        constant_kwargs['_path_to_item'],
-                        constant_kwargs['_spec_property_naming'],
-                        constant_kwargs['_check_type'],
-                        configuration=constant_kwargs['_configuration']
-                    )
-            oneof_instances.append(oneof_instance)
-        except Exception:
-            pass
-    if len(oneof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None "
-            "of the oneOf schemas matched the input data." %
-            cls.__name__
-        )
-    elif len(oneof_instances) > 1:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. Multiple "
-            "oneOf schemas matched the inputs, but a max of one is allowed." %
-            cls.__name__
-        )
-    return oneof_instances[0]
+class BoolSchema(
+    BoolBase,
+    Schema,
+    BoolMixin
+):
 
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: bool, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-def get_anyof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            The input data, e.g. the payload that must match at least one
-            anyOf child schema in the OpenAPI document.
-        constant_args (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Returns
-        anyof_instances (list)
-    """
-    anyof_instances = []
-    if len(self._composed_schemas['anyOf']) == 0:
-        return anyof_instances
-
-    for anyof_class in self._composed_schemas['anyOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if anyof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
+    def __new__(cls, _arg: bool, **kwargs: ValidationMetadata):
+        return super().__new__(cls, _arg, **kwargs)
 
-        try:
-            if constant_args.get('_spec_property_naming'):
-                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                anyof_instance = anyof_class(**model_args, **constant_args)
-            anyof_instances.append(anyof_instance)
-        except Exception:
-            pass
-    if len(anyof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None of the "
-            "anyOf schemas matched the inputs." %
-            self.__class__.__name__
+
+class AnyTypeSchema(
+    DictBase,
+    ListBase,
+    NumberBase,
+    StrBase,
+    BoolBase,
+    NoneBase,
+    Schema,
+    NoneFrozenDictTupleStrDecimalBoolFileBytesMixin
+):
+    # Python representation of a schema defined as true or {}
+    pass
+
+
+class UnsetAnyTypeSchema(AnyTypeSchema):
+    # Used when additionalProperties/items was not explicitly defined and a defining schema is needed
+    pass
+
+
+class NotAnyTypeSchema(
+    ComposedSchema,
+):
+    """
+    Python representation of a schema defined as false or {'not': {}}
+    Does not allow inputs in of AnyType
+    Note: validations on this class are never run because the code knows that no inputs will ever validate
+    """
+
+    class MetaOapg:
+        not_schema = AnyTypeSchema
+
+    def __new__(
+        cls,
+        *_args,
+        _configuration: typing.Optional[Configuration] = None,
+    ) -> 'NotAnyTypeSchema':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
         )
-    return anyof_instances
 
 
-def get_discarded_args(self, composed_instances, model_args):
+class DictSchema(
+    DictBase,
+    Schema,
+    FrozenDictMixin
+):
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.Dict[str, typing.Any], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+    def __new__(cls, *_args: typing.Union[dict, frozendict.frozendict], **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, bytes, Schema, Unset, ValidationMetadata]):
+        return super().__new__(cls, *_args, **kwargs)
+
+
+schema_type_classes = {NoneSchema, DictSchema, ListSchema, NumberSchema, StrSchema, BoolSchema, AnyTypeSchema}
+
+
+@functools.lru_cache()
+def get_new_class(
+    class_name: str,
+    bases: typing.Tuple[typing.Type[typing.Union[Schema, typing.Any]], ...]
+) -> typing.Type[Schema]:
     """
-    Gathers the args that were discarded by configuration.discard_unknown_keys
+    Returns a new class that is made with the subclass bases
     """
-    model_arg_keys = model_args.keys()
-    discarded_args = set()
-    # arguments passed to self were already converted to python names
-    # before __init__ was called
-    for instance in composed_instances:
-        if instance.__class__ in self._composed_schemas['allOf']:
-            try:
-                keys = instance.to_dict().keys()
-                discarded_keys = model_args - keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-        else:
-            try:
-                all_keys = set(model_to_dict(instance, serialize=False).keys())
-                js_keys = model_to_dict(instance, serialize=True).keys()
-                all_keys.update(js_keys)
-                discarded_keys = model_arg_keys - all_keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-    return discarded_args
+    new_cls: typing.Type[Schema] = type(class_name, bases, {})
+    return new_cls
 
 
-def validate_get_composed_info(constant_args, model_args, self):
-    """
-    For composed schemas, generate schema instances for
-    all schemas in the oneOf/anyOf/allOf definition. If additional
-    properties are allowed, also assign those properties on
-    all matched schemas that contain additionalProperties.
-    Openapi schemas are python classes.
+LOG_CACHE_USAGE = False
 
-    Exceptions are raised if:
-    - 0 or > 1 oneOf schema matches the model_args input data
-    - no anyOf schema matches the model_args input data
-    - any of the allOf schemas do not match the model_args input data
 
-    Args:
-        constant_args (dict): these are the args that every model requires
-        model_args (dict): these are the required and optional spec args that
-            were passed in to make this model
-        self (class): the class that we are instantiating
-            This class contains self._composed_schemas
-
-    Returns:
-        composed_info (list): length three
-            composed_instances (list): the composed instances which are not
-                self
-            var_name_to_model_instances (dict): a dict going from var_name
-                to the model_instance which holds that var_name
-                the model_instance may be self or an instance of one of the
-                classes in self.composed_instances()
-            additional_properties_model_instances (list): a list of the
-                model instances which have the property
-                additional_properties_type. This list can include self
-    """
-    # create composed_instances
-    composed_instances = []
-    allof_instances = get_allof_instances(self, model_args, constant_args)
-    composed_instances.extend(allof_instances)
-    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
-    if oneof_instance is not None:
-        composed_instances.append(oneof_instance)
-    anyof_instances = get_anyof_instances(self, model_args, constant_args)
-    composed_instances.extend(anyof_instances)
-    """
-    set additional_properties_model_instances
-    additional properties must be evaluated at the schema level
-    so self's additional properties are most important
-    If self is a composed schema with:
-    - no properties defined in self
-    - additionalProperties: False
-    Then for object payloads every property is an additional property
-    and they are not allowed, so only empty dict is allowed
-
-    Properties must be set on all matching schemas
-    so when a property is assigned toa composed instance, it must be set on all
-    composed instances regardless of additionalProperties presence
-    keeping it to prevent breaking changes in v5.0.1
-    TODO remove cls._additional_properties_model_instances in 6.0.0
-    """
-    additional_properties_model_instances = []
-    if self.additional_properties_type is not None:
-        additional_properties_model_instances = [self]
-
-    """
-    no need to set properties on self in here, they will be set in __init__
-    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
-    model_args
-    """
-    discarded_args = get_discarded_args(self, composed_instances, model_args)
-
-    # map variable names to composed_instances
-    var_name_to_model_instances = {}
-    for prop_name in model_args:
-        if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + composed_instances
-
-    return [
-      composed_instances,
-      var_name_to_model_instances,
-      additional_properties_model_instances,
-      discarded_args
-    ]
+def log_cache_usage(cache_fn):
+    if LOG_CACHE_USAGE:
+        print(cache_fn.__name__, cache_fn.cache_info())
```

### Comparing `fuse-client-1.0.7/fuse_client/models/__init__.py` & `fuse-client-1.0.8/fuse_client/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,79 @@
+# coding: utf-8
+
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from from fuse_client.model.pet import Pet
+# from fuse_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from fuse_client.model.account_subtype import AccountSubtype
 from fuse_client.model.account_type import AccountType
 from fuse_client.model.aggregator import Aggregator
 from fuse_client.model.country_code import CountryCode
 from fuse_client.model.create_asset_report_request import CreateAssetReportRequest
 from fuse_client.model.create_asset_report_response import CreateAssetReportResponse
 from fuse_client.model.create_entity_request import CreateEntityRequest
 from fuse_client.model.create_entity_response import CreateEntityResponse
 from fuse_client.model.create_link_token_request import CreateLinkTokenRequest
-from fuse_client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
-from fuse_client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
 from fuse_client.model.create_link_token_response import CreateLinkTokenResponse
 from fuse_client.model.create_session_request import CreateSessionRequest
 from fuse_client.model.create_session_response import CreateSessionResponse
 from fuse_client.model.currency import Currency
 from fuse_client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
 from fuse_client.model.entity import Entity
 from fuse_client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
 from fuse_client.model.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
 from fuse_client.model.financial_connection_data import FinancialConnectionData
 from fuse_client.model.financial_connection_details import FinancialConnectionDetails
-from fuse_client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
-from fuse_client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
-from fuse_client.model.financial_connection_details_teller import FinancialConnectionDetailsTeller
 from fuse_client.model.financial_connections_account import FinancialConnectionsAccount
 from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
 from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
 from fuse_client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
-from fuse_client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
-from fuse_client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
 from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
-from fuse_client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
-from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 from fuse_client.model.financial_connections_holding import FinancialConnectionsHolding
 from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
-from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
 from fuse_client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
 from fuse_client.model.financial_connections_owner import FinancialConnectionsOwner
-from fuse_client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
-from fuse_client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
-from fuse_client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
-from fuse_client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
-from fuse_client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
 from fuse_client.model.financial_institution import FinancialInstitution
-from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
 from fuse_client.model.fuse_api_error import FuseApiError
-from fuse_client.model.fuse_api_error_data import FuseApiErrorData
 from fuse_client.model.fuse_api_warning import FuseApiWarning
-from fuse_client.model.fuse_api_warning_data import FuseApiWarningData
-from fuse_client.model.fuse_api_warning_data_warnings import FuseApiWarningDataWarnings
 from fuse_client.model.get_asset_report_request import GetAssetReportRequest
 from fuse_client.model.get_asset_report_response import GetAssetReportResponse
-from fuse_client.model.get_asset_report_response_report import GetAssetReportResponseReport
-from fuse_client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
-from fuse_client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
-from fuse_client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
 from fuse_client.model.get_entity_response import GetEntityResponse
 from fuse_client.model.get_financial_connection_response import GetFinancialConnectionResponse
 from fuse_client.model.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
 from fuse_client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
 from fuse_client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
 from fuse_client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
 from fuse_client.model.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
-from fuse_client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
 from fuse_client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
 from fuse_client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
 from fuse_client.model.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
-from fuse_client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
 from fuse_client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
 from fuse_client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
 from fuse_client.model.get_financial_institution_response import GetFinancialInstitutionResponse
 from fuse_client.model.get_investment_holdings_request import GetInvestmentHoldingsRequest
-from fuse_client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 from fuse_client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
 from fuse_client.model.get_investment_transactions_request import GetInvestmentTransactionsRequest
-from fuse_client.model.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
 from fuse_client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
 from fuse_client.model.get_liabilities_request import GetLiabilitiesRequest
 from fuse_client.model.get_liabilities_response import GetLiabilitiesResponse
 from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-from fuse_client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
-from fuse_client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 from fuse_client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
-from fuse_client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
 from fuse_client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
 from fuse_client.model.product import Product
 from fuse_client.model.refresh_asset_report_request import RefreshAssetReportRequest
 from fuse_client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
 from fuse_client.model.sync_transactions_request import SyncTransactionsRequest
 from fuse_client.model.sync_transactions_response import SyncTransactionsResponse
-from fuse_client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
 from fuse_client.model.transaction import Transaction
-from fuse_client.model.transaction_merchant import TransactionMerchant
 from fuse_client.model.update_entity_request import UpdateEntityRequest
 from fuse_client.model.update_entity_response import UpdateEntityResponse
 from fuse_client.model.webhook_event import WebhookEvent
 from fuse_client.model.webhook_source import WebhookSource
 from fuse_client.model.webhook_type import WebhookType
```

### Comparing `fuse-client-1.0.7/test/test_account_subtype.py` & `fuse-client-1.0.8/test/test_models/test_account_subtype.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
 from fuse_client.model.account_subtype import AccountSubtype
+from fuse_client import configuration
 
 
 class TestAccountSubtype(unittest.TestCase):
     """AccountSubtype unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testAccountSubtype(self):
-        """Test AccountSubtype"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = AccountSubtype()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_account_type.py` & `fuse-client-1.0.8/test/test_models/test_fuse_api_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.account_type import AccountType
-
-
-class TestAccountType(unittest.TestCase):
-    """AccountType unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.fuse_api_error import FuseApiError
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testAccountType(self):
-        """Test AccountType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = AccountType()  # noqa: E501
-        pass
+class TestFuseApiError(unittest.TestCase):
+    """FuseApiError unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_aggregator.py` & `fuse-client-1.0.8/test/test_models/test_webhook_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.aggregator import Aggregator
-
-
-class TestAggregator(unittest.TestCase):
-    """Aggregator unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.webhook_source import WebhookSource
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testAggregator(self):
-        """Test Aggregator"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Aggregator()  # noqa: E501
-        pass
+class TestWebhookSource(unittest.TestCase):
+    """WebhookSource unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_country_code.py` & `fuse-client-1.0.8/test/test_models/test_create_session_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.country_code import CountryCode
-
-
-class TestCountryCode(unittest.TestCase):
-    """CountryCode unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.create_session_response import CreateSessionResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCountryCode(self):
-        """Test CountryCode"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CountryCode()  # noqa: E501
-        pass
+class TestCreateSessionResponse(unittest.TestCase):
+    """CreateSessionResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_create_asset_report_request.py` & `fuse-client-1.0.8/test/test_models/test_financial_connection_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.create_asset_report_request import CreateAssetReportRequest
-
-
-class TestCreateAssetReportRequest(unittest.TestCase):
-    """CreateAssetReportRequest unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connection_data import FinancialConnectionData
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCreateAssetReportRequest(self):
-        """Test CreateAssetReportRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CreateAssetReportRequest()  # noqa: E501
-        pass
+class TestFinancialConnectionData(unittest.TestCase):
+    """FinancialConnectionData unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_create_asset_report_response.py` & `fuse-client-1.0.8/test/test_models/test_create_asset_report_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
 from fuse_client.model.create_asset_report_response import CreateAssetReportResponse
+from fuse_client import configuration
 
 
 class TestCreateAssetReportResponse(unittest.TestCase):
     """CreateAssetReportResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testCreateAssetReportResponse(self):
-        """Test CreateAssetReportResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CreateAssetReportResponse()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_create_entity_response.py` & `fuse-client-1.0.8/test/test_models/test_aggregator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
 from fuse_client.model.aggregator import Aggregator
-globals()['Aggregator'] = Aggregator
-from fuse_client.model.create_entity_response import CreateEntityResponse
-
-
-class TestCreateEntityResponse(unittest.TestCase):
-    """CreateEntityResponse unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCreateEntityResponse(self):
-        """Test CreateEntityResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CreateEntityResponse()  # noqa: E501
-        pass
+class TestAggregator(unittest.TestCase):
+    """Aggregator unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_create_link_token_request_mx.py` & `fuse-client-1.0.8/test/test_models/test_create_link_token_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
-
-
-class TestCreateLinkTokenRequestMx(unittest.TestCase):
-    """CreateLinkTokenRequestMx unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.create_link_token_request import CreateLinkTokenRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCreateLinkTokenRequestMx(self):
-        """Test CreateLinkTokenRequestMx"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CreateLinkTokenRequestMx()  # noqa: E501
-        pass
+class TestCreateLinkTokenRequest(unittest.TestCase):
+    """CreateLinkTokenRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_create_link_token_request_plaid.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
-
-
-class TestCreateLinkTokenRequestPlaid(unittest.TestCase):
-    """CreateLinkTokenRequestPlaid unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCreateLinkTokenRequestPlaid(self):
-        """Test CreateLinkTokenRequestPlaid"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CreateLinkTokenRequestPlaid()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsOwnersRequest(unittest.TestCase):
+    """GetFinancialConnectionsOwnersRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_currency.py` & `fuse-client-1.0.8/test/test_models/test_webhook_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.currency import Currency
-
-
-class TestCurrency(unittest.TestCase):
-    """Currency unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.webhook_type import WebhookType
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCurrency(self):
-        """Test Currency"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Currency()  # noqa: E501
-        pass
+class TestWebhookType(unittest.TestCase):
+    """WebhookType unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_delete_financial_connection_response.py` & `fuse-client-1.0.8/test/test_models/test_financial_connections_account_liability.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.delete_financial_connection_response import DeleteFinancialConnectionResponse
-
-
-class TestDeleteFinancialConnectionResponse(unittest.TestCase):
-    """DeleteFinancialConnectionResponse unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testDeleteFinancialConnectionResponse(self):
-        """Test DeleteFinancialConnectionResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = DeleteFinancialConnectionResponse()  # noqa: E501
-        pass
+class TestFinancialConnectionsAccountLiability(unittest.TestCase):
+    """FinancialConnectionsAccountLiability unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_entity.py` & `fuse-client-1.0.8/test/test_models/test_sync_financial_connections_data_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.entity import Entity
-
-
-class TestEntity(unittest.TestCase):
-    """Entity unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEntity(self):
-        """Test Entity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Entity()  # noqa: E501
-        pass
+class TestSyncFinancialConnectionsDataResponse(unittest.TestCase):
+    """SyncFinancialConnectionsDataResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/test_post.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,43 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
+from fuse_client.paths.v1_financial_connections_balances import post  # noqa: E501
+from fuse_client import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestExchangeFinancialConnectionsPublicTokenRequest(unittest.TestCase):
-    """ExchangeFinancialConnectionsPublicTokenRequest unit test stubs"""
+
+class TestV1FinancialConnectionsBalances(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsBalances unit test stubs
+        Get balances  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testExchangeFinancialConnectionsPublicTokenRequest(self):
-        """Test ExchangeFinancialConnectionsPublicTokenRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ExchangeFinancialConnectionsPublicTokenRequest()  # noqa: E501
-        pass
+    response_status = 200
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connection_data.py` & `fuse-client-1.0.8/test/test_models/test_financial_connections_holding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connection_data import FinancialConnectionData
-
-
-class TestFinancialConnectionData(unittest.TestCase):
-    """FinancialConnectionData unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connections_holding import FinancialConnectionsHolding
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionData(self):
-        """Test FinancialConnectionData"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionData()  # noqa: E501
-        pass
+class TestFinancialConnectionsHolding(unittest.TestCase):
+    """FinancialConnectionsHolding unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connection_details_mx.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connection_details_mx import FinancialConnectionDetailsMx
-
-
-class TestFinancialConnectionDetailsMx(unittest.TestCase):
-    """FinancialConnectionDetailsMx unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionDetailsMx(self):
-        """Test FinancialConnectionDetailsMx"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionDetailsMx()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsAccountsRequest(unittest.TestCase):
+    """GetFinancialConnectionsAccountsRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connection_details_plaid.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
+from fuse_client.paths.v1_financial_connections_institutions_institution_id import get  # noqa: E501
+from fuse_client import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestFinancialConnectionDetailsPlaid(unittest.TestCase):
-    """FinancialConnectionDetailsPlaid unit test stubs"""
+class TestV1FinancialConnectionsInstitutionsInstitutionId(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsInstitutionsInstitutionId unit test stubs
+        Get a financial institution  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionDetailsPlaid(self):
-        """Test FinancialConnectionDetailsPlaid"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionDetailsPlaid()  # noqa: E501
-        pass
+    response_status = 200
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_account_balance.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+from fuse_client.paths.v1_financial_connections_financial_connection_id_to_delete import delete  # noqa: E501
+from fuse_client import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestFinancialConnectionsAccountBalance(unittest.TestCase):
-    """FinancialConnectionsAccountBalance unit test stubs"""
+class TestV1FinancialConnectionsFinancialConnectionIdToDelete(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsFinancialConnectionIdToDelete unit test stubs
+        Delete a financial connection  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionsAccountBalance(self):
-        """Test FinancialConnectionsAccountBalance"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountBalance()  # noqa: E501
-        pass
+    response_status = 200
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_account_cached_balance.py` & `fuse-client-1.0.8/test/test_models/test_get_investment_transactions_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-
-
-class TestFinancialConnectionsAccountCachedBalance(unittest.TestCase):
-    """FinancialConnectionsAccountCachedBalance unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_investment_transactions_response import GetInvestmentTransactionsResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsAccountCachedBalance(self):
-        """Test FinancialConnectionsAccountCachedBalance"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountCachedBalance()  # noqa: E501
-        pass
+class TestGetInvestmentTransactionsResponse(unittest.TestCase):
+    """GetInvestmentTransactionsResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_account_details_ach.py` & `fuse-client-1.0.8/test/test_models/test_financial_connections_account_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
-
-
-class TestFinancialConnectionsAccountDetailsAch(unittest.TestCase):
-    """FinancialConnectionsAccountDetailsAch unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsAccountDetailsAch(self):
-        """Test FinancialConnectionsAccountDetailsAch"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountDetailsAch()  # noqa: E501
-        pass
+class TestFinancialConnectionsAccountDetails(unittest.TestCase):
+    """FinancialConnectionsAccountDetails unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_account_liability_all_of_aprs.py` & `fuse-client-1.0.8/test/test_models/test_financial_connections_investment_transaction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
-
-
-class TestFinancialConnectionsAccountLiabilityAllOfAprs(unittest.TestCase):
-    """FinancialConnectionsAccountLiabilityAllOfAprs unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsAccountLiabilityAllOfAprs(self):
-        """Test FinancialConnectionsAccountLiabilityAllOfAprs"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsAccountLiabilityAllOfAprs()  # noqa: E501
-        pass
+class TestFinancialConnectionsInvestmentTransaction(unittest.TestCase):
+    """FinancialConnectionsInvestmentTransaction unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_investment_security.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.currency import Currency
-from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
-globals()['Currency'] = Currency
-globals()['FinancialConnectionsInvestmentSecurityExchange'] = FinancialConnectionsInvestmentSecurityExchange
-from fuse_client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+from fuse_client.paths.v1_financial_connections_investments_holdings import post  # noqa: E501
+from fuse_client import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestFinancialConnectionsInvestmentSecurity(unittest.TestCase):
-    """FinancialConnectionsInvestmentSecurity unit test stubs"""
+
+class TestV1FinancialConnectionsInvestmentsHoldings(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsInvestmentsHoldings unit test stubs
+        Get investment holdings  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testFinancialConnectionsInvestmentSecurity(self):
-        """Test FinancialConnectionsInvestmentSecurity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsInvestmentSecurity()  # noqa: E501
-        pass
+    response_status = 200
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_investment_security_exchange.py` & `fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
-
-
-class TestFinancialConnectionsInvestmentSecurityExchange(unittest.TestCase):
-    """FinancialConnectionsInvestmentSecurityExchange unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsInvestmentSecurityExchange(self):
-        """Test FinancialConnectionsInvestmentSecurityExchange"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsInvestmentSecurityExchange()  # noqa: E501
-        pass
+class TestMigrateFinancialConnectionsAggregatorConnectionData(unittest.TestCase):
+    """MigrateFinancialConnectionsAggregatorConnectionData unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_owner_emails.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
-
-
-class TestFinancialConnectionsOwnerEmails(unittest.TestCase):
-    """FinancialConnectionsOwnerEmails unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsOwnerEmails(self):
-        """Test FinancialConnectionsOwnerEmails"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsOwnerEmails()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsTransactionsRequest(unittest.TestCase):
+    """GetFinancialConnectionsTransactionsRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_owner_names.py` & `fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
-
-
-class TestFinancialConnectionsOwnerNames(unittest.TestCase):
-    """FinancialConnectionsOwnerNames unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsOwnerNames(self):
-        """Test FinancialConnectionsOwnerNames"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsOwnerNames()  # noqa: E501
-        pass
+class TestMigrateFinancialConnectionsTokenRequest(unittest.TestCase):
+    """MigrateFinancialConnectionsTokenRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_connections_owner_phone_numbers.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
-
-
-class TestFinancialConnectionsOwnerPhoneNumbers(unittest.TestCase):
-    """FinancialConnectionsOwnerPhoneNumbers unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialConnectionsOwnerPhoneNumbers(self):
-        """Test FinancialConnectionsOwnerPhoneNumbers"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialConnectionsOwnerPhoneNumbers()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsAccountDetailsResponse(unittest.TestCase):
+    """GetFinancialConnectionsAccountDetailsResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_institution.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/test_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.country_code import CountryCode
-from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
-globals()['CountryCode'] = CountryCode
-globals()['FinancialInstitutionLogo'] = FinancialInstitutionLogo
-from fuse_client.model.financial_institution import FinancialInstitution
+from fuse_client.paths.v1_financial_connections_liabilities import post  # noqa: E501
+from fuse_client import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestFinancialInstitution(unittest.TestCase):
-    """FinancialInstitution unit test stubs"""
+
+class TestV1FinancialConnectionsLiabilities(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsLiabilities unit test stubs
+        Get liabilities  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testFinancialInstitution(self):
-        """Test FinancialInstitution"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialInstitution()  # noqa: E501
-        pass
+    response_status = 200
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_financial_institution_logo.py` & `fuse-client-1.0.8/test/test_models/test_financial_institution.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_institution_logo import FinancialInstitutionLogo
-
-
-class TestFinancialInstitutionLogo(unittest.TestCase):
-    """FinancialInstitutionLogo unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_institution import FinancialInstitution
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFinancialInstitutionLogo(self):
-        """Test FinancialInstitutionLogo"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialInstitutionLogo()  # noqa: E501
-        pass
+class TestFinancialInstitution(unittest.TestCase):
+    """FinancialInstitution unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_get_asset_report_request.py` & `fuse-client-1.0.8/test/test_models/test_get_asset_report_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
 from fuse_client.model.get_asset_report_request import GetAssetReportRequest
+from fuse_client import configuration
 
 
 class TestGetAssetReportRequest(unittest.TestCase):
     """GetAssetReportRequest unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testGetAssetReportRequest(self):
-        """Test GetAssetReportRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetAssetReportRequest()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_get_financial_connections_owners_request.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
-
-
-class TestGetFinancialConnectionsOwnersRequest(unittest.TestCase):
-    """GetFinancialConnectionsOwnersRequest unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testGetFinancialConnectionsOwnersRequest(self):
-        """Test GetFinancialConnectionsOwnersRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsOwnersRequest()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsTransactionsResponse(unittest.TestCase):
+    """GetFinancialConnectionsTransactionsResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_get_financial_connections_transactions_response.py` & `fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.transaction import Transaction
-globals()['Transaction'] = Transaction
-from fuse_client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
-
-
-class TestGetFinancialConnectionsTransactionsResponse(unittest.TestCase):
-    """GetFinancialConnectionsTransactionsResponse unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testGetFinancialConnectionsTransactionsResponse(self):
-        """Test GetFinancialConnectionsTransactionsResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetFinancialConnectionsTransactionsResponse()  # noqa: E501
-        pass
+class TestGetFinancialConnectionsBalanceResponse(unittest.TestCase):
+    """GetFinancialConnectionsBalanceResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_get_liabilities_request.py` & `fuse-client-1.0.8/test/test_models/test_get_liabilities_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
 from fuse_client.model.get_liabilities_request import GetLiabilitiesRequest
+from fuse_client import configuration
 
 
 class TestGetLiabilitiesRequest(unittest.TestCase):
     """GetLiabilitiesRequest unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testGetLiabilitiesRequest(self):
-        """Test GetLiabilitiesRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetLiabilitiesRequest()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_get_liabilities_response.py` & `fuse-client-1.0.8/test/test_models/test_financial_connections_account_balance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.financial_connections_account_liability import FinancialConnectionsAccountLiability
-globals()['FinancialConnectionsAccountLiability'] = FinancialConnectionsAccountLiability
-from fuse_client.model.get_liabilities_response import GetLiabilitiesResponse
-
-
-class TestGetLiabilitiesResponse(unittest.TestCase):
-    """GetLiabilitiesResponse unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testGetLiabilitiesResponse(self):
-        """Test GetLiabilitiesResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetLiabilitiesResponse()  # noqa: E501
-        pass
+class TestFinancialConnectionsAccountBalance(unittest.TestCase):
+    """FinancialConnectionsAccountBalance unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_product.py` & `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/test_post.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,43 @@
+# coding: utf-8
+
 """
-    Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import fuse_client
-from fuse_client.model.product import Product
+from fuse_client.paths.v1_financial_connections_accounts import post  # noqa: E501
+from fuse_client import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestProduct(unittest.TestCase):
-    """Product unit test stubs"""
+
+class TestV1FinancialConnectionsAccounts(ApiTestMixin, unittest.TestCase):
+    """
+    V1FinancialConnectionsAccounts unit test stubs
+        Get accounts  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testProduct(self):
-        """Test Product"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Product()  # noqa: E501
-        pass
+    response_status = 200
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_refresh_asset_report_request.py` & `fuse-client-1.0.8/test/test_models/test_create_session_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.refresh_asset_report_request import RefreshAssetReportRequest
-
-
-class TestRefreshAssetReportRequest(unittest.TestCase):
-    """RefreshAssetReportRequest unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.create_session_request import CreateSessionRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testRefreshAssetReportRequest(self):
-        """Test RefreshAssetReportRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RefreshAssetReportRequest()  # noqa: E501
-        pass
+class TestCreateSessionRequest(unittest.TestCase):
+    """CreateSessionRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_sync_transactions_request.py` & `fuse-client-1.0.8/test/test_models/test_sync_transactions_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.sync_transactions_request import SyncTransactionsRequest
-
-
-class TestSyncTransactionsRequest(unittest.TestCase):
-    """SyncTransactionsRequest unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.sync_transactions_response import SyncTransactionsResponse
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testSyncTransactionsRequest(self):
-        """Test SyncTransactionsRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = SyncTransactionsRequest()  # noqa: E501
-        pass
+class TestSyncTransactionsResponse(unittest.TestCase):
+    """SyncTransactionsResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_transaction_merchant.py` & `fuse-client-1.0.8/test/test_models/test_account_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.transaction_merchant import TransactionMerchant
-
-
-class TestTransactionMerchant(unittest.TestCase):
-    """TransactionMerchant unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.account_type import AccountType
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testTransactionMerchant(self):
-        """Test TransactionMerchant"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = TransactionMerchant()  # noqa: E501
-        pass
+class TestAccountType(unittest.TestCase):
+    """AccountType unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_update_entity_response.py` & `fuse-client-1.0.8/test/test_models/test_update_entity_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.aggregator import Aggregator
-globals()['Aggregator'] = Aggregator
-from fuse_client.model.update_entity_response import UpdateEntityResponse
-
-
-class TestUpdateEntityResponse(unittest.TestCase):
-    """UpdateEntityResponse unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.update_entity_request import UpdateEntityRequest
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testUpdateEntityResponse(self):
-        """Test UpdateEntityResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = UpdateEntityResponse()  # noqa: E501
-        pass
+class TestUpdateEntityRequest(unittest.TestCase):
+    """UpdateEntityRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fuse-client-1.0.7/test/test_webhook_source.py` & `fuse-client-1.0.8/test/test_models/test_transaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+# coding: utf-8
+
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import fuse_client
-from fuse_client.model.webhook_source import WebhookSource
-
-
-class TestWebhookSource(unittest.TestCase):
-    """WebhookSource unit test stubs"""
-
-    def setUp(self):
-        pass
+from fuse_client.model.transaction import Transaction
+from fuse_client import configuration
 
-    def tearDown(self):
-        pass
 
-    def testWebhookSource(self):
-        """Test WebhookSource"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = WebhookSource()  # noqa: E501
-        pass
+class TestTransaction(unittest.TestCase):
+    """Transaction unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

