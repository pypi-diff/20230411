# Comparing `tmp/tigeropen-2.3.5.tar.gz` & `tmp/tigeropen-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.3.5.tar", last modified: Wed Mar 29 02:32:12 2023, max compression
+gzip compressed data, was "tigeropen-2.3.6.tar", last modified: Tue Apr 11 08:56:40 2023, max compression
```

## Comparing `tigeropen-2.3.5.tar` & `tigeropen-2.3.6.tar`

### file list

```diff
@@ -1,205 +1,207 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.848320 tigeropen-2.3.5/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.5/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-03-29 02:32:12.847941 tigeropen-2.3.5/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.5/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.5/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-03-29 02:32:12.848431 tigeropen-2.3.5/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1407 2023-02-16 07:36:42.000000 tigeropen-2.3.5/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.761104 tigeropen-2.3.5/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.767817 tigeropen-2.3.5/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.773558 tigeropen-2.3.5/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    18954 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.5/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.5/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2801 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.5/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.777892 tigeropen-2.3.5/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-02-16 07:36:42.000000 tigeropen-2.3.5/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.5/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.5/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.780233 tigeropen-2.3.5/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.780712 tigeropen-2.3.5/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.780983 tigeropen-2.3.5/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.781522 tigeropen-2.3.5/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.782516 tigeropen-2.3.5/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.785587 tigeropen-2.3.5/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.5/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.5/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.787588 tigeropen-2.3.5/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.790482 tigeropen-2.3.5/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.812558 tigeropen-2.3.5/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1030 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1749 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2314 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)     8946 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.5/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.813415 tigeropen-2.3.5/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.818551 tigeropen-2.3.5/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     8125 2023-02-16 07:36:42.000000 tigeropen-2.3.5/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    72752 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.819280 tigeropen-2.3.5/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    25132 2023-03-10 10:02:27.000000 tigeropen-2.3.5/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.836611 tigeropen-2.3.5/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.5/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.5/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.5/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1129 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.5/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.5/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.5/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.5/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.5/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.838015 tigeropen-2.3.5/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.840722 tigeropen-2.3.5/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     4117 2023-01-11 10:23:46.000000 tigeropen-2.3.5/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)     9743 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     1682 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.5/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.841703 tigeropen-2.3.5/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.5/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    29977 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.847386 tigeropen-2.3.5/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.5/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6627 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     3878 2021-08-30 08:30:28.000000 tigeropen-2.3.5/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.5/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.5/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    39155 2023-03-29 02:32:08.000000 tigeropen-2.3.5/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:12.764986 tigeropen-2.3.5/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-03-29 02:32:12.000000 tigeropen-2.3.5/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7256 2023-03-29 02:32:12.000000 tigeropen-2.3.5/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-03-29 02:32:12.000000 tigeropen-2.3.5/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-03-29 02:32:12.000000 tigeropen-2.3.5/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-03-29 02:32:12.000000 tigeropen-2.3.5/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.852808 tigeropen-2.3.6/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.6/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-04-11 08:56:40.852337 tigeropen-2.3.6/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.6/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.6/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-04-11 08:56:40.852957 tigeropen-2.3.6/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1407 2023-02-16 07:36:42.000000 tigeropen-2.3.6/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.780294 tigeropen-2.3.6/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-04-11 08:56:25.000000 tigeropen-2.3.6/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.784104 tigeropen-2.3.6/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.788206 tigeropen-2.3.6/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.6/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    18954 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.6/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2887 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.6/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.792018 tigeropen-2.3.6/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-02-16 07:36:42.000000 tigeropen-2.3.6/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.6/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.6/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.6/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.793868 tigeropen-2.3.6/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.794345 tigeropen-2.3.6/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.794764 tigeropen-2.3.6/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.795037 tigeropen-2.3.6/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.795594 tigeropen-2.3.6/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.798237 tigeropen-2.3.6/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.799595 tigeropen-2.3.6/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.803032 tigeropen-2.3.6/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.817382 tigeropen-2.3.6/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1030 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1749 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2314 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.6/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)     8946 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.817969 tigeropen-2.3.6/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.823029 tigeropen-2.3.6/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9598 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    76032 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.823956 tigeropen-2.3.6/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33338 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.842691 tigeropen-2.3.6/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.6/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.6/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.6/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1129 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.6/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.6/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.843402 tigeropen-2.3.6/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.845848 tigeropen-2.3.6/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4117 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9743 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1682 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.847154 tigeropen-2.3.6/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    29977 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.851624 tigeropen-2.3.6/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6627 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3878 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    39340 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.782340 tigeropen-2.3.6/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.3.5/PKG-INFO` & `tigeropen-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.5
+Version: 2.3.6
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.5/README.md` & `tigeropen-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/setup.py` & `tigeropen-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/__init__.py` & `tigeropen-2.3.6/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/filter_fields.py` & `tigeropen-2.3.6/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-2.3.6/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/params.py` & `tigeropen-2.3.6/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/push_types.py` & `tigeropen-2.3.6/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/quote_keys.py` & `tigeropen-2.3.6/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/service_types.py` & `tigeropen-2.3.6/tigeropen/common/consts/service_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 GRAB_QUOTE_PERMISSION = "grab_quote_permission"  # 抢占行情
 MARKET_SCANNER = "market_scanner"  # 选股器
 GET_QUOTE_PERMISSION = "get_quote_permission"
 TRADING_CALENDAR = "trading_calendar"
 STOCK_BROKER = "stock_broker"  # 港股股票实时经纪队列
 CAPITAL_DISTRIBUTION = "capital_distribution"  # 股票当日资金分布
 CAPITAL_FLOW = "capital_flow"  # 股票资金流向
