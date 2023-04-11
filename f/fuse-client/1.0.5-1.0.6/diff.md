# Comparing `tmp/fuse_client-1.0.5.tar.gz` & `tmp/fuse-client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuse_client-1.0.5.tar", last modified: Mon Apr 10 09:07:11 2023, max compression
+gzip compressed data, was "fuse-client-1.0.6.tar", last modified: Tue Apr 11 09:43:37 2023, max compression
```

## Comparing `fuse_client-1.0.5.tar` & `fuse-client-1.0.6.tar`

### file list

```diff
@@ -1,122 +1,226 @@
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817603 fuse_client-1.0.5/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse_client-1.0.5/LICENSE
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-10 09:07:11.817671 fuse_client-1.0.5/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.5/README.md
--rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-06 23:42:55.000000 fuse_client-1.0.5/pyproject.toml
--rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-10 09:07:11.817983 fuse_client-1.0.5/setup.cfg
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.796019 fuse_client-1.0.5/src/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.797143 fuse_client-1.0.5/src/fuse_client/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.798030 fuse_client-1.0.5/src/fuse_client/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    16910 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/apis/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      554 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/main.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817196 fuse_client-1.0.5/src/fuse_client/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1181 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1583 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1814 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      705 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/extra_models.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2052 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1984 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      961 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3676 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2243 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1468 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2210 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2196 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1628 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1072 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_emails_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_names_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_phone_numbers_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1329 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      946 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1353 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data_warnings_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      960 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1817 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1865 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1512 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1343 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1257 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1061 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      834 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1001 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1140 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      968 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      988 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1167 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2006 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1294 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1009 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1350 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1568 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1487 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1664 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response_removed_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1767 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1066 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1382 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8152 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/security_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.797838 fuse_client-1.0.5/src/fuse_client.egg-info/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6380 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/SOURCES.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/dependency_links.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       13 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/requires.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/top_level.txt
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817386 fuse_client-1.0.5/tests/
--rw-r--r--   0 adibpournazari   (501) staff       (20)    16557 2023-04-10 09:05:42.000000 fuse_client-1.0.5/tests/test_fuse_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.268054 fuse-client-1.0.6/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.6/LICENSE
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 09:43:37.268137 fuse-client-1.0.6/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.6/README.md
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.244811 fuse-client-1.0.6/fuse-client/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      739 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.245021 fuse-client-1.0.6/fuse-client/api/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      212 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    91158 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api/fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    36894 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/api_client.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.245196 fuse-client-1.0.6/fuse-client/apis/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      452 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/apis/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    21228 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/configuration.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5085 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/exceptions.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.256385 fuse-client-1.0.6/fuse-client/model/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      348 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    27574 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12061 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11690 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11513 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12371 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12132 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12167 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13358 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11510 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11929 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_request_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13654 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12128 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11360 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12294 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11715 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11350 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12404 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11587 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14438 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11530 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11616 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11687 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connection_details_teller.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14204 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12931 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12630 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11913 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_details_ach.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11124 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19419 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14183 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11559 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_account_liability_all_of_aprs.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13545 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14978 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11412 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_security_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    15583 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13181 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11708 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_addresses.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12117 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11797 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_emails.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11470 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_names.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_connections_owner_phone_numbers.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12712 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11967 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/financial_institution_logo.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11598 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_error_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12323 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11714 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11940 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/fuse_api_warning_data_warnings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11381 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11832 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13742 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12992 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11859 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12242 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_asset_report_response_report_historical_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13394 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12094 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11336 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12724 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11318 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12579 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11933 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11334 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12049 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11312 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11645 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12391 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_owners_response_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13137 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12694 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12065 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11293 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12451 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13477 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11313 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13115 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11267 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12271 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11448 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_aggregator_connection_data_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13344 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11333 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_request_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13168 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12017 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12370 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11603 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12286 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14669 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11153 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/sync_transactions_response_removed.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    45053 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11097 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/transaction_merchant.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11963 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12604 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    13317 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11759 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12227 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model/webhook_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    81904 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/model_utils.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.256489 fuse-client-1.0.6/fuse-client/models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9568 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/models/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12686 2023-04-11 09:43:23.000000 fuse-client-1.0.6/fuse-client/rest.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.257003 fuse-client-1.0.6/fuse_client.egg-info/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10416 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       32 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/requires.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-11 09:43:37.000000 fuse-client-1.0.6/fuse_client.egg-info/top_level.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 09:43:37.268405 fuse-client-1.0.6/setup.cfg
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1068 2023-04-11 09:43:23.000000 fuse-client-1.0.6/setup.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 09:43:37.267956 fuse-client-1.0.6/test/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      771 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      742 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      843 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      844 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      865 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_request_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      836 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1147 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      728 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      714 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      999 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1006 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1465 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      871 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      899 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connection_details_teller.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1480 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      913 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      956 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1114 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_details_ach.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      941 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2156 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1199 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      993 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of_aprs.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1259 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_security_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1247 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1586 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1081 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_addresses.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      878 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_emails.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      885 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_names.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      935 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_connections_owner_phone_numbers.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1054 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      842 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_financial_institution_logo.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3752 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      874 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      975 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_error_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1047 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_fuse_api_warning_data_warnings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      822 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      994 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1177 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1517 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      929 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1000 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_asset_report_response_report_historical_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1037 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1040 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1323 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      942 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1251 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1165 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      985 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1130 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1169 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1143 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_owners_response_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      970 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1022 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1064 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      921 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1108 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      821 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1580 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1049 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1070 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1518 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      992 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_request_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1214 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      721 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      850 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      928 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      835 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1111 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      892 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_sync_transactions_response_removed.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      875 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      806 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_transaction_merchant.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      896 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      903 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      953 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      764 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      750 2023-04-11 09:43:23.000000 fuse-client-1.0.6/test/test_webhook_type.py
```

### Comparing `fuse_client-1.0.5/LICENSE` & `fuse-client-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.5/src/fuse_client/main.py` & `fuse-client-1.0.6/test/test_entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-# coding: utf-8
-
 """
     Fuse
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-from fastapi import FastAPI
+import sys
+import unittest
+
+import fuse-client
+from fuse-client.model.entity import Entity
+
+
+class TestEntity(unittest.TestCase):
+    """Entity unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
 