+WARRANT_FILTER = "warrant_filter"
+WARRANT_REAL_TIME_QUOTE = "warrant_real_time_quote"
 
 # 期权行情
 OPTION_EXPIRATION = "option_expiration"
 OPTION_CHAIN = "option_chain"
 OPTION_BRIEF = "option_brief"
 OPTION_KLINE = "option_kline"
 OPTION_TRADE_TICK = "option_trade_tick"
```

### Comparing `tigeropen-2.3.5/tigeropen/common/consts/tick_constants.py` & `tigeropen-2.3.6/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/model.py` & `tigeropen-2.3.6/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/request.py` & `tigeropen-2.3.6/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/response.py` & `tigeropen-2.3.6/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/common_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/contract_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/order_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/price_util.py` & `tigeropen-2.3.6/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/signature_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/string_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/tick_util.py` & `tigeropen-2.3.6/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/common/util/web_utils.py` & `tigeropen-2.3.6/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/client_config.py` & `tigeropen-2.3.6/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/nasdaq100.py` & `tigeropen-2.3.6/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-2.3.6/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/push_client_demo.py` & `tigeropen-2.3.6/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-2.3.6/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/quote_client_demo.py` & `tigeropen-2.3.6/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/examples/trade_client_demo.py` & `tigeropen-2.3.6/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/request/model.py` & `tigeropen-2.3.6/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/fundamental/response/industry_response.py` & `tigeropen-2.3.6/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/__init__.py` & `tigeropen-2.3.6/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/connect.py` & `tigeropen-2.3.6/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/exception.py` & `tigeropen-2.3.6/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/listener.py` & `tigeropen-2.3.6/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/protocal.py` & `tigeropen-2.3.6/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/transport.py` & `tigeropen-2.3.6/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/network/utils.py` & `tigeropen-2.3.6/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/AssetData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PositionData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PushData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/Request.proto` & `tigeropen-2.3.6/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/Request_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/Response_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/pb/util.py` & `tigeropen-2.3.6/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/protobuf_push_client.py` & `tigeropen-2.3.6/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/push_client.py` & `tigeropen-2.3.6/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/push/stomp_push_client.py` & `tigeropen-2.3.6/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/domain/filter.py` & `tigeropen-2.3.6/tigeropen/quote/domain/filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -193,7 +193,50 @@
                 result_items.append(result_item)
                 symbols.add(item.get('symbol'))
         self.items = result_items
         self.symbols = list(symbols)
 
     def __repr__(self):
         return "ScannerResult(%s)" % self.__dict__
+
+
+class WarrantFilterItem:
+    def __init__(self, items=None, page=None, total_page=None, total_count=None, bounds=None):
+        self.items = items
+        self.page = page
+        self.total_page = total_page
+        self.total_count = total_count
+        self.bounds = bounds
+
+    def __repr__(self):
+        return "WarrantFilterItem(%s)" % self.__dict__
+
+
+class WarrantFilterBounds:
+    def __init__(self, issuer_name=None, expire_date=None, lot_size=None, entitlement_ratio=None,
+                 leverage_ratio=None, strike=None, premium=None, outstanding_ratio=None,
+                 implied_volatility=None, effective_leverage=None, call_price=None, state=None):
+
+        if expire_date is None:
+            expire_date = set()
+        if issuer_name is None:
+            issuer_name = set()
+        if entitlement_ratio is None:
+            entitlement_ratio = set()
+        if lot_size is None:
+            lot_size = set()
+
+        self.issuer_name = issuer_name
+        self.expire_date = expire_date
+        self.lot_size = lot_size
+        self.entitlement_ratio = entitlement_ratio
+        self.leverage_ratio = leverage_ratio
+        self.strike = strike
+        self.premium = premium
+        self.outstanding_ratio = outstanding_ratio
+        self.implied_volatility = implied_volatility
+        self.effective_leverage = effective_leverage
+        self.call_price = call_price
+
+    def __repr__(self):
+        return "FilterBounds(%s)" % self.__dict__
+
```

### Comparing `tigeropen-2.3.5/tigeropen/quote/domain/quote_brief.py` & `tigeropen-2.3.6/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/domain/stock_broker.py` & `tigeropen-2.3.6/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/quote_client.py` & `tigeropen-2.3.6/tigeropen/quote/quote_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from tigeropen.common.consts import Market, QuoteRight, BarPeriod, OPEN_API_SERVICE_VERSION_V3, \
     OPEN_API_SERVICE_VERSION_V1
 from tigeropen.common.consts import THREAD_LOCAL, SecurityType, CorporateActionType, IndustryLevel
 from tigeropen.common.consts.filter_fields import FieldBelongType
 from tigeropen.common.consts.service_types import GRAB_QUOTE_PERMISSION, QUOTE_DELAY, GET_QUOTE_PERMISSION, \
     HISTORY_TIMELINE, FUTURE_CONTRACT_BY_CONTRACT_CODE, TRADING_CALENDAR, FUTURE_CONTRACTS, MARKET_SCANNER, \
-    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION
+    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION, WARRANT_REAL_TIME_QUOTE, WARRANT_FILTER
 from tigeropen.common.consts.service_types import MARKET_STATE, ALL_SYMBOLS, ALL_SYMBOL_NAMES, BRIEF, \
     TIMELINE, KLINE, TRADE_TICK, OPTION_EXPIRATION, OPTION_CHAIN, FUTURE_EXCHANGE, OPTION_BRIEF, \
     OPTION_KLINE, OPTION_TRADE_TICK, FUTURE_KLINE, FUTURE_TICK, FUTURE_CONTRACT_BY_EXCHANGE_CODE, \
     FUTURE_TRADING_DATE, QUOTE_SHORTABLE_STOCKS, FUTURE_REAL_TIME_QUOTE, \
     FUTURE_CURRENT_CONTRACT, QUOTE_REAL_TIME, QUOTE_STOCK_TRADE, FINANCIAL_DAILY, FINANCIAL_REPORT, CORPORATE_ACTION, \
     QUOTE_DEPTH, INDUSTRY_LIST, INDUSTRY_STOCKS, STOCK_INDUSTRY, STOCK_DETAIL
 from tigeropen.common.exceptions import ApiException