-from fuse_client.apis.fuse_api import router as FuseApiRouter
+    def testEntity(self):
+        """Test Entity"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Entity()  # noqa: E501
+        pass
 
-app = FastAPI(
-    title="Fuse",
-    description="No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)",
-    version="1.0.5",
-)
 
-app.include_router(FuseApiRouter)
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/create_link_token_request.py` & `fuse-client-1.0.6/test/test_create_link_token_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.create_link_token_request_mx import CreateLinkTokenRequestMx
-from fuse_client.models.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
-from fuse_client.models.entity import Entity
 
+import sys
+import unittest
 
-class CreateLinkTokenRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.create_link_token_request_mx import CreateLinkTokenRequestMx
+from fuse-client.model.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
+from fuse-client.model.entity import Entity
+globals()['CreateLinkTokenRequestMx'] = CreateLinkTokenRequestMx
+globals()['CreateLinkTokenRequestPlaid'] = CreateLinkTokenRequestPlaid
+globals()['Entity'] = Entity
+from fuse-client.model.create_link_token_request import CreateLinkTokenRequest
 
-    Do not edit the class manually.
 
-    CreateLinkTokenRequest - a model defined in OpenAPI
+class TestCreateLinkTokenRequest(unittest.TestCase):
+    """CreateLinkTokenRequest unit test stubs"""
 
-        institution_id: The institution_id of this CreateLinkTokenRequest.
-        entity: The entity of this CreateLinkTokenRequest.
-        client_name: The client_name of this CreateLinkTokenRequest.
-        session_client_secret: The session_client_secret of this CreateLinkTokenRequest.
-        mx: The mx of this CreateLinkTokenRequest [Optional].
-        plaid: The plaid of this CreateLinkTokenRequest [Optional].
-    """
+    def setUp(self):
+        pass
 
-    institution_id: str = Field(alias="institution_id")
-    entity: Entity = Field(alias="entity")
-    client_name: str = Field(alias="client_name")
-    session_client_secret: str = Field(alias="session_client_secret")
-    mx: Optional[CreateLinkTokenRequestMx] = Field(alias="mx", default=None)
-    plaid: Optional[CreateLinkTokenRequestPlaid] = Field(alias="plaid", default=None)
+    def tearDown(self):
+        pass
 
-CreateLinkTokenRequest.update_forward_refs()
+    def testCreateLinkTokenRequest(self):
+        """Test CreateLinkTokenRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = CreateLinkTokenRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/delete_financial_connection_response.py` & `fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class DeleteFinancialConnectionResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+globals()['FinancialConnectionsAccountLiabilityAllOfAprs'] = FinancialConnectionsAccountLiabilityAllOfAprs
+from fuse-client.model.financial_connections_account_liability_all_of import FinancialConnectionsAccountLiabilityAllOf
 
-    Do not edit the class manually.
 
-    DeleteFinancialConnectionResponse - a model defined in OpenAPI
+class TestFinancialConnectionsAccountLiabilityAllOf(unittest.TestCase):
+    """FinancialConnectionsAccountLiabilityAllOf unit test stubs"""
 
-        financial_connection_id: The financial_connection_id of this DeleteFinancialConnectionResponse.
-        access_token: The access_token of this DeleteFinancialConnectionResponse.
-        request_id: The request_id of this DeleteFinancialConnectionResponse.
-    """
+    def setUp(self):
+        pass
 
-    financial_connection_id: str = Field(alias="financial_connection_id")
-    access_token: str = Field(alias="access_token")
-    request_id: str = Field(alias="request_id")
+    def tearDown(self):
+        pass
 
-DeleteFinancialConnectionResponse.update_forward_refs()
+    def testFinancialConnectionsAccountLiabilityAllOf(self):
+        """Test FinancialConnectionsAccountLiabilityAllOf"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsAccountLiabilityAllOf()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.6/test/test_exchange_financial_connections_public_token_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class ExchangeFinancialConnectionsPublicTokenRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
 
-    Do not edit the class manually.
 
-    ExchangeFinancialConnectionsPublicTokenRequest - a model defined in OpenAPI
+class TestExchangeFinancialConnectionsPublicTokenRequest(unittest.TestCase):
+    """ExchangeFinancialConnectionsPublicTokenRequest unit test stubs"""
 
-        public_token: The public_token of this ExchangeFinancialConnectionsPublicTokenRequest [Optional].
-    """
+    def setUp(self):
+        pass
 
-    public_token: Optional[str] = Field(alias="public_token", default=None)
+    def tearDown(self):
+        pass
 
-ExchangeFinancialConnectionsPublicTokenRequest.update_forward_refs()
+    def testExchangeFinancialConnectionsPublicTokenRequest(self):
+        """Test ExchangeFinancialConnectionsPublicTokenRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ExchangeFinancialConnectionsPublicTokenRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_response.py` & `fuse-client-1.0.6/test/test_sync_financial_connections_data_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class ExchangeFinancialConnectionsPublicTokenResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
 
-    Do not edit the class manually.
 
-    ExchangeFinancialConnectionsPublicTokenResponse - a model defined in OpenAPI
+class TestSyncFinancialConnectionsDataResponse(unittest.TestCase):
+    """SyncFinancialConnectionsDataResponse unit test stubs"""
 
-        access_token: The access_token of this ExchangeFinancialConnectionsPublicTokenResponse.
-        financial_connection_id: The financial_connection_id of this ExchangeFinancialConnectionsPublicTokenResponse.
-        request_id: The request_id of this ExchangeFinancialConnectionsPublicTokenResponse.
-    """
+    def setUp(self):
+        pass
 
-    access_token: str = Field(alias="access_token")
-    financial_connection_id: str = Field(alias="financial_connection_id")
-    request_id: str = Field(alias="request_id")
+    def tearDown(self):
+        pass
 
-ExchangeFinancialConnectionsPublicTokenResponse.update_forward_refs()
+    def testSyncFinancialConnectionsDataResponse(self):
+        """Test SyncFinancialConnectionsDataResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = SyncFinancialConnectionsDataResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connection_data.py` & `fuse-client-1.0.6/test/test_financial_connections_owner_emails.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionData(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
 
-    Do not edit the class manually.
 
-    FinancialConnectionData - a model defined in OpenAPI
+class TestFinancialConnectionsOwnerEmails(unittest.TestCase):
+    """FinancialConnectionsOwnerEmails unit test stubs"""
 
-        id: The id of this FinancialConnectionData.
-        institution_id: The institution_id of this FinancialConnectionData.
-    """
+    def setUp(self):
+        pass
 
-    id: str = Field(alias="id")
-    institution_id: str = Field(alias="institution_id")
+    def tearDown(self):
+        pass
 
-FinancialConnectionData.update_forward_refs()
+    def testFinancialConnectionsOwnerEmails(self):
+        """Test FinancialConnectionsOwnerEmails"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsOwnerEmails()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details.py` & `fuse-client-1.0.6/test/test_financial_connections_owner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.aggregator import Aggregator
-from fuse_client.models.financial_connection_details_mx import FinancialConnectionDetailsMx
-from fuse_client.models.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
-from fuse_client.models.financial_connection_details_teller import FinancialConnectionDetailsTeller
-
-
-class FinancialConnectionDetails(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
-
-    Do not edit the class manually.
-
-    FinancialConnectionDetails - a model defined in OpenAPI
-
-        id: The id of this FinancialConnectionDetails.
-        connection_status: The connection_status of this FinancialConnectionDetails.
-        connection_status_updated_at: The connection_status_updated_at of this FinancialConnectionDetails.
-        is_oauth: The is_oauth of this FinancialConnectionDetails.
-        aggregator: The aggregator of this FinancialConnectionDetails.
-        plaid: The plaid of this FinancialConnectionDetails [Optional].
-        teller: The teller of this FinancialConnectionDetails [Optional].
-        mx: The mx of this FinancialConnectionDetails [Optional].
-    """
-
-    id: str = Field(alias="id")
-    connection_status: str = Field(alias="connection_status")
-    connection_status_updated_at: str = Field(alias="connection_status_updated_at")
-    is_oauth: bool = Field(alias="is_oauth")
-    aggregator: Aggregator = Field(alias="aggregator")
-    plaid: Optional[FinancialConnectionDetailsPlaid] = Field(alias="plaid", default=None)
-    teller: Optional[FinancialConnectionDetailsTeller] = Field(alias="teller", default=None)
-    mx: Optional[FinancialConnectionDetailsMx] = Field(alias="mx", default=None)
 