@@ -36,15 +36,15 @@
 from tigeropen.fundamental.response.financial_report_response import FinancialReportResponse
 from tigeropen.fundamental.response.industry_response import IndustryListResponse, IndustryStocksResponse, \
     StockIndustryResponse
 from tigeropen.quote.domain.filter import OptionFilter
 from tigeropen.quote.request.model import MarketParams, MultipleQuoteParams, MultipleContractParams, \
     FutureQuoteParams, FutureExchangeParams, FutureContractParams, FutureTradingTimeParams, SingleContractParams, \
     SingleOptionQuoteParams, DepthQuoteParams, OptionChainParams, TradingCalendarParams, MarketScannerParams, \
-    StockBrokerParams, CapitalParams
+    StockBrokerParams, CapitalParams, WarrantFilterParams
 from tigeropen.quote.response.capital_distribution_response import CapitalDistributionResponse
 from tigeropen.quote.response.capital_flow_response import CapitalFlowResponse
 from tigeropen.quote.response.future_briefs_response import FutureBriefsResponse
 from tigeropen.quote.response.future_contract_response import FutureContractResponse
 from tigeropen.quote.response.future_exchange_response import FutureExchangeResponse
 from tigeropen.quote.response.future_quote_bar_response import FutureQuoteBarResponse
 from tigeropen.quote.response.future_quote_ticks_response import FutureTradeTickResponse
@@ -68,14 +68,16 @@
 from tigeropen.quote.response.stock_broker_response import StockBrokerResponse
 from tigeropen.quote.response.stock_details_response import StockDetailsResponse
 from tigeropen.quote.response.stock_short_interest_response import ShortInterestResponse
 from tigeropen.quote.response.stock_trade_meta_response import TradeMetaResponse
 from tigeropen.quote.response.symbol_names_response import SymbolNamesResponse
 from tigeropen.quote.response.symbols_response import SymbolsResponse
 from tigeropen.quote.response.trading_calendar_response import TradingCalendarResponse
+from tigeropen.quote.response.warrant_briefs_response import WarrantBriefsResponse
+from tigeropen.quote.response.warrant_filter_response import WarrantFilterResponse
 from tigeropen.tiger_open_client import TigerOpenClient
 from tigeropen.tiger_open_config import LANGUAGE
 
 
 class QuoteClient(TigerOpenClient):
 
     def __init__(self, client_config, logger=None, is_grab_permission=True):
@@ -729,23 +731,24 @@
             if response.is_success():
                 return response.briefs
             else:
                 raise ApiException(response.code, response.message)
 
         return None
 