-FinancialConnectionDetails.update_forward_refs()
+import sys
+import unittest
+
+import fuse-client
+from fuse-client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
+from fuse-client.model.financial_connections_owner_emails import FinancialConnectionsOwnerEmails
+from fuse-client.model.financial_connections_owner_names import FinancialConnectionsOwnerNames
+from fuse-client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
+globals()['FinancialConnectionsOwnerAddresses'] = FinancialConnectionsOwnerAddresses
+globals()['FinancialConnectionsOwnerEmails'] = FinancialConnectionsOwnerEmails
+globals()['FinancialConnectionsOwnerNames'] = FinancialConnectionsOwnerNames
+globals()['FinancialConnectionsOwnerPhoneNumbers'] = FinancialConnectionsOwnerPhoneNumbers
+from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
+
+
+class TestFinancialConnectionsOwner(unittest.TestCase):
+    """FinancialConnectionsOwner unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testFinancialConnectionsOwner(self):
+        """Test FinancialConnectionsOwner"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsOwner()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_plaid.py` & `fuse-client-1.0.6/test/test_financial_connections_account_details_ach.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionDetailsPlaid(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
 
-    Do not edit the class manually.
 
-    FinancialConnectionDetailsPlaid - a model defined in OpenAPI
+class TestFinancialConnectionsAccountDetailsAch(unittest.TestCase):
+    """FinancialConnectionsAccountDetailsAch unit test stubs"""
 
-        access_token: The access_token of this FinancialConnectionDetailsPlaid.
-        item_id: The item_id of this FinancialConnectionDetailsPlaid.
-    """
+    def setUp(self):
+        pass
 
-    access_token: str = Field(alias="access_token")
-    item_id: str = Field(alias="item_id")
+    def tearDown(self):
+        pass
 
-FinancialConnectionDetailsPlaid.update_forward_refs()
+    def testFinancialConnectionsAccountDetailsAch(self):
+        """Test FinancialConnectionsAccountDetailsAch"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsAccountDetailsAch()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_teller.py` & `fuse-client-1.0.6/test/test_financial_connections_account_liability_all_of_aprs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionDetailsTeller(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 
-    Do not edit the class manually.
 
-    FinancialConnectionDetailsTeller - a model defined in OpenAPI
+class TestFinancialConnectionsAccountLiabilityAllOfAprs(unittest.TestCase):
+    """FinancialConnectionsAccountLiabilityAllOfAprs unit test stubs"""
 