-    def get_option_bars(self, identifiers, begin_time=-1, end_time=4070880000000, period=BarPeriod.DAY):
+    def get_option_bars(self, identifiers, begin_time=-1, end_time=4070880000000, period=BarPeriod.DAY, limit=None):
         """
         获取期权日K数据
         :param identifiers: 期权代码列表
         :param begin_time: 开始时间. 若是时间戳需要精确到毫秒, 为13位整数;
                                     或是日期时间格式的字符串, 如 "2019-01-01" 或 "2019-01-01 12:00:00"
         :param end_time: 结束时间. 格式同 begin_time
         :param period: 时间间隔. 可选值: DAY("day"), ONE_MINUTE("1min"), FIVE_MINUTES("5min"), HALF_HOUR("30min"),
             ONE_HOUR("60min");
+        :param limit: 每个期权的返回k线数量
         :return: pandas.DataFrame, 各 column 含义如下：
             time: 毫秒级时间戳
             open: 开盘价
             high: 最高价
             low: 最低价
             close: 收盘价
             volume: 成交量
@@ -764,14 +767,15 @@
             param.symbol = symbol
             param.expiry = date_str_to_timestamp(expiry, self._timezone)
             param.put_call = put_call
             param.strike = strike
             param.period = get_enum_value(period)
             param.begin_time = date_str_to_timestamp(begin_time, self._timezone)
             param.end_time = date_str_to_timestamp(end_time, self._timezone)
+            param.limit = limit
             contracts.append(param)
         params.contracts = contracts
         request = OpenApiRequest(OPTION_KLINE, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OptionQuoteBarResponse()
             response.parse_response_content(response_content)
@@ -1541,8 +1545,67 @@
         response_content = self.__fetch_data(request)
         if response_content:
             response = CapitalDistributionResponse()
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.result
             else:
+                raise ApiException(response.code, response.message)
+
+    def get_warrant_briefs(self, symbols):
+        """
+        get warrant/iopt quote
+        :param symbols:
+        :return:
+        """
+        params = MultipleQuoteParams()
+        params.symbols = symbols if isinstance(symbols, list) else [symbols]
+        params.lang = get_enum_value(self._lang)
+        request = OpenApiRequest(WARRANT_REAL_TIME_QUOTE, biz_model=params)
+        response_content = self.__fetch_data(request)
+        if response_content:
+            response = WarrantBriefsResponse()
+            response.parse_response_content(response_content)
+            if response.is_success():
+                return response.result
+            else:
+                raise ApiException(response.code, response.message)
+
+    def get_warrant_filter(self, symbol, page=None, page_size=None, sort_field_name=None, sort_dir=None,
+                           filter_params=None):
+        """
+        :param sort_dir: tigeropen.common.consts.SortDirection, e.g. SortDirection.DESC
+        :param filter_params: tigeropen.quote.request.model.WarrantFilterParams
+        :return:
+        """
+        params = WarrantFilterParams()
+        params.lang = get_enum_value(self._lang)
+        params.symbol = symbol or (filter_params.symbol if filter_params else None)
+        params.page = page or (filter_params.page if filter_params else None)
+        params.page_size = page_size or (filter_params.page_size if filter_params else None)
+        params.sort_field_name = sort_field_name or (filter_params.sort_field_name if filter_params else None)
+        params.sort_dir = get_enum_value(sort_dir or (filter_params.sort_dir if filter_params else None))
+        if filter_params:
+            params.warrant_type = filter_params.warrant_type
+            params.in_out_price = filter_params.in_out_price
+            params.issuer_name = filter_params.issuer_name
+            params.expire_ym = filter_params.expire_ym
+            params.lot_size = filter_params.lot_size
+            params.entitlement_ratio = filter_params.entitlement_ratio
+            params.leverage_ratio = filter_params.leverage_ratio
+            params.strike = filter_params.strike
+            params.premium = filter_params.premium
+            params.outstanding_ratio = filter_params.outstanding_ratio
+            params.implied_volatility = filter_params.implied_volatility
+            params.effective_leverage = filter_params.effective_leverage
+            params.call_price = filter_params.call_price
+            params.state = filter_params.state
+
+        request = OpenApiRequest(WARRANT_FILTER, biz_model=params)
+        response_content = self.__fetch_data(request)
+        if response_content:
+            response = WarrantFilterResponse()
+            response.parse_response_content(response_content)
+            if response.is_success():
+                return response.result
+            else:
                 raise ApiException(response.code, response.message)
```

### Comparing `tigeropen-2.3.5/tigeropen/quote/request/model.py` & `tigeropen-2.3.6/tigeropen/quote/request/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/9/20
 
 @author: gaoan
 """
 from tigeropen.common.model import BaseParams
+from tigeropen.common.util.string_utils import underline_to_camel
 
 
 class MarketParams(BaseParams):
     def __init__(self):
         super(MarketParams, self).__init__()
         self._market = None  # 市场
         self._sec_type = None  # 交易品种