-        access_token: The access_token of this FinancialConnectionDetailsTeller.
-        enrollment_id: The enrollment_id of this FinancialConnectionDetailsTeller.
-    """
+    def setUp(self):
+        pass
 
-    access_token: str = Field(alias="access_token")
-    enrollment_id: str = Field(alias="enrollment_id")
+    def tearDown(self):
+        pass
 
-FinancialConnectionDetailsTeller.update_forward_refs()
+    def testFinancialConnectionsAccountLiabilityAllOfAprs(self):
+        """Test FinancialConnectionsAccountLiabilityAllOfAprs"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsAccountLiabilityAllOfAprs()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account.py` & `fuse-client-1.0.6/test/test_financial_connections_account.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.account_subtype import AccountSubtype
-from fuse_client.models.account_type import AccountType
-from fuse_client.models.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-from fuse_client.models.financial_connections_account_institution import FinancialConnectionsAccountInstitution
-
-
-class FinancialConnectionsAccount(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
-
-    Do not edit the class manually.
-
-    FinancialConnectionsAccount - a model defined in OpenAPI
-
-        remote_id: The remote_id of this FinancialConnectionsAccount.
-        fingerprint: The fingerprint of this FinancialConnectionsAccount.
-        institution: The institution of this FinancialConnectionsAccount [Optional].
-        mask: The mask of this FinancialConnectionsAccount [Optional].
-        name: The name of this FinancialConnectionsAccount.
-        type: The type of this FinancialConnectionsAccount.
-        subtype: The subtype of this FinancialConnectionsAccount [Optional].
-        balance: The balance of this FinancialConnectionsAccount.
-    """
-
-    remote_id: str = Field(alias="remote_id")
-    fingerprint: str = Field(alias="fingerprint")
-    institution: Optional[FinancialConnectionsAccountInstitution] = Field(alias="institution", default=None)
-    mask: Optional[str] = Field(alias="mask", default=None)
-    name: str = Field(alias="name")
-    type: AccountType = Field(alias="type")
-    subtype: Optional[AccountSubtype] = Field(alias="subtype", default=None)
-    balance: FinancialConnectionsAccountCachedBalance = Field(alias="balance")
 
-FinancialConnectionsAccount.update_forward_refs()
+import sys
+import unittest
+
+import fuse-client
+from fuse-client.model.account_subtype import AccountSubtype
+from fuse-client.model.account_type import AccountType
+from fuse-client.model.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+from fuse-client.model.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+globals()['AccountSubtype'] = AccountSubtype
+globals()['AccountType'] = AccountType
+globals()['FinancialConnectionsAccountCachedBalance'] = FinancialConnectionsAccountCachedBalance
+globals()['FinancialConnectionsAccountInstitution'] = FinancialConnectionsAccountInstitution
+from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+
+
+class TestFinancialConnectionsAccount(unittest.TestCase):
+    """FinancialConnectionsAccount unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testFinancialConnectionsAccount(self):
+        """Test FinancialConnectionsAccount"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsAccount()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details.py` & `fuse-client-1.0.6/test/test_financial_connections_investment_security.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
 
+import sys
+import unittest
 
-class FinancialConnectionsAccountDetails(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.currency import Currency
+from fuse-client.model.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
+globals()['Currency'] = Currency
+globals()['FinancialConnectionsInvestmentSecurityExchange'] = FinancialConnectionsInvestmentSecurityExchange
+from fuse-client.model.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 
-    Do not edit the class manually.
 
-    FinancialConnectionsAccountDetails - a model defined in OpenAPI
+class TestFinancialConnectionsInvestmentSecurity(unittest.TestCase):
+    """FinancialConnectionsInvestmentSecurity unit test stubs"""
 
-        remote_id: The remote_id of this FinancialConnectionsAccountDetails.
-        ach: The ach of this FinancialConnectionsAccountDetails.
-    """
+    def setUp(self):
+        pass
 
-    remote_id: str = Field(alias="remote_id")
-    ach: FinancialConnectionsAccountDetailsAch = Field(alias="ach")
+    def tearDown(self):
+        pass
 
-FinancialConnectionsAccountDetails.update_forward_refs()
+    def testFinancialConnectionsInvestmentSecurity(self):
+        """Test FinancialConnectionsInvestmentSecurity"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsInvestmentSecurity()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details_ach.py` & `fuse-client-1.0.6/test/test_financial_connections_account_details.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionsAccountDetailsAch(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
+globals()['FinancialConnectionsAccountDetailsAch'] = FinancialConnectionsAccountDetailsAch
+from fuse-client.model.financial_connections_account_details import FinancialConnectionsAccountDetails
 
-    Do not edit the class manually.
 
-    FinancialConnectionsAccountDetailsAch - a model defined in OpenAPI
+class TestFinancialConnectionsAccountDetails(unittest.TestCase):
+    """FinancialConnectionsAccountDetails unit test stubs"""
 
-        account: The account of this FinancialConnectionsAccountDetailsAch [Optional].
-        routing: The routing of this FinancialConnectionsAccountDetailsAch [Optional].
-        wire_routing: The wire_routing of this FinancialConnectionsAccountDetailsAch [Optional].
-        bacs_routing: The bacs_routing of this FinancialConnectionsAccountDetailsAch [Optional].
-    """
+    def setUp(self):
+        pass
 
-    account: Optional[str] = Field(alias="account", default=None)
-    routing: Optional[str] = Field(alias="routing", default=None)
-    wire_routing: Optional[str] = Field(alias="wire_routing", default=None)
-    bacs_routing: Optional[str] = Field(alias="bacs_routing", default=None)
+    def tearDown(self):
+        pass
 
-FinancialConnectionsAccountDetailsAch.update_forward_refs()
+    def testFinancialConnectionsAccountDetails(self):
+        """Test FinancialConnectionsAccountDetails"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsAccountDetails()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security.py` & `fuse-client-1.0.6/test/test_migrate_financial_connections_aggregator_connection_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.currency import Currency
-from fuse_client.models.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
-
-
-class FinancialConnectionsInvestmentSecurity(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
-
-    Do not edit the class manually.
-
-    FinancialConnectionsInvestmentSecurity - a model defined in OpenAPI
-
-        remote_id: The remote_id of this FinancialConnectionsInvestmentSecurity.
-        symbol: The symbol of this FinancialConnectionsInvestmentSecurity.
-        isin: The isin of this FinancialConnectionsInvestmentSecurity [Optional].
-        sedol: The sedol of this FinancialConnectionsInvestmentSecurity [Optional].
-        cusip: The cusip of this FinancialConnectionsInvestmentSecurity [Optional].
-        close_price: The close_price of this FinancialConnectionsInvestmentSecurity.
-        currency: The currency of this FinancialConnectionsInvestmentSecurity.
-        name: The name of this FinancialConnectionsInvestmentSecurity [Optional].
-        type: The type of this FinancialConnectionsInvestmentSecurity [Optional].
-        exchange: The exchange of this FinancialConnectionsInvestmentSecurity [Optional].
-    """
-
-    remote_id: str = Field(alias="remote_id")
-    symbol: str = Field(alias="symbol")
-    isin: Optional[str] = Field(alias="isin", default=None)
-    sedol: Optional[str] = Field(alias="sedol", default=None)
-    cusip: Optional[str] = Field(alias="cusip", default=None)
-    close_price: float = Field(alias="close_price")
-    currency: Currency = Field(alias="currency")
-    name: Optional[str] = Field(alias="name", default=None)
-    type: Optional[str] = Field(alias="type", default=None)
-    exchange: Optional[FinancialConnectionsInvestmentSecurityExchange] = Field(alias="exchange", default=None)
 
-FinancialConnectionsInvestmentSecurity.update_forward_refs()
+import sys
+import unittest
+
+import fuse-client
+from fuse-client.model.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
+from fuse-client.model.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
+globals()['MigrateFinancialConnectionsAggregatorConnectionDataMx'] = MigrateFinancialConnectionsAggregatorConnectionDataMx
+globals()['MigrateFinancialConnectionsAggregatorConnectionDataPlaid'] = MigrateFinancialConnectionsAggregatorConnectionDataPlaid
+from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+
+
+class TestMigrateFinancialConnectionsAggregatorConnectionData(unittest.TestCase):
+    """MigrateFinancialConnectionsAggregatorConnectionData unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMigrateFinancialConnectionsAggregatorConnectionData(self):
+        """Test MigrateFinancialConnectionsAggregatorConnectionData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MigrateFinancialConnectionsAggregatorConnectionData()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner.py` & `fuse-client-1.0.6/test/test_get_financial_connections_accounts_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.financial_connections_owner_addresses_inner import FinancialConnectionsOwnerAddressesInner
-from fuse_client.models.financial_connections_owner_emails_inner import FinancialConnectionsOwnerEmailsInner
-from fuse_client.models.financial_connections_owner_names_inner import FinancialConnectionsOwnerNamesInner
-from fuse_client.models.financial_connections_owner_phone_numbers_inner import FinancialConnectionsOwnerPhoneNumbersInner
 
+import sys
+import unittest
 
-class FinancialConnectionsOwner(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connection_data import FinancialConnectionData
+from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+globals()['FinancialConnectionData'] = FinancialConnectionData
+globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
+from fuse-client.model.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
 
-    Do not edit the class manually.
 
-    FinancialConnectionsOwner - a model defined in OpenAPI
+class TestGetFinancialConnectionsAccountsResponse(unittest.TestCase):
+    """GetFinancialConnectionsAccountsResponse unit test stubs"""
 
-        addresses: The addresses of this FinancialConnectionsOwner.
-        emails: The emails of this FinancialConnectionsOwner.
-        names: The names of this FinancialConnectionsOwner.
-        phone_numbers: The phone_numbers of this FinancialConnectionsOwner.
-    """
+    def setUp(self):
+        pass
 
-    addresses: List[FinancialConnectionsOwnerAddressesInner] = Field(alias="addresses")
-    emails: List[FinancialConnectionsOwnerEmailsInner] = Field(alias="emails")
-    names: List[FinancialConnectionsOwnerNamesInner] = Field(alias="names")
-    phone_numbers: List[FinancialConnectionsOwnerPhoneNumbersInner] = Field(alias="phone_numbers")
+    def tearDown(self):
+        pass
 
-FinancialConnectionsOwner.update_forward_refs()
+    def testGetFinancialConnectionsAccountsResponse(self):
+        """Test GetFinancialConnectionsAccountsResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsAccountsResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner_data.py` & `fuse-client-1.0.6/test/test_financial_connections_owner_addresses.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionsOwnerAddressesInnerData(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
+globals()['FinancialConnectionsOwnerData'] = FinancialConnectionsOwnerData
+from fuse-client.model.financial_connections_owner_addresses import FinancialConnectionsOwnerAddresses
 
-    Do not edit the class manually.
 
-    FinancialConnectionsOwnerAddressesInnerData - a model defined in OpenAPI
+class TestFinancialConnectionsOwnerAddresses(unittest.TestCase):
+    """FinancialConnectionsOwnerAddresses unit test stubs"""
 
-        city: The city of this FinancialConnectionsOwnerAddressesInnerData [Optional].
-        country: The country of this FinancialConnectionsOwnerAddressesInnerData [Optional].
-        postal_code: The postal_code of this FinancialConnectionsOwnerAddressesInnerData [Optional].
-        region: The region of this FinancialConnectionsOwnerAddressesInnerData [Optional].
-        street: The street of this FinancialConnectionsOwnerAddressesInnerData [Optional].
-    """
+    def setUp(self):
+        pass
 
-    city: Optional[str] = Field(alias="city", default=None)
-    country: Optional[str] = Field(alias="country", default=None)
-    postal_code: Optional[str] = Field(alias="postal_code", default=None)
-    region: Optional[str] = Field(alias="region", default=None)
-    street: Optional[str] = Field(alias="street", default=None)
+    def tearDown(self):
+        pass
 
-FinancialConnectionsOwnerAddressesInnerData.update_forward_refs()
+    def testFinancialConnectionsOwnerAddresses(self):
+        """Test FinancialConnectionsOwnerAddresses"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsOwnerAddresses()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_emails_inner.py` & `fuse-client-1.0.6/test/test_financial_connections_owner_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionsOwnerEmailsInner(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner_data import FinancialConnectionsOwnerData
 
-    Do not edit the class manually.
 
-    FinancialConnectionsOwnerEmailsInner - a model defined in OpenAPI
+class TestFinancialConnectionsOwnerData(unittest.TestCase):
+    """FinancialConnectionsOwnerData unit test stubs"""
 
-        data: The data of this FinancialConnectionsOwnerEmailsInner.
-        primary: The primary of this FinancialConnectionsOwnerEmailsInner [Optional].
-        type: The type of this FinancialConnectionsOwnerEmailsInner [Optional].
-    """
+    def setUp(self):
+        pass
 
-    data: str = Field(alias="data")
-    primary: Optional[bool] = Field(alias="primary", default=None)
-    type: Optional[str] = Field(alias="type", default=None)
+    def tearDown(self):
+        pass
 
-FinancialConnectionsOwnerEmailsInner.update_forward_refs()
+    def testFinancialConnectionsOwnerData(self):
+        """Test FinancialConnectionsOwnerData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsOwnerData()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_phone_numbers_inner.py` & `fuse-client-1.0.6/test/test_financial_connections_owner_phone_numbers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class FinancialConnectionsOwnerPhoneNumbersInner(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner_phone_numbers import FinancialConnectionsOwnerPhoneNumbers
 
-    Do not edit the class manually.
 
-    FinancialConnectionsOwnerPhoneNumbersInner - a model defined in OpenAPI
+class TestFinancialConnectionsOwnerPhoneNumbers(unittest.TestCase):
+    """FinancialConnectionsOwnerPhoneNumbers unit test stubs"""
 
-        data: The data of this FinancialConnectionsOwnerPhoneNumbersInner.
-        primary: The primary of this FinancialConnectionsOwnerPhoneNumbersInner [Optional].
-        type: The type of this FinancialConnectionsOwnerPhoneNumbersInner [Optional].
-    """
+    def setUp(self):
+        pass
 
-    data: str = Field(alias="data")
-    primary: Optional[bool] = Field(alias="primary", default=None)
-    type: Optional[str] = Field(alias="type", default=None)
+    def tearDown(self):
+        pass
 
-FinancialConnectionsOwnerPhoneNumbersInner.update_forward_refs()
+    def testFinancialConnectionsOwnerPhoneNumbers(self):
+        """Test FinancialConnectionsOwnerPhoneNumbers"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FinancialConnectionsOwnerPhoneNumbers()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/fuse_api_error_data.py` & `fuse-client-1.0.6/test/test_fuse_api_error_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.aggregator import Aggregator
-from fuse_client.models.fuse_api_error import FuseApiError
 
+import sys
+import unittest
 
-class FuseApiErrorData(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.aggregator import Aggregator
+from fuse-client.model.fuse_api_error import FuseApiError
+globals()['Aggregator'] = Aggregator
+globals()['FuseApiError'] = FuseApiError
+from fuse-client.model.fuse_api_error_data import FuseApiErrorData
 
-    Do not edit the class manually.
 
-    FuseApiErrorData - a model defined in OpenAPI
+class TestFuseApiErrorData(unittest.TestCase):
+    """FuseApiErrorData unit test stubs"""
 
-        aggregator: The aggregator of this FuseApiErrorData [Optional].
-        errors: The errors of this FuseApiErrorData [Optional].
-    """
+    def setUp(self):
+        pass
 
-    aggregator: Optional[Aggregator] = Field(alias="aggregator", default=None)
-    errors: Optional[List[FuseApiError]] = Field(alias="errors", default=None)
+    def tearDown(self):
+        pass
 
-FuseApiErrorData.update_forward_refs()
+    def testFuseApiErrorData(self):
+        """Test FuseApiErrorData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FuseApiErrorData()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_request.py` & `fuse-client-1.0.6/test/test_get_asset_report_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class GetAssetReportRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.get_asset_report_response_report import GetAssetReportResponseReport
+globals()['GetAssetReportResponseReport'] = GetAssetReportResponseReport
+from fuse-client.model.get_asset_report_response import GetAssetReportResponse
 
-    Do not edit the class manually.
 
-    GetAssetReportRequest - a model defined in OpenAPI
+class TestGetAssetReportResponse(unittest.TestCase):
+    """GetAssetReportResponse unit test stubs"""
 
-        asset_report_token: The asset_report_token of this GetAssetReportRequest.
-    """
+    def setUp(self):
+        pass
 
-    asset_report_token: str = Field(alias="asset_report_token")
+    def tearDown(self):
+        pass
 
-GetAssetReportRequest.update_forward_refs()
+    def testGetAssetReportResponse(self):
+        """Test GetAssetReportResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetAssetReportResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report.py` & `fuse-client-1.0.6/test/test_get_asset_report_response_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.fuse_api_warning import FuseApiWarning
-from fuse_client.models.get_asset_report_response_report_accounts_inner import GetAssetReportResponseReportAccountsInner
 
+import sys
+import unittest
 
-class GetAssetReportResponseReport(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.fuse_api_warning import FuseApiWarning
+from fuse-client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
+globals()['FuseApiWarning'] = FuseApiWarning
+globals()['GetAssetReportResponseReportAccounts'] = GetAssetReportResponseReportAccounts
+from fuse-client.model.get_asset_report_response_report import GetAssetReportResponseReport
 
-    Do not edit the class manually.
 
-    GetAssetReportResponseReport - a model defined in OpenAPI
+class TestGetAssetReportResponseReport(unittest.TestCase):
+    """GetAssetReportResponseReport unit test stubs"""
 
-        asset_report_id: The asset_report_id of this GetAssetReportResponseReport [Optional].
-        client_report_id: The client_report_id of this GetAssetReportResponseReport [Optional].
-        date_generated: The date_generated of this GetAssetReportResponseReport [Optional].
-        days_requested: The days_requested of this GetAssetReportResponseReport [Optional].
-        accounts: The accounts of this GetAssetReportResponseReport [Optional].
-        warnings: The warnings of this GetAssetReportResponseReport [Optional].
-    """
+    def setUp(self):
+        pass
 
-    asset_report_id: Optional[str] = Field(alias="asset_report_id", default=None)
-    client_report_id: Optional[str] = Field(alias="client_report_id", default=None)
-    date_generated: Optional[str] = Field(alias="date_generated", default=None)
-    days_requested: Optional[int] = Field(alias="days_requested", default=None)
-    accounts: Optional[List[GetAssetReportResponseReportAccountsInner]] = Field(alias="accounts", default=None)
-    warnings: Optional[List[FuseApiWarning]] = Field(alias="warnings", default=None)
+    def tearDown(self):
+        pass
 
-GetAssetReportResponseReport.update_forward_refs()
+    def testGetAssetReportResponseReport(self):
+        """Test GetAssetReportResponseReport"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetAssetReportResponseReport()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner.py` & `fuse-client-1.0.6/test/test_get_asset_report_response_report_accounts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.financial_connections_owner import FinancialConnectionsOwner
-from fuse_client.models.get_asset_report_response_report_accounts_inner_balances import GetAssetReportResponseReportAccountsInnerBalances
-from fuse_client.models.get_asset_report_response_report_accounts_inner_historical_balances_inner import GetAssetReportResponseReportAccountsInnerHistoricalBalancesInner
 
+import sys
+import unittest
 
-class GetAssetReportResponseReportAccountsInner(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
+from fuse-client.model.get_asset_report_response_report_balances import GetAssetReportResponseReportBalances
+from fuse-client.model.get_asset_report_response_report_historical_balances import GetAssetReportResponseReportHistoricalBalances
+globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
+globals()['GetAssetReportResponseReportBalances'] = GetAssetReportResponseReportBalances
+globals()['GetAssetReportResponseReportHistoricalBalances'] = GetAssetReportResponseReportHistoricalBalances
+from fuse-client.model.get_asset_report_response_report_accounts import GetAssetReportResponseReportAccounts
 
-    Do not edit the class manually.
 
-    GetAssetReportResponseReportAccountsInner - a model defined in OpenAPI
+class TestGetAssetReportResponseReportAccounts(unittest.TestCase):
+    """GetAssetReportResponseReportAccounts unit test stubs"""
 
-        remote_account_id: The remote_account_id of this GetAssetReportResponseReportAccountsInner [Optional].
-        balances: The balances of this GetAssetReportResponseReportAccountsInner [Optional].
-        historical_balances: The historical_balances of this GetAssetReportResponseReportAccountsInner [Optional].
-        owners: The owners of this GetAssetReportResponseReportAccountsInner [Optional].
-    """
+    def setUp(self):
+        pass
 
-    remote_account_id: Optional[str] = Field(alias="remote_account_id", default=None)
-    balances: Optional[GetAssetReportResponseReportAccountsInnerBalances] = Field(alias="balances", default=None)
-    historical_balances: Optional[List[GetAssetReportResponseReportAccountsInnerHistoricalBalancesInner]] = Field(alias="historical_balances", default=None)
-    owners: Optional[List[FinancialConnectionsOwner]] = Field(alias="owners", default=None)
+    def tearDown(self):
+        pass
 
-GetAssetReportResponseReportAccountsInner.update_forward_refs()
+    def testGetAssetReportResponseReportAccounts(self):
+        """Test GetAssetReportResponseReportAccounts"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetAssetReportResponseReportAccounts()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_response.py` & `fuse-client-1.0.6/test/test_migrate_financial_connections_token_request_entity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.financial_connection_data import FinancialConnectionData
-from fuse_client.models.financial_connections_account import FinancialConnectionsAccount
 
+import sys
+import unittest
 
-class GetFinancialConnectionsAccountsResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
 
-    Do not edit the class manually.
 
-    GetFinancialConnectionsAccountsResponse - a model defined in OpenAPI
+class TestMigrateFinancialConnectionsTokenRequestEntity(unittest.TestCase):
+    """MigrateFinancialConnectionsTokenRequestEntity unit test stubs"""
 
-        accounts: The accounts of this GetFinancialConnectionsAccountsResponse.
-        financial_connection: The financial_connection of this GetFinancialConnectionsAccountsResponse.
-        request_id: The request_id of this GetFinancialConnectionsAccountsResponse.
-    """
+    def setUp(self):
+        pass
 
-    accounts: List[FinancialConnectionsAccount] = Field(alias="accounts")
-    financial_connection: FinancialConnectionData = Field(alias="financial_connection")
-    request_id: str = Field(alias="request_id")
+    def tearDown(self):
+        pass
 
-GetFinancialConnectionsAccountsResponse.update_forward_refs()
+    def testMigrateFinancialConnectionsTokenRequestEntity(self):
+        """Test MigrateFinancialConnectionsTokenRequestEntity"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MigrateFinancialConnectionsTokenRequestEntity()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request.py` & `fuse-client-1.0.6/test/test_get_financial_connections_balance_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
 
+import sys
+import unittest
 
-class GetFinancialConnectionsBalanceRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account_balance import FinancialConnectionsAccountBalance
+globals()['FinancialConnectionsAccountBalance'] = FinancialConnectionsAccountBalance
+from fuse-client.model.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
 
-    Do not edit the class manually.
 
-    GetFinancialConnectionsBalanceRequest - a model defined in OpenAPI
+class TestGetFinancialConnectionsBalanceResponse(unittest.TestCase):
+    """GetFinancialConnectionsBalanceResponse unit test stubs"""
 
-        access_token: The access_token of this GetFinancialConnectionsBalanceRequest.
-        options: The options of this GetFinancialConnectionsBalanceRequest [Optional].
-    """
+    def setUp(self):
+        pass
 
-    access_token: str = Field(alias="access_token")
-    options: Optional[GetFinancialConnectionsBalanceRequestOptions] = Field(alias="options", default=None)
+    def tearDown(self):
+        pass
 
-GetFinancialConnectionsBalanceRequest.update_forward_refs()
+    def testGetFinancialConnectionsBalanceResponse(self):
+        """Test GetFinancialConnectionsBalanceResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsBalanceResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response.py` & `fuse-client-1.0.6/test/test_get_financial_connections_owners_response_accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.get_financial_connections_owners_response_accounts_inner import GetFinancialConnectionsOwnersResponseAccountsInner
 
+import sys
+import unittest
 
-class GetFinancialConnectionsOwnersResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_owner import FinancialConnectionsOwner
+globals()['FinancialConnectionsOwner'] = FinancialConnectionsOwner
+from fuse-client.model.get_financial_connections_owners_response_accounts import GetFinancialConnectionsOwnersResponseAccounts
 
-    Do not edit the class manually.
 
-    GetFinancialConnectionsOwnersResponse - a model defined in OpenAPI
+class TestGetFinancialConnectionsOwnersResponseAccounts(unittest.TestCase):
+    """GetFinancialConnectionsOwnersResponseAccounts unit test stubs"""
 
-        accounts: The accounts of this GetFinancialConnectionsOwnersResponse.
-    """
+    def setUp(self):
+        pass
 
-    accounts: List[GetFinancialConnectionsOwnersResponseAccountsInner] = Field(alias="accounts")
+    def tearDown(self):
+        pass
 
-GetFinancialConnectionsOwnersResponse.update_forward_refs()
+    def testGetFinancialConnectionsOwnersResponseAccounts(self):
+        """Test GetFinancialConnectionsOwnersResponseAccounts"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsOwnersResponseAccounts()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_response.py` & `fuse-client-1.0.6/test/test_get_financial_connections_transactions_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.transaction import Transaction
 
+import sys
+import unittest
 
-class GetFinancialConnectionsTransactionsResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
 
-    Do not edit the class manually.
 
-    GetFinancialConnectionsTransactionsResponse - a model defined in OpenAPI
+class TestGetFinancialConnectionsTransactionsRequest(unittest.TestCase):
+    """GetFinancialConnectionsTransactionsRequest unit test stubs"""
 
-        transactions: The transactions of this GetFinancialConnectionsTransactionsResponse.
-        total_transactions: The total_transactions of this GetFinancialConnectionsTransactionsResponse.
-        request_id: The request_id of this GetFinancialConnectionsTransactionsResponse.
-    """
+    def setUp(self):
+        pass
 
-    transactions: List[Transaction] = Field(alias="transactions")
-    total_transactions: float = Field(alias="total_transactions")
-    request_id: str = Field(alias="request_id")
+    def tearDown(self):
+        pass
 
-GetFinancialConnectionsTransactionsResponse.update_forward_refs()
+    def testGetFinancialConnectionsTransactionsRequest(self):
+        """Test GetFinancialConnectionsTransactionsRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsTransactionsRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request.py` & `fuse-client-1.0.6/test/test_get_investment_holdings_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 
+import sys
+import unittest
 
-class GetInvestmentHoldingsRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.financial_connections_account import FinancialConnectionsAccount
+from fuse-client.model.financial_connections_holding import FinancialConnectionsHolding
+globals()['FinancialConnectionsAccount'] = FinancialConnectionsAccount
+globals()['FinancialConnectionsHolding'] = FinancialConnectionsHolding
+from fuse-client.model.get_investment_holdings_response import GetInvestmentHoldingsResponse
 
-    Do not edit the class manually.
 
-    GetInvestmentHoldingsRequest - a model defined in OpenAPI
+class TestGetInvestmentHoldingsResponse(unittest.TestCase):
+    """GetInvestmentHoldingsResponse unit test stubs"""
 
-        access_token: The access_token of this GetInvestmentHoldingsRequest.
-        options: The options of this GetInvestmentHoldingsRequest [Optional].
-    """
+    def setUp(self):
+        pass
 
-    access_token: str = Field(alias="access_token")
-    options: Optional[GetInvestmentHoldingsRequestOptions] = Field(alias="options", default=None)
+    def tearDown(self):
+        pass
 
-GetInvestmentHoldingsRequest.update_forward_refs()
+    def testGetInvestmentHoldingsResponse(self):
+        """Test GetInvestmentHoldingsResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetInvestmentHoldingsResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request_options.py` & `fuse-client-1.0.6/test/test_get_investment_holdings_request_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,35 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
+import sys
+import unittest
 
-class GetInvestmentTransactionsRequestOptions(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 
-    Do not edit the class manually.
 
-    GetInvestmentTransactionsRequestOptions - a model defined in OpenAPI
+class TestGetInvestmentHoldingsRequestOptions(unittest.TestCase):
+    """GetInvestmentHoldingsRequestOptions unit test stubs"""
 
-        remote_account_ids: The remote_account_ids of this GetInvestmentTransactionsRequestOptions [Optional].
-    """
+    def setUp(self):
+        pass
 
-    remote_account_ids: Optional[List[str]] = Field(alias="remote_account_ids", default=None)
+    def tearDown(self):
+        pass
 
-GetInvestmentTransactionsRequestOptions.update_forward_refs()
+    def testGetInvestmentHoldingsRequestOptions(self):
+        """Test GetInvestmentHoldingsRequestOptions"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetInvestmentHoldingsRequestOptions()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_response.py` & `fuse-client-1.0.6/test/test_get_financial_connections_transactions_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.financial_connections_account import FinancialConnectionsAccount
-from fuse_client.models.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
 
+import sys
+import unittest
 
-class GetInvestmentTransactionsResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.transaction import Transaction
+globals()['Transaction'] = Transaction
+from fuse-client.model.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
 
-    Do not edit the class manually.
 
-    GetInvestmentTransactionsResponse - a model defined in OpenAPI
+class TestGetFinancialConnectionsTransactionsResponse(unittest.TestCase):
+    """GetFinancialConnectionsTransactionsResponse unit test stubs"""
 
-        accounts: The accounts of this GetInvestmentTransactionsResponse.
-        investment_transactions: The investment_transactions of this GetInvestmentTransactionsResponse.
-        request_id: The request_id of this GetInvestmentTransactionsResponse.
-    """
+    def setUp(self):
+        pass
 
-    accounts: List[FinancialConnectionsAccount] = Field(alias="accounts")
-    investment_transactions: List[FinancialConnectionsInvestmentTransaction] = Field(alias="investment_transactions")
-    request_id: str = Field(alias="request_id")
+    def tearDown(self):
+        pass
 
-GetInvestmentTransactionsResponse.update_forward_refs()
+    def testGetFinancialConnectionsTransactionsResponse(self):
+        """Test GetFinancialConnectionsTransactionsResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsTransactionsResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data.py` & `fuse-client-1.0.6/test/test_migrate_financial_connections_token_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
-from fuse_client.models.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 
+import sys
+import unittest
 
-class MigrateFinancialConnectionsAggregatorConnectionData(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse-client.model.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
+from fuse-client.model.product import Product
+globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
+globals()['MigrateFinancialConnectionsTokenRequestEntity'] = MigrateFinancialConnectionsTokenRequestEntity
+globals()['Product'] = Product
+from fuse-client.model.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
 
-    Do not edit the class manually.
 
-    MigrateFinancialConnectionsAggregatorConnectionData - a model defined in OpenAPI
+class TestMigrateFinancialConnectionsTokenRequest(unittest.TestCase):
+    """MigrateFinancialConnectionsTokenRequest unit test stubs"""
 
-        plaid: The plaid of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
-        mx: The mx of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
-    """
+    def setUp(self):
+        pass
 
-    plaid: Optional[MigrateFinancialConnectionsAggregatorConnectionDataPlaid] = Field(alias="plaid", default=None)
-    mx: Optional[MigrateFinancialConnectionsAggregatorConnectionDataMx] = Field(alias="mx", default=None)
+    def tearDown(self):
+        pass
 
-MigrateFinancialConnectionsAggregatorConnectionData.update_forward_refs()
+    def testMigrateFinancialConnectionsTokenRequest(self):
+        """Test MigrateFinancialConnectionsTokenRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MigrateFinancialConnectionsTokenRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request.py` & `fuse-client-1.0.6/test/test_migrate_financial_connections_token_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-from fuse_client.models.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
-from fuse_client.models.product import Product
 
+import sys
+import unittest
 
-class MigrateFinancialConnectionsTokenRequest(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+globals()['MigrateFinancialConnectionsAggregatorConnectionData'] = MigrateFinancialConnectionsAggregatorConnectionData
+from fuse-client.model.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
 
-    Do not edit the class manually.
 
-    MigrateFinancialConnectionsTokenRequest - a model defined in OpenAPI
+class TestMigrateFinancialConnectionsTokenResponse(unittest.TestCase):
+    """MigrateFinancialConnectionsTokenResponse unit test stubs"""
 
-        connection_data: The connection_data of this MigrateFinancialConnectionsTokenRequest.
-        aggregator: The aggregator of this MigrateFinancialConnectionsTokenRequest.
-        entity: The entity of this MigrateFinancialConnectionsTokenRequest.
-        fuse_products: The fuse_products of this MigrateFinancialConnectionsTokenRequest.
-    """
+    def setUp(self):
+        pass
 
-    connection_data: MigrateFinancialConnectionsAggregatorConnectionData = Field(alias="connection_data")
-    aggregator: str = Field(alias="aggregator")
-    entity: MigrateFinancialConnectionsTokenRequestEntity = Field(alias="entity")
-    fuse_products: List[Product] = Field(alias="fuse_products")
+    def tearDown(self):
+        pass
 
-MigrateFinancialConnectionsTokenRequest.update_forward_refs()
+    def testMigrateFinancialConnectionsTokenResponse(self):
+        """Test MigrateFinancialConnectionsTokenResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MigrateFinancialConnectionsTokenResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_response.py` & `fuse-client-1.0.6/test/test_get_financial_connections_balance_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
 
+import sys
+import unittest
 
-class MigrateFinancialConnectionsTokenResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
+globals()['GetFinancialConnectionsBalanceRequestOptions'] = GetFinancialConnectionsBalanceRequestOptions
+from fuse-client.model.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
 
-    Do not edit the class manually.
 
-    MigrateFinancialConnectionsTokenResponse - a model defined in OpenAPI
+class TestGetFinancialConnectionsBalanceRequest(unittest.TestCase):
+    """GetFinancialConnectionsBalanceRequest unit test stubs"""
 
-        connection_data: The connection_data of this MigrateFinancialConnectionsTokenResponse.
-        fuse_access_token: The fuse_access_token of this MigrateFinancialConnectionsTokenResponse.
-        fuse_financial_connection_id: The fuse_financial_connection_id of this MigrateFinancialConnectionsTokenResponse.
-        request_id: The request_id of this MigrateFinancialConnectionsTokenResponse [Optional].
-    """
+    def setUp(self):
+        pass
 
-    connection_data: MigrateFinancialConnectionsAggregatorConnectionData = Field(alias="connection_data")
-    fuse_access_token: str = Field(alias="fuse_access_token")
-    fuse_financial_connection_id: str = Field(alias="fuse_financial_connection_id")
-    request_id: Optional[str] = Field(alias="request_id", default=None)
+    def tearDown(self):
+        pass
 
-MigrateFinancialConnectionsTokenResponse.update_forward_refs()
+    def testGetFinancialConnectionsBalanceRequest(self):
+        """Test GetFinancialConnectionsBalanceRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = GetFinancialConnectionsBalanceRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response.py` & `fuse-client-1.0.6/test/test_sync_transactions_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# coding: utf-8
+"""
+    Fuse
 
-from __future__ import annotations
-from datetime import date, datetime  # noqa: F401
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-import re  # noqa: F401
-from typing import Any, Dict, List, Optional  # noqa: F401
+    The version of the OpenAPI document: 1.0.0
+    Generated by: https://openapi-generator.tech
+"""
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from fuse_client.models.sync_transactions_response_removed_inner import SyncTransactionsResponseRemovedInner
-from fuse_client.models.transaction import Transaction
 
+import sys
+import unittest
 
-class SyncTransactionsResponse(BaseModel):
-    """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
+import fuse-client
+from fuse-client.model.sync_transactions_response_removed import SyncTransactionsResponseRemoved
+from fuse-client.model.transaction import Transaction
+globals()['SyncTransactionsResponseRemoved'] = SyncTransactionsResponseRemoved
+globals()['Transaction'] = Transaction
+from fuse-client.model.sync_transactions_response import SyncTransactionsResponse
 
-    Do not edit the class manually.
 
-    SyncTransactionsResponse - a model defined in OpenAPI
+class TestSyncTransactionsResponse(unittest.TestCase):
+    """SyncTransactionsResponse unit test stubs"""
 
-        added: The added of this SyncTransactionsResponse [Optional].
-        modified: The modified of this SyncTransactionsResponse [Optional].
-        removed: The removed of this SyncTransactionsResponse [Optional].
-        next_cursor: The next_cursor of this SyncTransactionsResponse [Optional].
-        has_next: The has_next of this SyncTransactionsResponse [Optional].
-        request_id: The request_id of this SyncTransactionsResponse [Optional].
-    """
+    def setUp(self):
+        pass
 
-    added: Optional[List[Transaction]] = Field(alias="added", default=None)
-    modified: Optional[List[Transaction]] = Field(alias="modified", default=None)
-    removed: Optional[List[SyncTransactionsResponseRemovedInner]] = Field(alias="removed", default=None)
-    next_cursor: Optional[str] = Field(alias="next_cursor", default=None)
-    has_next: Optional[bool] = Field(alias="has_next", default=None)
-    request_id: Optional[str] = Field(alias="request_id", default=None)
+    def tearDown(self):
+        pass
 
-SyncTransactionsResponse.update_forward_refs()
+    def testSyncTransactionsResponse(self):
+        """Test SyncTransactionsResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = SyncTransactionsResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