@@ -1052,7 +1053,293 @@
         if self.begin_time:
             params['begin_time'] = self.begin_time
         if self.end_time:
             params['end_time'] = self.end_time
         if self.limit:
             params['limit'] = self.limit
         return params
+
+
+class WarrantFilterParams(BaseParams):
+    def __init__(self):
+        super().__init__()
+        self._symbol = None
+        self._page = None
+        self._page_size = None
+        self._sort_field_name = None
+        # sort directions
+        self._sort_dir = None
+        # 1:Call, 2: Put, 3: Bull,4: Bear, 0: All
+        self._warrant_type: set[int] = set()
+        self._issuer_name = None
+        # expiry date: yyyy-MM
+        self._expire_ym = None
+        # 0 All, 1 Normal, 2 Terminate Trades, 3 Waiting to be listed
+        self._state: int = None
+        # -1:out the money, 1: in the money
+        self._in_out_price: set[int] = set()
+        self._lot_size: set[int] = set()
+        self._entitlement_ratio: set[float] = set()
+
+        self._strike: tuple[float, float] = tuple()
+        self._effective_leverage: tuple[float, float] = tuple()
+        self._leverage_ratio: tuple[float, float] = tuple()
+        self._call_price: tuple[float, float] = tuple()
+        self._volume: tuple[int, int] = tuple()
+        self._premium: tuple[float, float] = tuple()
+        self._outstanding_ratio: tuple[float, float] = tuple()
+        self._implied_volatility: tuple[int, int] = tuple()
+
+    def set_state(self, value):
+        self._state = value
+
+    def set_issuer_name(self, value):
+        self._issuer_name = value
+
+    def set_expire_ym(self, value):
+        self._expire_ym = value
+
+    def add_warrant_type(self, value):
+        self._warrant_type.add(value)
+
+    def add_in_out_price(self, value):
+        self._in_out_price.add(value)
+
+    def add_lot_size(self, value):
+        self._lot_size.add(value)
+
+    def add_entitlement_ratio(self, value):
+        self._entitlement_ratio.add(value)
+
+    def set_strike_range(self, min_value, max_value):
+        self._strike = (min_value, max_value)
+
+    def set_effective_leverage_range(self, min_value, max_value):
+        self._effective_leverage = (min_value, max_value)
+
+    def set_leverage_ratio_range(self, min_value, max_value):
+        self._leverage_ratio = (min_value, max_value)
+
+    def set_call_price_range(self, min_value, max_value):
+        self._call_price = (min_value, max_value)
+
+    def set_volume_range(self, min_value, max_value):
+        self._volume = (min_value, max_value)
+
+    def set_premium_range(self, min_value, max_value):
+        self._premium = (min_value, max_value)
+
+    def set_outstanding_ratio_range(self, min_value, max_value):
+        self._outstanding_ratio = (min_value, max_value)
+
+    def set_implied_volatility_range(self, min_value, max_value):
+        self._implied_volatility = (min_value, max_value)
+
+    @property
+    def symbol(self):
+        return self._symbol
+
+    @symbol.setter
+    def symbol(self, value):
+        self._symbol = value
+
+    @property
+    def page(self):
+        return self._page
+
+    @page.setter
+    def page(self, value):
+        self._page = value
+
+    @property
+    def page_size(self):
+        return self._page_size
+
+    @page_size.setter
+    def page_size(self, value):
+        self._page_size = value
+
+    @property
+    def sort_field_name(self):
+        return self._sort_field_name
+
+    @sort_field_name.setter
+    def sort_field_name(self, value):
+        self._sort_field_name = value
+
+    @property
+    def sort_dir(self):
+        return self._sort_dir
+
+    @sort_dir.setter
+    def sort_dir(self, value):
+        self._sort_dir = value
+
+    @property
+    def warrant_type(self):
+        return self._warrant_type
+
+    @warrant_type.setter
+    def warrant_type(self, value):
+        self._warrant_type = value
+
+    @property
+    def issuer_name(self):
+        return self._issuer_name
+
+    @issuer_name.setter
+    def issuer_name(self, value):
+        self._issuer_name = value
+
+    @property
+    def expire_ym(self):
+        return self._expire_ym
+
+    @expire_ym.setter
+    def expire_ym(self, value):
+        self._expire_ym = value
+
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, value):
+        self._state = value
+
+    @property
+    def in_out_price(self):
+        return self._in_out_price
+
+    @in_out_price.setter
+    def in_out_price(self, value):
+        self._in_out_price = value
+
+    @property
+    def lot_size(self):
+        return self._lot_size
+
+    @lot_size.setter
+    def lot_size(self, value):
+        self._lot_size = value
+
+    @property
+    def entitlement_ratio(self):
+        return self._entitlement_ratio
+
+    @entitlement_ratio.setter
+    def entitlement_ratio(self, value):
+        self._entitlement_ratio = value
+
+    @property
+    def strike(self):
+        return self._strike
+
+    @strike.setter
+    def strike(self, value):
+        self._strike = value
+
+    @property
+    def effective_leverage(self):
+        return self._effective_leverage
+
+    @effective_leverage.setter
+    def effective_leverage(self, value):
+        self._effective_leverage = value
+
+    @property
+    def leverage_ratio(self):
+        return self._leverage_ratio
+
+    @leverage_ratio.setter
+    def leverage_ratio(self, value):
+        self._leverage_ratio = value
+
+    @property
+    def call_price(self):
+        return self._call_price
+
+    @call_price.setter
+    def call_price(self, value):
+        self._call_price = value
+
+    @property
+    def volume(self):
+        return self._volume
+
+    @volume.setter
+    def volume(self, value):
+        self._volume = value
+
+    @property
+    def premium(self):
+        return self._premium
+
+    @premium.setter
+    def premium(self, value):
+        self._premium = value
+
+    @property
+    def outstanding_ratio(self):
+        return self._outstanding_ratio
+
+    @outstanding_ratio.setter
+    def outstanding_ratio(self, value):
+        self._outstanding_ratio = value
+
+    @property
+    def implied_volatility(self):
+        return self._implied_volatility
+
+    @implied_volatility.setter
+    def implied_volatility(self, value):
+        self._implied_volatility = value
+
+    def convert_range_param(self, value: tuple):
+        if (isinstance(value, tuple) or isinstance(value, list)) and len(value) == 2:
+            return {'min': value[0], 'max': value[1]}
+        return value
+
+    def to_openapi_dict(self):
+        params = super().to_openapi_dict()
+        if self.symbol:
+            params['symbol'] = self.symbol
+        if self.page:
+            params['page'] = self.page
+        if self.page_size:
+            params['page_size'] = self.page_size
+        if self.sort_field_name:
+            params['sort_field_name'] = underline_to_camel(self.sort_field_name)
+        if self.sort_dir:
+            params['sort_dir'] = self.sort_dir
+        if self.issuer_name:
+            params['issuer_name'] = self.issuer_name
+        if self.expire_ym:
+            params['expire_ym'] = self.expire_ym
+        if self.in_out_price:
+            params['in_out_price'] = list(self.in_out_price)
+        if self.lot_size:
+            params['lot_size'] = list(self.lot_size)
+        if self.entitlement_ratio:
+            params['entitlement_ratio'] = list(self.entitlement_ratio)
+        if self.warrant_type:
+            params['warrant_type'] = list(self.warrant_type)
+        if self.state:
+            params['state'] = self.state
+        # tuple params
+        if self.strike:
+            params['strike'] = self.convert_range_param(self.strike)
+        if self.effective_leverage:
+            params['effective_leverage'] = self.convert_range_param(self.effective_leverage)
+        if self.leverage_ratio:
+            params['leverage_ratio'] = self.convert_range_param(self.leverage_ratio)
+        if self.call_price:
+            params['call_price'] = self.convert_range_param(self.call_price)
+        if self.volume:
+            params['volume'] = self.convert_range_param(self.volume)
+        if self.premium:
+            params['premium'] = self.convert_range_param(self.premium)
+        if self.outstanding_ratio:
+            params['outstanding_ratio'] = self.convert_range_param(self.outstanding_ratio)
+        if self.implied_volatility:
+            params['implied_volatility'] = self.convert_range_param(self.implied_volatility)
+        return params
```

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_contract_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/market_status_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/option_chains_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/stock_details_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/symbols_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-2.3.6/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/tiger_open_client.py` & `tigeropen-2.3.6/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/tiger_open_config.py` & `tigeropen-2.3.6/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/domain/account.py` & `tigeropen-2.3.6/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/domain/contract.py` & `tigeropen-2.3.6/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/domain/order.py` & `tigeropen-2.3.6/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/domain/position.py` & `tigeropen-2.3.6/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/domain/prime_account.py` & `tigeropen-2.3.6/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/request/model.py` & `tigeropen-2.3.6/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/__init__.py` & `tigeropen-2.3.6/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/account_profile_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/assets_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/contracts_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/forex_order_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/order_id_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/order_preview_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/orders_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/positions_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/response/transactions_response.py` & `tigeropen-2.3.6/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.5/tigeropen/trade/trade_client.py` & `tigeropen-2.3.6/tigeropen/trade/trade_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,41 +731,44 @@
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.result
             else:
                 raise ApiException(response.code, response.message)
         return None
 
-    def get_segment_fund_available(self):
+    def get_segment_fund_available(self, from_segment=None, currency=None):
         """
         get segment fund available
         :return:
         """
         params = SegmentFundParams()
         params.account = self._account
+        params.from_segment = get_enum_value(from_segment)
+        params.currency = get_enum_value(currency)
         params.secret_key = self._secret_key
         params.lang = get_enum_value(self._lang)
         request = OpenApiRequest(SEGMENT_FUND_AVAILABLE, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = SegmentFundAvailableResponse()
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.data
             else:
                 raise ApiException(response.code, response.message)
         return None
 
-    def get_segment_fund_history(self):
+    def get_segment_fund_history(self, limit=None):
         """
         get segment fund history
         :return:
         """
         params = SegmentFundParams()
         params.account = self._account
+        params.limit = limit
         params.secret_key = self._secret_key
         params.lang = get_enum_value(self._lang)
         request = OpenApiRequest(SEGMENT_FUND_HISTORY, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = SegmentFundHistoryResponse()
             response.parse_response_content(response_content)
```

### Comparing `tigeropen-2.3.5/tigeropen.egg-info/PKG-INFO` & `tigeropen-2.3.6/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.5
+Version: 2.3.6
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.5/tigeropen.egg-info/SOURCES.txt` & `tigeropen-2.3.6/tigeropen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
 tigeropen/quote/response/stock_broker_response.py
 tigeropen/quote/response/stock_details_response.py
 tigeropen/quote/response/stock_short_interest_response.py
 tigeropen/quote/response/stock_trade_meta_response.py
 tigeropen/quote/response/symbol_names_response.py
 tigeropen/quote/response/symbols_response.py
 tigeropen/quote/response/trading_calendar_response.py
+tigeropen/quote/response/warrant_briefs_response.py
+tigeropen/quote/response/warrant_filter_response.py
 tigeropen/trade/__init__.py
 tigeropen/trade/trade_client.py
 tigeropen/trade/domain/__init__.py
 tigeropen/trade/domain/account.py
 tigeropen/trade/domain/contract.py
 tigeropen/trade/domain/order.py
 tigeropen/trade/domain/position.py
```

