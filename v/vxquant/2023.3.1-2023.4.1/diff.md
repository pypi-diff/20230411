# Comparing `tmp/vxquant-2023.3.1.tar.gz` & `tmp/vxquant-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxquant-2023.3.1.tar", max compression
+gzip compressed data, was "vxquant-2023.4.1.tar", max compression
```

## Comparing `vxquant-2023.3.1.tar` & `vxquant-2023.4.1.tar`

### file list

```diff
@@ -1,106 +1,118 @@
--rw-r--r--   0        0        0     1064 2023-02-20 05:11:28.653883 vxquant-2023.3.1/LICENSE
--rw-r--r--   0        0        0     1428 2023-02-20 05:11:28.653992 vxquant-2023.3.1/README.md
--rw-r--r--   0        0        0     1982 2023-03-01 11:54:26.801205 vxquant-2023.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.655025 vxquant-2023.3.1/src/vxdataset/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.655094 vxquant-2023.3.1/src/vxdataset/cache.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.655206 vxquant-2023.3.1/src/vxdataset/collector/__init__.py
--rw-r--r--   0        0        0     1032 2023-02-20 05:11:28.655405 vxquant-2023.3.1/src/vxdataset/collector/__main__.py
--rw-r--r--   0        0        0     1318 2023-02-20 05:11:28.655525 vxquant-2023.3.1/src/vxdataset/collector/calendar1111.py
--rw-r--r--   0        0        0     5471 2023-02-20 05:11:28.655680 vxquant-2023.3.1/src/vxdataset/collector/dumpall.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.655817 vxquant-2023.3.1/src/vxdataset/datasource/__init__.py
--rw-r--r--   0        0        0     9159 2023-02-20 05:11:28.656015 vxquant-2023.3.1/src/vxdataset/datasource/ifind.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.656207 vxquant-2023.3.1/src/vxdataset/expr/__init__.py
--rw-r--r--   0        0        0      825 2023-02-20 05:11:28.656366 vxquant-2023.3.1/src/vxdataset/expr/functions.py
--rw-r--r--   0        0        0    12470 2023-02-20 05:11:28.656518 vxquant-2023.3.1/src/vxdataset/expr/ops.py
--rw-r--r--   0        0        0     2620 2023-02-20 05:11:28.656654 vxquant-2023.3.1/src/vxdataset/handler.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.656776 vxquant-2023.3.1/src/vxdataset/loaders/__init__.py
--rw-r--r--   0        0        0     3312 2023-02-20 05:11:28.656948 vxquant-2023.3.1/src/vxdataset/loaders/base.py
--rw-r--r--   0        0        0     1574 2023-02-20 05:11:28.657066 vxquant-2023.3.1/src/vxdataset/loaders/csv.py
--rw-r--r--   0        0        0     2204 2023-02-20 05:11:28.657184 vxquant-2023.3.1/src/vxdataset/loaders/gm.py
--rw-r--r--   0        0        0        0 2023-02-20 05:11:28.657224 vxquant-2023.3.1/src/vxdataset/loaders/mongo.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:08:42.000000 vxquant-2023.3.1/src/vxquant/__init__.py
--rwxr-xr-x   0        0        0     2927 2023-02-21 01:03:23.210842 vxquant-2023.3.1/src/vxquant/__main__.py
--rwxr-xr-x   0        0        0     2862 2023-03-05 02:18:03.220734 vxquant-2023.3.1/src/vxquant/apis.py
--rw-r--r--   0        0        0     1439 2023-02-20 06:16:20.250478 vxquant-2023.3.1/src/vxquant/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-01 04:48:51.217194 vxquant-2023.3.1/src/vxquant/factor/__init__.py
--rw-r--r--   0        0        0     6334 2023-03-02 13:46:11.815748 vxquant-2023.3.1/src/vxquant/factor/builder.py
--rw-r--r--   0        0        0        0 2023-03-01 04:48:55.276562 vxquant-2023.3.1/src/vxquant/factor/expr/__init__.py
--rw-r--r--   0        0        0      825 2023-03-01 04:48:55.277467 vxquant-2023.3.1/src/vxquant/factor/expr/functions.py
--rw-r--r--   0        0        0    13165 2023-03-02 14:08:46.272159 vxquant-2023.3.1/src/vxquant/factor/expr/ops.py
--rw-r--r--   0        0        0     4754 2023-03-03 03:33:26.747319 vxquant-2023.3.1/src/vxquant/factor/normalizer.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:08:50.000000 vxquant-2023.3.1/src/vxquant/model/__init__.py
--rw-r--r--   0        0        0     3399 2023-03-05 09:16:07.674763 vxquant-2023.3.1/src/vxquant/model/account.py
--rwxr-xr-x   0        0        0     6778 2023-02-16 13:08:52.000000 vxquant-2023.3.1/src/vxquant/model/contants.py
--rwxr-xr-x   0        0        0    15894 2023-02-16 13:08:51.000000 vxquant-2023.3.1/src/vxquant/model/dbaccount.py
--rwxr-xr-x   0        0        0    14066 2023-03-05 02:11:04.936177 vxquant-2023.3.1/src/vxquant/model/exchange.py
--rwxr-xr-x   0        0        0    11089 2023-03-02 09:15:24.762866 vxquant-2023.3.1/src/vxquant/model/instruments.py
--rwxr-xr-x   0        0        0     2708 2023-02-16 13:08:52.000000 vxquant-2023.3.1/src/vxquant/model/nomalize.py
--rwxr-xr-x   0        0        0    54845 2023-02-16 13:08:52.000000 vxquant-2023.3.1/src/vxquant/model/portfolio.py
--rwxr-xr-x   0        0        0     9880 2023-02-16 13:08:52.000000 vxquant-2023.3.1/src/vxquant/model/preset.py
--rwxr-xr-x   0        0        0       47 2023-02-16 13:08:54.000000 vxquant-2023.3.1/src/vxquant/model/tools/__init__.py
--rwxr-xr-x   0        0        0     7261 2023-02-25 13:32:22.498666 vxquant-2023.3.1/src/vxquant/model/tools/gmData.py
--rwxr-xr-x   0        0        0     8969 2023-02-16 13:08:54.000000 vxquant-2023.3.1/src/vxquant/model/tools/qmtData.py
--rwxr-xr-x   0        0        0     5234 2023-02-25 14:22:59.832882 vxquant-2023.3.1/src/vxquant/model/tools/tdxData.py
--rwxr-xr-x   0        0        0      150 2023-02-16 13:08:49.000000 vxquant-2023.3.1/src/vxquant/model/typehint.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:08:45.000000 vxquant-2023.3.1/src/vxquant/modules/agent/__init__.py
--rwxr-xr-x   0        0        0     4019 2023-02-20 00:51:55.000000 vxquant-2023.3.1/src/vxquant/modules/agent/__main__.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:08:57.000000 vxquant-2023.3.1/src/vxquant/modules/agent/mod/__init__.py
--rwxr-xr-x   0        0        0     4706 2023-02-16 13:08:57.000000 vxquant-2023.3.1/src/vxquant/modules/agent.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:09:17.000000 vxquant-2023.3.1/src/vxquant/modules/broker/__init__.py
--rwxr-xr-x   0        0        0     8297 2023-02-16 13:09:18.000000 vxquant-2023.3.1/src/vxquant/modules/broker/__main__.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:09:21.000000 vxquant-2023.3.1/src/vxquant/modules/broker/mod/__init__.py
--rwxr-xr-x   0        0        0     1267 2023-02-16 13:09:22.000000 vxquant-2023.3.1/src/vxquant/modules/broker/mod/system.py
--rwxr-xr-x   0        0        0      834 2023-02-16 13:09:19.000000 vxquant-2023.3.1/src/vxquant/modules/broker/utils.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:08:43.000000 vxquant-2023.3.1/src/vxquant/modules/gateway/__init__.py
--rwxr-xr-x   0        0        0      236 2023-02-16 13:08:43.000000 vxquant-2023.3.1/src/vxquant/modules/gateway/rpc.py
--rwxr-xr-x   0        0        0      426 2023-02-16 13:08:43.000000 vxquant-2023.3.1/src/vxquant/modules/gateway/system.py
--rwxr-xr-x   0        0        0        0 2023-02-18 14:17:07.000000 vxquant-2023.3.1/src/vxquant/providers/__init__.py
--rwxr-xr-x   0        0        0    11387 2023-03-01 00:08:34.220627 vxquant-2023.3.1/src/vxquant/providers/base.py
--rwxr-xr-x   0        0        0     6812 2023-02-20 06:33:41.648256 vxquant-2023.3.1/src/vxquant/providers/ftp.py
--rwxr-xr-x   0        0        0     5618 2023-02-24 10:37:59.057020 vxquant-2023.3.1/src/vxquant/providers/gmapi.py
--rw-r--r--   0        0        0     2751 2023-03-02 04:04:18.187553 vxquant-2023.3.1/src/vxquant/providers/local.py
--rwxr-xr-x   0        0        0    15079 2023-02-25 14:32:53.669316 vxquant-2023.3.1/src/vxquant/providers/miniqmt.py
--rw-r--r--   0        0        0     8172 2023-03-03 14:17:09.721637 vxquant-2023.3.1/src/vxquant/providers/mongo.py
--rwxr-xr-x   0        0        0     1716 2023-02-20 12:36:35.042880 vxquant-2023.3.1/src/vxquant/providers/spiders/calendar_sse.py
--rwxr-xr-x   0        0        0     4764 2023-02-16 13:09:34.000000 vxquant-2023.3.1/src/vxquant/providers/spiders/hq_tencent.py
--rwxr-xr-x   0        0        0    18509 2023-02-28 07:25:02.169890 vxquant-2023.3.1/src/vxquant/providers/tdx.py
--rwxr-xr-x   0        0        0     6960 2023-02-20 06:24:13.986291 vxquant-2023.3.1/src/vxquant/providers/zeromq.py
--rw-r--r--   0        0        0     2350 2023-02-20 05:11:28.663766 vxquant-2023.3.1/src/vxquant/scripts/__init__.py
--rw-r--r--   0        0        0     8464 2023-02-20 05:11:28.663902 vxquant-2023.3.1/src/vxquant/scripts/broker.py
--rwxr-xr-x   0        0        0     9524 2023-02-16 13:08:45.000000 vxquant-2023.3.1/src/vxquant/scripts/gmagent.py
--rwxr-xr-x   0        0        0     9658 2023-02-16 13:08:46.000000 vxquant-2023.3.1/src/vxquant/scripts/qmtagent.py
--rw-r--r--   0        0        0     4051 2023-02-20 05:11:28.664017 vxquant-2023.3.1/src/vxquant/scripts/worker.py
--rwxr-xr-x   0        0        0        0 2023-02-16 13:09:29.000000 vxquant-2023.3.1/src/vxquant/tdapi/__init__.py
--rwxr-xr-x   0        0        0     4121 2023-02-16 13:09:26.000000 vxquant-2023.3.1/src/vxquant/tdapi/base.py
--rwxr-xr-x   0        0        0     4822 2023-02-16 13:09:27.000000 vxquant-2023.3.1/src/vxquant/tdapi/gm.py
--rwxr-xr-x   0        0        0     1523 2023-02-16 13:09:29.000000 vxquant-2023.3.1/src/vxquant/tdapi/gmtrade.py
--rwxr-xr-x   0        0        0     5576 2023-02-16 13:09:25.000000 vxquant-2023.3.1/src/vxquant/tdapi/miniqmt.py
--rwxr-xr-x   0        0        0     8935 2023-02-16 13:09:28.000000 vxquant-2023.3.1/src/vxquant/tdapi/sim.py
--rw-r--r--   0        0        0      501 2023-02-20 05:47:18.142720 vxquant-2023.3.1/src/vxsched/__init__.py
--rw-r--r--   0        0        0      719 2023-02-20 05:27:59.367680 vxquant-2023.3.1/src/vxsched/__main__.py
--rw-r--r--   0        0        0     4459 2023-02-21 00:59:59.761933 vxquant-2023.3.1/src/vxsched/context.py
--rw-r--r--   0        0        0    11325 2023-02-23 08:01:19.044489 vxquant-2023.3.1/src/vxsched/core.py
--rw-r--r--   0        0        0     6652 2023-02-23 07:53:22.943128 vxquant-2023.3.1/src/vxsched/event.py
--rw-r--r--   0        0        0      267 2023-02-20 05:11:28.664150 vxquant-2023.3.1/src/vxsched/triggers/__init__.py
--rw-r--r--   0        0        0      968 2023-02-20 05:11:28.664255 vxquant-2023.3.1/src/vxsched/triggers/daily.py
--rw-r--r--   0        0        0      890 2023-02-20 05:11:28.664350 vxquant-2023.3.1/src/vxsched/triggers/interval.py
--rw-r--r--   0        0        0      336 2023-02-20 05:11:28.664450 vxquant-2023.3.1/src/vxsched/triggers/once.py
--rw-r--r--   0        0        0     2107 2023-02-20 05:11:28.664557 vxquant-2023.3.1/src/vxsched/triggers/weekly.py
--rw-r--r--   0        0        0     2733 2023-02-20 09:57:24.672212 vxquant-2023.3.1/src/vxutils/__init__.py
--rw-r--r--   0        0        0     9407 2023-03-03 11:38:47.900900 vxquant-2023.3.1/src/vxutils/cache.py
--rw-r--r--   0        0        0    11372 2023-02-20 05:11:28.665006 vxquant-2023.3.1/src/vxutils/convertors.py
--rw-r--r--   0        0        0     3852 2023-02-20 05:11:28.665169 vxquant-2023.3.1/src/vxutils/database/__init__.py
--rw-r--r--   0        0        0     9864 2023-03-03 11:38:58.973126 vxquant-2023.3.1/src/vxutils/database/mongodb.py
--rw-r--r--   0        0        0     8101 2023-02-20 05:11:28.665427 vxquant-2023.3.1/src/vxutils/database/sqlite.py
--rw-r--r--   0        0        0    18158 2023-02-25 13:37:25.348442 vxquant-2023.3.1/src/vxutils/dataclass.py
--rw-r--r--   0        0        0     4783 2023-03-03 13:55:42.240826 vxquant-2023.3.1/src/vxutils/dbproxy.py
--rw-r--r--   0        0        0     1438 2023-02-20 05:11:28.665737 vxquant-2023.3.1/src/vxutils/debug.py
--rw-r--r--   0        0        0     6888 2023-03-03 11:39:24.215373 vxquant-2023.3.1/src/vxutils/decorators.py
--rw-r--r--   0        0        0     1725 2023-02-20 05:11:28.665962 vxquant-2023.3.1/src/vxutils/exceptions.py
--rw-r--r--   0        0        0     3314 2023-02-20 05:26:21.936962 vxquant-2023.3.1/src/vxutils/log.py
--rw-r--r--   0        0        0     9335 2023-02-20 05:11:28.666206 vxquant-2023.3.1/src/vxutils/net.py
--rw-r--r--   0        0        0     2704 2023-02-20 05:11:28.666321 vxquant-2023.3.1/src/vxutils/time.py
--rw-r--r--   0        0        0     7212 2023-03-01 11:49:05.191121 vxquant-2023.3.1/src/vxutils/wrappers.py
--rw-r--r--   0        0        0    12124 2023-02-20 05:28:01.319653 vxquant-2023.3.1/src/vxutils/zmqsocket.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 vxquant-2023.3.1/setup.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 vxquant-2023.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-03-06 04:47:42.000000 vxquant-2023.4.1/LICENSE
+-rwxr-xr-x   0        0        0     1511 2023-03-06 04:47:42.000000 vxquant-2023.4.1/README.md
+-rwxr-xr-x   0        0        0     2125 2023-04-02 14:06:17.873419 vxquant-2023.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/cache.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/collector/__init__.py
+-rwxr-xr-x   0        0        0     1070 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/collector/__main__.py
+-rwxr-xr-x   0        0        0     1362 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/collector/calendar1111.py
+-rwxr-xr-x   0        0        0     5804 2023-03-27 07:01:09.525154 vxquant-2023.4.1/src/vxdataset/collector/dumpall.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/datasource/__init__.py
+-rwxr-xr-x   0        0        0     9464 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/datasource/ifind.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/expr/__init__.py
+-rwxr-xr-x   0        0        0      855 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/expr/functions.py
+-rwxr-xr-x   0        0        0    13098 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/expr/ops.py
+-rwxr-xr-x   0        0        0     2707 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/handler.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/loaders/__init__.py
+-rwxr-xr-x   0        0        0     3425 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/loaders/base.py
+-rwxr-xr-x   0        0        0     1621 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/loaders/csv.py
+-rwxr-xr-x   0        0        0     2283 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/loaders/gm.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxdataset/loaders/mongo.py
+-rwxr-xr-x   0        0        0        2 2023-03-11 03:14:18.000000 vxquant-2023.4.1/src/vxquant/__init__.py
+-rwxr-xr-x   0        0        0     3816 2023-04-05 07:07:18.411840 vxquant-2023.4.1/src/vxquant/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-23 13:14:56.105985 vxquant-2023.4.1/src/vxquant/accountdb/__init__.py
+-rw-r--r--   0        0        0    13968 2023-04-11 15:59:47.792209 vxquant-2023.4.1/src/vxquant/accountdb/base.py
+-rw-r--r--   0        0        0        0 2023-03-23 13:15:20.240915 vxquant-2023.4.1/src/vxquant/accountdb/mongodb.py
+-rw-r--r--   0        0        0    17753 2023-04-11 15:59:58.360985 vxquant-2023.4.1/src/vxquant/accountdb/sqlitedb.py
+-rwxr-xr-x   0        0        0    28159 2023-04-11 13:44:50.562533 vxquant-2023.4.1/src/vxquant/apis.py
+-rwxr-xr-x   0        0        0      839 2023-04-06 07:46:25.980939 vxquant-2023.4.1/src/vxquant/cli/__init__.py
+-rwxr-xr-x   0        0        0     2680 2023-04-10 11:55:54.522545 vxquant-2023.4.1/src/vxquant/cli/base.py
+-rwxr-xr-x   0        0        0    15084 2023-04-10 16:30:54.912797 vxquant-2023.4.1/src/vxquant/cli/gmagent.py
+-rwxr-xr-x   0        0        0     7413 2023-04-10 14:28:30.379107 vxquant-2023.4.1/src/vxquant/cli/qmtagent.py
+-rw-r--r--   0        0        0     7123 2023-04-11 13:56:37.619629 vxquant-2023.4.1/src/vxquant/config.py
+-rwxr-xr-x   0        0        0     1536 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/exceptions.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/factor/__init__.py
+-rwxr-xr-x   0        0        0     7158 2023-04-01 15:46:53.007537 vxquant-2023.4.1/src/vxquant/factor/builder.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/factor/expr/__init__.py
+-rwxr-xr-x   0        0        0      855 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/factor/expr/functions.py
+-rwxr-xr-x   0        0        0    13833 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/factor/expr/ops.py
+-rw-r--r--   0        0        0     7029 2023-04-06 04:54:05.820330 vxquant-2023.4.1/src/vxquant/factor/loader.py
+-rwxr-xr-x   0        0        0     4898 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/factor/normalizer.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/model/__init__.py
+-rwxr-xr-x   0        0        0    17857 2023-03-07 09:00:59.000000 vxquant-2023.4.1/src/vxquant/model/account.py
+-rwxr-xr-x   0        0        0     7035 2023-03-06 14:54:42.000000 vxquant-2023.4.1/src/vxquant/model/contants.py
+-rwxr-xr-x   0        0        0    16434 2023-03-15 08:12:42.628178 vxquant-2023.4.1/src/vxquant/model/dbaccount.py
+-rwxr-xr-x   0        0        0    14231 2023-04-07 07:20:20.284686 vxquant-2023.4.1/src/vxquant/model/exchange.py
+-rwxr-xr-x   0        0        0    11471 2023-03-28 15:27:12.904581 vxquant-2023.4.1/src/vxquant/model/instruments.py
+-rwxr-xr-x   0        0        0     2806 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/model/nomalize.py
+-rwxr-xr-x   0        0        0    56399 2023-03-15 08:12:42.859226 vxquant-2023.4.1/src/vxquant/model/portfolio.py
+-rwxr-xr-x   0        0        0    10767 2023-04-06 01:46:53.205883 vxquant-2023.4.1/src/vxquant/model/preset.py
+-rwxr-xr-x   0        0        0       49 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/model/tools/__init__.py
+-rwxr-xr-x   0        0        0     7506 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/model/tools/gmData.py
+-rwxr-xr-x   0        0        0     9441 2023-03-31 07:55:40.405707 vxquant-2023.4.1/src/vxquant/model/tools/qmtData.py
+-rwxr-xr-x   0        0        0     5410 2023-03-15 08:12:42.564695 vxquant-2023.4.1/src/vxquant/model/tools/tdxData.py
+-rwxr-xr-x   0        0        0      155 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/model/typehint.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/agent/__init__.py
+-rwxr-xr-x   0        0        0     4151 2023-03-07 12:31:01.000000 vxquant-2023.4.1/src/vxquant/modules/agent/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/agent/mod/__init__.py
+-rwxr-xr-x   0        0        0     4837 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/agent.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/broker/__init__.py
+-rwxr-xr-x   0        0        0     8563 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/broker/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/broker/mod/__init__.py
+-rwxr-xr-x   0        0        0     1300 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/broker/mod/system.py
+-rwxr-xr-x   0        0        0      861 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/broker/utils.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/gateway/__init__.py
+-rwxr-xr-x   0        0        0      246 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/gateway/rpc.py
+-rwxr-xr-x   0        0        0      440 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/modules/gateway/system.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/providers/__init__.py
+-rw-r--r--   0        0        0     4567 2023-03-28 14:06:06.714095 vxquant-2023.4.1/src/vxquant/providers/baostock_api.py
+-rwxr-xr-x   0        0        0    17004 2023-04-06 08:34:46.941091 vxquant-2023.4.1/src/vxquant/providers/base.py
+-rwxr-xr-x   0        0        0     7023 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/providers/ftp.py
+-rwxr-xr-x   0        0        0    13535 2023-04-10 15:06:33.571744 vxquant-2023.4.1/src/vxquant/providers/gmapi.py
+-rwxr-xr-x   0        0        0     3010 2023-04-02 14:14:32.259786 vxquant-2023.4.1/src/vxquant/providers/local.py
+-rwxr-xr-x   0        0        0    14199 2023-04-10 07:31:13.413999 vxquant-2023.4.1/src/vxquant/providers/miniqmt.py
+-rwxr-xr-x   0        0        0     8406 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/providers/mongo.py
+-rw-r--r--   0        0        0      131 2023-03-22 13:38:55.253234 vxquant-2023.4.1/src/vxquant/providers/spiders/__init__.py
+-rwxr-xr-x   0        0        0     2008 2023-04-05 02:27:07.913696 vxquant-2023.4.1/src/vxquant/providers/spiders/calendar_sse.py
+-rwxr-xr-x   0        0        0     4921 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/providers/spiders/hq_tencent.py
+-rwxr-xr-x   0        0        0    18580 2023-04-04 05:59:26.900256 vxquant-2023.4.1/src/vxquant/providers/tdx.py
+-rwxr-xr-x   0        0        0     7183 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/providers/zeromq.py
+-rwxr-xr-x   0        0        0     2438 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/scripts/__init__.py
+-rwxr-xr-x   0        0        0     8719 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/scripts/broker.py
+-rwxr-xr-x   0        0        0     9813 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/scripts/gmagent.py
+-rwxr-xr-x   0        0        0     9953 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/scripts/qmtagent.py
+-rwxr-xr-x   0        0        0     4180 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/scripts/worker.py
+-rwxr-xr-x   0        0        0        0 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/tdapi/__init__.py
+-rwxr-xr-x   0        0        0     4274 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/tdapi/base.py
+-rwxr-xr-x   0        0        0     4971 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/tdapi/gm.py
+-rwxr-xr-x   0        0        0     1579 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/tdapi/gmtrade.py
+-rwxr-xr-x   0        0        0     5736 2023-04-10 03:40:44.638089 vxquant-2023.4.1/src/vxquant/tdapi/miniqmt.py
+-rwxr-xr-x   0        0        0     9231 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxquant/tdapi/sim.py
+-rwxr-xr-x   0        0        0      523 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/__init__.py
+-rwxr-xr-x   0        0        0      746 2023-03-11 01:03:48.000000 vxquant-2023.4.1/src/vxsched/__main__.py
+-rwxr-xr-x   0        0        0     4641 2023-04-09 14:08:26.735530 vxquant-2023.4.1/src/vxsched/context.py
+-rwxr-xr-x   0        0        0    11339 2023-04-10 12:08:34.700548 vxquant-2023.4.1/src/vxsched/core.py
+-rwxr-xr-x   0        0        0     6888 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/event.py
+-rwxr-xr-x   0        0        0      282 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/triggers/__init__.py
+-rwxr-xr-x   0        0        0     1004 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/triggers/daily.py
+-rwxr-xr-x   0        0        0      922 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/triggers/interval.py
+-rwxr-xr-x   0        0        0      352 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/triggers/once.py
+-rwxr-xr-x   0        0        0     2181 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxsched/triggers/weekly.py
+-rwxr-xr-x   0        0        0     3017 2023-04-04 04:12:11.262998 vxquant-2023.4.1/src/vxutils/__init__.py
+-rwxr-xr-x   0        0        0    17380 2023-04-07 07:09:07.289149 vxquant-2023.4.1/src/vxutils/cache.py
+-rwxr-xr-x   0        0        0    11833 2023-04-09 14:38:13.867949 vxquant-2023.4.1/src/vxutils/convertors.py
+-rwxr-xr-x   0        0        0     6015 2023-03-26 12:05:33.678819 vxquant-2023.4.1/src/vxutils/database/__init__.py
+-rw-r--r--   0        0        0     5140 2023-04-07 12:46:03.338312 vxquant-2023.4.1/src/vxutils/database/base.py
+-rwxr-xr-x   0        0        0    10294 2023-03-15 08:12:42.718770 vxquant-2023.4.1/src/vxutils/database/mongodb.py
+-rwxr-xr-x   0        0        0    15430 2023-04-10 13:34:49.001153 vxquant-2023.4.1/src/vxutils/database/sqlite.py
+-rwxr-xr-x   0        0        0    19092 2023-04-07 07:18:29.547245 vxquant-2023.4.1/src/vxutils/dataclass.py
+-rwxr-xr-x   0        0        0     4963 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxutils/dbproxy.py
+-rwxr-xr-x   0        0        0     1498 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxutils/debug.py
+-rwxr-xr-x   0        0        0     7179 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxutils/decorators.py
+-rwxr-xr-x   0        0        0     1797 2023-03-11 01:37:22.000000 vxquant-2023.4.1/src/vxutils/exceptions.py
+-rwxr-xr-x   0        0        0     3416 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxutils/log.py
+-rwxr-xr-x   0        0        0    12501 2023-03-23 11:18:42.541440 vxquant-2023.4.1/src/vxutils/net.py
+-rwxr-xr-x   0        0        0     4320 2023-04-05 06:39:34.771258 vxquant-2023.4.1/src/vxutils/time.py
+-rwxr-xr-x   0        0        0     7418 2023-04-10 08:02:25.257162 vxquant-2023.4.1/src/vxutils/wrappers.py
+-rwxr-xr-x   0        0        0    12507 2023-03-06 04:47:42.000000 vxquant-2023.4.1/src/vxutils/zmqsocket.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 vxquant-2023.4.1/PKG-INFO
```

### Comparing `vxquant-2023.3.1/LICENSE` & `vxquant-2023.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 vex1023
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 vex1023
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `vxquant-2023.3.1/pyproject.toml` & `vxquant-2023.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-[tool.poetry]
-name = "vxquant"
-version = "2023.03.01"
-description = "一个简单、易用、面向中国股市实盘的python量化交易框架"
-license = "MIT"
-authors = ["vex1023 <vex1023@qq.com>"]
-homepage = "https://gitee.com/vxquant/vxquant"
-keywords = ["quant", "tools"]
-readme = "README.md"
-
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-]
-packages = [
-    { include = "vxquant",from = "src/" },
-    { include = "vxutils",from = "src/" },
-    { include = "vxsched",from = "src/" },
-    { include = "vxdataset",from = "src/" },
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pyzmq = "*"
-pymongo = "*"
-python-dateutil = "*"
-requests = "*"
-six = "*"
-numpy = "*"
-pandas = "*"
-tqdm = "*"
-scipy = "*"
-polars = {version = "*", extras = ["pyarrow"]}
-
-
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "*"
-pylint = "*"
-twine = "*"
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0",'setuptools','Cython','numpy']
-build-backend = "poetry.core.masonry.api"
-
-
-
-[tool.isort]
-py_version = 38
-profile = "black"
-force_single_line = true
-combine_as_imports = true
-lines_between_types = 1
-lines_after_imports = 2
-src_paths = ["src", "tests"]
-extend_skip = ["setup.py"]
-known_third_party = ["poetry.core"]
-
-
-[tool.black]
-target-version = ['py38']
-preview = true
-force-exclude = '''
-.*/setup\.py$
-'''
-
-
-[tool.mypy]
-files = "src"
-mypy_path = "src"
-namespace_packages = true
-explicit_package_bases = true
-show_error_codes = true
-strict = true
-enable_error_code = [
-    "ignore-without-code",
-    "redundant-expr",
-    "truthy-bool",
-]
+[tool.poetry]
+name = "vxquant"
+version = "2023.04.01"
+description = "一个简单、易用、面向中国股市实盘的python量化交易框架"
+license = "MIT"
+authors = ["vex1023 <vex1023@qq.com>"]
+homepage = "https://gitee.com/vxquant/vxquant"
+keywords = ["quant", "tools"]
+readme = "README.md"
+
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
+packages = [
+    { include = "vxquant",from = "src/" },
+    { include = "vxutils",from = "src/" },
+    { include = "vxsched",from = "src/" },
+    { include = "vxdataset",from = "src/" },
+]
+
+[tool.poetry.scripts]
+vxquant = 'vxquant.__main__:main'
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pyzmq = "*"
+pymongo = "*"
+python-dateutil = "*"
+requests = "*"
+six = "*"
+numpy = "*"
+pandas = "*"
+tqdm = "*"
+scipy = "*"
+polars = {version = "*", extras = ["pyarrow"]}
+
+[tool.poetry.dev-dependencies]
+pytest = "^5.2"
+flake8 = "*"
+pylint = "*"
+twine = "*"
+
+[build-system]
+requires = ["poetry-core>=1.0.0",'setuptools','Cython','numpy']
+build-backend = "poetry.core.masonry.api"
+
+
+
+[tool.isort]
+py_version = 38
+profile = "black"
+force_single_line = true
+combine_as_imports = true
+lines_between_types = 1
+lines_after_imports = 2
+src_paths = ["src", "tests"]
+extend_skip = ["setup.py"]
+known_third_party = ["poetry.core"]
+
+
+[tool.black]
+target-version = ['py38']
+preview = true
+force-exclude = '''
+.*/setup\.py$
+'''
+
+
+[tool.mypy]
+files = "src"
+mypy_path = "src"
+namespace_packages = true
+explicit_package_bases = true
+show_error_codes = true
+strict = true
+enable_error_code = [
+    "ignore-without-code",
+    "redundant-expr",
+    "truthy-bool",
+]
```

### Comparing `vxquant-2023.3.1/src/vxdataset/collector/calendar1111.py` & `vxquant-2023.4.1/src/vxdataset/collector/calendar1111.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-""" 日历"""
-
-
-"""日历采集器"""
-
-import polars as pl
-import datetime
-from pathlib import Path
-from vxsched import vxengine
-from vxutils import vxtime, to_datetime, logger, to_timestring
-
-
-@vxengine.event_handler("on_hans", 30)
-@vxengine.event_handler("init", 30)
-def collector_calendar_init(context, _):
-    """初始化
-
-    交易所 SSE上交所,SZSE深交所,CFFEX 中金所,SHFE 上期所,CZCE 郑商所,DCE 大商所,INE 上能源
-
-    """
-    start_date = to_datetime("1990-01-01")
-    end_date = start_date
-
-    data_path = context.params.get("data_path", "~/.vxdataset/")
-    calendar_file = Path(data_path, "calendar.csv")
-    if calendar_file.exists():
-        calendars = pl.read_csv(calendar_file, parse_dates=True).sort(by="date")
-        end_date = calendars["date"][-1] + datetime.timedelta(days=1)
-
-    today = to_datetime(vxtime.today())
-    if end_date > today:
-        logger.info(f"交易日历最后一天{end_date}，并未更新")
-        return
-
-    df = context.ts_pro.trade_cal(
-        "SSE",
-        start_date=to_timestring(end_date, "%Y%m%d"),
-        end_date=to_timestring(today, "%Y%m%d"),
-        is_open=1,
-    )
-    if df.empty():
-        logger.info(f"交易日历最后一天{end_date}，并未更新")
-        return
-    vxengine.submit_event("load_date", df["cal_date"])
+""" 日历"""
+
+
+"""日历采集器"""
+
+import polars as pl
+import datetime
+from pathlib import Path
+from vxsched import vxengine
+from vxutils import vxtime, to_datetime, logger, to_timestring
+
+
+@vxengine.event_handler("on_hans", 30)
+@vxengine.event_handler("init", 30)
+def collector_calendar_init(context, _):
+    """初始化
+
+    交易所 SSE上交所,SZSE深交所,CFFEX 中金所,SHFE 上期所,CZCE 郑商所,DCE 大商所,INE 上能源
+
+    """
+    start_date = to_datetime("1990-01-01")
+    end_date = start_date
+
+    data_path = context.params.get("data_path", "~/.vxdataset/")
+    calendar_file = Path(data_path, "calendar.csv")
+    if calendar_file.exists():
+        calendars = pl.read_csv(calendar_file, parse_dates=True).sort(by="date")
+        end_date = calendars["date"][-1] + datetime.timedelta(days=1)
+
+    today = to_datetime(vxtime.today())
+    if end_date > today:
+        logger.info(f"交易日历最后一天{end_date}，并未更新")
+        return
+
+    df = context.ts_pro.trade_cal(
+        "SSE",
+        start_date=to_timestring(end_date, "%Y%m%d"),
+        end_date=to_timestring(today, "%Y%m%d"),
+        is_open=1,
+    )
+    if df.empty():
+        logger.info(f"交易日历最后一天{end_date}，并未更新")
+        return
+    vxengine.submit_event("load_date", df["cal_date"])
```

### Comparing `vxquant-2023.3.1/src/vxdataset/expr/ops.py` & `vxquant-2023.4.1/src/vxdataset/expr/ops.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,628 +1,628 @@
-"""操作"""
-import numpy as np
-import polars as pl
-from scipy.stats import percentileofscore, linregress, pearsonr
-from .functions import rolling_apply_cols
-
-
-Feature = pl.col
-
-
-def Abs(feature: Feature):
-    """Feature Abs
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with Abs
-    """
-    return Feature.abs()
-
-
-def Sign(feature: Feature):
-    """Feature Sign
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with Sign
-    """
-    return Feature.sign()
-
-
-def Log(feature: Feature):
-    """Feature Log
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with log
-    """
-    return feature.log()
-
-
-def Log10(feature: Feature):
-    """Feature Log10
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with log10
-    """
-    return feature.log10()
-
-
-# * def Mask(feature: Feature):
-# *
-# * class Mask(NpElemOperator):
-# *    """Feature Mask
-# *
-# *    Parameters
-# *    ----------
-# *    feature : Expression
-# *        feature instance
-# *    instrument : str
-# *        instrument mask
-# *
-# *    Returns
-# *    ----------
-# *    Expression
-# *        a feature instance with masked instrument
-# *    """
-# *
-# *    def __init__(self, feature, instrument):
-# *        super(Mask, self).__init__(feature, "mask")
-# *        self.instrument = instrument
-# *
-# *    def __str__(self):
-# *        return f"{type(self).__name__}({self.feature},{self.instrument.lower()})"
-# *
-# *    def _load_internal(self, instrument, start_index, end_index, *args):
-# *        return self.feature.load(self.instrument, start_index, end_index, *args)
-
-
-def Not(feature: Feature):
-    """Not Operator
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-
-    Returns
-    ----------
-    Feature:
-        feature elementwise not output
-    """
-    return feature.is_not()
-
-
-def Power(left: Feature, right: Feature):
-    """Power Operator
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-
-    Returns
-    ----------
-    Feature:
-        The bases in feature_left raised to the exponents in feature_right
-    """
-    return left.pow(right)
-
-
-def If(condition: Feature, left: Feature, right: Feature) -> Feature:
-    return pl.when(condition).then(left).otherwise(right)
-
-
-def Ref(feature: Feature, N: int) -> Feature:
-    """Feature Reference
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        N = 0, retrieve the first data; N > 0, retrieve data of N periods ago; N < 0, future data
-
-    Returns
-    ----------
-    Expression
-        a feature instance with target reference
-    """
-    return feature.shift(N)
-
-
-def Mean(feature: Feature, N: int) -> Feature:
-    """Rolling Mean (MA)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling average
-    """
-    return feature.rolling_mean(N)
-
-
-def Sum(feature: Feature, N: int) -> Feature:
-    """Rolling Sum
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling sum
-    """
-    return feature.rolling_sum(N)
-
-
-def Std(feature: Feature, N: int) -> Feature:
-    """Rolling Std
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling std
-    """
-    return feature.rolling_std(N)
-
-
-def Var(feature: Feature, N: int) -> Feature:
-    """Rolling Variance
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling variance
-    """
-    return feature.rolling_var(N)
-
-
-def Skew(feature: Feature, N: int) -> Feature:
-    """Rolling Skewness
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling skewness
-    """
-    return feature.rolling_skew(N)
-
-
-def Kurt(feature: Feature, N: int) -> Feature:
-    """Rolling Kurtosis
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling kurtosis
-    """
-    return feature.rolling_apply(lambda x: x.kurtosis(), N)
-
-
-def Max(feature: False, N: int) -> Feature:
-    """Rolling Max
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max
-    """
-    return feature.rolling_max(N)
-
-
-def IdxMax(feature: Feature, N: int) -> Feature:
-    """Rolling Max Index
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max index
-    """
-    return feature.rolling_apply(lambda s: s.arr.arg_max(), N)
-
-
-def Min(feature: Feature, N: int) -> Feature:
-    """Rolling Min
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling min
-    """
-    return feature.rolling_min(N)
-
-
-def IdxMin(feature: Feature, N: int) -> Feature:
-    """Rolling Min Index
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling min index
-    """
-    return feature.rolling_apply(lambda s: s.arr.arg_min(), N)
-
-
-def Quantile(feature: Feature, N: int) -> Feature:
-    """Rolling Quantile
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling quantile
-    """
-    return feature.rollout_quantile(N)
-
-
-def Med(feature: Feature, N: int) -> Feature:
-    """Rolling Median
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling median
-    """
-
-    return feature.rolling_median(N)
-
-
-def Mad(feature: Feature, N: int) -> Feature:
-    """Rolling Mean Absolute Deviation
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling mean absolute deviation
-    """
-    return (feature - feature.rolling_mean(N)).abs().rolling_mean(N)
-
-
-def _rank(x):
-    x = x.to_numpy()
-    if np.isnan(x[-1]):
-        return np.nan
-    x1 = x[~np.isnan(x)]
-    return np.nan if x1.shape[0] == 0 else percentileofscore(x1, x1[-1]) / len(x1)
-
-
-def Rank(feature: Feature, N: int) -> Feature:
-    """Rolling Rank (Percentile)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling rank
-    """
-    return feature.rolling_apply(_rank, N)
-
-
-def Count(feature: Feature, N: int) -> Feature:
-    """Rolling Count
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling count of number of non-NaN elements
-    """
-    return feature.rolling_apply(lambda x: x.count(), N)
-
-
-def Delta(feature: Feature, N: int) -> Feature:
-    """Rolling Delta
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with end minus start in rolling window
-    """
-    return feature - feature.shift(N)
-
-
-def Slope(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling Slope `Slope(A, B, N)`
-    This operator calculate the slope between `left` and `right`.
-
-    Usage Example:
-    - "Slope($high, %low, 10)/$close"
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with linear regression slope of given window
-    """
-
-    def _slope(x, y):
-        slope_ret, _ = linregress(x, y)
-        return slope_ret
-
-    return rolling_apply_cols([left, right], _slope, N)
-
-
-def Rsquare(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling R-value Square
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with linear regression r-value square of given window
-    """
-
-    def _r_value(x, y):
-        _, _, r, _, _ = linregress(x, y)
-        return r
-
-    return rolling_apply_cols([left, right], _r_value, N)
-
-
-def Resi(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling Regression Residuals
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with regression residuals of given window
-    """
-
-    def _resi(x, y):
-        slope, intercept, r_value, p_value, std_err = linregress(x, y)
-        return std_err
-
-    return rolling_apply_cols([left, right], _resi, N)
-
-
-def WMA(feature: Feature, N: int) -> pl.Expr:
-    """Rolling WMA
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with weighted moving average output
-    """
-
-    def weighted_mean(x):
-        w = np.arange(len(x))
-        w = w / w.sum()
-        return np.nanmean(w * x)
-
-    return feature.rolling_apply(weighted_mean, N)
-
-
-def EMA(feature: Feature, N: int) -> pl.Expr:
-    """Rolling Exponential Mean (EMA)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int, float
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with regression r-value square of given window
-    """
-
-    def exp_weighted_mean(x):
-        a = 1 - 2 / (1 + len(x))
-        w = a ** np.arange(len(x))[::-1]
-        w /= w.sum()
-        return np.nansum(w * x)
-
-    return feature.rolling_apply(exp_weighted_mean, N)
-
-
-def Corr(left: Feature, right: Feature, N: int) -> pl.Expr:
-    """Rolling Correlation
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling correlation of two input features
-    """
-    return rolling_apply_cols([left, right], pearsonr, N)
-
-
-def Cov(left: Feature, right: Feature, N: int) -> pl.Expr:
-    """Rolling Covariance
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max of two input features
-    """
-
-    def _cov(x, y):
-        return np.cov(x, y)[0, 1]
-
-    return rolling_apply_cols([left, right], _cov, N)
+"""操作"""
+import numpy as np
+import polars as pl
+from scipy.stats import percentileofscore, linregress, pearsonr
+from .functions import rolling_apply_cols
+
+
+Feature = pl.col
+
+
+def Abs(feature: Feature):
+    """Feature Abs
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with Abs
+    """
+    return Feature.abs()
+
+
+def Sign(feature: Feature):
+    """Feature Sign
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with Sign
+    """
+    return Feature.sign()
+
+
+def Log(feature: Feature):
+    """Feature Log
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with log
+    """
+    return feature.log()
+
+
+def Log10(feature: Feature):
+    """Feature Log10
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with log10
+    """
+    return feature.log10()
+
+
+# * def Mask(feature: Feature):
+# *
+# * class Mask(NpElemOperator):
+# *    """Feature Mask
+# *
+# *    Parameters
+# *    ----------
+# *    feature : Expression
+# *        feature instance
+# *    instrument : str
+# *        instrument mask
+# *
+# *    Returns
+# *    ----------
+# *    Expression
+# *        a feature instance with masked instrument
+# *    """
+# *
+# *    def __init__(self, feature, instrument):
+# *        super(Mask, self).__init__(feature, "mask")
+# *        self.instrument = instrument
+# *
+# *    def __str__(self):
+# *        return f"{type(self).__name__}({self.feature},{self.instrument.lower()})"
+# *
+# *    def _load_internal(self, instrument, start_index, end_index, *args):
+# *        return self.feature.load(self.instrument, start_index, end_index, *args)
+
+
+def Not(feature: Feature):
+    """Not Operator
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+
+    Returns
+    ----------
+    Feature:
+        feature elementwise not output
+    """
+    return feature.is_not()
+
+
+def Power(left: Feature, right: Feature):
+    """Power Operator
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+
+    Returns
+    ----------
+    Feature:
+        The bases in feature_left raised to the exponents in feature_right
+    """
+    return left.pow(right)
+
+
+def If(condition: Feature, left: Feature, right: Feature) -> Feature:
+    return pl.when(condition).then(left).otherwise(right)
+
+
+def Ref(feature: Feature, N: int) -> Feature:
+    """Feature Reference
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        N = 0, retrieve the first data; N > 0, retrieve data of N periods ago; N < 0, future data
+
+    Returns
+    ----------
+    Expression
+        a feature instance with target reference
+    """
+    return feature.shift(N)
+
+
+def Mean(feature: Feature, N: int) -> Feature:
+    """Rolling Mean (MA)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling average
+    """
+    return feature.rolling_mean(N)
+
+
+def Sum(feature: Feature, N: int) -> Feature:
+    """Rolling Sum
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling sum
+    """
+    return feature.rolling_sum(N)
+
+
+def Std(feature: Feature, N: int) -> Feature:
+    """Rolling Std
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling std
+    """
+    return feature.rolling_std(N)
+
+
+def Var(feature: Feature, N: int) -> Feature:
+    """Rolling Variance
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling variance
+    """
+    return feature.rolling_var(N)
+
+
+def Skew(feature: Feature, N: int) -> Feature:
+    """Rolling Skewness
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling skewness
+    """
+    return feature.rolling_skew(N)
+
+
+def Kurt(feature: Feature, N: int) -> Feature:
+    """Rolling Kurtosis
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling kurtosis
+    """
+    return feature.rolling_apply(lambda x: x.kurtosis(), N)
+
+
+def Max(feature: False, N: int) -> Feature:
+    """Rolling Max
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max
+    """
+    return feature.rolling_max(N)
+
+
+def IdxMax(feature: Feature, N: int) -> Feature:
+    """Rolling Max Index
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max index
+    """
+    return feature.rolling_apply(lambda s: s.arr.arg_max(), N)
+
+
+def Min(feature: Feature, N: int) -> Feature:
+    """Rolling Min
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling min
+    """
+    return feature.rolling_min(N)
+
+
+def IdxMin(feature: Feature, N: int) -> Feature:
+    """Rolling Min Index
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling min index
+    """
+    return feature.rolling_apply(lambda s: s.arr.arg_min(), N)
+
+
+def Quantile(feature: Feature, N: int) -> Feature:
+    """Rolling Quantile
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling quantile
+    """
+    return feature.rollout_quantile(N)
+
+
+def Med(feature: Feature, N: int) -> Feature:
+    """Rolling Median
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling median
+    """
+
+    return feature.rolling_median(N)
+
+
+def Mad(feature: Feature, N: int) -> Feature:
+    """Rolling Mean Absolute Deviation
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling mean absolute deviation
+    """
+    return (feature - feature.rolling_mean(N)).abs().rolling_mean(N)
+
+
+def _rank(x):
+    x = x.to_numpy()
+    if np.isnan(x[-1]):
+        return np.nan
+    x1 = x[~np.isnan(x)]
+    return np.nan if x1.shape[0] == 0 else percentileofscore(x1, x1[-1]) / len(x1)
+
+
+def Rank(feature: Feature, N: int) -> Feature:
+    """Rolling Rank (Percentile)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling rank
+    """
+    return feature.rolling_apply(_rank, N)
+
+
+def Count(feature: Feature, N: int) -> Feature:
+    """Rolling Count
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling count of number of non-NaN elements
+    """
+    return feature.rolling_apply(lambda x: x.count(), N)
+
+
+def Delta(feature: Feature, N: int) -> Feature:
+    """Rolling Delta
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with end minus start in rolling window
+    """
+    return feature - feature.shift(N)
+
+
+def Slope(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling Slope `Slope(A, B, N)`
+    This operator calculate the slope between `left` and `right`.
+
+    Usage Example:
+    - "Slope($high, %low, 10)/$close"
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with linear regression slope of given window
+    """
+
+    def _slope(x, y):
+        slope_ret, _ = linregress(x, y)
+        return slope_ret
+
+    return rolling_apply_cols([left, right], _slope, N)
+
+
+def Rsquare(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling R-value Square
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with linear regression r-value square of given window
+    """
+
+    def _r_value(x, y):
+        _, _, r, _, _ = linregress(x, y)
+        return r
+
+    return rolling_apply_cols([left, right], _r_value, N)
+
+
+def Resi(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling Regression Residuals
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with regression residuals of given window
+    """
+
+    def _resi(x, y):
+        slope, intercept, r_value, p_value, std_err = linregress(x, y)
+        return std_err
+
+    return rolling_apply_cols([left, right], _resi, N)
+
+
+def WMA(feature: Feature, N: int) -> pl.Expr:
+    """Rolling WMA
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with weighted moving average output
+    """
+
+    def weighted_mean(x):
+        w = np.arange(len(x))
+        w = w / w.sum()
+        return np.nanmean(w * x)
+
+    return feature.rolling_apply(weighted_mean, N)
+
+
+def EMA(feature: Feature, N: int) -> pl.Expr:
+    """Rolling Exponential Mean (EMA)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int, float
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with regression r-value square of given window
+    """
+
+    def exp_weighted_mean(x):
+        a = 1 - 2 / (1 + len(x))
+        w = a ** np.arange(len(x))[::-1]
+        w /= w.sum()
+        return np.nansum(w * x)
+
+    return feature.rolling_apply(exp_weighted_mean, N)
+
+
+def Corr(left: Feature, right: Feature, N: int) -> pl.Expr:
+    """Rolling Correlation
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling correlation of two input features
+    """
+    return rolling_apply_cols([left, right], pearsonr, N)
+
+
+def Cov(left: Feature, right: Feature, N: int) -> pl.Expr:
+    """Rolling Covariance
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max of two input features
+    """
+
+    def _cov(x, y):
+        return np.cov(x, y)[0, 1]
+
+    return rolling_apply_cols([left, right], _cov, N)
```

### Comparing `vxquant-2023.3.1/src/vxdataset/handler.py` & `vxquant-2023.4.1/src/vxdataset/handler.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""数据指标计算器"""
-import re
-import abc
-from vxutils import vxtime
-from vxdataset.expr.ops import *
-from typing import Callable, Any
-from tdqm import tdqm
-
-
-class vxDataHandler(abc.ABC):
-    def __init__(self, loader):
-        self._loader = loader
-        self._datas = None
-
-    @classmethod
-    def from_dataloader(
-        cls, loader: Callable, symbols: str, start_date: Any, end_date: Any
-    ):
-        return cls(loader(symbols, start_date, end_date))
-
-    def _parser_expr(self, name, feature):
-        # Following patterns will be matched:
-        # - $close -> Feature("close")
-        # - $close5 -> Feature("close5")
-        # - $open+$close -> Feature("open")+Feature("close")
-        # TODO: this maybe used in the feature if we want to support the computation of different frequency data
-        # - $close@5min -> Feature("close", "5min")
-
-        if not isinstance(feature, str):
-            feature = str(feature)
-        # Chinese punctuation regex:
-        # \u3001 -> 、
-        # \uff1a -> ：
-        # \uff08 -> (
-        # \uff09 -> )
-        chinese_punctuation_regex = r"\u3001\uff1a\uff08\uff09"
-        for pattern, new in [
-            (
-                rf"\$\$([\w{chinese_punctuation_regex}]+)",
-                r'PFeature("\1")',
-            ),  # $$ must be before $
-            (rf"\$([\w{chinese_punctuation_regex}]+)", r'Feature("\1")'),
-            # (r"(\w+\s*)\(", r"Operators.\1("),
-        ]:  # Features  # Operators
-            feature = re.sub(pattern, new, feature)
-
-        return eval(feature).over("symbol").alias(name)
-
-    def _handle(self, data, exprs):
-        return data.with_columns(exprs)
-
-    def calc_features(self, features):
-        exprs = [self._parser_expr(name, feature) for name, feature in features.items()]
-
-        with vxtime.timeit("build features"):
-            self._datas = list(
-                map(lambda x: self._handle(x, exprs), self._datas.values())
-            )
-
-        return self
-
-    def to_pandas(self):
-        return self._datas.to_pandas()
-
-    def to_polars(self):
-        return self._datas
-
-    def to_csv(self, filename):
-        with open(filename, "w") as f:
-            self._datas.write_csv(f)
-
-
-if __name__ == "__main__":
-    from vxdataset.loaders.csv import vxCSVLoader
-
-    loader = vxCSVLoader("examples/data/")
-    d = loader.load(["sh000300"])
-
-    features = {
-        "high": "$high",
-        "mom20": "Ref($close, 20)/$close",
-        "ret": "$close/Ref($close,1)-1",
-        "roc20": "Rank($high,252)",
-    }
-    handler = vxDataHandler(loader)
-    ds = handler.calc_features(features)
-    print(ds)
+"""数据指标计算器"""
+import re
+import abc
+from vxutils import vxtime
+from vxdataset.expr.ops import *
+from typing import Callable, Any
+from tdqm import tdqm
+
+
+class vxDataHandler(abc.ABC):
+    def __init__(self, loader):
+        self._loader = loader
+        self._datas = None
+
+    @classmethod
+    def from_dataloader(
+        cls, loader: Callable, symbols: str, start_date: Any, end_date: Any
+    ):
+        return cls(loader(symbols, start_date, end_date))
+
+    def _parser_expr(self, name, feature):
+        # Following patterns will be matched:
+        # - $close -> Feature("close")
+        # - $close5 -> Feature("close5")
+        # - $open+$close -> Feature("open")+Feature("close")
+        # TODO: this maybe used in the feature if we want to support the computation of different frequency data
+        # - $close@5min -> Feature("close", "5min")
+
+        if not isinstance(feature, str):
+            feature = str(feature)
+        # Chinese punctuation regex:
+        # \u3001 -> 、
+        # \uff1a -> ：
+        # \uff08 -> (
+        # \uff09 -> )
+        chinese_punctuation_regex = r"\u3001\uff1a\uff08\uff09"
+        for pattern, new in [
+            (
+                rf"\$\$([\w{chinese_punctuation_regex}]+)",
+                r'PFeature("\1")',
+            ),  # $$ must be before $
+            (rf"\$([\w{chinese_punctuation_regex}]+)", r'Feature("\1")'),
+            # (r"(\w+\s*)\(", r"Operators.\1("),
+        ]:  # Features  # Operators
+            feature = re.sub(pattern, new, feature)
+
+        return eval(feature).over("symbol").alias(name)
+
+    def _handle(self, data, exprs):
+        return data.with_columns(exprs)
+
+    def calc_features(self, features):
+        exprs = [self._parser_expr(name, feature) for name, feature in features.items()]
+
+        with vxtime.timeit("build features"):
+            self._datas = list(
+                map(lambda x: self._handle(x, exprs), self._datas.values())
+            )
+
+        return self
+
+    def to_pandas(self):
+        return self._datas.to_pandas()
+
+    def to_polars(self):
+        return self._datas
+
+    def to_csv(self, filename):
+        with open(filename, "w") as f:
+            self._datas.write_csv(f)
+
+
+if __name__ == "__main__":
+    from vxdataset.loaders.csv import vxCSVLoader
+
+    loader = vxCSVLoader("examples/data/")
+    d = loader.load(["sh000300"])
+
+    features = {
+        "high": "$high",
+        "mom20": "Ref($close, 20)/$close",
+        "ret": "$close/Ref($close,1)-1",
+        "roc20": "Rank($high,252)",
+    }
+    handler = vxDataHandler(loader)
+    ds = handler.calc_features(features)
+    print(ds)
```

### Comparing `vxquant-2023.3.1/src/vxdataset/loaders/base.py` & `vxquant-2023.4.1/src/vxdataset/loaders/base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-"""数据加载器"""
-import abc
-import datetime
-import polars as pl
-from pathlib import Path
-from typing import List, Union
-from tqdm import tqdm
-
-Date = Union[float, str, datetime.date, datetime.datetime]
-PathType = Union[str, Path]
-
-
-class vxDataLoader(abc.ABC):
-    """
-    vxDataLoader is designed for loading raw data from original data source.
-    """
-
-    __cache_dir__ = Path("~/.vxdataset/cache/")
-
-    @classmethod
-    def set_cache_dir(cls, cache_dir: PathType) -> None:
-        if isinstance(cache_dir, str):
-            cache_dir = Path(cache_dir)
-
-        cache_dir.mkdir(parents=True, exist_ok=True)
-        cls.__cache_dir__ = cache_dir
-
-    @abc.abstractmethod
-    def _load_basics(
-        self,
-        symbols: List[str],
-        freq: str = "day",
-        start_date: Date = None,
-        end_date: Date = None,
-    ) -> pl.DataFrame:
-        """加载基础量价信息
-
-        Arguments:
-            symbols {list} -- 证券代码列表
-            start_date {Date} -- 开始日期
-            end_date {Date} -- 结束日期
-
-        Returns:
-            pl.Dateframe: ['date','symbol','freq','open','high','low','close','amount','volume','factor','instert']
-
-        """
-        pass
-
-    @abc.abstractmethod
-    def _load_indicators(
-        self,
-        symbols: List[str],
-        freq: str = "day",
-        start_date: Date = None,
-        end_date: Date = None,
-    ) -> pl.DataFrame:
-        """加载不同证券类型的指标
-
-        Arguments:
-            symbols {list} -- 证券代码列表，此处所有的证券代码的类型必须一致
-            start_date {Date} -- 开始日期
-            end_date {Date} -- 结束日期
-        """
-        pass
-
-    def load(
-        self,
-        symbols: List,
-        freq: str = "day",
-        start_date: Date = None,
-        end_date: Date = None,
-    ) -> pl.DataFrame:
-        """
-        load the data as pl.DataFrame.
-
-        Example of the data :
-
-            .. code-block:: python
-
-                datetime    instrument  close      volume            high              ma3          oml    ret
-
-                2010-01-04  SH600000    81.807068  17145150.0       83.737389        83.016739    2.741058  0.0032
-                2010-01-04  SH600004    13.313329  11800983.0       13.313329        13.317701    0.183632  0.0042
-                2010-01-04  SH600005    37.796539  12231662.0       38.258602        37.919757    0.970325  0.0289
-
-
-        Parameters
-        ----------
-        instruments : str or dict
-            it can either be the market name or the config file of instruments generated by InstrumentProvider.
-        start_time : str
-            start of the time range.
-        end_time : str
-            end of the time range.
-
-        Returns
-        -------
-        pl.DataFrame:
-            data load from the under layer source
-        """
-        basics_cache_file = Path(self.__cache_dir__, freq, "basics.parquet")
-        if basics_cache_file.exists():
-            basics_data = pl.read_parquet(basics_cache_file)
-        else:
-            basics_data = pl.DataFrame([], columns=["date", "symbol", "freq"])
-
-        return pl.concat(
-            [self.load_one_df(symbol, start_date, end_date) for symbol in tqdm(symbols)]
-        )
-
-
-if __name__ == "__main__":
-    d = vxDataLoader()
+"""数据加载器"""
+import abc
+import datetime
+import polars as pl
+from pathlib import Path
+from typing import List, Union
+from tqdm import tqdm
+
+Date = Union[float, str, datetime.date, datetime.datetime]
+PathType = Union[str, Path]
+
+
+class vxDataLoader(abc.ABC):
+    """
+    vxDataLoader is designed for loading raw data from original data source.
+    """
+
+    __cache_dir__ = Path("~/.vxdataset/cache/")
+
+    @classmethod
+    def set_cache_dir(cls, cache_dir: PathType) -> None:
+        if isinstance(cache_dir, str):
+            cache_dir = Path(cache_dir)
+
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        cls.__cache_dir__ = cache_dir
+
+    @abc.abstractmethod
+    def _load_basics(
+        self,
+        symbols: List[str],
+        freq: str = "day",
+        start_date: Date = None,
+        end_date: Date = None,
+    ) -> pl.DataFrame:
+        """加载基础量价信息
+
+        Arguments:
+            symbols {list} -- 证券代码列表
+            start_date {Date} -- 开始日期
+            end_date {Date} -- 结束日期
+
+        Returns:
+            pl.Dateframe: ['date','symbol','freq','open','high','low','close','amount','volume','factor','instert']
+
+        """
+        pass
+
+    @abc.abstractmethod
+    def _load_indicators(
+        self,
+        symbols: List[str],
+        freq: str = "day",
+        start_date: Date = None,
+        end_date: Date = None,
+    ) -> pl.DataFrame:
+        """加载不同证券类型的指标
+
+        Arguments:
+            symbols {list} -- 证券代码列表，此处所有的证券代码的类型必须一致
+            start_date {Date} -- 开始日期
+            end_date {Date} -- 结束日期
+        """
+        pass
+
+    def load(
+        self,
+        symbols: List,
+        freq: str = "day",
+        start_date: Date = None,
+        end_date: Date = None,
+    ) -> pl.DataFrame:
+        """
+        load the data as pl.DataFrame.
+
+        Example of the data :
+
+            .. code-block:: python
+
+                datetime    instrument  close      volume            high              ma3          oml    ret
+
+                2010-01-04  SH600000    81.807068  17145150.0       83.737389        83.016739    2.741058  0.0032
+                2010-01-04  SH600004    13.313329  11800983.0       13.313329        13.317701    0.183632  0.0042
+                2010-01-04  SH600005    37.796539  12231662.0       38.258602        37.919757    0.970325  0.0289
+
+
+        Parameters
+        ----------
+        instruments : str or dict
+            it can either be the market name or the config file of instruments generated by InstrumentProvider.
+        start_time : str
+            start of the time range.
+        end_time : str
+            end of the time range.
+
+        Returns
+        -------
+        pl.DataFrame:
+            data load from the under layer source
+        """
+        basics_cache_file = Path(self.__cache_dir__, freq, "basics.parquet")
+        if basics_cache_file.exists():
+            basics_data = pl.read_parquet(basics_cache_file)
+        else:
+            basics_data = pl.DataFrame([], columns=["date", "symbol", "freq"])
+
+        return pl.concat(
+            [self.load_one_df(symbol, start_date, end_date) for symbol in tqdm(symbols)]
+        )
+
+
+if __name__ == "__main__":
+    d = vxDataLoader()
```

### Comparing `vxquant-2023.3.1/src/vxquant/__main__.py` & `vxquant-2023.4.1/src/vxquant/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """配置文件"""
-
+import sys
 import json
+import textwrap
 import argparse
 from typing import Union
 from pathlib import Path
+
 from concurrent.futures import ThreadPoolExecutor as Executor
 from vxsched import vxContext
 from vxsched.core import vxscheduler
 from vxutils import vxLRUCache, logger, DiskCacheUnit
 from vxquant.apis import vxMdAPI, vxTdAPI
-
+from vxquant.cli import vxCommand
 
 _cache_path = Path.home().joinpath(".vxcache").absolute()
 
 _default_config = {
     "params": {},
     "providers": {
         "mdapi": {},
@@ -72,28 +74,56 @@
         for key in ["params", "settings", "providers"]:
             _context[key] = context[key]
 
         # _context.save_json(config_file)
         logger.info(f"保存配置文件: {config_file}")
 
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="config json file path: etc/config.json",
-        default="etc/config.json",
-        type=str,
-    )
-    parser.add_argument(
-        "-m", "--mod", help="module directory path : mod/ ", default="mod/", type=str
+desc = """
+vxquant是一个量化金融框架Python包，用于为个人提供实盘交易以及量化研究支持，使用户更加专注于交易策略的编写。
+框架具有以下特点：
+1. 支持多账户体系运行
+2. 支持掘金量化实盘以及模拟盘
+3. 支持miniQMT实盘以及模拟盘
+本命令为vxquant框架命令行接口，本接口可方便执行以下命令.
+"""
+
+
+def main(args=None) -> int:
+    if args is None:
+        args = sys.argv[1:]
+    if len(args) == 0:
+        args = ["-h"]
+
+    parser = argparse.ArgumentParser(
+        prog="vxquant",
+        usage="vxquant <command> [options]",
+        description=textwrap.dedent(desc),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        add_help=False,
     )
+
     parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+        "-v",
+        "--version",
+        help="显示vxquant版本",
+        action="version",
+        version="2023.3.1",
     )
-    args = parser.parse_args()
+    parser.add_argument("-h", "--help", help="显示当前帮助信息", action="help")
+    sub_parser = parser.add_subparsers(metavar="命令列表", dest="cmd")
+
+    for command in vxCommand.cmds.values():
+        command.set_parser(sub_parser)
+
+    args = parser.parse_args(args)
+    command = vxCommand.cmds[args.cmd]
+    command(args)
 
-    if args.verbose:
-        logger.setLevel("DEBUG")
+    # if args.verbose:
+    #    logger.setLevel("DEBUG")
 
-    run_quant(config_file=args.config, mod_path=args.mod)
+    # run_quant(config_file=args.config, mod_path=args.mod)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `vxquant-2023.3.1/src/vxquant/exceptions.py` & `vxquant-2023.4.1/src/vxquant/exceptions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-"""账户异常类"""
-
-
-__all__ = []
-
-
-class vxQuantException(Exception):
-    pass
-
-
-class RiskRuleCheckFailed(vxQuantException):
-    # 不符合风控规则
-    pass
-
-
-class NoEnoughCash(vxQuantException):
-    # 资金不足
-    pass
-
-
-class NoEnoughPosition(vxQuantException):
-    pass
-
-
-class IllegalAccountId(vxQuantException):
-    # 非法账户ID
-    pass
-
-
-class IllegalStrategyId(vxQuantException):
-    # 非法策略ID
-    pass
-
-
-class IllegalSymbol(vxQuantException):
-    # 非法交易标的
-    pass
-
-
-class IllegalVolume(vxQuantException):
-    # 非法委托量
-    pass
-
-
-class IllegalPrice(vxQuantException):
-    # 非法委托价
-    pass
-
-
-class AccountDisabled(vxQuantException):
-    # 交易账号被禁止交易
-    pass
-
-
-class AccountDisconnected(vxQuantException):
-    # 交易账号未连接
-    pass
-
-
-class AccountLoggedout(vxQuantException):
-    # 交易账号未登录
-    pass
-
-
-class NotInTradingSession(vxQuantException):
-    # 非交易时段
-    pass
-
-
-class OrderTypeNotSupported(vxQuantException):
-    # 委托类型不支持
-    pass
-
-
-class Throttle(vxQuantException):
-    # 流控限制
-    pass
-
-
-class IllegalOrder(vxQuantException):
-    # 交易委托不支持
-    pass
-
-
-class OrderFinalized(vxQuantException):
-    # 委托已经完成
-    pass
-
-
-class UnknownOrder(vxQuantException):
-    # 未知委托
-    pass
-
-
-class AlreadyInPendingCancel(vxQuantException):
-    # 已经在撤单中
-    pass
+"""账户异常类"""
+
+
+__all__ = []
+
+
+class vxQuantException(Exception):
+    pass
+
+
+class RiskRuleCheckFailed(vxQuantException):
+    # 不符合风控规则
+    pass
+
+
+class NoEnoughCash(vxQuantException):
+    # 资金不足
+    pass
+
+
+class NoEnoughPosition(vxQuantException):
+    pass
+
+
+class IllegalAccountId(vxQuantException):
+    # 非法账户ID
+    pass
+
+
+class IllegalStrategyId(vxQuantException):
+    # 非法策略ID
+    pass
+
+
+class IllegalSymbol(vxQuantException):
+    # 非法交易标的
+    pass
+
+
+class IllegalVolume(vxQuantException):
+    # 非法委托量
+    pass
+
+
+class IllegalPrice(vxQuantException):
+    # 非法委托价
+    pass
+
+
+class AccountDisabled(vxQuantException):
+    # 交易账号被禁止交易
+    pass
+
+
+class AccountDisconnected(vxQuantException):
+    # 交易账号未连接
+    pass
+
+
+class AccountLoggedout(vxQuantException):
+    # 交易账号未登录
+    pass
+
+
+class NotInTradingSession(vxQuantException):
+    # 非交易时段
+    pass
+
+
+class OrderTypeNotSupported(vxQuantException):
+    # 委托类型不支持
+    pass
+
+
+class Throttle(vxQuantException):
+    # 流控限制
+    pass
+
+
+class IllegalOrder(vxQuantException):
+    # 交易委托不支持
+    pass
+
+
+class OrderFinalized(vxQuantException):
+    # 委托已经完成
+    pass
+
+
+class UnknownOrder(vxQuantException):
+    # 未知委托
+    pass
+
+
+class AlreadyInPendingCancel(vxQuantException):
+    # 已经在撤单中
+    pass
```

### Comparing `vxquant-2023.3.1/src/vxquant/factor/expr/ops.py` & `vxquant-2023.4.1/src/vxquant/factor/expr/ops.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,668 +1,668 @@
-"""操作"""
-import numpy as np
-import polars as pl
-from scipy.stats import percentileofscore, linregress, pearsonr, spearmanr
-from .functions import rolling_apply_cols
-
-
-Feature = pl.col
-
-
-def Abs(feature: Feature):
-    """Feature Abs
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with Abs
-    """
-    return Feature.abs()
-
-
-def Sign(feature: Feature):
-    """Feature Sign
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with Sign
-    """
-    return Feature.sign()
-
-
-def Log(feature: Feature):
-    """Feature Log
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with log
-    """
-    return feature.log()
-
-
-def Log10(feature: Feature):
-    """Feature Log10
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-
-    Returns
-    ----------
-    Expression
-        a feature instance with log10
-    """
-    return feature.log10()
-
-
-# * def Mask(feature: Feature):
-# *
-# * class Mask(NpElemOperator):
-# *    """Feature Mask
-# *
-# *    Parameters
-# *    ----------
-# *    feature : Expression
-# *        feature instance
-# *    instrument : str
-# *        instrument mask
-# *
-# *    Returns
-# *    ----------
-# *    Expression
-# *        a feature instance with masked instrument
-# *    """
-# *
-# *    def __init__(self, feature, instrument):
-# *        super(Mask, self).__init__(feature, "mask")
-# *        self.instrument = instrument
-# *
-# *    def __str__(self):
-# *        return f"{type(self).__name__}({self.feature},{self.instrument.lower()})"
-# *
-# *    def _load_internal(self, instrument, start_index, end_index, *args):
-# *        return self.feature.load(self.instrument, start_index, end_index, *args)
-
-
-def Not(feature: Feature):
-    """Not Operator
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-
-    Returns
-    ----------
-    Feature:
-        feature elementwise not output
-    """
-    return feature.is_not()
-
-
-def Power(left: Feature, right: Feature):
-    """Power Operator
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-
-    Returns
-    ----------
-    Feature:
-        The bases in feature_left raised to the exponents in feature_right
-    """
-    return left.pow(right)
-
-
-def If(condition: Feature, left: Feature, right: Feature) -> Feature:
-    return pl.when(condition).then(left).otherwise(right)
-
-
-def Ref(feature: Feature, N: int) -> Feature:
-    """Feature Reference
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        N = 0, retrieve the first data; N > 0, retrieve data of N periods ago; N < 0, future data
-
-    Returns
-    ----------
-    Expression
-        a feature instance with target reference
-    """
-    return feature.shift(N)
-
-
-def Mean(feature: Feature, N: int) -> Feature:
-    """Rolling Mean (MA)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling average
-    """
-    return feature.rolling_mean(N)
-
-
-def Sum(feature: Feature, N: int) -> Feature:
-    """Rolling Sum
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling sum
-    """
-    return feature.rolling_sum(N)
-
-
-def Std(feature: Feature, N: int) -> Feature:
-    """Rolling Std
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling std
-    """
-    return feature.rolling_std(N)
-
-
-def Var(feature: Feature, N: int) -> Feature:
-    """Rolling Variance
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling variance
-    """
-    return feature.rolling_var(N)
-
-
-def Skew(feature: Feature, N: int) -> Feature:
-    """Rolling Skewness
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling skewness
-    """
-    return feature.rolling_skew(N)
-
-
-def Kurt(feature: Feature, N: int) -> Feature:
-    """Rolling Kurtosis
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling kurtosis
-    """
-    return feature.rolling_apply(lambda x: x.kurtosis(), N)
-
-
-def Max(feature: False, N: int) -> Feature:
-    """Rolling Max
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max
-    """
-    return feature.rolling_max(N)
-
-
-def IdxMax(feature: Feature, N: int) -> Feature:
-    """Rolling Max Index
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max index
-    """
-    return feature.rolling_apply(lambda s: s.arr.arg_max(), N)
-
-
-def Min(feature: Feature, N: int) -> Feature:
-    """Rolling Min
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling min
-    """
-    return feature.rolling_min(N)
-
-
-def IdxMin(feature: Feature, N: int) -> Feature:
-    """Rolling Min Index
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling min index
-    """
-    return feature.rolling_apply(lambda s: s.arr.arg_min(), N)
-
-
-def Quantile(feature: Feature, N: int) -> Feature:
-    """Rolling Quantile
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling quantile
-    """
-    return feature.rollout_quantile(N)
-
-
-def Med(feature: Feature, N: int) -> Feature:
-    """Rolling Median
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling median
-    """
-
-    return feature.rolling_median(N)
-
-
-def Mad(feature: Feature, N: int) -> Feature:
-    """Rolling Mean Absolute Deviation
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling mean absolute deviation
-    """
-    return (feature - feature.rolling_mean(N)).abs().rolling_mean(N)
-
-
-def _rank(x):
-    x = x.to_numpy()
-    if np.isnan(x[-1]):
-        return np.nan
-    x1 = x[~np.isnan(x)]
-    return np.nan if x1.shape[0] == 0 else percentileofscore(x1, x1[-1]) / len(x1)
-
-
-def Rank(feature: Feature, N: int) -> Feature:
-    """Rolling Rank (Percentile)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling rank
-    """
-    return feature.rolling_apply(_rank, N)
-
-
-def Count(feature: Feature, N: int) -> Feature:
-    """Rolling Count
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling count of number of non-NaN elements
-    """
-    return feature.rolling_apply(lambda x: x.count(), N)
-
-
-def Delta(feature: Feature, N: int) -> Feature:
-    """Rolling Delta
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with end minus start in rolling window
-    """
-    return feature - feature.shift(N)
-
-
-def Slope(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling Slope `Slope(A, B, N)`
-    This operator calculate the slope between `left` and `right`.
-
-    Usage Example:
-    - "Slope($high, %low, 10)/$close"
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with linear regression slope of given window
-    """
-
-    def _slope(x, y):
-        slope_ret, _ = linregress(x, y)
-        return slope_ret
-
-    return rolling_apply_cols([left, right], _slope, N)
-
-
-def Rsquare(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling R-value Square
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with linear regression r-value square of given window
-    """
-
-    def _r_value(x, y):
-        _, _, r, _, _ = linregress(x, y)
-        return r
-
-    return rolling_apply_cols([left, right], _r_value, N)
-
-
-def Resi(left: Feature, right: Feature, N: int) -> Feature:
-    """Rolling Regression Residuals
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with regression residuals of given window
-    """
-
-    def _resi(x, y):
-        slope, intercept, r_value, p_value, std_err = linregress(x, y)
-        return std_err
-
-    return rolling_apply_cols([left, right], _resi, N)
-
-
-def WMA(feature: Feature, N: int) -> pl.Expr:
-    """Rolling WMA
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with weighted moving average output
-    """
-
-    w = np.arange(N)
-    w = w / w.sum()
-
-    return feature.rolling_mean(N, weights=w)
-
-
-def WSTD(feature: Feature, N: int) -> pl.Expr:
-    """Rolling Weight Std
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with weighted moving  std output
-    """
-    w = np.arange(N)
-    w = w / w.sum()
-
-    return feature.rolling_std(N, weights=w)
-
-
-def EMA(feature: Feature, N: int) -> pl.Expr:
-    """Rolling Exponential Mean (EMA)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int, float
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with regression r-value square of given window
-    """
-
-    a = 1 - 2 / (1 + N)
-    w = a ** np.arange(N)[::-1]
-    w /= w.sum()
-
-    return feature.rolling_mean(N, weights=w)
-
-
-def ESTD(feature: Feature, N: int) -> pl.Expr:
-    """Rolling Exponential Std (ESTD)
-
-    Parameters
-    ----------
-    feature : Expression
-        feature instance
-    N : int, float
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with regression r-value square of given window
-    """
-
-    a = 1 - 2 / (1 + N)
-    w = a ** np.arange(N)[::-1]
-    w /= w.sum()
-
-    return feature.rolling_std(N, weights=w)
-
-
-def Corr(left: Feature, right: Feature, N: int) -> pl.Expr:
-    """Rolling Correlation
-
-    Parameters
-    ----------
-    left : Expression
-        feature instance
-    right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling correlation of two input features
-    """
-    return rolling_apply_cols([left, right], pearsonr, N)
-
-
-def Cov(left: Feature, right: Feature, N: int) -> pl.Expr:
-    """Rolling Covariance
-
-    Parameters
-    ----------
-    feature_left : Expression
-        feature instance
-    feature_right : Expression
-        feature instance
-    N : int
-        rolling window size
-
-    Returns
-    ----------
-    Expression
-        a feature instance with rolling max of two input features
-    """
-
-    def _cov(x, y):
-        return np.cov(x, y)[0, 1]
-
-    return rolling_apply_cols([left, right], _cov, N)
+"""操作"""
+import numpy as np
+import polars as pl
+from scipy.stats import percentileofscore, linregress, pearsonr, spearmanr
+from .functions import rolling_apply_cols
+
+
+Feature = pl.col
+
+
+def Abs(feature: Feature):
+    """Feature Abs
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with Abs
+    """
+    return Feature.abs()
+
+
+def Sign(feature: Feature):
+    """Feature Sign
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with Sign
+    """
+    return Feature.sign()
+
+
+def Log(feature: Feature):
+    """Feature Log
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with log
+    """
+    return feature.log()
+
+
+def Log10(feature: Feature):
+    """Feature Log10
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+
+    Returns
+    ----------
+    Expression
+        a feature instance with log10
+    """
+    return feature.log10()
+
+
+# * def Mask(feature: Feature):
+# *
+# * class Mask(NpElemOperator):
+# *    """Feature Mask
+# *
+# *    Parameters
+# *    ----------
+# *    feature : Expression
+# *        feature instance
+# *    instrument : str
+# *        instrument mask
+# *
+# *    Returns
+# *    ----------
+# *    Expression
+# *        a feature instance with masked instrument
+# *    """
+# *
+# *    def __init__(self, feature, instrument):
+# *        super(Mask, self).__init__(feature, "mask")
+# *        self.instrument = instrument
+# *
+# *    def __str__(self):
+# *        return f"{type(self).__name__}({self.feature},{self.instrument.lower()})"
+# *
+# *    def _load_internal(self, instrument, start_index, end_index, *args):
+# *        return self.feature.load(self.instrument, start_index, end_index, *args)
+
+
+def Not(feature: Feature):
+    """Not Operator
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+
+    Returns
+    ----------
+    Feature:
+        feature elementwise not output
+    """
+    return feature.is_not()
+
+
+def Power(left: Feature, right: Feature):
+    """Power Operator
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+
+    Returns
+    ----------
+    Feature:
+        The bases in feature_left raised to the exponents in feature_right
+    """
+    return left.pow(right)
+
+
+def If(condition: Feature, left: Feature, right: Feature) -> Feature:
+    return pl.when(condition).then(left).otherwise(right)
+
+
+def Ref(feature: Feature, N: int) -> Feature:
+    """Feature Reference
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        N = 0, retrieve the first data; N > 0, retrieve data of N periods ago; N < 0, future data
+
+    Returns
+    ----------
+    Expression
+        a feature instance with target reference
+    """
+    return feature.shift(N)
+
+
+def Mean(feature: Feature, N: int) -> Feature:
+    """Rolling Mean (MA)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling average
+    """
+    return feature.rolling_mean(N)
+
+
+def Sum(feature: Feature, N: int) -> Feature:
+    """Rolling Sum
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling sum
+    """
+    return feature.rolling_sum(N)
+
+
+def Std(feature: Feature, N: int) -> Feature:
+    """Rolling Std
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling std
+    """
+    return feature.rolling_std(N)
+
+
+def Var(feature: Feature, N: int) -> Feature:
+    """Rolling Variance
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling variance
+    """
+    return feature.rolling_var(N)
+
+
+def Skew(feature: Feature, N: int) -> Feature:
+    """Rolling Skewness
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling skewness
+    """
+    return feature.rolling_skew(N)
+
+
+def Kurt(feature: Feature, N: int) -> Feature:
+    """Rolling Kurtosis
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling kurtosis
+    """
+    return feature.rolling_apply(lambda x: x.kurtosis(), N)
+
+
+def Max(feature: False, N: int) -> Feature:
+    """Rolling Max
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max
+    """
+    return feature.rolling_max(N)
+
+
+def IdxMax(feature: Feature, N: int) -> Feature:
+    """Rolling Max Index
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max index
+    """
+    return feature.rolling_apply(lambda s: s.arr.arg_max(), N)
+
+
+def Min(feature: Feature, N: int) -> Feature:
+    """Rolling Min
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling min
+    """
+    return feature.rolling_min(N)
+
+
+def IdxMin(feature: Feature, N: int) -> Feature:
+    """Rolling Min Index
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling min index
+    """
+    return feature.rolling_apply(lambda s: s.arr.arg_min(), N)
+
+
+def Quantile(feature: Feature, N: int) -> Feature:
+    """Rolling Quantile
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling quantile
+    """
+    return feature.rollout_quantile(N)
+
+
+def Med(feature: Feature, N: int) -> Feature:
+    """Rolling Median
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling median
+    """
+
+    return feature.rolling_median(N)
+
+
+def Mad(feature: Feature, N: int) -> Feature:
+    """Rolling Mean Absolute Deviation
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling mean absolute deviation
+    """
+    return (feature - feature.rolling_mean(N)).abs().rolling_mean(N)
+
+
+def _rank(x):
+    x = x.to_numpy()
+    if np.isnan(x[-1]):
+        return np.nan
+    x1 = x[~np.isnan(x)]
+    return np.nan if x1.shape[0] == 0 else percentileofscore(x1, x1[-1]) / len(x1)
+
+
+def Rank(feature: Feature, N: int) -> Feature:
+    """Rolling Rank (Percentile)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling rank
+    """
+    return feature.rolling_apply(_rank, N)
+
+
+def Count(feature: Feature, N: int) -> Feature:
+    """Rolling Count
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling count of number of non-NaN elements
+    """
+    return feature.rolling_apply(lambda x: x.count(), N)
+
+
+def Delta(feature: Feature, N: int) -> Feature:
+    """Rolling Delta
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with end minus start in rolling window
+    """
+    return feature - feature.shift(N)
+
+
+def Slope(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling Slope `Slope(A, B, N)`
+    This operator calculate the slope between `left` and `right`.
+
+    Usage Example:
+    - "Slope($high, %low, 10)/$close"
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with linear regression slope of given window
+    """
+
+    def _slope(x, y):
+        slope_ret, _ = linregress(x, y)
+        return slope_ret
+
+    return rolling_apply_cols([left, right], _slope, N)
+
+
+def Rsquare(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling R-value Square
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with linear regression r-value square of given window
+    """
+
+    def _r_value(x, y):
+        _, _, r, _, _ = linregress(x, y)
+        return r
+
+    return rolling_apply_cols([left, right], _r_value, N)
+
+
+def Resi(left: Feature, right: Feature, N: int) -> Feature:
+    """Rolling Regression Residuals
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with regression residuals of given window
+    """
+
+    def _resi(x, y):
+        slope, intercept, r_value, p_value, std_err = linregress(x, y)
+        return std_err
+
+    return rolling_apply_cols([left, right], _resi, N)
+
+
+def WMA(feature: Feature, N: int) -> pl.Expr:
+    """Rolling WMA
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with weighted moving average output
+    """
+
+    w = np.arange(N)
+    w = w / w.sum()
+
+    return feature.rolling_mean(N, weights=w)
+
+
+def WSTD(feature: Feature, N: int) -> pl.Expr:
+    """Rolling Weight Std
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with weighted moving  std output
+    """
+    w = np.arange(N)
+    w = w / w.sum()
+
+    return feature.rolling_std(N, weights=w)
+
+
+def EMA(feature: Feature, N: int) -> pl.Expr:
+    """Rolling Exponential Mean (EMA)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int, float
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with regression r-value square of given window
+    """
+
+    a = 1 - 2 / (1 + N)
+    w = a ** np.arange(N)[::-1]
+    w /= w.sum()
+
+    return feature.rolling_mean(N, weights=w)
+
+
+def ESTD(feature: Feature, N: int) -> pl.Expr:
+    """Rolling Exponential Std (ESTD)
+
+    Parameters
+    ----------
+    feature : Expression
+        feature instance
+    N : int, float
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with regression r-value square of given window
+    """
+
+    a = 1 - 2 / (1 + N)
+    w = a ** np.arange(N)[::-1]
+    w /= w.sum()
+
+    return feature.rolling_std(N, weights=w)
+
+
+def Corr(left: Feature, right: Feature, N: int) -> pl.Expr:
+    """Rolling Correlation
+
+    Parameters
+    ----------
+    left : Expression
+        feature instance
+    right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling correlation of two input features
+    """
+    return rolling_apply_cols([left, right], pearsonr, N)
+
+
+def Cov(left: Feature, right: Feature, N: int) -> pl.Expr:
+    """Rolling Covariance
+
+    Parameters
+    ----------
+    feature_left : Expression
+        feature instance
+    feature_right : Expression
+        feature instance
+    N : int
+        rolling window size
+
+    Returns
+    ----------
+    Expression
+        a feature instance with rolling max of two input features
+    """
+
+    def _cov(x, y):
+        return np.cov(x, y)[0, 1]
+
+    return rolling_apply_cols([left, right], _cov, N)
```

### Comparing `vxquant-2023.3.1/src/vxquant/factor/normalizer.py` & `vxquant-2023.4.1/src/vxquant/factor/normalizer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-"""因子标准化"""
-
-import polars as pl
-from tqdm import tqdm
-from typing import List, Any
-from scipy.stats import linregress
-from concurrent.futures import ThreadPoolExecutor as Executor
-
-
-class vxFactorNormalizer:
-    def __init__(self, factors: pl.DataFrame):
-        self._factors = factors.drop_nulls()
-
-    def fix_nan(
-        self,
-        factor_names: List[str] = None,
-        method: str = "drop",
-        fill_value: Any = None,
-    ):
-        """修复缺失值
-
-        Arguments:
-            factor_names {List[str]} -- 因子名称
-
-        Keyword Arguments:
-            method {str} -- 修复方法：drop / fill_mad / fill_mean / fill_forward (default: {"drop"})
-
-        """
-        pass
-
-    def standardize(
-        self, factor_names: List[str] = None, n: float = 3, method: str = "mad"
-    ) -> "vxFactorNormalizer":
-        """去极值以及标准化
-
-        Keyword Arguments:
-            factor_names {List[str]} -- 因子名称 (default: {None})
-            n {float} -- 倍数 (default: {3})
-            method {str} -- 去极值的方法 (mad or winsorize_std) (default: {"MAD"})
-
-        Raises:
-            ValueError: 不支持的去极值方法
-
-        """
-        if not factor_names:
-            factor_names = self._factors.columns
-
-        if method == "mad":
-
-            def filter_extreme(factor_col) -> pl.Series:
-                median = factor_col.median()
-                new_median = (factor_col - median).abs().median()
-
-                return factor_col.clip(
-                    factor_col.median() - n * new_median,
-                    factor_col.median() + n * new_median,
-                )
-
-        elif method == "winsorize_std":
-
-            def filter_extreme(factor_cal) -> pl.Expr:
-                return factor_cal.clip(
-                    factor_cal.mean() - n * factor_cal.std(),
-                    factor_cal.mean() + n * factor_cal.std(),
-                ).over("trade_date")
-
-        else:
-            raise ValueError(f"filter extreme method: {method} 暂不支持")
-
-        print("=" * 60)
-        self._factors = self._factors.with_columns(
-            pl.col(
-                [
-                    factor_name
-                    for factor_name in factor_names
-                    if factor_name not in ["trade_date", "symbol", "mask"]
-                ]
-            )
-            .apply(filter_extreme)
-            .over("trade_date")
-        )
-        self._factors = self._factors.with_columns(
-            [
-                (pl.col(factor_name) - pl.col(factor_name).mean())
-                / pl.col(factor_name).std()
-                for factor_name in factor_names
-                if factor_name not in ["trade_date", "symbol", "mask"]
-            ]
-        )
-
-        return self
-
-    def neutralization(
-        self, factor_names: List[str], neutralize_factors: pl.DataFrame
-    ) -> "vxFactorNormalizer":
-        x = neutralize_factors.select(
-            [
-                pl.col("trade_date", "symbol"),
-                pl.concat_list(pl.exclude(["trade_date", "symbol"])).alias("x"),
-            ]
-        )
-        factor_datas = self._factors.join(x, on=["trade_date", "symbol"], how="left")
-        executor = Executor()
-        import numpy as np
-
-        with tqdm(total=len(factor_datas["trade_date"].unique())) as pbar:
-
-            def _neutralize(group_df: pl.DataFrame) -> pl.DataFrame:
-                x = group_df["x"]
-                y = group_df["vxFactor001"]
-                print(x, y)
-                print(linregress(x, y))
-
-                # print(group_df)
-                # print(x)
-
-                for name in factor_names:
-                    # resi = linregress(x, group_df[name])
-                    # print(resi)
-                    print(name)
-                # pbar.update(1)
-                # return pl.DataFrame(
-                #    dict(
-                #        executor.map(
-                #            lambda name: (
-                #                name,
-                #                linregress(x, group_df[name].to_numpy())[-1],
-                #            ),
-                #            factor_names,
-                #        )
-                #    )
-                # ).vstack(group_df.select(["trade_date", "symbol"]), in_place=False)
-
-            factor_datas.groupby("trade_date").apply(_neutralize)
-
-
-if __name__ == "__main__":
-    factor_data = pl.read_parquet("./dist/factor.parquet")
-    print(factor_data.fill_null(strategy="backward"))
-    normalizer = vxFactorNormalizer(factor_data)
-    normalizer.standardize(["vxFactor001"])
-    neutralize_factors = factor_data.select(["trade_date", "symbol", "amount"])
-    normalizer.neutralization(["vxFactor001"], neutralize_factors)
-    print(normalizer._factors)
+"""因子标准化"""
+
+import polars as pl
+from tqdm import tqdm
+from typing import List, Any
+from scipy.stats import linregress
+from concurrent.futures import ThreadPoolExecutor as Executor
+
+
+class vxFactorNormalizer:
+    def __init__(self, factors: pl.DataFrame):
+        self._factors = factors.drop_nulls()
+
+    def fix_nan(
+        self,
+        factor_names: List[str] = None,
+        method: str = "drop",
+        fill_value: Any = None,
+    ):
+        """修复缺失值
+
+        Arguments:
+            factor_names {List[str]} -- 因子名称
+
+        Keyword Arguments:
+            method {str} -- 修复方法：drop / fill_mad / fill_mean / fill_forward (default: {"drop"})
+
+        """
+        pass
+
+    def standardize(
+        self, factor_names: List[str] = None, n: float = 3, method: str = "mad"
+    ) -> "vxFactorNormalizer":
+        """去极值以及标准化
+
+        Keyword Arguments:
+            factor_names {List[str]} -- 因子名称 (default: {None})
+            n {float} -- 倍数 (default: {3})
+            method {str} -- 去极值的方法 (mad or winsorize_std) (default: {"MAD"})
+
+        Raises:
+            ValueError: 不支持的去极值方法
+
+        """
+        if not factor_names:
+            factor_names = self._factors.columns
+
+        if method == "mad":
+
+            def filter_extreme(factor_col) -> pl.Series:
+                median = factor_col.median()
+                new_median = (factor_col - median).abs().median()
+
+                return factor_col.clip(
+                    factor_col.median() - n * new_median,
+                    factor_col.median() + n * new_median,
+                )
+
+        elif method == "winsorize_std":
+
+            def filter_extreme(factor_cal) -> pl.Expr:
+                return factor_cal.clip(
+                    factor_cal.mean() - n * factor_cal.std(),
+                    factor_cal.mean() + n * factor_cal.std(),
+                ).over("trade_date")
+
+        else:
+            raise ValueError(f"filter extreme method: {method} 暂不支持")
+
+        print("=" * 60)
+        self._factors = self._factors.with_columns(
+            pl.col(
+                [
+                    factor_name
+                    for factor_name in factor_names
+                    if factor_name not in ["trade_date", "symbol", "mask"]
+                ]
+            )
+            .apply(filter_extreme)
+            .over("trade_date")
+        )
+        self._factors = self._factors.with_columns(
+            [
+                (pl.col(factor_name) - pl.col(factor_name).mean())
+                / pl.col(factor_name).std()
+                for factor_name in factor_names
+                if factor_name not in ["trade_date", "symbol", "mask"]
+            ]
+        )
+
+        return self
+
+    def neutralization(
+        self, factor_names: List[str], neutralize_factors: pl.DataFrame
+    ) -> "vxFactorNormalizer":
+        x = neutralize_factors.select(
+            [
+                pl.col("trade_date", "symbol"),
+                pl.concat_list(pl.exclude(["trade_date", "symbol"])).alias("x"),
+            ]
+        )
+        factor_datas = self._factors.join(x, on=["trade_date", "symbol"], how="left")
+        executor = Executor()
+        import numpy as np
+
+        with tqdm(total=len(factor_datas["trade_date"].unique())) as pbar:
+
+            def _neutralize(group_df: pl.DataFrame) -> pl.DataFrame:
+                x = group_df["x"]
+                y = group_df["vxFactor001"]
+                print(x, y)
+                print(linregress(x, y))
+
+                # print(group_df)
+                # print(x)
+
+                for name in factor_names:
+                    # resi = linregress(x, group_df[name])
+                    # print(resi)
+                    print(name)
+                # pbar.update(1)
+                # return pl.DataFrame(
+                #    dict(
+                #        executor.map(
+                #            lambda name: (
+                #                name,
+                #                linregress(x, group_df[name].to_numpy())[-1],
+                #            ),
+                #            factor_names,
+                #        )
+                #    )
+                # ).vstack(group_df.select(["trade_date", "symbol"]), in_place=False)
+
+            factor_datas.groupby("trade_date").apply(_neutralize)
+
+
+if __name__ == "__main__":
+    factor_data = pl.read_parquet("./dist/factor.parquet")
+    print(factor_data.fill_null(strategy="backward"))
+    normalizer = vxFactorNormalizer(factor_data)
+    normalizer.standardize(["vxFactor001"])
+    neutralize_factors = factor_data.select(["trade_date", "symbol", "amount"])
+    normalizer.neutralization(["vxFactor001"], neutralize_factors)
+    print(normalizer._factors)
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/contants.py` & `vxquant-2023.4.1/src/vxquant/model/contants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-""" 各类常量定义 """
-
-from enum import Enum
-
-
-class TradeTime(Enum):
-    """交易时段"""
-
-    DayBegin = "09:00:00"
-    BeforeTrade = "09:15:00"
-    OnTrade = "09:30:01"
-    OnHans = "10:00:00"
-    BeforeClose = "14:45:00"
-    OnClose = "14:55:00"
-    AfterClose = "15:30:00"
-    DayEnd = "16:00:00"
-
-
-class MarketSignal(Enum):
-    """市场信号"""
-
-    Bull = 1
-    Monkey = 0
-    Bear = -1
-    Undefined = 99
-
-
-class BarAdjustType(Enum):
-    """复权形式"""
-
-    NotAdj = 0  # 不复权
-    PrevAdj = 1  # 前复权
-    PostAdj = 2  # 后复权
-
-
-class SecType(Enum):
-    """标的类别"""
-
-    CASH = 0  # 现金
-    STOCK = 1  # 股票
-    FUND = 2  # 基金
-    INDEX = 3  # 指数
-    FUTURE = 4  # 期货
-    OPTION = 5  # 期权
-    CREDIT = 6  # 信用交易
-    BOND = 7  # 债券
-    BOND_CONVERTIBLE = 8  # 可转债
-    REPO = 9  # 回购
-    CONFUTURE = 10  # 虚拟合约
-    ETFLOF = 11  # ETF-LOF
-    OTHER = 99  # 其他
-
-
-class SecStatus(Enum):
-    """标的状态"""
-
-    NORMAL = 1  # -正常
-    ST = 2  # -ST 股票,
-    STAR_ST = 3  # -*ST 股票,
-    TRANSFER = 4  # -股份转让,
-    REARRANGEMENT = 5  # -处于退市整理期的证券,
-    LOF = 6  # - 上市开放基金LOF,
-    ETF = 7  # - 交易型开放式指数基金(ETF),
-    OFUND_TRADE = 8  # - 非交易型开放式基金(暂不交易, 仅揭示基金净值及开放申购赎回业务),
-    OFUND = 9  # - 仅提供净值揭示服务的开放式基金,
-    SEC10 = 10  # - 仅在协议交易平台挂牌交易的证券,
-    SEC11 = 11  # - 仅在固定收益平台挂牌交易的证券,
-    SEC12 = 12  # - 风险警示产品,
-    SEC13 = 13  # - 退市整理产品,
-    OTHER = 99  # - 其它
-
-
-class Exchange(Enum):
-    """交易所代码
-    上交所: SHSE
-    深交所: SZSE
-    中金所: CFFEX
-    上期所: SHFE
-    大商所: DCE
-    郑商所: CZCE
-    上海国际能源交易中心: INE
-    """
-
-    SHSE = "SHSE"
-    SZSE = "SZSE"
-    CFFEX = "CFFEX"
-    SHFE = "SHFE"
-    DCE = "DCE"
-    CZCE = "CZCE"
-    INE = "INE"
-    OTHER = "OTHER"
-
-
-class AccountType(Enum):
-    """账户类型"""
-
-    Normal = 0
-    Credit = 1
-    Unknown = 99
-
-
-class OrderStatus(Enum):
-    """委托状态"""
-
-    Unknown = 0
-    New = 1
-    PartiallyFilled = 2
-    Filled = 3
-    Canceled = 5
-    PendingCancel = 6
-    Rejected = 8
-    Suspended = 9
-    PendingNew = 10
-    Expired = 12
-
-
-class OrderDirection(Enum):
-    """委托方向"""
-
-    Unknown = 0
-    Buy = 1
-    Sell = 2
-
-
-class OrderOffset(Enum):
-    """委托开平仓类型"""
-
-    Unknown = 0
-    Open = 1  # 开仓
-    Close = 2  # 平仓, 具体语义取决于对应的交易所
-    CloseToday = 3  # 平今仓
-    CloseYesterday = 4  # 平昨仓
-
-
-class OrderType(Enum):
-    """委托类型"""
-
-    Unknown = 0
-    Limit = 1
-    Market = 2
-    Stop = 3
-    Automated = 4
-    T0TrailingStop = 5
-
-
-class OrderDuration(Enum):
-    """委托时间属性，仅实盘有效"""
-
-    Unknown = 0
-    FAK = 1  # 即时成交剩余撤销(fill and kill)
-    FOK = 2  # 即时全额成交或撤销(fill or kill)
-    GFD = 3  # 当日有效(good for day)
-    GFS = 4  # 本节有效(good for section)
-    GTD = 5  # 指定日期前有效(goodltilldate)
-    GTC = 6  # 撤销前有效(goodtillcancel)
-    GFA = 7  # 集合竞价前有效(good for auction)
-    AHT = 8  # 盘后定价交易(after hour trading)
-
-
-class OrderQualifier(Enum):
-    """委托业务类型"""
-
-    Unknown = 0
-    BOC = 1  # 对方最优价格(best of counterparty)
-    BOP = 2  # 己方最优价格(best of party)
-    B5TC = 3  # 最优五档剩余撤销(best 5 then cancel)
-    B5TL = 4  # 最优五档剩余转限价(best 5 then limit)
-
-
-class TradeStatus(Enum):
-    """成交回报类型"""
-
-    Unknown = 0
-    New = 1  # 已报
-    Canceled = 5  # 已撤销
-    PendingCancel = 6  # 待撤销
-    Rejected = 8  # 已拒绝
-    Suspended = 9  # 挂起
-    PendingNew = 10  # 待报
-    Expired = 12  # 过期
-    Trade = 15  # 成交   (有效)
-    OrderStatus = 18  # 委托状态
-    CancelRejected = 19  # 撤单被拒绝  (有效)
-    OrderFinalized = 101  # 委托已完成
-    UnknownOrder = 102  # 未知委托
-    BrokerOption = 103  # 柜台设置
-    AlreadyInPendingCancel = 104  # 委托撤销中
-
-
-class PositionEffect(Enum):
-    """持仓头寸开平仓类型"""
-
-    Unknown = 0
-    Open = 1  # 开仓
-    Close = 2  # 平仓, 具体语义取决于对应的交易所
-    CloseToday = 3  # 平今仓
-    CloseYesterday = 4  # 平昨仓
-
-
-class PositionSide(Enum):
-    """持仓方向"""
-
-    Unknown = 0
-    Long = 1  # 多方向
-    Short = 2  # 空方向
-
-
-class OrderRejectReason(Enum):
-    """订单拒绝原因"""
-
-    Unknown = 0  # 未知原因
-    RiskRuleCheckFailed = 1  # 不符合风控规则
-    NoEnoughCash = 2  # 资金不足
-    NoEnoughPosition = 3  # 仓位不足
-    IllegalAccountId = 4  # 非法账户ID
-    IllegalStrategyId = 5  # 非法策略ID
-    IllegalSymbol = 6  # 非法交易标的
-    IllegalVolume = 7  # 非法委托量
-    IllegalPrice = 8  # 非法委托价
-    AccountDisabled = 10  # 交易账号被禁止交易
-    AccountDisconnected = 11  # 交易账号未连接
-    AccountLoggedout = 12  # 交易账号未登录
-    NotInTradingSession = 13  # 非交易时段
-    OrderTypeNotSupported = 14  # 委托类型不支持
-    Throttle = 15  # 流控限制
-    IllegalOrder = 103  # 交易委托不支持
-    OrderFinalized = 101  # 委托已经完成
-    UnknownOrder = 102  # 未知委托
-    AlreadyInPendingCancel = 104  # 已经在撤单中
-
-
-class CancelOrderRejectReason(Enum):
-    """取消订单拒绝原因"""
-
-    OrderFinalized = 101  # 委托已完成
-    UnknownOrder = 102  # 未知委托
-    BrokerOption = 103  # 柜台设置
-    AlreadyInPendingCancel = 104  # 委托撤销中
-
-
-class CashPositionChangeReason(Enum):
-    """仓位变更原因"""
-
-    Unknown = 0
-    Trade = 1  # 交易
-    Inout = 2  # 出入金 / 出入持仓
-
-
-class AccountStatus(Enum):
-    """交易账户状态"""
-
-    UNKNOWN = 0  # 未知
-    CONNECTING = 1  # 连接中
-    CONNECTED = 2  # 已连接
-    LOGGEDIN = 3  # 已登录
-    DISCONNECTING = 4  # 断开中
-    DISCONNECTED = 5  # 已断开
-    ERROR = 6  # 错误
-
-
-class PositionSrc(Enum):
-    """头寸来源(仅适用融券融券)"""
-
-    Unknown = 0
-    L1 = 1  # 普通池
-    L2 = 2  # 专项池
-
-
-class AlgoOrderStatus(Enum):
-    """组合委托状态"""
-
-    Unknown = 99  # 未知
-    New = 0  # 新增
-    Operating = 1  # 运行中
-    Completed = 2  # 已完成
-    Canceled = 3  # 已撤销
-    Stopped = 4  # 已暂停
-    Expired = 5  # 已过期
-
-
-class AlgoOrderType(Enum):
-    """算法委托类型"""
-
-    Unknown = 0  # 未知
-    Rebalance = 1  # 组合
-    AssetGrids = 3  # 市值网格
-    T0Bot = 4  # T+0机器人
+""" 各类常量定义 """
+
+from enum import Enum
+
+
+class TradeTime(Enum):
+    """交易时段"""
+
+    DayBegin = "09:00:00"
+    BeforeTrade = "09:15:00"
+    OnTrade = "09:30:01"
+    OnHans = "10:00:00"
+    BeforeClose = "14:45:00"
+    OnClose = "14:55:00"
+    AfterClose = "15:30:00"
+    DayEnd = "16:00:00"
+
+
+class MarketSignal(Enum):
+    """市场信号"""
+
+    Bull = 1
+    Monkey = 0
+    Bear = -1
+    Undefined = 99
+
+
+class BarAdjustType(Enum):
+    """复权形式"""
+
+    NotAdj = 0  # 不复权
+    PrevAdj = 1  # 前复权
+    PostAdj = 2  # 后复权
+
+
+class SecType(Enum):
+    """标的类别"""
+
+    CASH = 0  # 现金
+    STOCK = 1  # 股票
+    FUND = 2  # 基金
+    INDEX = 3  # 指数
+    FUTURE = 4  # 期货
+    OPTION = 5  # 期权
+    CREDIT = 6  # 信用交易
+    BOND = 7  # 债券
+    BOND_CONVERTIBLE = 8  # 可转债
+    REPO = 9  # 回购
+    CONFUTURE = 10  # 虚拟合约
+    ETFLOF = 11  # ETF-LOF
+    OTHER = 99  # 其他
+
+
+class SecStatus(Enum):
+    """标的状态"""
+
+    NORMAL = 1  # -正常
+    ST = 2  # -ST 股票,
+    STAR_ST = 3  # -*ST 股票,
+    TRANSFER = 4  # -股份转让,
+    REARRANGEMENT = 5  # -处于退市整理期的证券,
+    LOF = 6  # - 上市开放基金LOF,
+    ETF = 7  # - 交易型开放式指数基金(ETF),
+    OFUND_TRADE = 8  # - 非交易型开放式基金(暂不交易, 仅揭示基金净值及开放申购赎回业务),
+    OFUND = 9  # - 仅提供净值揭示服务的开放式基金,
+    SEC10 = 10  # - 仅在协议交易平台挂牌交易的证券,
+    SEC11 = 11  # - 仅在固定收益平台挂牌交易的证券,
+    SEC12 = 12  # - 风险警示产品,
+    SEC13 = 13  # - 退市整理产品,
+    OTHER = 99  # - 其它
+
+
+class Exchange(Enum):
+    """交易所代码
+    上交所: SHSE
+    深交所: SZSE
+    中金所: CFFEX
+    上期所: SHFE
+    大商所: DCE
+    郑商所: CZCE
+    上海国际能源交易中心: INE
+    """
+
+    SHSE = "SHSE"
+    SZSE = "SZSE"
+    CFFEX = "CFFEX"
+    SHFE = "SHFE"
+    DCE = "DCE"
+    CZCE = "CZCE"
+    INE = "INE"
+    OTHER = "OTHER"
+
+
+class AccountType(Enum):
+    """账户类型"""
+
+    Normal = 0
+    Credit = 1
+    Unknown = 99
+
+
+class OrderStatus(Enum):
+    """委托状态"""
+
+    Unknown = 0
+    New = 1
+    PartiallyFilled = 2
+    Filled = 3
+    Canceled = 5
+    PendingCancel = 6
+    Rejected = 8
+    Suspended = 9
+    PendingNew = 10
+    Expired = 12
+
+
+class OrderDirection(Enum):
+    """委托方向"""
+
+    Unknown = 0
+    Buy = 1
+    Sell = 2
+
+
+class OrderOffset(Enum):
+    """委托开平仓类型"""
+
+    Unknown = 0
+    Open = 1  # 开仓
+    Close = 2  # 平仓, 具体语义取决于对应的交易所
+    CloseToday = 3  # 平今仓
+    CloseYesterday = 4  # 平昨仓
+
+
+class OrderType(Enum):
+    """委托类型"""
+
+    Unknown = 0
+    Limit = 1
+    Market = 2
+    Stop = 3
+    Automated = 4
+    T0TrailingStop = 5
+
+
+class OrderDuration(Enum):
+    """委托时间属性，仅实盘有效"""
+
+    Unknown = 0
+    FAK = 1  # 即时成交剩余撤销(fill and kill)
+    FOK = 2  # 即时全额成交或撤销(fill or kill)
+    GFD = 3  # 当日有效(good for day)
+    GFS = 4  # 本节有效(good for section)
+    GTD = 5  # 指定日期前有效(goodltilldate)
+    GTC = 6  # 撤销前有效(goodtillcancel)
+    GFA = 7  # 集合竞价前有效(good for auction)
+    AHT = 8  # 盘后定价交易(after hour trading)
+
+
+class OrderQualifier(Enum):
+    """委托业务类型"""
+
+    Unknown = 0
+    BOC = 1  # 对方最优价格(best of counterparty)
+    BOP = 2  # 己方最优价格(best of party)
+    B5TC = 3  # 最优五档剩余撤销(best 5 then cancel)
+    B5TL = 4  # 最优五档剩余转限价(best 5 then limit)
+
+
+class TradeStatus(Enum):
+    """成交回报类型"""
+
+    Unknown = 0
+    New = 1  # 已报
+    Canceled = 5  # 已撤销
+    PendingCancel = 6  # 待撤销
+    Rejected = 8  # 已拒绝
+    Suspended = 9  # 挂起
+    PendingNew = 10  # 待报
+    Expired = 12  # 过期
+    Trade = 15  # 成交   (有效)
+    OrderStatus = 18  # 委托状态
+    CancelRejected = 19  # 撤单被拒绝  (有效)
+    OrderFinalized = 101  # 委托已完成
+    UnknownOrder = 102  # 未知委托
+    BrokerOption = 103  # 柜台设置
+    AlreadyInPendingCancel = 104  # 委托撤销中
+
+
+class PositionEffect(Enum):
+    """持仓头寸开平仓类型"""
+
+    Unknown = 0
+    Open = 1  # 开仓
+    Close = 2  # 平仓, 具体语义取决于对应的交易所
+    CloseToday = 3  # 平今仓
+    CloseYesterday = 4  # 平昨仓
+
+
+class PositionSide(Enum):
+    """持仓方向"""
+
+    Unknown = 0
+    Long = 1  # 多方向
+    Short = 2  # 空方向
+
+
+class OrderRejectReason(Enum):
+    """订单拒绝原因"""
+
+    Unknown = 0  # 未知原因
+    RiskRuleCheckFailed = 1  # 不符合风控规则
+    NoEnoughCash = 2  # 资金不足
+    NoEnoughPosition = 3  # 仓位不足
+    IllegalAccountId = 4  # 非法账户ID
+    IllegalStrategyId = 5  # 非法策略ID
+    IllegalSymbol = 6  # 非法交易标的
+    IllegalVolume = 7  # 非法委托量
+    IllegalPrice = 8  # 非法委托价
+    AccountDisabled = 10  # 交易账号被禁止交易
+    AccountDisconnected = 11  # 交易账号未连接
+    AccountLoggedout = 12  # 交易账号未登录
+    NotInTradingSession = 13  # 非交易时段
+    OrderTypeNotSupported = 14  # 委托类型不支持
+    Throttle = 15  # 流控限制
+    IllegalOrder = 103  # 交易委托不支持
+    OrderFinalized = 101  # 委托已经完成
+    UnknownOrder = 102  # 未知委托
+    AlreadyInPendingCancel = 104  # 已经在撤单中
+
+
+class CancelOrderRejectReason(Enum):
+    """取消订单拒绝原因"""
+
+    OrderFinalized = 101  # 委托已完成
+    UnknownOrder = 102  # 未知委托
+    BrokerOption = 103  # 柜台设置
+    AlreadyInPendingCancel = 104  # 委托撤销中
+
+
+class TransferDirection(Enum):
+    """仓位变更原因"""
+
+    Unknown = 0
+    In = 1  # 转入
+    Out = 2  # 转出
+
+
+class AccountStatus(Enum):
+    """交易账户状态"""
+
+    UNKNOWN = 0  # 未知
+    CONNECTING = 1  # 连接中
+    CONNECTED = 2  # 已连接
+    LOGGEDIN = 3  # 已登录
+    DISCONNECTING = 4  # 断开中
+    DISCONNECTED = 5  # 已断开
+    ERROR = 6  # 错误
+
+
+class PositionSrc(Enum):
+    """头寸来源(仅适用融券融券)"""
+
+    Unknown = 0
+    L1 = 1  # 普通池
+    L2 = 2  # 专项池
+
+
+class AlgoOrderStatus(Enum):
+    """组合委托状态"""
+
+    Unknown = 99  # 未知
+    New = 0  # 新增
+    Operating = 1  # 运行中
+    Completed = 2  # 已完成
+    Canceled = 3  # 已撤销
+    Stopped = 4  # 已暂停
+    Expired = 5  # 已过期
+
+
+class AlgoOrderType(Enum):
+    """算法委托类型"""
+
+    Unknown = 0  # 未知
+    Rebalance = 1  # 组合
+    AssetGrids = 3  # 市值网格
+    T0Bot = 4  # T+0机器人
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/exchange.py` & `vxquant-2023.4.1/src/vxquant/model/exchange.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,484 +1,467 @@
-# encoding=utf-8
-""" 委托及成交回报 数据模型 """
-
-from .nomalize import to_symbol
-from vxutils import vxtime
-from vxutils.dataclass import (
-    vxDataClass,
-    vxField,
-    vxPropertyField,
-    vxUUIDField,
-    vxEnumField,
-    vxFloatField,
-    vxIntField,
-    vxBoolField,
-    vxDatetimeField,
-)
-
-from vxquant.model.contants import (
-    TradeStatus,
-    OrderType,
-    OrderStatus,
-    OrderDirection,
-    OrderOffset,
-    PositionSide,
-    OrderRejectReason,
-    AlgoOrderStatus,
-    AlgoOrderType,
-    SecType,
-    SecStatus,
-    CashPositionChangeReason,
-)
-
-
-__all__ = [
-    "vxTrade",
-    "vxOrder",
-    "vxAlgoOrder",
-    "vxPosition",
-    "vxCashPosition",
-    "vxAccountInfo",
-    "vxPortfolioInfo",
-    "vxTick",
-    "vxBar",
-]
-
-ONEDAY = 60 * 60 * 24
-
-
-def _filled_vwap(vxorder: "vxOrder") -> float:
-    """成交均价"""
-    return round(vxorder.filled_amount / vxorder.filled_volume, 4)
-
-
-class vxTrade(vxDataClass):
-    """成交回报"""
-
-    # 账户id
-    account_id: str = vxUUIDField(False)
-    # 委托id
-    order_id: str = vxUUIDField(False)
-    # 交易所委托id
-    exchange_order_id: str = vxUUIDField(False)
-    # 成交id
-    trade_id: str = vxUUIDField()
-    # 证券代码
-    symbol: str = vxField("", to_symbol)
-    # 买卖方向
-    order_direction: OrderDirection = vxEnumField(OrderDirection.Unknown)
-    # 开平仓标志
-    order_offset: OrderOffset = vxEnumField(OrderOffset.Unknown)
-    # 成交价格
-    price: float = vxFloatField(0, ndigits=4, _min=0.0)
-    # 成交数量
-    volume: int = vxIntField(0, _min=0)
-    # 交易佣金
-    commission: float = vxFloatField(0, ndigits=2, _min=0.0)
-    # 成交状态
-    status: TradeStatus = vxEnumField(TradeStatus.Unknown)
-    # 拒绝代码
-    reject_code: OrderRejectReason = vxEnumField(OrderRejectReason.Unknown)
-    # 拒绝原因
-    reject_reason: str = vxField("", str)
-
-
-class vxOrder(vxDataClass):
-    """委托订单"""
-
-    # 账号id
-    account_id: str = vxUUIDField(False)
-    # 委托id
-    order_id: str = vxUUIDField()
-    # 算法委托id
-    algo_order_id: str = vxUUIDField(False)
-    # 交易所委托id
-    exchange_order_id: str = vxUUIDField(False)
-    # 冻结持仓id
-    frozen_position_id: str = vxUUIDField(False)
-    # 证券代码
-    symbol: str = vxField("", to_symbol)
-    # 买卖方向
-    order_direction: OrderDirection = vxEnumField(OrderDirection.Unknown)
-    # 开平仓标志
-    order_offset: OrderOffset = vxEnumField(OrderOffset.Unknown)
-    # 订单类型
-    order_type: OrderType = vxEnumField(OrderType.Unknown)
-    # 委托数量
-    volume: int = vxIntField(0, _min=0)
-    # 委托价格
-    price: float = vxFloatField(0.0, 4, _min=0)
-    # 成交数量
-    filled_volume: int = vxIntField(0, _min=0)
-    # 成交均价
-    filled_vwap: float = vxPropertyField(_filled_vwap, 0.0)
-    # 成交总额（含手续费）
-    filled_amount: float = vxFloatField(0.0, 2)
-    # 订单状态
-    status: OrderStatus = vxEnumField(OrderStatus.PendingNew)
-    # 订单超时时间
-    due_dt: float = vxDatetimeField(default_factory=lambda: vxtime.today("15:00:00"))
-    # 拒绝代码
-    reject_code: OrderRejectReason = vxEnumField(OrderRejectReason.Unknown)
-    # 拒绝原因
-    reject_reason: str = vxField(default_factory="", convertor_factory=str)
-
-
-class vxAlgoOrder(vxDataClass):
-    """算法订单"""
-
-    # 账户id
-    account_id: str = vxUUIDField(False)
-    # 算法委托id
-    algo_order_id: str = vxUUIDField()
-    # 算法委托类型
-    algo_order_type: AlgoOrderType = vxEnumField(AlgoOrderType.Unknown)
-    # 算法委托参数
-    params: dict = vxField(default_factory={})
-    # 算法委托状态
-    status: AlgoOrderStatus = vxEnumField(AlgoOrderStatus.Unknown)
-    # 订单超时时间
-    due_dt: float = vxDatetimeField(default_factory=lambda: vxtime.today("15:00:00"))
-
-
-def _available_volume(obj):
-    """可用仓位计算规则"""
-    return max(
-        (obj.volume - obj.frozen) if obj.allow_t0 else obj.volume_his - obj.frozen, 0
-    )
-
-
-class vxPosition(vxDataClass):
-    """股票持仓"""
-
-    # 组合ID
-    portfolio_id: str = vxUUIDField(False)
-    # 账户id
-    account_id: str = vxUUIDField(False)
-    # 仓位id
-    position_id: str = vxUUIDField()
-    # 证券类型
-    security_type: SecType = vxEnumField(SecType.OTHER)
-    # 证券代码
-    symbol: str = vxField("", to_symbol)
-    # 持仓方向
-    position_side: PositionSide = vxEnumField(PositionSide.Long)
-    # 今日持仓数量
-    volume_today: float = vxFloatField(0.0, 2, 0)
-    # 昨日持仓数量
-    volume_his: float = vxFloatField(0.0, 2, 0)
-    # 持仓数量 --- 自动计算字段，由 volume_today + volume_his 计算所得
-    volume: float = vxPropertyField(
-        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
-    )
-    # 冻结数量
-    frozen: float = vxFloatField(0.0, 2, 0)
-    # 可用数量  --- 自动计算字段，由 volume - frozen计算
-    available: int = vxPropertyField(_available_volume, default_factory=0)
-    # 持仓市值
-    marketvalue: float = vxPropertyField(
-        lambda obj: round(obj.volume * obj.lasttrade, 2), default_factory=0
-    )
-    # 持仓成本
-    cost: float = vxFloatField(0, 2)
-    # 浮动盈利
-    fnl: float = vxPropertyField(lambda obj: round(obj.marketvalue - obj.cost, 4), 0)
-    # 持仓成本均价
-    vwap: float = vxPropertyField(lambda obj: round(obj.cost / obj.volume, 4), 0)
-    # 最近成交价
-    lasttrade: float = vxFloatField(1.0, 4)
-    # 是否T0
-    allow_t0: bool = vxBoolField(False)
-
-
-class vxCashPosition(vxDataClass):
-    """现金持仓"""
-
-    # 组合ID
-    portfolio_id: str = vxUUIDField(False)
-    # 账户id
-    account_id: str = vxUUIDField(False)
-    # 仓位id
-    position_id: str = vxUUIDField()
-    # 证券类型
-    security_type: SecType = vxEnumField(SecType.CASH)
-    # 证券代码
-    symbol: str = vxField("CNY", to_symbol)
-    # 持仓方向
-    position_side: PositionSide = vxEnumField(PositionSide.Long)
-    # 今日持仓数量
-    volume_today: float = vxFloatField(0, 2, 0)
-    # 昨日持仓数量
-    volume_his: float = vxFloatField(0, 2, 0)
-    # 持仓数量
-    volume: float = vxPropertyField(
-        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
-    )
-    # 冻结数量
-    frozen: float = vxFloatField(0, 2, 0)
-    # 可用数量
-    available: float = vxPropertyField(_available_volume, default_factory=0)
-    # 持仓市值
-    marketvalue: float = vxPropertyField(
-        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
-    )
-    # 持仓成本
-    cost: float = vxPropertyField(
-        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
-    )
-    # 浮动盈利
-    fnl: float = vxPropertyField(lambda obj: 0.0, 0)
-    # 持仓成本均价
-    vwap: float = vxPropertyField(lambda obj: 1.0, 1.0)
-    # 最近成交价
-    lasttrade: float = vxPropertyField(lambda obj: 1.0, default_factory=1.0)
-    # 是否T0
-    allow_t0: bool = vxBoolField(True)
-
-
-class vxTransferInfo(vxDataClass):
-    # 转账流水id
-    transfer_id: str = vxUUIDField(True)
-    # 账号id
-    account_id: str = vxUUIDField(False)
-    # 仓位变动原因
-    cash_change_reason: CashPositionChangeReason = vxEnumField(
-        CashPositionChangeReason.Unknown
-    )
-    # 发生总金额
-    amount: float = vxFloatField(0.0, 2)
-
-
-class vxAccountInfo(vxDataClass):
-    """账户信息类型"""
-
-    # 组合ID
-    portfolio_id: str = vxUUIDField(False)
-    # 账户id
-    account_id: str = vxUUIDField()
-    # 账户币种
-    currency: str = vxField("CNY")
-    # 今日转入金额
-    deposit: float = vxFloatField(0, 2, 0)
-    # 今日转出金额
-    withdraw: float = vxFloatField(0, 2, 0)
-    # 总资产
-    asset: float = vxPropertyField(lambda obj: obj.balance + obj.marketvalue, 0)
-    # 净资产
-    nav: float = vxPropertyField(lambda obj: obj.asset - obj.debt)
-    # 总负债
-    debt: float = vxFloatField(0, 2)
-    # 资金余额
-    balance: float = vxFloatField(0, 2)
-    # 冻结金额
-    frozen: float = vxFloatField(0, 2)
-    # 可用金额
-    available: float = vxPropertyField(lambda obj: max(obj.balance - obj.frozen, 0), 0)
-    # 融资融券可用
-    margin_available: float = vxFloatField(0, 2)
-    # 总市值
-    marketvalue: float = vxFloatField(0, 2)
-    # 今日盈利
-    today_profit: float = vxPropertyField(
-        lambda obj: obj.nav - obj.nav_yd + obj.doposit - obj.withdraw, 0
-    )
-    # 浮动盈亏
-    fnl: float = vxFloatField(0, 2)
-    # 基金份额
-    fund_shares: float = vxFloatField(0, 4)
-    # 基金净值估算
-    fund_nav: float = vxPropertyField(
-        lambda obj: round(obj.nav / obj.fund_shares, 4), 1.0
-    )
-    # 昨日总资产
-    asset_yd: float = vxFloatField(0, 2)
-    # 昨日净资产
-    nav_yd: float = vxFloatField(0, 2)
-    # 昨日基金金额
-    fund_nav_yd: float = vxFloatField(1, 4)
-    # 最近结算日
-    settle_day: float = vxDatetimeField(
-        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY, formatter_string="%F"
-    )
-    # 下单channel
-    channel: str = vxField("simtrade")
-
-
-class vxPortfolioInfo(vxDataClass):
-    """FOF组合信息"""
-
-    # 组合id
-    portfolio_id: str = vxUUIDField(True)
-    # 组合名称
-    name: str = vxField("", str)
-    # 组合说明
-    description: str = vxField("", str)
-    # 业绩基准
-    benchmark: str = vxField("SHSE.000300", str)
-    # 基金净资产
-    nav: float = vxFloatField(0.0, 2)
-    # 昨日净资产
-    nav_yd: float = vxFloatField(0, 2)
-    # 基金净值
-    fund_nav: float = vxPropertyField(
-        lambda obj: round(obj.nav / obj.fund_shares, 4), 1.0
-    )
-    # 昨日基金净值
-    fund_nav_yd: float = vxPropertyField(
-        lambda obj: round(obj.nav / obj.fund_shares, 4), 1.0
-    )
-    # 基金份额
-    fund_shares: float = vxFloatField(1.0, 4)
-    # 昨日基金份额
-    fund_shares_yd: float = vxFloatField(1.0, 4)
-    # 最近结算日
-    settle_day: float = vxDatetimeField(
-        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY, formatter_string="%F"
-    )
-    # 管理人
-    manager: str = vxField("", str)
-
-
-class vxPortfolioUnderlying(vxDataClass):
-    """投资组合底层策略账户"""
-
-    # 投资组合id
-    portfolio_id: str = vxUUIDField(auto=False)
-    # 账户id
-    account_id: str = vxUUIDField(auto=False)
-    # 持有资产净值
-    nav: float = vxFloatField(0.0, 2)
-    # 购入成本
-    cost: float = vxFloatField(0.0, 2)
-    # 浮动盈亏
-    fnl: float = vxFloatField(0.0, 2)
-    # 持仓权重
-    weights: float = vxFloatField(0.0, 6)
-    # 基准资产净额
-    benchmark_nav: float = vxFloatField(0.0, 2)
-    # 持仓资产上限
-    uplimit_nav: float = vxFloatField(0.0, 2)
-    # 持仓资产下限
-    downlimit_nav: float = vxFloatField(0.0, 2)
-    # 最近结算日
-    settle_day: float = vxDatetimeField(
-        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY, formatter_string="%F"
-    )
-
-
-class vxTick(vxDataClass):
-    """行情模型"""
-
-    # 证券标的
-    symbol: str = vxField("", to_symbol)
-    # 开盘价
-    open: float = vxFloatField(0, 4)
-    # 最高价
-    high: float = vxFloatField(0, 4)
-    # 最低价
-    low: float = vxFloatField(0, 4)
-    # 最近成交价
-    lasttrade: float = vxFloatField(0, 4)
-    # 昨日收盘价
-    yclose: float = vxFloatField(0, 4)
-    # 成交量
-    volume: int = vxIntField(0, 0)
-    # 成交金额
-    amount: float = vxFloatField(0, 4)
-    # 换手率
-    turnoverratio: float = vxFloatField(0, 6, 0, 100)
-    # 卖1量
-    bid1_v: int = vxIntField(0, 0)
-    # 卖1价
-    bid1_p: float = vxFloatField(0, 4)
-    # 卖2量
-    bid2_v: int = vxIntField(0, 0)
-    # 卖2价
-    bid2_p: float = vxFloatField(0, 4)
-    # 卖3量
-    bid3_v: int = vxIntField(0, 0)
-    # 卖3价
-    bid3_p: float = vxFloatField(0, 4)
-    # 卖4量
-    bid4_v: int = vxIntField(0, 0)
-    # 卖4价
-    bid4_p: float = vxFloatField(0, 4)
-    # 卖5量
-    bid5_v: int = vxIntField(0, 0)
-    # 卖5价
-    bid5_p: float = vxFloatField(0, 4)
-    # 买1量
-    ask1_v: int = vxIntField(0, 0)
-    # 买1价
-    ask1_p: float = vxFloatField(0, 4)
-    # 买2量
-    ask2_v: int = vxIntField(0, 0)
-    # 买2价
-    ask2_p: float = vxFloatField(0, 4)
-    # 买3量
-    ask3_v: int = vxIntField(0, 0)
-    # 买3价
-    ask3_p: float = vxFloatField(0, 4)
-    # 买4量
-    ask4_v: int = vxIntField(0, 0)
-    # 买4价
-    ask4_p: float = vxFloatField(0, 4)
-    # 买5量
-    ask5_v: int = vxIntField(0, 0)
-    # 买5价
-    ask5_p: float = vxFloatField(0, 4)
-    # 持仓量
-    interest: int = vxIntField(0, 0)
-    # 停牌状态
-    status: SecStatus = vxEnumField(SecStatus.NORMAL)
-
-
-class vxBar(vxDataClass):
-    """K线模型"""
-
-    # 证券标的
-    symbol: str = vxField("", to_symbol)
-    # 周期
-    frequency: str = vxField("", str)
-    # 开盘价
-    open: float = vxFloatField(0, 4)
-    # 最高价
-    high: float = vxFloatField(0, 4)
-    # 最低价
-    low: float = vxFloatField(0, 4)
-    # 收盘价
-    close: float = vxFloatField(0, 4)
-    # 昨收盘价
-    yclose: float = vxFloatField(0, 4)
-    # 成交金额
-    amount: float = vxFloatField(0, 4)
-    # 成交量
-    volume: int = vxIntField(0, 0)
-    # 换手率
-    turnoverratio: float = vxFloatField(0, 6, 0, 100)
-    # 成交笔数
-    transactioncount: int = vxIntField(0, 0)
-    # 持仓量
-    interest: int = vxIntField(0, 0)
-    # 涨跌幅(%)
-    pct_change: float = vxFloatField(0, 6)
-    # 总市值
-    total_capital: float = vxFloatField(0, 2)
-    # 流通市值
-    flow_capital: float = vxFloatField(0, 2)
-    # 市盈率（TTM）
-    pe_ttm: float = vxFloatField(0, 2)
-    # 市净率
-    pb: float = vxFloatField(0, 2)
-    # 股息率
-    dy: float = vxFloatField(0, 2)
-    # 复权因子
-    factor: float = vxFloatField(0, 6)
-    # 交易状态
-    status: float = vxEnumField(SecStatus.NORMAL)
-
-
-class vxInstrument(vxDataClass):
-    # 证券代码
-    symbol: str = vxField("", str)
-    # 证券名称
-    name: str = vxField("", str)
+# encoding=utf-8
+""" 委托及成交回报 数据模型 """
+
+from .nomalize import to_symbol
+from vxutils import vxtime, combine_datetime
+from vxutils.dataclass import (
+    vxDataClass,
+    vxField,
+    vxPropertyField,
+    vxUUIDField,
+    vxEnumField,
+    vxFloatField,
+    vxIntField,
+    vxBoolField,
+    vxDatetimeField,
+)
+
+from vxquant.model.contants import (
+    TradeStatus,
+    OrderType,
+    OrderStatus,
+    OrderDirection,
+    OrderOffset,
+    PositionSide,
+    OrderRejectReason,
+    AlgoOrderStatus,
+    AlgoOrderType,
+    SecType,
+    SecStatus,
+    TransferDirection,
+)
+
+
+__all__ = [
+    "vxTrade",
+    "vxOrder",
+    "vxAlgoOrder",
+    "vxPosition",
+    "vxCashPosition",
+    "vxAccountInfo",
+    "vxPortfolioInfo",
+    "vxTick",
+    "vxBar",
+]
+
+ONEDAY = 60 * 60 * 24
+
+
+def _filled_vwap(vxorder: "vxOrder") -> float:
+    """成交均价"""
+    return round(vxorder.filled_amount / vxorder.filled_volume, 4)
+
+
+class vxTrade(vxDataClass):
+    """成交回报"""
+
+    # 账户id
+    account_id: str = vxUUIDField(False)
+    # 委托id
+    order_id: str = vxUUIDField(False)
+    # 交易所委托id
+    exchange_order_id: str = vxField(convertor_factory=str)
+    # 成交id
+    trade_id: str = vxUUIDField()
+    # 证券代码
+    symbol: str = vxField("", to_symbol)
+    # 买卖方向
+    order_direction: OrderDirection = vxEnumField(OrderDirection.Unknown)
+    # 开平仓标志
+    order_offset: OrderOffset = vxEnumField(OrderOffset.Unknown)
+    # 成交价格
+    price: float = vxFloatField(0, ndigits=4, _min=0.0)
+    # 成交数量
+    volume: int = vxIntField(0, _min=0)
+    # 交易佣金
+    commission: float = vxFloatField(0, ndigits=2, _min=0.0)
+    # 成交状态
+    status: TradeStatus = vxEnumField(TradeStatus.Unknown)
+    # 拒绝代码
+    reject_code: OrderRejectReason = vxEnumField(OrderRejectReason.Unknown)
+    # 拒绝原因
+    reject_reason: str = vxField("", str)
+
+
+class vxOrder(vxDataClass):
+    """委托订单"""
+
+    # 账号id
+    account_id: str = vxUUIDField(False)
+    # 委托id
+    order_id: str = vxUUIDField()
+    # 算法委托id
+    algo_order_id: str = vxUUIDField(False)
+    # 交易所委托id
+    exchange_order_id: str = vxField(convertor_factory=str)
+    # 冻结持仓id
+    frozen_position_id: str = vxUUIDField(False)
+    # 证券代码
+    symbol: str = vxField("", to_symbol)
+    # 买卖方向
+    order_direction: OrderDirection = vxEnumField(OrderDirection.Unknown)
+    # 开平仓标志
+    order_offset: OrderOffset = vxEnumField(OrderOffset.Unknown)
+    # 订单类型
+    order_type: OrderType = vxEnumField(OrderType.Unknown)
+    # 委托数量
+    volume: int = vxIntField(0, _min=0)
+    # 委托价格
+    price: float = vxFloatField(0.0, 4, _min=0)
+    # 成交数量
+    filled_volume: int = vxIntField(0, _min=0)
+    # 成交均价
+    filled_vwap: float = vxPropertyField(_filled_vwap, 0.0)
+    # 成交总额（含手续费）
+    filled_amount: float = vxFloatField(0.0, 2)
+    # 订单状态
+    status: OrderStatus = vxEnumField(OrderStatus.PendingNew)
+    # 订单超时时间
+    due_dt: float = vxDatetimeField(default_factory=lambda: vxtime.today("15:00:00"))
+    # 拒绝代码
+    reject_code: OrderRejectReason = vxEnumField(OrderRejectReason.Unknown)
+    # 拒绝原因
+    reject_reason: str = vxField(default_factory="", convertor_factory=str)
+
+
+class vxAlgoOrder(vxDataClass):
+    """算法订单"""
+
+    # 账户id
+    account_id: str = vxUUIDField(False)
+    # 算法委托id
+    algo_order_id: str = vxUUIDField()
+    # 算法委托类型
+    algo_order_type: AlgoOrderType = vxEnumField(AlgoOrderType.Unknown)
+    # 算法委托参数
+    params: dict = vxField(default_factory={})
+    # 算法委托状态
+    status: AlgoOrderStatus = vxEnumField(AlgoOrderStatus.Unknown)
+    # 订单超时时间
+    due_dt: float = vxDatetimeField(default_factory=lambda: vxtime.today("15:00:00"))
+
+
+def _available_volume(obj):
+    """可用仓位计算规则"""
+    return max(
+        (obj.volume - obj.frozen) if obj.allow_t0 else obj.volume_his - obj.frozen, 0
+    )
+
+
+class vxPosition(vxDataClass):
+    """股票持仓"""
+
+    # 组合ID
+    portfolio_id: str = vxUUIDField(False)
+    # 账户id
+    account_id: str = vxUUIDField(False)
+    # 仓位id
+    position_id: str = vxUUIDField()
+    # 证券类型
+    security_type: SecType = vxEnumField(SecType.OTHER)
+    # 证券代码
+    symbol: str = vxField("", to_symbol)
+    # 持仓方向
+    position_side: PositionSide = vxEnumField(PositionSide.Long)
+    # 今日持仓数量
+    volume_today: float = vxFloatField(0.0, 2, 0)
+    # 昨日持仓数量
+    volume_his: float = vxFloatField(0.0, 2, 0)
+    # 持仓数量 --- 自动计算字段，由 volume_today + volume_his 计算所得
+    volume: float = vxPropertyField(
+        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
+    )
+    # 冻结数量
+    frozen: float = vxFloatField(0.0, 2, 0)
+    # 可用数量  --- 自动计算字段，由 volume - frozen计算
+    available: int = vxPropertyField(_available_volume, default_factory=0)
+    # 持仓市值
+    marketvalue: float = vxPropertyField(
+        lambda obj: round(obj.volume * obj.lasttrade, 2), default_factory=0
+    )
+    # 持仓成本
+    cost: float = vxFloatField(0, 2)
+    # 浮动盈利
+    fnl: float = vxPropertyField(lambda obj: round(obj.marketvalue - obj.cost, 4), 0)
+    # 持仓成本均价
+    vwap: float = vxPropertyField(lambda obj: round(obj.cost / obj.volume, 4), 0)
+    # 最近成交价
+    lasttrade: float = vxFloatField(1.0, 4)
+    # 是否T0
+    allow_t0: bool = vxBoolField(False)
+    # 结算日
+    settle_date: float = vxDatetimeField(
+        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY,
+        formatter_string="%Y-%m-%d",
+        convertor_factory=lambda x: combine_datetime(x, "23:59:59"),
+    )
+
+
+class vxCashPosition(vxDataClass):
+    """现金持仓"""
+
+    # 组合ID
+    portfolio_id: str = vxUUIDField(False)
+    # 账户id
+    account_id: str = vxUUIDField(False)
+    # 仓位id
+    position_id: str = vxUUIDField(True)
+    # 证券类型
+    security_type: SecType = vxEnumField(SecType.CASH)
+    # 证券代码
+    symbol: str = vxField("CNY", to_symbol)
+    # 持仓方向
+    position_side: PositionSide = vxEnumField(PositionSide.Long)
+    # 今日持仓数量
+    volume_today: float = vxFloatField(0, 2, 0)
+    # 昨日持仓数量
+    volume_his: float = vxFloatField(0, 2, 0)
+    # 持仓数量
+    volume: float = vxPropertyField(
+        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
+    )
+    # 冻结数量
+    frozen: float = vxFloatField(0, 2, 0)
+    # 可用数量
+    available: float = vxPropertyField(_available_volume, default_factory=0)
+    # 持仓市值
+    marketvalue: float = vxPropertyField(
+        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
+    )
+    # 持仓成本
+    cost: float = vxPropertyField(
+        lambda obj: obj.volume_his + obj.volume_today, default_factory=0
+    )
+    # 浮动盈利
+    fnl: float = vxPropertyField(lambda obj: 0.0, 0)
+    # 持仓成本均价
+    vwap: float = vxPropertyField(lambda obj: 1.0, 1.0)
+    # 最近成交价
+    lasttrade: float = vxPropertyField(lambda obj: 1.0, default_factory=1.0)
+    # 是否T0
+    allow_t0: bool = vxBoolField(True)
+    # 结算日
+    settle_date: float = vxDatetimeField(
+        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY,
+        formatter_string="%Y-%m-%d",
+        convertor_factory=lambda x: combine_datetime(x, "23:59:59"),
+    )
+
+
+class vxTransferInfo(vxDataClass):
+    # 转账流水id
+    transfer_id: str = vxUUIDField(True)
+    # 账号id
+    account_id: str = vxUUIDField(False)
+    # 转账风向：转入 / 转出
+    transfer_direction: TransferDirection = vxEnumField(TransferDirection.Unknown)
+    # 发生总金额
+    amount: float = vxFloatField(0.0, 2)
+
+
+class vxAccountInfo(vxDataClass):
+    """账户信息类型"""
+
+    # 组合ID
+    portfolio_id: str = vxUUIDField(False)
+    # 账户id
+    account_id: str = vxUUIDField()
+    # 账户币种
+    currency: str = vxField("CNY")
+    # 今日转入金额
+    deposit: float = vxFloatField(0, 2, 0)
+    # 今日转出金额
+    withdraw: float = vxFloatField(0, 2, 0)
+    # 总资产
+    asset: float = vxPropertyField(lambda obj: obj.balance + obj.marketvalue, 0)
+    # 净资产
+    nav: float = vxPropertyField(lambda obj: obj.asset - obj.debt)
+    # 总负债
+    debt: float = vxFloatField(0, 2)
+    # 资金余额
+    balance: float = vxFloatField(0, 2)
+    # 冻结金额
+    frozen: float = vxFloatField(0, 2)
+    # 可用金额
+    available: float = vxPropertyField(lambda obj: max(obj.balance - obj.frozen, 0), 0)
+    # 融资融券可用
+    margin_available: float = vxFloatField(0, 2)
+    # 总市值
+    marketvalue: float = vxFloatField(0, 2)
+    # 今日盈利
+    today_profit: float = vxPropertyField(
+        lambda obj: round(obj.nav - obj.nav_yd - obj.deposit + obj.withdraw, 2), 0
+    )
+    # 浮动盈亏
+    fnl: float = vxFloatField(0, 2)
+    # 基金份额
+    fund_shares: float = vxFloatField(0, 4)
+    # 基金净值估算
+    fund_nav: float = vxPropertyField(
+        lambda obj: round(obj.nav / obj.fund_shares, 4), 1.0
+    )
+    # 昨日总资产
+    asset_yd: float = vxFloatField(0, 2)
+    # 昨日净资产
+    nav_yd: float = vxFloatField(0, 2)
+    # 昨日基金金额
+    fund_nav_yd: float = vxFloatField(1, 4)
+    # 结算日
+    settle_date: float = vxDatetimeField(
+        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY,
+        formatter_string="%Y-%m-%d",
+        convertor_factory=lambda x: combine_datetime(x, "23:59:59"),
+    )
+    # 下单channel
+    channel: str = vxField("simtrade")
+
+
+class vxPortfolioInfo(vxDataClass):
+    """FOF组合信息"""
+
+    # 组合id
+    portfolio_id: str = vxUUIDField(True)
+    # 组合名称
+    name: str = vxField("", str)
+    # 组合说明
+    description: str = vxField("", str)
+    # 业绩基准
+    benchmark: str = vxField("SHSE.000300", str)
+    # 基金净资产
+    nav: float = vxFloatField(0.0, 2)
+    # 昨日净资产
+    nav_yd: float = vxFloatField(0, 2)
+    # 基金净值
+    fund_nav: float = vxPropertyField(
+        lambda obj: round(obj.nav / obj.fund_shares, 4), 1.0
+    )
+    # 昨日基金净值
+    fund_nav_yd: float = vxFloatField(1.0, 4)
+    # 基金份额
+    fund_shares: float = vxFloatField(1.0, 4)
+    # 结算日
+    settle_date: float = vxDatetimeField(
+        default_factory=lambda: vxtime.today("23:59:59") - ONEDAY,
+        formatter_string="%Y-%m-%d",
+        convertor_factory=lambda x: combine_datetime(x, "23:59:59"),
+    )
+    # 管理人
+    manager: str = vxField("", str)
+
+
+class vxTick(vxDataClass):
+    """行情模型"""
+
+    # 证券标的
+    symbol: str = vxField("", to_symbol)
+    # 开盘价
+    open: float = vxFloatField(0, 4)
+    # 最高价
+    high: float = vxFloatField(0, 4)
+    # 最低价
+    low: float = vxFloatField(0, 4)
+    # 最近成交价
+    lasttrade: float = vxFloatField(0, 4)
+    # 昨日收盘价
+    yclose: float = vxFloatField(0, 4)
+    # 成交量
+    volume: int = vxIntField(0, 0)
+    # 成交金额
+    amount: float = vxFloatField(0, 4)
+    # 换手率
+    turnoverratio: float = vxFloatField(0, 6, 0, 100)
+    # 卖1量
+    bid1_v: int = vxIntField(0, 0)
+    # 卖1价
+    bid1_p: float = vxFloatField(0, 4)
+    # 卖2量
+    bid2_v: int = vxIntField(0, 0)
+    # 卖2价
+    bid2_p: float = vxFloatField(0, 4)
+    # 卖3量
+    bid3_v: int = vxIntField(0, 0)
+    # 卖3价
+    bid3_p: float = vxFloatField(0, 4)
+    # 卖4量
+    bid4_v: int = vxIntField(0, 0)
+    # 卖4价
+    bid4_p: float = vxFloatField(0, 4)
+    # 卖5量
+    bid5_v: int = vxIntField(0, 0)
+    # 卖5价
+    bid5_p: float = vxFloatField(0, 4)
+    # 买1量
+    ask1_v: int = vxIntField(0, 0)
+    # 买1价
+    ask1_p: float = vxFloatField(0, 4)
+    # 买2量
+    ask2_v: int = vxIntField(0, 0)
+    # 买2价
+    ask2_p: float = vxFloatField(0, 4)
+    # 买3量
+    ask3_v: int = vxIntField(0, 0)
+    # 买3价
+    ask3_p: float = vxFloatField(0, 4)
+    # 买4量
+    ask4_v: int = vxIntField(0, 0)
+    # 买4价
+    ask4_p: float = vxFloatField(0, 4)
+    # 买5量
+    ask5_v: int = vxIntField(0, 0)
+    # 买5价
+    ask5_p: float = vxFloatField(0, 4)
+    # 持仓量
+    interest: int = vxIntField(0, 0)
+    # 停牌状态
+    status: SecStatus = vxEnumField(SecStatus.NORMAL)
+
+
+class vxBar(vxDataClass):
+    """K线模型"""
+
+    # 证券标的
+    symbol: str = vxField("", to_symbol)
+    # 周期
+    frequency: str = vxField("", str)
+    # 开盘价
+    open: float = vxFloatField(0, 4)
+    # 最高价
+    high: float = vxFloatField(0, 4)
+    # 最低价
+    low: float = vxFloatField(0, 4)
+    # 收盘价
+    close: float = vxFloatField(0, 4)
+    # 昨收盘价
+    yclose: float = vxFloatField(0, 4)
+    # 成交金额
+    amount: float = vxFloatField(0, 4)
+    # 成交量
+    volume: int = vxIntField(0, 0)
+    # 换手率
+    turnoverratio: float = vxFloatField(0, 6, 0, 100)
+    # 成交笔数
+    transactioncount: int = vxIntField(0, 0)
+    # 持仓量
+    interest: int = vxIntField(0, 0)
+    # 涨跌幅(%)
+    pct_change: float = vxFloatField(0, 6)
+    # 总市值
+    total_capital: float = vxFloatField(0, 2)
+    # 流通市值
+    flow_capital: float = vxFloatField(0, 2)
+    # 市盈率（TTM）
+    pe_ttm: float = vxFloatField(0, 2)
+    # 市净率
+    pb: float = vxFloatField(0, 2)
+    # 股息率
+    dy: float = vxFloatField(0, 2)
+    # 复权因子
+    factor: float = vxFloatField(0, 6)
+    # 交易状态
+    status: float = vxEnumField(SecStatus.NORMAL)
+
+
+class vxInstrument(vxDataClass):
+    # 证券代码
+    symbol: str = vxField("", str)
+    # 证券名称
+    name: str = vxField("", str)
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/nomalize.py` & `vxquant-2023.4.1/src/vxquant/model/nomalize.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import re
-from typing import Tuple, Callable, Union
-from functools import lru_cache
-
-
-def normalize_freq(freq: str) -> Tuple[int, str]:
-    """
-    Parse freq into a unified format
-
-    Parameters
-    ----------
-    freq : str
-        Raw freq, supported freq should match the re '^([0-9]*)(month|mon|week|w|day|d|minute|min)$'
-
-    Returns
-    -------
-    freq: Tuple[int, str]
-        Unified freq, including freq count and unified freq unit. The freq unit should be '[month|week|day|minute]'.
-            Example:
-
-            .. code-block::
-
-                print(freq_parse("day"))
-                (1, "day" )
-                print(freq_parse("2mon"))
-                (2, "month")
-                print(freq_parse("10w"))
-                (10, "week")
-
-    """
-    freq = freq.lower()
-    match_obj = re.match("^([0-9]*)(month|mon|week|w|day|d|minute|min)$", freq)
-    if match_obj is None:
-        raise ValueError(
-            "freq format is not supported, the freq should be like (n)month/mon,"
-            " (n)week/w, (n)day/d, (n)minute/min"
-        )
-    _count = int(match_obj[1]) if match_obj[1] else 1
-    _freq = match_obj[2]
-    _freq_format_dict = {
-        "month": "month",
-        "mon": "month",
-        "week": "week",
-        "w": "week",
-        "day": "day",
-        "d": "day",
-        "minute": "minute",
-        "min": "minute",
-    }
-    return _count, _freq_format_dict[_freq]
-
-
-def normalize_symbol(symbol: str):
-    # todo 用正则表达式进行进一步优化
-
-    match_obj = re.match(r"^[A-Za-z]{2,4}.?([0-9]{6,10})$", symbol)
-
-    if match_obj:
-        code = match_obj[1]
-    else:
-        match_obj = re.match(r"^([0-9]{6,10}).?[A-Za-z]{2,4}$", symbol)
-
-    if match_obj is None:
-        raise ValueError(f"{symbol} format is not support.")
-
-    code = match_obj[1]
-    exchange = (
-        symbol.replace("se", "").replace("SE", "").replace(".", "").replace(code, "")
-    )
-    if exchange.upper() in {"OF", "ETF", "LOF", ""}:
-        exchange = "SZSE" if code[0] in ["0", "1", "2", "3", "4"] else "SHSE"
-    else:
-        exchange = exchange if len(exchange) > 2 else f"{exchange}SE"
-
-    return (exchange.upper(), code)
-
-
-@lru_cache(200)
-def to_symbol(instrument: str):
-    if instrument.upper() in {"CNY", "CACH"}:
-        return "CNY"
-
-    match_obj = re.match(r"^(SHSE|SZSE).(\d{6})$", instrument)
-
-    if match_obj:
-        return instrument
-
-    exchange, code = normalize_symbol(instrument)
-    return f"{exchange}.{code}"
-
-
-if __name__ == "__main__":
-    print(to_symbol("SHSE.600000"))
-    print(to_symbol("SH600000"))
-    print(to_symbol("sh600000"))
-    print(to_symbol("600000.sh"))
-    print(to_symbol("600000.SHSE"))
-    print(to_symbol("600000sh"))
+import re
+from typing import Tuple, Callable, Union
+from functools import lru_cache
+
+
+def normalize_freq(freq: str) -> Tuple[int, str]:
+    """
+    Parse freq into a unified format
+
+    Parameters
+    ----------
+    freq : str
+        Raw freq, supported freq should match the re '^([0-9]*)(month|mon|week|w|day|d|minute|min)$'
+
+    Returns
+    -------
+    freq: Tuple[int, str]
+        Unified freq, including freq count and unified freq unit. The freq unit should be '[month|week|day|minute]'.
+            Example:
+
+            .. code-block::
+
+                print(freq_parse("day"))
+                (1, "day" )
+                print(freq_parse("2mon"))
+                (2, "month")
+                print(freq_parse("10w"))
+                (10, "week")
+
+    """
+    freq = freq.lower()
+    match_obj = re.match("^([0-9]*)(month|mon|week|w|day|d|minute|min)$", freq)
+    if match_obj is None:
+        raise ValueError(
+            "freq format is not supported, the freq should be like (n)month/mon,"
+            " (n)week/w, (n)day/d, (n)minute/min"
+        )
+    _count = int(match_obj[1]) if match_obj[1] else 1
+    _freq = match_obj[2]
+    _freq_format_dict = {
+        "month": "month",
+        "mon": "month",
+        "week": "week",
+        "w": "week",
+        "day": "day",
+        "d": "day",
+        "minute": "minute",
+        "min": "minute",
+    }
+    return _count, _freq_format_dict[_freq]
+
+
+def normalize_symbol(symbol: str):
+    # todo 用正则表达式进行进一步优化
+
+    match_obj = re.match(r"^[A-Za-z]{2,4}.?([0-9]{6,10})$", symbol)
+
+    if match_obj:
+        code = match_obj[1]
+    else:
+        match_obj = re.match(r"^([0-9]{6,10}).?[A-Za-z]{2,4}$", symbol)
+
+    if match_obj is None:
+        raise ValueError(f"{symbol} format is not support.")
+
+    code = match_obj[1]
+    exchange = (
+        symbol.replace("se", "").replace("SE", "").replace(".", "").replace(code, "")
+    )
+    if exchange.upper() in {"OF", "ETF", "LOF", ""}:
+        exchange = "SZSE" if code[0] in ["0", "1", "2", "3", "4"] else "SHSE"
+    else:
+        exchange = exchange if len(exchange) > 2 else f"{exchange}SE"
+
+    return (exchange.upper(), code)
+
+
+@lru_cache(200)
+def to_symbol(instrument: str):
+    if instrument.upper() in {"CNY", "CACH"}:
+        return "CNY"
+
+    match_obj = re.match(r"^(SHSE|SZSE).(\d{6})$", instrument)
+
+    if match_obj:
+        return instrument
+
+    exchange, code = normalize_symbol(instrument)
+    return f"{exchange}.{code}"
+
+
+if __name__ == "__main__":
+    print(to_symbol("SHSE.600000"))
+    print(to_symbol("SH600000"))
+    print(to_symbol("sh600000"))
+    print(to_symbol("600000.sh"))
+    print(to_symbol("600000.SHSE"))
+    print(to_symbol("600000sh"))
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/portfolio.py` & `vxquant-2023.4.1/src/vxquant/model/portfolio.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1482 +1,1484 @@
-"""组合相关数据模型"""
-
-
-import uuid
-import pymongo
-
-from typing import Optional, Union, Dict
-from multiprocessing import Lock
-
-from vxsched import vxZMQPublisher, vxZMQSubscriber
-from vxutils import vxtime, logger
-from vxutils.database import vxMongoDB
-from vxutils.convertors import to_timestring
-from vxquant.exceptions import (
-    NoEnoughCash,
-    NoEnoughPosition,
-    IllegalVolume,
-    IllegalPrice,
-    # * RiskRuleCheckFailed,
-    # * IllegalAccountId,
-    # * IllegalStrategyId,
-    # * IllegalSymbol,
-    # * AccountDisabled,
-    # * AccountDisconnected,
-    # * AccountLoggedout,
-    # * NotInTradingSession,
-    # * OrderTypeNotSupported,
-    # * Throttle,
-    # * IllegalOrder,
-    # * OrderFinalized,
-    # * UnknownOrder,
-    # * AlreadyInPendingCancel,
-)
-from vxquant.mdapi.hq import vxTdxHQ
-from vxquant.model.preset import vxMarketPreset
-from vxquant.model.contants import (
-    OrderOffset,
-    TradeStatus,
-    OrderType,
-    OrderStatus,
-    OrderDirection,
-    AccountType,
-)
-from vxquant.model.exchange import (
-    vxAccountInfo,
-    vxPosition,
-    vxOrder,
-    vxTrade,
-    vxCashPosition,
-    vxTick,
-)
-
-
-class vxAccountBase:
-    """证券账户基类"""
-
-    @property
-    def account_id(self):
-        """账户id"""
-        raise NotImplementedError
-
-    @property
-    def account_info(self):
-        """账户信息"""
-        raise NotImplementedError
-
-    def get_positions(self, symbol=None):
-        """获取持仓信息"""
-        raise NotImplementedError
-
-
-class vxStockAccount:
-    """股票账户"""
-
-    def __init__(
-        self,
-        account_id=None,
-        balance=100_0000,
-        account_type=AccountType.Normal,
-        portfolio_id=None,
-        publisher=None,
-    ):
-        self._account_type = account_type
-        self._account_info = vxAccountInfo(
-            account_id=account_id, portfolio_id=portfolio_id
-        )
-        self._positions = {}
-        self._algo_orders = {}
-        self._orders = {}
-        self._trades = {}
-        self._publisher = publisher
-
-        self._positions["CNY"] = vxCashPosition(
-            account_id=account_id,
-            symbol="CNY",
-            security_type="CASH",
-            allow_t0=True,
-            lasttrade=1.0,
-        )
-
-        self._lock = Lock()
-
-        self.deposit(balance)
-        self.on_settle()
-
-    def __str__(self):
-        return f"< {self.__class__.__name__}({id(self)}) :\n {self.account_info} >"
-
-    __repr__ = __str__
-
-    @property
-    def account_id(self):
-        """账户id"""
-        return self._account_info.account_id
-
-    @property
-    def account_info(self):
-        """账户信息"""
-        return self._account_info
-
-    def get_positions(
-        self, symbol: Optional[str] = None
-    ) -> Union[Dict, vxPosition, vxCashPosition]:
-        """获取持仓信息"""
-        if not symbol:
-            return self._positions
-
-        if symbol in self._positions:
-            return self._positions[symbol]
-
-        preset = vxMarketPreset(symbol)
-        return vxPosition(
-            account_id=self.account_id,
-            symbol=symbol,
-            security_type=preset.security_type,
-            allow_t0=preset.allow_t0,
-        )
-
-    def get_orders(
-        self,
-        order_id: Optional[str] = None,
-        algo_order_id: Optional[str] = None,
-        exchange_order_id: Optional[str] = None,
-    ) -> Dict[str, Optional[vxOrder]]:
-        """获取当日委托信息"""
-        if order_id:
-            return (
-                {order_id: self._orders[order_id]} if order_id in self._orders else {}
-            )
-
-        if algo_order_id:
-            return {
-                order_id: order
-                for order in self._orders.values()
-                if order.algo_order_id == algo_order_id
-            }
-
-        if exchange_order_id:
-            return {
-                order.order_id: order
-                for order in self._orders.values()
-                if order.exchange_order_id == exchange_order_id
-            }
-
-        return self._orders
-
-    def get_trades(
-        self, order_id: Optional[str] = None, trade_id: Optional[str] = None
-    ) -> dict:
-        """获取当日成交回报"""
-        if order_id:
-            return {
-                trade.trade_id: trade
-                for trade in self._trades.values()
-                if trade.order_id == order_id
-            }
-
-        if trade_id:
-            return (
-                {trade_id: self._trades[trade_id]} if trade_id in self._trades else {}
-            )
-
-        return self._trades
-
-    def deposit(self, money: float) -> None:
-        """转入金额"""
-        if money <= 0:
-            raise IllegalPrice(f"转入金额 {money} <= 0 错误.")
-
-        with self._lock:
-            self.account_info.deposit += money
-            self.account_info.fund_shares += money / self.account_info.fund_nav
-            self._positions["CNY"].volume_today += money
-            self._positions["CNY"].cost += money
-            self.update_account_info()
-
-    def withdraw(self, money: float) -> None:
-        """转出金额"""
-        if money <= 0:
-            raise IllegalPrice(f"转出金额 {money} <= 0 错误.")
-
-        cash = self._positions["CNY"]
-        if money > cash.available:
-            raise NoEnoughCash(f"转出金额{money} 大于可用金额 {cash.available}。 ")
-        with self._lock:
-            self.account_info.withdraw += money
-            self.account_info.fund_shares -= money / self.account_info.fund_nav
-            if money < cash.volume_his:
-                cash.volume_his -= money
-            else:
-                money -= cash.volume_his
-                cash.volume_his = 0
-                cash.volume_today -= money
-            cash.cost = cash.marketvalue
-            self.update_account_info()
-
-    def set_bechmark_marketvalue(
-        self,
-        symbol: str,
-        benchmark_marketvalue: float = -1,
-        uplimit: float = -1,
-        downlimit: float = -1,
-    ) -> None:
-        """设置持仓基准市值、持仓市值上限，持仓市值下限
-
-        Arguments:
-            symbol {str} -- 证券代码
-            benchmark_marketvalue {float} -- 持仓基准市值，若市值小于0，则不做持仓市值监控 (default: {-1})
-            uplimit {float} -- 持仓市值上限，市值突破上限时，减仓至基准市值。 若小于0，则不做上限管理  (default: {-1})
-            downlimit {float} -- 持仓市值下限，市值跌破下限时，加仓至基准市值。若小于0，则不做下限管理 (default: {-1})
-        """
-        position = self.get_positions(symbol)
-        position.benchmark_marketvalue = benchmark_marketvalue
-        position.uplimit_marketvalue = uplimit
-        position.downlimit_marketvalue = downlimit
-        self._positions[position.position_id] = position
-
-    def check_benchmark_marketvalue(self):
-        """检查目标市值是否突破"""
-
-    def submit_order(self, symbol: str, volume: float, price=0) -> vxOrder:
-        """提交订单
-        进行下单前的检查，并且冻结资金及股票，形成一个PendingNew状态的order 以便提交
-
-        Arguments:
-            symbol {str} -- 下单标的
-            volume {float} -- 下单数量
-            price {int} -- 交易价格，若交易价格为0，则适用市价单，否则采用限价单 (default: {0})
-
-        Returns:
-            vxOrder -- 委托订单
-        """
-        if volume == 0:
-            raise IllegalVolume("volume不能为0.")
-
-        with self._lock:
-            if volume > 0:
-                if not price:
-                    tick = self.current(symbol)
-                    amount = (tick.lasttrade * volume) * 1.003
-                else:
-                    amount = price * volume * 1.003
-
-                position = self.get_positions("CNY")
-                if position.available < amount:
-                    raise NoEnoughCash(
-                        f"Not enough cash({position.available}) < need({amount})"
-                    )
-            else:
-                position = self.get_positions(symbol)
-                if position.available < volume:
-                    raise NoEnoughPosition(
-                        f"Not enough volume {symbol} {position.available} < amount"
-                    )
-
-            vxorder = vxOrder(
-                account_id=self.account_id,
-                symbol=symbol,
-                order_direction=OrderDirection.Buy
-                if volume > 0
-                else OrderDirection.Sell,
-                order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
-                order_type=OrderType.Limit if price <= 0 else OrderType.Market,
-                volume=abs(volume),
-                price=price,
-                status=OrderStatus.PendingNew,
-            )
-            self._orders[vxorder.order_id] = vxorder
-            self.update_account_info()
-
-        if self._publisher:
-            logger.debug(f"通过 {self._publisher.channel_name} 下单: {vxorder}")
-            self._publisher("on_submit_broker_order", vxorder)
-
-        return vxorder
-
-    @property
-    def message(self) -> dict:
-        """账户消息"""
-        return {
-            "account_info": self.account_info,
-            "positions": self.get_positions(),
-            "orders": self.get_orders(),
-            "trades": self.get_trades(),
-        }
-
-    def update_account_info(self) -> None:
-        """更新账户信息"""
-
-        self._account_info.marketvalue = 0
-        self._account_info.fnl = 0
-
-        for position in self._positions.values():
-            position.frozen = 0
-            if position.symbol != "CNY":
-                self._account_info.marketvalue += position.marketvalue
-                self._account_info.fnl += position.fnl
-            else:
-                self._account_info.balance = position.marketvalue
-                position.cost = position.marketvalue
-
-        for order in self._orders.values():
-            if order.status not in [
-                OrderStatus.PendingNew,
-                OrderStatus.New,
-                OrderStatus.PartiallyFilled,
-            ]:
-                continue
-
-            if order.order_direction == OrderDirection.Buy:
-                need_amount = (order.volume - order.filled_volume) * order.price * 1.003
-                self._positions["CNY"].frozen += need_amount
-
-            else:
-                self._positions[order.symbol].frozen += (
-                    order.volume - order.filled_volume
-                )
-        self.account_info.frozen = self._positions["CNY"].frozen
-        logger.debug(f"更新后账户信息: {self.message}")
-
-    def on_tick(self, ticks: dict) -> None:
-        """更新交易价格"""
-        update_symbols = set(self._positions.keys()) | set(ticks.keys())
-        with self._lock:
-            for symbol in update_symbols.items():
-                self._positions[symbol].lasttrade = ticks[symbol].lasttrade
-                self._positions[symbol].updated_dt = ticks[symbol].created_dt
-            self.account_info.marketvalue = sum(
-                p.marketvalue for p in self._positions.values() if p.symbol != "CNY"
-            )
-
-    def on_order_status(self, agent_order: vxOrder) -> None:
-        """更新订单状态"""
-
-        if agent_order.order_id not in self._orders:
-            with self._lock:
-                self._orders[agent_order.order_id] = vxOrder(agent_order.message)
-                self.update_account_info()
-                return
-
-        vxorder = self._orders[agent_order.order_id]
-        if vxorder.status in (
-            OrderStatus.Canceled,
-            OrderStatus.Expired,
-            OrderStatus.Filled,
-            OrderStatus.Rejected,
-            OrderStatus.Suspended,
-        ):
-            logger.info(
-                f"已经完结的委托信息，收到更新委托: {agent_order.status} {agent_order.filled_volume}"
-            )
-            return
-
-        if vxorder.filled_volume > agent_order.filled_volume:
-            logger.info(
-                f"收到早前的委托订单更新信息.filled_volume: vxorder{vxorder.filled_volume} >"
-                f" agent_order:{agent_order.filled_volume}."
-            )
-            return
-
-        with self._lock:
-            vxorder.exchange_order_id = agent_order.exchange_order_id
-            vxorder.filled_volume = agent_order.filled_volume
-            vxorder.filled_amount = agent_order.filled_amount
-            vxorder.status = agent_order.status
-            vxorder.updated_dt = agent_order.updated_dt
-            self.update_account_info()
-
-    def _handler_open_position(
-        self,
-        position: Union[vxPosition, vxCashPosition],
-        volume: float,
-        filled_amount: float,
-    ):
-        """处理开仓仓位"""
-        position.volume_today += volume
-        position.cost += filled_amount
-        self._positions[position.symbol] = position
-
-    def _handler_close_position(
-        self,
-        position: Union[vxPosition, vxCashPosition],
-        volume: float,
-        filled_amount: float,
-    ):
-        """处理平仓仓位"""
-        deta = position.volume_his - volume
-        position.volume_his = max(deta, 0)
-        position.volume_today = (
-            position.volume_today if deta >= 0 else position.volume_today + deta
-        )
-        position.cost -= filled_amount
-        self._positions[position.symbol] = position
-
-    def on_execution_report(self, agent_trade: vxTrade) -> None:
-        """更新成交回报信息"""
-        if agent_trade.status != TradeStatus.Trade:
-            logger.warning(f"收到非成交回报信息。 {agent_trade}")
-            return
-
-        if agent_trade.trade_id in self._trades:
-            logger.warning(f"收到重复的委托订单信息 {agent_trade.trade_id} {agent_trade}")
-            return
-
-        with self._lock:
-            self._trades[agent_trade.trade_id] = vxTrade(agent_trade.message)
-
-            cash_position = self.get_positions("CNY")
-            symbol_position = self.get_positions(agent_trade.symbol)
-            symbol_position.lasttrade = agent_trade.price
-
-            if agent_trade.order_direction == OrderDirection.Buy:
-                filled_amount = (
-                    agent_trade.price * agent_trade.volume + agent_trade.commission
-                )
-                # 扣减现金仓位
-                self._handler_close_position(
-                    cash_position, filled_amount, filled_amount
-                )
-                self._handler_open_position(
-                    symbol_position, agent_trade.volume, filled_amount
-                )
-            else:
-                filled_amount = (
-                    agent_trade.price * agent_trade.volume - agent_trade.commission
-                )
-                # 扣减symbol 持仓
-                self._handler_close_position(
-                    symbol_position, agent_trade.volume, filled_amount
-                )
-                self._handler_open_position(cash_position, filled_amount, filled_amount)
-            cash_position.updated_dt = agent_trade.updated_dt
-            symbol_position.updated_dt = agent_trade.updated_dt
-
-            self._handle_order_status(agent_trade, filled_amount)
-            self.update_account_info()
-
-    def _handle_order_status(self, agent_trade: vxTrade, filled_amount: float) -> None:
-        vxorder = self.get_orders(agent_trade.order_id).get(agent_trade.order_id, None)
-
-        if vxorder is None:
-            logger.warning(f"未知订单{agent_trade.order_id}")
-            return
-
-        if vxorder.status in (
-            OrderStatus.Canceled,
-            OrderStatus.Expired,
-            OrderStatus.Rejected,
-            OrderStatus.Suspended,
-        ):
-            logger.warning(f"已终止订单{vxorder.order_id} 收到成交信息:{agent_trade}")
-            return
-
-        vxorder.filled_volume += agent_trade.volume
-        vxorder.filled_amount += filled_amount
-        vxorder.status = (
-            OrderStatus.PartiallyFilled
-            if vxorder.filled_volume < vxorder.volume
-            else OrderStatus.Filled
-        )
-        vxorder.updated_dt = max(agent_trade.updated_dt, vxorder.updated_dt)
-
-    def on_settle(self):
-        """日结函数"""
-        now = vxtime.now()
-        logger.debug(f"开始执行日结{to_timestring(now,'%Y-%m-%d')}")
-
-        expired_orders = []
-        with self._lock:
-            # 1. 去掉超时以及当天已完成订单
-            orders = self._orders
-            self._orders = {}
-            for order in orders.values():
-                if order.status in [
-                    OrderStatus.Canceled,
-                    OrderStatus.Expired,
-                    OrderStatus.Filled,
-                    OrderStatus.Rejected,
-                    OrderStatus.Suspended,
-                ]:
-                    continue
-
-                if order.due_dt >= now:
-                    expired_orders.append(order)
-
-                self._orders[order.order_id] = order
-
-            # 超时的成交信息去掉
-            self._trades = {
-                trade_id: trade
-                for trade_id, trade in self._trades.items()
-                if trade.order_id in self._orders
-            }
-            # position
-            positions = self._positions
-            self._positions = {}
-            for symbol, position in positions.items():
-                if position.volume == 0 and position.symbol != "CNY":
-                    continue
-                position.volume_his, position.volume_today = position.volume, 0
-                self._positions[symbol] = position
-
-            self.update_account_info()
-            self.account_info.deposit = 0
-            self.account_info.withdraw = 0
-            self.account_info.asset_yd = self.account_info.asset
-            self.account_info.fund_nav_yd = self.account_info.fund_nav
-            self.account_info.nav_yd = self.account_info.nav
-
-    def update(
-        self,
-        account_info: Optional[vxAccountInfo] = None,
-        positions: Dict[str, Union[vxCashPosition, vxPosition]] = None,
-        orders: Dict[str, vxOrder] = None,
-        trades: Dict[str, vxTrade] = None,
-    ) -> None:
-        """直接账户基本信息"""
-        with self._lock:
-            if account_info:
-                self._account_info = account_info
-
-            if positions:
-                self._positions = positions
-
-            if orders:
-                self._orders = orders
-
-            if trades:
-                self._trades = trades
-            self.update_account_info()
-
-    @classmethod
-    def load_account(
-        cls,
-        account_info: vxAccountInfo,
-        positions: Dict[str, Union[vxCashPosition, vxPosition]],
-        orders: Dict[str, vxOrder],
-        trades: Dict[str, vxTrade],
-    ) -> "vxStockAccount":
-        """加载账户信息"""
-        instance = cls.__new__(cls=cls)
-        instance.update(account_info, positions, orders, trades)
-        return instance
-
-
-class vxPortfolioManager:
-    """组合管理"""
-
-    def __init__(self, portfolio_id: str, dbwriter):
-        pass
-
-    def create_portfolio(self, balance: float = 10_000_000.00, account_ids=None):
-        """创建组合"""
-
-    def create_account(self, account_id, balance=1_000_000.00):
-        """创建账户"""
-
-
-class vxAccountsManager:
-    def __init__(self, db_uri, db_name, publisher=None, hqfetcher=None):
-        self._database = vxMongoDB(db_uri, db_name)
-        self._database.mapping("accounts", vxAccountInfo, ["account_id"])
-        self._database.mapping("positions", vxPosition, ["account_id", "symbol"])
-        self._database.mapping("orders", vxOrder, ["order_id"])
-        self._database.mapping("trades", vxTrade, ["trade_id"])
-        self._database.mapping("current", vxTick, ["symbol"])
-
-        self._publisher = publisher
-        self._hqfetcher = hqfetcher or vxTdxHQ()
-        cur = self._database.agent_mapping.find({})
-        self._agent_map = {item.account_id: item.channel_name for item in cur}
-
-    def create_account(
-        self,
-        account_id: str = None,
-        balance: float = 1_000_000,
-        portfolio_id: str = "",
-        channel_name: str = None,
-        if_exists: str = "skip",
-    ) -> str:
-        """创建账户
-
-        Keyword Arguments:
-            account_id {str} -- 账户id (default: {None})
-            balance {float} -- 初始余额 (default: {1_000_000})
-            portfolio_id {str} -- 组合id (default: {""})
-            channel_name {str} -- 下单通道，缺省为空 (default: {None})
-            if_exists {str} -- 若存在账户已存在(default: {"skip"})
-                                'delete' ---> 删除原来账户
-                                'skip' --->  跳过
-                                'raise' ---> raise 一个exception
-
-
-        Raises:
-            ValueError: 账户已存在时，且if_exists == 'raise' 则raise一个exception
-
-        Returns:
-            str -- _description_
-        """
-
-        channel_name = channel_name or "simtest"
-
-        if self._database.accounts.count_documents({"account_id": account_id}) > 0:
-            if if_exists == "skip":
-                return account_id
-            elif if_exists == "delete":
-                self._database.accounts.delete_many({"account_id": account_id})
-                self._database.positions.delete_many({"account_id": account_id})
-                self._database.orders.delete_many({"account_id": account_id})
-                self._database.trades.delete_many({"account_id": account_id})
-            elif if_exists == "raise":
-                raise ValueError(f"account_id({account_id}) 已存在。")
-
-        account_id = account_id or str(uuid.uuid4())
-        account_info = vxAccountInfo(
-            account_id=account_id,
-            portfolio_id=portfolio_id,
-            deposit=balance,
-            balance=balance,
-            fund_shares=balance,
-            fund_nav_yd=1.0,
-            settle_day=vxtime.today("00:00:00") - 60 * 60 * 24,
-        )
-
-        cash_position = vxCashPosition(
-            portfolio_id=portfolio_id,
-            account_id=account_id,
-            volume_today=balance,
-        )
-
-        with self._database.start_session() as session:
-            self._database.save("accounts", account_info, session=session)
-            self._database.save("positions", cash_position, session=session)
-            self._database.agent_mapping.update_one(
-                {"account_id": account_id},
-                {"$set": {"channel_name": channel_name}},
-                upsert=True,
-            )
-            self._agent_map[account_id] = channel_name
-        self._update_account_info([account_id])
-
-        return account_id
-
-    def deposit(self, account_id, money: float) -> None:
-        """转入金额"""
-
-        account_info = self._database.accounts.find_one(
-            {"account_id": account_id}, {"_id": 0}
-        )
-        if account_info is None:
-            raise ValueError(f"账户信息不存在: {account_id}")
-        account_info = vxAccountInfo(account_info)
-
-        cash_position = self._database.positions.find_one(
-            {"account_id": account_id, "symbol": "CNY"}, {"_id": 0}
-        )
-        cash_position = vxCashPosition(cash_position)
-        logger.info(f"{account_info.nav}, {money}")
-
-        account_info.fund_shares += money / account_info.fund_nav
-        account_info.deposit += money
-        account_info.balance += money
-        cash_position.volume_today += money
-        logger.info(f"{account_info.nav}, {money},{cash_position.marketvalue}")
-
-        with self._database.start_session() as session:
-            self._database.save("accounts", account_info, session=session)
-            self._database.save("positions", cash_position, session=session)
-
-            self._update_account_info([account_id], session=session)
-
-    def withdraw(self, account_id, money: float) -> None:
-        """转出金额"""
-        if money <= 0:
-            raise IllegalPrice(f"转出金额 {money} <= 0 错误.")
-
-        with self._database.start_session(causal_consistency=True) as session:
-            cash = self._database.query_one(
-                "positions",
-                {"account_id": account_id, "symbol": "CNY"},
-                session=session,
-            )
-            cash = vxCashPosition(cash)
-            if money > cash.available:
-                raise NoEnoughCash(f"转出金额{money} 大于可用金额 {cash.available}。 ")
-            account_info = self._database.query_one(
-                "accounts", {"account_id": account_id}, session=session
-            )
-
-            account_info.withdraw += money
-            account_info.fund_shares -= money / account_info.fund_nav
-            account_info.balance -= money
-
-            if money < cash.volume_his:
-                cash.volume_his -= money
-            else:
-                money -= cash.volume_his
-                cash.volume_his = 0
-                cash.volume_today -= money
-
-            self._database.save("accounts", account_info, session=session)
-            self._database.save("positions", cash, session=session)
-            self._update_account_info([account_id], session=session)
-
-    def _update_account_info(self, account_ids, session=None):
-        """重新计算账户值"""
-
-        positions = self._database.query(
-            "positions", {"account_id": {"$in": account_ids}}, session=session
-        )
-        account_infos = {}
-        update_positions = []
-        for position in positions:
-            if position.account_id not in account_infos:
-                account_infos[position.account_id] = {
-                    "balance": 0,
-                    "frozen": 0,
-                    "marketvalue": 0,
-                    "fnl": 0,
-                }
-            if position.symbol == "CNY":
-                cash = vxCashPosition(position)
-                account_infos[position.account_id]["balance"] = cash.marketvalue
-                account_infos[position.account_id]["frozen"] = cash.frozen
-                update_positions.append(cash)
-            else:
-                account_infos[position.account_id][
-                    "marketvalue"
-                ] += position.marketvalue
-                account_infos[position.account_id]["fnl"] += position.fnl
-                update_positions.append(position)
-
-        cur = self._database.query(
-            "accounts", {"account_id": {"$in": list(account_ids)}}, session=session
-        )
-
-        update_account_infos = []
-        for account_info in cur:
-            update_dict = account_infos.get(account_info.account_id, {})
-            account_info.update(**update_dict)
-            logger.debug(f"更新后account_info:{account_info}")
-            update_account_infos.append(account_info)
-
-        self._database.save_many("positions", update_positions, session=session)
-        self._database.save_many("accounts", update_account_infos, session=session)
-
-    def _update_frozens(self, account_ids, session=None):
-        """重新计算持仓冻结信息"""
-        modify_position_ids = self._database.orders.distinct(
-            "frozen_position_id", {"account_id": {"$in": account_ids}}, session=session
-        )
-        agg_position_frozens = self._database.orders.aggregate(
-            [
-                {
-                    "$match": {
-                        "frozen_position_id": {"$in": modify_position_ids},
-                        "status": {"$in": ["New", "PartiallyFilled", "PendingNew"]},
-                    }
-                },
-                {
-                    "$project": {
-                        "account_id": "$account_id",
-                        "order_id": "$order_id",
-                        "frozen_position_id": "$frozen_position_id",
-                        "order_direction": "$order_direction",
-                        "left_volume": {"$subtract": ["$volume", "$filled_volume"]},
-                        "price": "$price",
-                        "cost": {
-                            "$multiply": [
-                                {"$subtract": ["$volume", "$filled_volume"]},
-                                "$price",
-                            ]
-                        },
-                    }
-                },
-                {
-                    "$group": {
-                        "_id": {
-                            "account_id": "$account_id",
-                            "position_id": "$frozen_position_id",
-                            "order_direction": "$order_direction",
-                        },
-                        "left_volume": {"$sum": "$left_volume"},
-                        "cost": {"$sum": "$cost"},
-                    }
-                },
-            ],
-            session=session,
-        )
-        update_position_cmds = [
-            pymongo.UpdateMany(
-                {"position_id": {"$in": modify_position_ids}}, {"$set": {"frozen": 0.0}}
-            )
-        ]
-        update_account_cmds = []
-
-        for agg_position_frozen in agg_position_frozens:
-            position_id = agg_position_frozen["_id"]["position_id"]
-            order_direction = agg_position_frozen["_id"]["order_direction"]
-
-            if order_direction == "Buy":
-                update_cmd = pymongo.UpdateOne(
-                    {"position_id": position_id},
-                    {"$set": {"frozen": (agg_position_frozen["cost"] * 1.003)}},
-                )
-                update_account_cmd = pymongo.UpdateOne(
-                    {"accountt_id": agg_position_frozen["_id"]["account_id"]},
-                    {"$set": {"frozen": (agg_position_frozen["cost"] * 1.003)}},
-                )
-                update_account_cmds.append(update_account_cmd)
-                logger.info(f"更新SQL accounts: {update_account_cmd}")
-
-            else:
-                update_cmd = pymongo.UpdateOne(
-                    {"position_id": position_id},
-                    {"$set": {"frozen": (agg_position_frozen["left_volume"])}},
-                )
-
-            update_position_cmds.append(update_cmd)
-            logger.info(f"更新SQL positions: {update_cmd}")
-
-        self._database.positions.bulk_write(
-            update_position_cmds, ordered=True, session=session
-        )
-        if update_account_cmds:
-            self._database.accounts.bulk_write(
-                update_account_cmds,
-                ordered=True,
-            )
-            logger.warning(f"更新SQL accounts: {update_account_cmds}")
-        return modify_position_ids
-
-    def _update_order_filled_volumes(self, account_ids, session=None):
-        """重新计算委托订单成交信息"""
-        unfinished_order_ids = self._database.distinct(
-            "orders",
-            "order_id",
-            {
-                "status": {"$in": ["New", "PendingNew", "PartiallyFilled", "Unknown"]},
-                "account_id": {"$in": account_ids},
-            },
-            session=session,
-        )
-        logger.info(f"共有{len(unfinished_order_ids)}个未完成订单.")
-        agg_filled_volumes = self._database.trades.aggregate(
-            [
-                {"$match": {"order_id": {"$in": unfinished_order_ids}}},
-                {
-                    "$group": {
-                        "_id": {
-                            "order_id": "$order_id",
-                            "order_direction": "$order_direction",
-                        },
-                        "volume": {"$max": "$volume"},
-                        "filled_volume": {"$sum": "$volume"},
-                        "commission": {"$sum": "$commission"},
-                        "cost": {"$sum": {"$multiply": ["$price", "$volume"]}},
-                    }
-                },
-                {"$match": {"filled_volume": {"$gt": 0}}},
-            ],
-            session=session,
-        )
-
-        update_order_cmds = []
-        modify_order_ids = []
-        for agg_filled_volume in agg_filled_volumes:
-            order_id = agg_filled_volume["_id"]["order_id"]
-            order_direction = agg_filled_volume["_id"]["order_direction"]
-            filled_amount = (
-                (agg_filled_volume["cost"] + agg_filled_volume["cost"])
-                if order_direction == "Buy"
-                else (agg_filled_volume["cost"] - agg_filled_volume["cost"])
-            )
-            filled_vwap = filled_amount / agg_filled_volume["filled_volume"]
-            logger.info(
-                f"订单{order_id} {order_direction} filled_amount={filled_amount} filled_vwap={filled_vwap}."
-            )
-
-            update_order_cmd = pymongo.UpdateOne(
-                {"order_id": order_id},
-                {
-                    "$set": {
-                        "filled_volume": agg_filled_volume["filled_volume"],
-                        "filled_amount": filled_amount,
-                        "filled_vwap": filled_vwap,
-                        "status": "Filled"
-                        if agg_filled_volume["filled_volume"]
-                        >= agg_filled_volume["volume"]
-                        else "PartiallyFilled",
-                    }
-                },
-            )
-            update_order_cmds.append(update_order_cmd)
-            modify_order_ids.append(order_id)
-        if update_order_cmds:
-            self._database.accounts.bulk_write(update_order_cmds, session=session)
-        return modify_order_ids
-
-    def get_account(self, account_id: str, session=None) -> vxAccountInfo:
-        """获取账户信息
-
-        Arguments:
-            account_id {str} -- 账户id
-
-        Returns:
-            vxAccountInfo -- 账户信息
-        """
-        logger.info(f"account_id({account_id}) session: {session}")
-        item = self._database.accounts.find_one(
-            {"account_id": account_id}, session=session
-        )
-
-        return vxAccountInfo(item)
-
-    def get_positions(self, account_id: str, symbol: str = None) -> Dict:
-        """获取相应的持仓信息
-
-        Arguments:
-            account_id {str} -- account_id 账户id
-            symbol {str} -- 持仓信息 (default: {None})
-
-        Returns:
-            Dict -- Dict['account_id': vxAccountInfo]
-        """
-        filter_ = {"account_id": account_id}
-        if symbol:
-            filter_["symbol"] = symbol
-        cur = self._database.query("positions", filter_)
-        return {position.symbol: position for position in cur}
-
-    def get_orders(
-        self,
-        account_id: str,
-        order_id: str = None,
-        exchange_order_id: str = None,
-        is_unfinished=False,
-    ) -> Dict:
-        """获取成交订单信息
-
-        Arguments:
-            account_id {str} -- 账户id
-
-        Keyword Arguments:
-            order_id {str} -- 委托订单id (default: {None})
-            exchange_order_id {str} -- 交易所委托订单id (default: {None})
-            is_unfinished {bool} -- 是否未完成 (default: {False})
-
-        Returns:
-            Dict -- Dict['order_id': vxOrder]
-        """
-        filter_ = {"account_id": account_id}
-        if order_id:
-            filter_["order_id"] = order_id
-        if exchange_order_id:
-            filter_["exchange_order_id"] = exchange_order_id
-        if is_unfinished:
-            filter_["status"] = {"$in": ["New", "PendingNew", "PartiallyFilled"]}
-
-        cur = self._database.query("orders", filter_)
-        return {o.order_id: o for o in cur}
-
-    def get_trades(
-        self,
-        account_id: str,
-        order_id: str = None,
-        trade_id: str = None,
-        exchange_order_id: str = None,
-    ) -> Dict:
-        """获取成交信息
-
-        Arguments:
-            account_id {str} -- 账户id
-
-        Keyword Arguments:
-            order_id {str} -- 委托订单id (default: {None})
-            trade_id {str} -- 成交回报id (default: {None})
-            exchange_order_id {str} -- 交易所委托订单id (default: {None})
-
-        Returns:
-            Dict -- Dict['trade_id':vxTrade]
-        """
-        filter_ = {"account_id": account_id}
-        if order_id:
-            filter_["order_id"] = order_id
-
-        if trade_id:
-            filter_["trade_id"] = trade_id
-
-        if exchange_order_id:
-            filter_["exchange_order_id"] = exchange_order_id
-
-        cur = self._database.query("trades", filter_)
-        return {t.trade_id: t for t in cur}
-
-    def _update_ticks(self, *symbols) -> Dict:
-        """更新ticks数据
-
-        Returns:
-            Dict -- Dict['symbol':vxTick]
-        """
-        now = vxtime.now()
-        cached_symbols = self._database.distinct(
-            "current",
-            "symbol",
-            {"symbol": {"$in": symbols}, "created_dt": {"$gt": now - 3}},
-        )
-        missing_symbols = set(symbols) - set(cached_symbols)
-        if len(missing_symbols) > 0:
-            vxticks = self._hqfetcher(*missing_symbols)
-
-            self._database.save_many("current", vxticks.values())
-        cur = self._database.query("current", {"symbol": {"$in": symbols}})
-        return {vxtick.symbol: vxtick for vxtick in cur}
-
-    def order_volume(
-        self,
-        account_id: str,
-        symbol: str,
-        volume: int,
-        price: float = 0.0,
-        algo_order_id: str = "",
-    ) -> vxOrder:
-        """委托交易volume的symbol证券
-
-        Arguments:
-            account_id {str} -- 交易账号
-            symbol {str} -- 目标证券代码
-            volume {int} -- volume> 0时，表示买入，volume < 0时，表示卖出
-            price {float} -- price 为0 时，则表示市价单，price > 0 时，表示限价单 (default: {0.0})
-
-        Returns:
-            vxOrder -- 委托订单号
-        """
-        with self._database.start_session(
-            causal_consistency=True, lock=True
-        ) as session:
-            order = vxOrder(
-                account_id=account_id,
-                algo_order_id=algo_order_id,
-                symbol=symbol,
-                status="PendingNew",
-            )
-
-            if price < 0.0:
-                raise ValueError(f"委托价格({price})必须大于等于0.")
-            elif price == 0:
-                order.order_type = "Market"
-                tick = self._update_ticks(order.symbol)
-
-                order.price = (
-                    tick[order.symbol].bid1_p
-                    if volume < 0
-                    else tick[order.symbol].ask1_p
-                )
-            else:
-                order.order_type = "Limit"
-                order.price = price
-
-            if volume == 0:
-                raise ValueError("委托volume 不可以为0.")
-
-            elif volume > 0:
-                order.order_direction = "Buy"
-                order.order_offset = "Open"
-                order.volume = volume
-                frozen_position = self._database.query_one(
-                    "positions",
-                    {"account_id": account_id, "symbol": "CNY"},
-                    session=session,
-                )
-                frozen_position = vxCashPosition(frozen_position)
-                frozen_amount = order.volume * order.price * 1.003
-                if frozen_amount > frozen_position.available:
-                    raise NoEnoughCash(
-                        f"Buy {symbol} volume({order.volume}) on price({order.price})"
-                        f" frozen {frozen_amount} > {frozen_position.available}"
-                    )
-                order.frozen_position_id = frozen_position.position_id
-                frozen_position.frozen += frozen_amount
-            else:
-                order.order_direction = "Sell"
-                order.order_offset = "Close"
-                order.volume = abs(volume)
-                frozen_position = self._database.query_one(
-                    "positions",
-                    {"account_id": account_id, "symbol": symbol},
-                    session=session,
-                )
-                if not frozen_position or frozen_position.available < order.volume:
-                    raise NoEnoughPosition(
-                        f"Sell {symbol} volume({order.volume})"
-                        f" 可用持仓:({frozen_position.available if frozen_position else 0})."
-                    )
-                order.frozen_position_id = frozen_position.position_id
-                frozen_position.available += order.volume
-
-            self._database.save("orders", order, session=session)
-            self._database.save("positions", frozen_position, session=session)
-
-            self._update_frozens([account_id], session=session)
-            self._update_account_info([account_id], session=session)
-
-            channel = self._agent_map.get(account_id, "simtest")
-            self._publisher("on_submit_broker_order", data=order, channel=channel)
-            logger.warning(
-                f"account({account_id}) 通过channel({channel}) 发送"
-                f" on_submit_broker_order 委托订单: {order}"
-            )
-            return order
-
-    def order_cancel(self, *orders):
-        """取消委托订单"""
-
-        cancel_order_ids = [order.order_id for order in orders]
-
-        cur = self._database.query(
-            "orders",
-            {
-                "order_id": {"$in": cancel_order_ids},
-                "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
-                "exchange_order_id": {"$ne": ""},
-            },
-        )
-        for order in cur:
-            channel = self._agent_map.get(order.account_id, "simtest")
-            self._publisher("on_submit_broker_order_cancel", order, channel=channel)
-            logger.warning(
-                f"account({order.account_id})通过 {channel} 发送 on_submit_broker_cancel"
-                f" 取消委托订单: {order}"
-            )
-        return
-
-    def on_order_status(self, context, event) -> None:
-        """订单状态更新"""
-        with self._database.start_session(causal_consistency=True) as session:
-            # 1. 更新order 状态信息
-            broker_order = event.data
-            if broker_order.status not in [
-                OrderStatus.PartiallyFilled,
-                OrderStatus.New,
-                OrderStatus.PendingNew,
-            ]:
-                # 已终结订单，根据返回信息更新数据库订单
-                self._database.orders.update_one(
-                    {
-                        "order_id": broker_order.order_id,
-                        "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
-                    },
-                    {
-                        "$set": {
-                            "filled_volume": broker_order.filled_volume,
-                            "filled_amount": broker_order.filled_amount,
-                            "filled_vwap": broker_order.filled_vwap,
-                            "status": broker_order.status.name,
-                            "exchange_order_id": broker_order.exchange_order_id,
-                            "updated_dt": broker_order.updated_dt,
-                        }
-                    },
-                    upsert=True,
-                    session=session,
-                )
-            else:
-                self._database.orders.update_one(
-                    {
-                        "order_id": broker_order.order_id,
-                        "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
-                    },
-                    {
-                        "$set": {
-                            "filled_volume": broker_order.filled_volume,
-                            "filled_amount": broker_order.filled_amount,
-                            "filled_vwap": broker_order.filled_vwap,
-                            "status": broker_order.status.name,
-                            "exchange_order_id": broker_order.exchange_order_id,
-                            "updated_dt": broker_order.updated_dt,
-                        }
-                    },
-                    session=session,
-                )
-            self._update_frozens([broker_order.account_id], session=session)
-            self._update_account_info([broker_order.account_id], session=session)
-
-    def on_trade_status(self, context, event) -> None:
-        """收到成交回报信息"""
-
-        with self._database.start_session(
-            causal_consistency=True, lock=True
-        ) as session:
-            broker_trade = event.data
-            # 保存trades 层数据
-            self._database.save("trades", broker_trade, session=session)
-
-            # 处理order filled_volumes
-            self._update_order_filled_volumes(
-                [broker_trade.account_id], session=session
-            )
-
-            # 处理 position volume数据
-            if broker_trade.order_direction == OrderDirection.Buy:
-                self._update_position_buy(broker_trade, session)
-            else:
-                self._update_position_sell(broker_trade, session)
-            self._update_frozens([broker_trade.account_id], session=session)
-            self._update_account_info([broker_trade.account_id], session=session)
-
-            # *cash = self._database.positions.find_one(
-            # *    {"account_id": broker_trade.account_id, "symbol": "CNY"},
-            # *    {"_id": 0},
-            # *    session=session,
-            # *)
-            # *cash = vxCashPosition(cash)
-            # *
-            # *symbol_position = self._database.query_one(
-            # *    "positions",
-            # *    {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
-            # *    session=session,
-            # *)
-            # *if not symbol_position:
-            # *    preset = vxMarketPreset(broker_trade.symbol)
-            # *    symbol_position = vxPosition(
-            # *        account_id=broker_trade.account_id,
-            # *        symbol=broker_trade.symbol,
-            # *        security_type=preset.security_type,
-            # *        allow_t0=preset.allow_t0,
-            # *    )
-            # *
-            # *filled_amount = broker_trade.price * broker_trade.volume
-            # *commission = broker_trade.commission
-            # *
-            # *if broker_trade.order_direction == OrderDirection.Buy:
-            # *    delta = cash.volume_his - filled_amount - commission
-            # *    cash.volume_his = max(delta, 0)
-            # *    cash.volume_today = cash.volume_today + min(delta, 0)
-            # *    cash.frozen = max(cash.frozen - filled_amount - commission, 0)
-            # *
-            # *    symbol_position.volume_today += broker_trade.volume
-            # *    symbol_position.lasttrade = broker_trade.price
-            # *    symbol_position.cost += filled_amount + commission
-            # *
-            # *else:
-            # *    delta = symbol_position.volume_his - broker_trade.volume
-            # *    symbol_position.volume_his = max(delta, 0)
-            # *    symbol_position.volume_today = symbol_position.volume_today + min(
-            # *        delta, 0
-            # *    )
-            # *    symbol_position.frozen = max(
-            # *        symbol_position.frozen - broker_trade.volume, 0
-            # *    )
-            # *    symbol_position.lasttrade = broker_trade.price
-            # *    symbol_position.cost += commission - filled_amount
-            # *    cash.volume_today += filled_amount - commission
-            # *self._database.save_many(
-            # *    "positions", [cash, symbol_position], session=session
-            # *)
-            # *self._update_account_info([broker_trade.account_id], session=session)
-
-    def _update_position_buy(self, broker_trade, session=None):
-        filled_amount = broker_trade.price * broker_trade.volume
-        commission = broker_trade.commission
-
-        item = self._database.positions.find_one(
-            {
-                "account_id": broker_trade.account_id,
-                "symbol": "CNY",
-            },
-            {"_id": 0},
-        )
-
-        cash = vxCashPosition(item)
-        delta = cash.volume_his - filled_amount - commission
-        cash.volume_his = max(delta, 0)
-        cash.volume_today += min(delta, 0)
-        self._database.save("positions", cash, session=session)
-
-        preset = vxMarketPreset(broker_trade.symbol)
-        # * item = (
-        # *     self._database.positions.find_one(
-        # *         {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
-        # *         {"_id": 0},
-        # *     )
-        # *     or {}
-        # * )
-
-        self._database.positions.update_one(
-            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
-            {
-                "$set": {
-                    "lasttrade": broker_trade.price,
-                },
-                "$inc": {
-                    "volume_today": broker_trade.volume,
-                    "cost": filled_amount + commission,
-                },
-                "$setOnInsert": {
-                    "position_id": str(uuid.uuid4()),
-                    "position_side": "Long",
-                    "volume_his": 0,
-                    "volume": broker_trade.volume,
-                    "security_type": preset.security_type.name,
-                    "allow_t0": preset.allow_t0,
-                    "frozen": 0,
-                    "available": broker_trade.volume if preset.allow_t0 else 0,
-                    "fnl": -commission,
-                    "benchmark_marketvalue": -1,
-                    "uplimit_marketvalue": -1,
-                    "downlimit_marketvalue": -1,
-                },
-            },
-            upsert=True,
-            session=session,
-        )
-
-        return
-
-    def _update_position_sell(self, broker_trade, session=None):
-        filled_amount = broker_trade.price * broker_trade.volume
-        commission = broker_trade.commission
-        item = self._database.positions.find_one(
-            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol}
-        )
-        symbol_position = vxPosition(item)
-        delta = symbol_position.volume_his - symbol_position.volume
-        symbol_position.volume_his = max(delta, 0)
-        symbol_position.volume_today += min(delta, 0)
-        symbol_position.lasttrade = broker_trade.price
-        symbol_position.cost = symbol_position.cost - filled_amount + commission
-
-        self._database.positions.update_one(
-            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
-            {"$set": symbol_position.message},
-        )
-
-        self._database.positions.update_one(
-            {"account_id": broker_trade.account_id, "symbol": "CNY"},
-            {
-                "$inc": {
-                    "volume_today": +filled_amount - commission,
-                    "volume": +filled_amount - commission,
-                    "available": +filled_amount - commission,
-                    "marketvalue": +filled_amount - commission,
-                    "cost": +filled_amount - commission,
-                }
-            },
-        )
-
-
-if __name__ == "__main__":
-    publisher = vxZMQPublisher(
-        "simtest",
-        "tcp://uat.vxquant.com:12307",
-        "/Users/libao/src/git/all/vxquantlib/etc/frontend.key",
-    )
-    subscriber = vxZMQSubscriber(
-        "gateway",
-        "tcp://uat.vxquant.com:12309",
-        "/Users/libao/src/git/all/vxquantlib/examples/backend.key",
-    )
-
-    m = vxAccountsManager("mongodb://uat:uat@localhost:27017/uat", "uat", publisher)
-    m.create_account("test", if_exists="delete", channel_name="simtest")
-    # m.deposit("test", 1000)
-    # m.withdraw("test", 1000)
-    # logger.info(m.get_account("test"))
-    # logger.info(m.get_positions("test"))
-    # logger.info(m.get_orders("test"))
-    # logger.info(m.get_trades("test"))
-    order = m.order_volume("test", "SHSE.600000", 1000, 0)
-    # print(order)
-    # account = m.get_account("test")
-
-    # cash = m.get_positions("test", "CNY")
-    # print(cash)
-    # orders = m.get_orders("test")
-    # print(orders)
-    update_trade = False
-    update_order = False
-
-    while True:
-        reply_events = subscriber()
-        for reply_event in reply_events:
-            if reply_event.type == "on_execution_report":
-                reply_trade = reply_event.data
-                logger.info(
-                    f"{reply_trade.exchange_order_id},"
-                    f"{reply_trade.volume},"
-                    f"{reply_trade.price},"
-                )
-                m.on_trade_status(1, reply_event)
-                update_trade = True
-
-            elif reply_event.type == "on_order_status":
-                reply_order = reply_event.data
-                logger.info(
-                    f"{reply_order.exchange_order_id},"
-                    f"{reply_order.filled_volume},"
-                    f"{reply_order.status},"
-                )
-
-                m.on_order_status(None, reply_event)
-
-                if reply_order.status in (
-                    OrderStatus.Filled,
-                    OrderStatus.Canceled,
-                    OrderStatus.Rejected,
-                    OrderStatus.Expired,
-                ):
-                    update_order = True
-
-        if update_order and update_trade:
-            logger.info(f"订单已结束: {reply_order}")
-            a = input("wait ...")
-            trades = m.get_trades("test", order_id=order.order_id)
-            logger.info(f"trades: {trades}")
-
-            a = input("wait ...")
-            orders = m.get_orders("test", order_id=order.order_id)
-            logger.info(f"orders: {orders}")
-
-            a = input("wait ...")
-            positions = m.get_positions("test")
-            logger.info(f"positions:{positions}")
-
-            a = input("wait ...")
-            account = m.get_account("test")
-            logger.info(f"account:{account}")
-
-            break
-
-        vxtime.sleep(1)
-
-    # * while True:
-    # *     vxticks = m._update_ticks(
-    # *         "SHSE.600000",
-    # *         "SZSE.000001",
-    # *         "SHSE.000001",
-    # *         "SZSE.399001",
-    # *         "SZSE.300059",
-    # *         "SHSE.000001",
-    # *         "SHSE.000688",
-    # *         "SHSE.511880",
-    # *         "SHSE.510300",
-    # *         "SHSE.511990",
-    # *         "SHSE.511660",
-    # *         "SHSE.204001",
-    # *         "SZSE.399001",
-    # *         "SZSE.399673",
-    # *         "SZSE.159001",
-    # *         "SZSE.159919",
-    # *         "SZSE.159915",
-    # *         "SZSE.159937",
-    # *         "SZSE.131810",
-    # *     )
-    # *     logger.info("=" * 60)
-    # *     for symbol, tick in vxticks.items():
-    # *         logger.info(
-    # *             f"更新时间:{to_timestring(tick.created_dt,'%X.%f')}"
-    # *             f" {symbol} : 最新: {tick.lasttrade} 涨幅(%):"
-    # *             f" {tick.lasttrade*100/tick.yclose-100:.2f}%"
-    # *         )
-
-    # *     vxtime.sleep(3)
+"""组合相关数据模型"""
+
+
+import uuid
+import pymongo
+
+from typing import Optional, Union, Dict
+from multiprocessing import Lock
+
+from vxsched import vxZMQPublisher, vxZMQSubscriber
+from vxutils import vxtime, logger
+from vxutils.database import vxMongoDB
+from vxutils.convertors import to_timestring
+from vxquant.exceptions import (
+    NoEnoughCash,
+    NoEnoughPosition,
+    IllegalVolume,
+    IllegalPrice,
+    # * RiskRuleCheckFailed,
+    # * IllegalAccountId,
+    # * IllegalStrategyId,
+    # * IllegalSymbol,
+    # * AccountDisabled,
+    # * AccountDisconnected,
+    # * AccountLoggedout,
+    # * NotInTradingSession,
+    # * OrderTypeNotSupported,
+    # * Throttle,
+    # * IllegalOrder,
+    # * OrderFinalized,
+    # * UnknownOrder,
+    # * AlreadyInPendingCancel,
+)
+from vxquant.mdapi.hq import vxTdxHQ
+from vxquant.model.preset import vxMarketPreset
+from vxquant.model.contants import (
+    OrderOffset,
+    TradeStatus,
+    OrderType,
+    OrderStatus,
+    OrderDirection,
+    AccountType,
+)
+from vxquant.model.exchange import (
+    vxAccountInfo,
+    vxPosition,
+    vxOrder,
+    vxTrade,
+    vxCashPosition,
+    vxTick,
+)
+
+
+class vxAccountBase:
+    """证券账户基类"""
+
+    @property
+    def account_id(self):
+        """账户id"""
+        raise NotImplementedError
+
+    @property
+    def account_info(self):
+        """账户信息"""
+        raise NotImplementedError
+
+    def get_positions(self, symbol=None):
+        """获取持仓信息"""
+        raise NotImplementedError
+
+
+class vxStockAccount:
+    """股票账户"""
+
+    def __init__(
+        self,
+        account_id=None,
+        balance=100_0000,
+        account_type=AccountType.Normal,
+        portfolio_id=None,
+        publisher=None,
+    ):
+        self._account_type = account_type
+        self._account_info = vxAccountInfo(
+            account_id=account_id, portfolio_id=portfolio_id
+        )
+        self._positions = {}
+        self._algo_orders = {}
+        self._orders = {}
+        self._trades = {}
+        self._publisher = publisher
+
+        self._positions["CNY"] = vxCashPosition(
+            account_id=account_id,
+            symbol="CNY",
+            security_type="CASH",
+            allow_t0=True,
+            lasttrade=1.0,
+        )
+
+        self._lock = Lock()
+
+        self.deposit(balance)
+        self.on_settle()
+
+    def __str__(self):
+        return f"< {self.__class__.__name__}({id(self)}) :\n {self.account_info} >"
+
+    __repr__ = __str__
+
+    @property
+    def account_id(self):
+        """账户id"""
+        return self._account_info.account_id
+
+    @property
+    def account_info(self):
+        """账户信息"""
+        return self._account_info
+
+    def get_positions(
+        self, symbol: Optional[str] = None
+    ) -> Union[Dict, vxPosition, vxCashPosition]:
+        """获取持仓信息"""
+        if not symbol:
+            return self._positions
+
+        if symbol in self._positions:
+            return self._positions[symbol]
+
+        preset = vxMarketPreset(symbol)
+        return vxPosition(
+            account_id=self.account_id,
+            symbol=symbol,
+            security_type=preset.security_type,
+            allow_t0=preset.allow_t0,
+        )
+
+    def get_orders(
+        self,
+        order_id: Optional[str] = None,
+        algo_order_id: Optional[str] = None,
+        exchange_order_id: Optional[str] = None,
+    ) -> Dict[str, Optional[vxOrder]]:
+        """获取当日委托信息"""
+        if order_id:
+            return (
+                {order_id: self._orders[order_id]} if order_id in self._orders else {}
+            )
+
+        if algo_order_id:
+            return {
+                order_id: order
+                for order in self._orders.values()
+                if order.algo_order_id == algo_order_id
+            }
+
+        if exchange_order_id:
+            return {
+                order.order_id: order
+                for order in self._orders.values()
+                if order.exchange_order_id == exchange_order_id
+            }
+
+        return self._orders
+
+    def get_trades(
+        self, order_id: Optional[str] = None, trade_id: Optional[str] = None
+    ) -> dict:
+        """获取当日成交回报"""
+        if order_id:
+            return {
+                trade.trade_id: trade
+                for trade in self._trades.values()
+                if trade.order_id == order_id
+            }
+
+        if trade_id:
+            return (
+                {trade_id: self._trades[trade_id]} if trade_id in self._trades else {}
+            )
+
+        return self._trades
+
+    def deposit(self, money: float) -> None:
+        """转入金额"""
+        if money <= 0:
+            raise IllegalPrice(f"转入金额 {money} <= 0 错误.")
+
+        with self._lock:
+            self.account_info.deposit += money
+            self.account_info.fund_shares += money / self.account_info.fund_nav
+            self._positions["CNY"].volume_today += money
+            self._positions["CNY"].cost += money
+            self.update_account_info()
+
+    def withdraw(self, money: float) -> None:
+        """转出金额"""
+        if money <= 0:
+            raise IllegalPrice(f"转出金额 {money} <= 0 错误.")
+
+        cash = self._positions["CNY"]
+        if money > cash.available:
+            raise NoEnoughCash(f"转出金额{money} 大于可用金额 {cash.available}。 ")
+        with self._lock:
+            self.account_info.withdraw += money
+            self.account_info.fund_shares -= money / self.account_info.fund_nav
+            if money < cash.volume_his:
+                cash.volume_his -= money
+            else:
+                money -= cash.volume_his
+                cash.volume_his = 0
+                cash.volume_today -= money
+            cash.cost = cash.marketvalue
+            self.update_account_info()
+
+    def set_bechmark_marketvalue(
+        self,
+        symbol: str,
+        benchmark_marketvalue: float = -1,
+        uplimit: float = -1,
+        downlimit: float = -1,
+    ) -> None:
+        """设置持仓基准市值、持仓市值上限，持仓市值下限
+
+        Arguments:
+            symbol {str} -- 证券代码
+            benchmark_marketvalue {float} -- 持仓基准市值，若市值小于0，则不做持仓市值监控 (default: {-1})
+            uplimit {float} -- 持仓市值上限，市值突破上限时，减仓至基准市值。 若小于0，则不做上限管理  (default: {-1})
+            downlimit {float} -- 持仓市值下限，市值跌破下限时，加仓至基准市值。若小于0，则不做下限管理 (default: {-1})
+        """
+        position = self.get_positions(symbol)
+        position.benchmark_marketvalue = benchmark_marketvalue
+        position.uplimit_marketvalue = uplimit
+        position.downlimit_marketvalue = downlimit
+        self._positions[position.position_id] = position
+
+    def check_benchmark_marketvalue(self):
+        """检查目标市值是否突破"""
+
+    def submit_order(self, symbol: str, volume: float, price=0) -> vxOrder:
+        """提交订单
+        进行下单前的检查，并且冻结资金及股票，形成一个PendingNew状态的order 以便提交
+
+        Arguments:
+            symbol {str} -- 下单标的
+            volume {float} -- 下单数量
+            price {int} -- 交易价格，若交易价格为0，则适用市价单，否则采用限价单 (default: {0})
+
+        Returns:
+            vxOrder -- 委托订单
+        """
+        if volume == 0:
+            raise IllegalVolume("volume不能为0.")
+
+        with self._lock:
+            if volume > 0:
+                if not price:
+                    tick = self.current(symbol)
+                    amount = (tick.lasttrade * volume) * 1.003
+                else:
+                    amount = price * volume * 1.003
+
+                position = self.get_positions("CNY")
+                if position.available < amount:
+                    raise NoEnoughCash(
+                        f"Not enough cash({position.available}) < need({amount})"
+                    )
+            else:
+                position = self.get_positions(symbol)
+                if position.available < volume:
+                    raise NoEnoughPosition(
+                        f"Not enough volume {symbol} {position.available} < amount"
+                    )
+
+            vxorder = vxOrder(
+                account_id=self.account_id,
+                symbol=symbol,
+                order_direction=(
+                    OrderDirection.Buy if volume > 0 else OrderDirection.Sell
+                ),
+                order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
+                order_type=OrderType.Limit if price <= 0 else OrderType.Market,
+                volume=abs(volume),
+                price=price,
+                status=OrderStatus.PendingNew,
+            )
+            self._orders[vxorder.order_id] = vxorder
+            self.update_account_info()
+
+        if self._publisher:
+            logger.debug(f"通过 {self._publisher.channel_name} 下单: {vxorder}")
+            self._publisher("on_submit_broker_order", vxorder)
+
+        return vxorder
+
+    @property
+    def message(self) -> dict:
+        """账户消息"""
+        return {
+            "account_info": self.account_info,
+            "positions": self.get_positions(),
+            "orders": self.get_orders(),
+            "trades": self.get_trades(),
+        }
+
+    def update_account_info(self) -> None:
+        """更新账户信息"""
+
+        self._account_info.marketvalue = 0
+        self._account_info.fnl = 0
+
+        for position in self._positions.values():
+            position.frozen = 0
+            if position.symbol != "CNY":
+                self._account_info.marketvalue += position.marketvalue
+                self._account_info.fnl += position.fnl
+            else:
+                self._account_info.balance = position.marketvalue
+                position.cost = position.marketvalue
+
+        for order in self._orders.values():
+            if order.status not in [
+                OrderStatus.PendingNew,
+                OrderStatus.New,
+                OrderStatus.PartiallyFilled,
+            ]:
+                continue
+
+            if order.order_direction == OrderDirection.Buy:
+                need_amount = (order.volume - order.filled_volume) * order.price * 1.003
+                self._positions["CNY"].frozen += need_amount
+
+            else:
+                self._positions[order.symbol].frozen += (
+                    order.volume - order.filled_volume
+                )
+        self.account_info.frozen = self._positions["CNY"].frozen
+        logger.debug(f"更新后账户信息: {self.message}")
+
+    def on_tick(self, ticks: dict) -> None:
+        """更新交易价格"""
+        update_symbols = set(self._positions.keys()) | set(ticks.keys())
+        with self._lock:
+            for symbol in update_symbols.items():
+                self._positions[symbol].lasttrade = ticks[symbol].lasttrade
+                self._positions[symbol].updated_dt = ticks[symbol].created_dt
+            self.account_info.marketvalue = sum(
+                p.marketvalue for p in self._positions.values() if p.symbol != "CNY"
+            )
+
+    def on_order_status(self, agent_order: vxOrder) -> None:
+        """更新订单状态"""
+
+        if agent_order.order_id not in self._orders:
+            with self._lock:
+                self._orders[agent_order.order_id] = vxOrder(agent_order.message)
+                self.update_account_info()
+                return
+
+        vxorder = self._orders[agent_order.order_id]
+        if vxorder.status in (
+            OrderStatus.Canceled,
+            OrderStatus.Expired,
+            OrderStatus.Filled,
+            OrderStatus.Rejected,
+            OrderStatus.Suspended,
+        ):
+            logger.info(
+                f"已经完结的委托信息，收到更新委托: {agent_order.status} {agent_order.filled_volume}"
+            )
+            return
+
+        if vxorder.filled_volume > agent_order.filled_volume:
+            logger.info(
+                f"收到早前的委托订单更新信息.filled_volume: vxorder{vxorder.filled_volume} >"
+                f" agent_order:{agent_order.filled_volume}."
+            )
+            return
+
+        with self._lock:
+            vxorder.exchange_order_id = agent_order.exchange_order_id
+            vxorder.filled_volume = agent_order.filled_volume
+            vxorder.filled_amount = agent_order.filled_amount
+            vxorder.status = agent_order.status
+            vxorder.updated_dt = agent_order.updated_dt
+            self.update_account_info()
+
+    def _handler_open_position(
+        self,
+        position: Union[vxPosition, vxCashPosition],
+        volume: float,
+        filled_amount: float,
+    ):
+        """处理开仓仓位"""
+        position.volume_today += volume
+        position.cost += filled_amount
+        self._positions[position.symbol] = position
+
+    def _handler_close_position(
+        self,
+        position: Union[vxPosition, vxCashPosition],
+        volume: float,
+        filled_amount: float,
+    ):
+        """处理平仓仓位"""
+        deta = position.volume_his - volume
+        position.volume_his = max(deta, 0)
+        position.volume_today = (
+            position.volume_today if deta >= 0 else position.volume_today + deta
+        )
+        position.cost -= filled_amount
+        self._positions[position.symbol] = position
+
+    def on_execution_report(self, agent_trade: vxTrade) -> None:
+        """更新成交回报信息"""
+        if agent_trade.status != TradeStatus.Trade:
+            logger.warning(f"收到非成交回报信息。 {agent_trade}")
+            return
+
+        if agent_trade.trade_id in self._trades:
+            logger.warning(f"收到重复的委托订单信息 {agent_trade.trade_id} {agent_trade}")
+            return
+
+        with self._lock:
+            self._trades[agent_trade.trade_id] = vxTrade(agent_trade.message)
+
+            cash_position = self.get_positions("CNY")
+            symbol_position = self.get_positions(agent_trade.symbol)
+            symbol_position.lasttrade = agent_trade.price
+
+            if agent_trade.order_direction == OrderDirection.Buy:
+                filled_amount = (
+                    agent_trade.price * agent_trade.volume + agent_trade.commission
+                )
+                # 扣减现金仓位
+                self._handler_close_position(
+                    cash_position, filled_amount, filled_amount
+                )
+                self._handler_open_position(
+                    symbol_position, agent_trade.volume, filled_amount
+                )
+            else:
+                filled_amount = (
+                    agent_trade.price * agent_trade.volume - agent_trade.commission
+                )
+                # 扣减symbol 持仓
+                self._handler_close_position(
+                    symbol_position, agent_trade.volume, filled_amount
+                )
+                self._handler_open_position(cash_position, filled_amount, filled_amount)
+            cash_position.updated_dt = agent_trade.updated_dt
+            symbol_position.updated_dt = agent_trade.updated_dt
+
+            self._handle_order_status(agent_trade, filled_amount)
+            self.update_account_info()
+
+    def _handle_order_status(self, agent_trade: vxTrade, filled_amount: float) -> None:
+        vxorder = self.get_orders(agent_trade.order_id).get(agent_trade.order_id, None)
+
+        if vxorder is None:
+            logger.warning(f"未知订单{agent_trade.order_id}")
+            return
+
+        if vxorder.status in (
+            OrderStatus.Canceled,
+            OrderStatus.Expired,
+            OrderStatus.Rejected,
+            OrderStatus.Suspended,
+        ):
+            logger.warning(f"已终止订单{vxorder.order_id} 收到成交信息:{agent_trade}")
+            return
+
+        vxorder.filled_volume += agent_trade.volume
+        vxorder.filled_amount += filled_amount
+        vxorder.status = (
+            OrderStatus.PartiallyFilled
+            if vxorder.filled_volume < vxorder.volume
+            else OrderStatus.Filled
+        )
+        vxorder.updated_dt = max(agent_trade.updated_dt, vxorder.updated_dt)
+
+    def on_settle(self):
+        """日结函数"""
+        now = vxtime.now()
+        logger.debug(f"开始执行日结{to_timestring(now,'%Y-%m-%d')}")
+
+        expired_orders = []
+        with self._lock:
+            # 1. 去掉超时以及当天已完成订单
+            orders = self._orders
+            self._orders = {}
+            for order in orders.values():
+                if order.status in [
+                    OrderStatus.Canceled,
+                    OrderStatus.Expired,
+                    OrderStatus.Filled,
+                    OrderStatus.Rejected,
+                    OrderStatus.Suspended,
+                ]:
+                    continue
+
+                if order.due_dt >= now:
+                    expired_orders.append(order)
+
+                self._orders[order.order_id] = order
+
+            # 超时的成交信息去掉
+            self._trades = {
+                trade_id: trade
+                for trade_id, trade in self._trades.items()
+                if trade.order_id in self._orders
+            }
+            # position
+            positions = self._positions
+            self._positions = {}
+            for symbol, position in positions.items():
+                if position.volume == 0 and position.symbol != "CNY":
+                    continue
+                position.volume_his, position.volume_today = position.volume, 0
+                self._positions[symbol] = position
+
+            self.update_account_info()
+            self.account_info.deposit = 0
+            self.account_info.withdraw = 0
+            self.account_info.asset_yd = self.account_info.asset
+            self.account_info.fund_nav_yd = self.account_info.fund_nav
+            self.account_info.nav_yd = self.account_info.nav
+
+    def update(
+        self,
+        account_info: Optional[vxAccountInfo] = None,
+        positions: Dict[str, Union[vxCashPosition, vxPosition]] = None,
+        orders: Dict[str, vxOrder] = None,
+        trades: Dict[str, vxTrade] = None,
+    ) -> None:
+        """直接账户基本信息"""
+        with self._lock:
+            if account_info:
+                self._account_info = account_info
+
+            if positions:
+                self._positions = positions
+
+            if orders:
+                self._orders = orders
+
+            if trades:
+                self._trades = trades
+            self.update_account_info()
+
+    @classmethod
+    def load_account(
+        cls,
+        account_info: vxAccountInfo,
+        positions: Dict[str, Union[vxCashPosition, vxPosition]],
+        orders: Dict[str, vxOrder],
+        trades: Dict[str, vxTrade],
+    ) -> "vxStockAccount":
+        """加载账户信息"""
+        instance = cls.__new__(cls=cls)
+        instance.update(account_info, positions, orders, trades)
+        return instance
+
+
+class vxPortfolioManager:
+    """组合管理"""
+
+    def __init__(self, portfolio_id: str, dbwriter):
+        pass
+
+    def create_portfolio(self, balance: float = 10_000_000.00, account_ids=None):
+        """创建组合"""
+
+    def create_account(self, account_id, balance=1_000_000.00):
+        """创建账户"""
+
+
+class vxAccountsManager:
+    def __init__(self, db_uri, db_name, publisher=None, hqfetcher=None):
+        self._database = vxMongoDB(db_uri, db_name)
+        self._database.mapping("accounts", vxAccountInfo, ["account_id"])
+        self._database.mapping("positions", vxPosition, ["account_id", "symbol"])
+        self._database.mapping("orders", vxOrder, ["order_id"])
+        self._database.mapping("trades", vxTrade, ["trade_id"])
+        self._database.mapping("current", vxTick, ["symbol"])
+
+        self._publisher = publisher
+        self._hqfetcher = hqfetcher or vxTdxHQ()
+        cur = self._database.agent_mapping.find({})
+        self._agent_map = {item.account_id: item.channel_name for item in cur}
+
+    def create_account(
+        self,
+        account_id: str = None,
+        balance: float = 1_000_000,
+        portfolio_id: str = "",
+        channel_name: str = None,
+        if_exists: str = "skip",
+    ) -> str:
+        """创建账户
+
+        Keyword Arguments:
+            account_id {str} -- 账户id (default: {None})
+            balance {float} -- 初始余额 (default: {1_000_000})
+            portfolio_id {str} -- 组合id (default: {""})
+            channel_name {str} -- 下单通道，缺省为空 (default: {None})
+            if_exists {str} -- 若存在账户已存在(default: {"skip"})
+                                'delete' ---> 删除原来账户
+                                'skip' --->  跳过
+                                'raise' ---> raise 一个exception
+
+
+        Raises:
+            ValueError: 账户已存在时，且if_exists == 'raise' 则raise一个exception
+
+        Returns:
+            str -- _description_
+        """
+
+        channel_name = channel_name or "simtest"
+
+        if self._database.accounts.count_documents({"account_id": account_id}) > 0:
+            if if_exists == "skip":
+                return account_id
+            elif if_exists == "delete":
+                self._database.accounts.delete_many({"account_id": account_id})
+                self._database.positions.delete_many({"account_id": account_id})
+                self._database.orders.delete_many({"account_id": account_id})
+                self._database.trades.delete_many({"account_id": account_id})
+            elif if_exists == "raise":
+                raise ValueError(f"account_id({account_id}) 已存在。")
+
+        account_id = account_id or str(uuid.uuid4())
+        account_info = vxAccountInfo(
+            account_id=account_id,
+            portfolio_id=portfolio_id,
+            deposit=balance,
+            balance=balance,
+            fund_shares=balance,
+            fund_nav_yd=1.0,
+            settle_day=vxtime.today("00:00:00") - 60 * 60 * 24,
+        )
+
+        cash_position = vxCashPosition(
+            portfolio_id=portfolio_id,
+            account_id=account_id,
+            volume_today=balance,
+        )
+
+        with self._database.start_session() as session:
+            self._database.save("accounts", account_info, session=session)
+            self._database.save("positions", cash_position, session=session)
+            self._database.agent_mapping.update_one(
+                {"account_id": account_id},
+                {"$set": {"channel_name": channel_name}},
+                upsert=True,
+            )
+            self._agent_map[account_id] = channel_name
+        self._update_account_info([account_id])
+
+        return account_id
+
+    def deposit(self, account_id, money: float) -> None:
+        """转入金额"""
+
+        account_info = self._database.accounts.find_one(
+            {"account_id": account_id}, {"_id": 0}
+        )
+        if account_info is None:
+            raise ValueError(f"账户信息不存在: {account_id}")
+        account_info = vxAccountInfo(account_info)
+
+        cash_position = self._database.positions.find_one(
+            {"account_id": account_id, "symbol": "CNY"}, {"_id": 0}
+        )
+        cash_position = vxCashPosition(cash_position)
+        logger.info(f"{account_info.nav}, {money}")
+
+        account_info.fund_shares += money / account_info.fund_nav
+        account_info.deposit += money
+        account_info.balance += money
+        cash_position.volume_today += money
+        logger.info(f"{account_info.nav}, {money},{cash_position.marketvalue}")
+
+        with self._database.start_session() as session:
+            self._database.save("accounts", account_info, session=session)
+            self._database.save("positions", cash_position, session=session)
+
+            self._update_account_info([account_id], session=session)
+
+    def withdraw(self, account_id, money: float) -> None:
+        """转出金额"""
+        if money <= 0:
+            raise IllegalPrice(f"转出金额 {money} <= 0 错误.")
+
+        with self._database.start_session(causal_consistency=True) as session:
+            cash = self._database.query_one(
+                "positions",
+                {"account_id": account_id, "symbol": "CNY"},
+                session=session,
+            )
+            cash = vxCashPosition(cash)
+            if money > cash.available:
+                raise NoEnoughCash(f"转出金额{money} 大于可用金额 {cash.available}。 ")
+            account_info = self._database.query_one(
+                "accounts", {"account_id": account_id}, session=session
+            )
+
+            account_info.withdraw += money
+            account_info.fund_shares -= money / account_info.fund_nav
+            account_info.balance -= money
+
+            if money < cash.volume_his:
+                cash.volume_his -= money
+            else:
+                money -= cash.volume_his
+                cash.volume_his = 0
+                cash.volume_today -= money
+
+            self._database.save("accounts", account_info, session=session)
+            self._database.save("positions", cash, session=session)
+            self._update_account_info([account_id], session=session)
+
+    def _update_account_info(self, account_ids, session=None):
+        """重新计算账户值"""
+
+        positions = self._database.query(
+            "positions", {"account_id": {"$in": account_ids}}, session=session
+        )
+        account_infos = {}
+        update_positions = []
+        for position in positions:
+            if position.account_id not in account_infos:
+                account_infos[position.account_id] = {
+                    "balance": 0,
+                    "frozen": 0,
+                    "marketvalue": 0,
+                    "fnl": 0,
+                }
+            if position.symbol == "CNY":
+                cash = vxCashPosition(position)
+                account_infos[position.account_id]["balance"] = cash.marketvalue
+                account_infos[position.account_id]["frozen"] = cash.frozen
+                update_positions.append(cash)
+            else:
+                account_infos[position.account_id][
+                    "marketvalue"
+                ] += position.marketvalue
+                account_infos[position.account_id]["fnl"] += position.fnl
+                update_positions.append(position)
+
+        cur = self._database.query(
+            "accounts", {"account_id": {"$in": list(account_ids)}}, session=session
+        )
+
+        update_account_infos = []
+        for account_info in cur:
+            update_dict = account_infos.get(account_info.account_id, {})
+            account_info.update(**update_dict)
+            logger.debug(f"更新后account_info:{account_info}")
+            update_account_infos.append(account_info)
+
+        self._database.save_many("positions", update_positions, session=session)
+        self._database.save_many("accounts", update_account_infos, session=session)
+
+    def _update_frozens(self, account_ids, session=None):
+        """重新计算持仓冻结信息"""
+        modify_position_ids = self._database.orders.distinct(
+            "frozen_position_id", {"account_id": {"$in": account_ids}}, session=session
+        )
+        agg_position_frozens = self._database.orders.aggregate(
+            [
+                {
+                    "$match": {
+                        "frozen_position_id": {"$in": modify_position_ids},
+                        "status": {"$in": ["New", "PartiallyFilled", "PendingNew"]},
+                    }
+                },
+                {
+                    "$project": {
+                        "account_id": "$account_id",
+                        "order_id": "$order_id",
+                        "frozen_position_id": "$frozen_position_id",
+                        "order_direction": "$order_direction",
+                        "left_volume": {"$subtract": ["$volume", "$filled_volume"]},
+                        "price": "$price",
+                        "cost": {
+                            "$multiply": [
+                                {"$subtract": ["$volume", "$filled_volume"]},
+                                "$price",
+                            ]
+                        },
+                    }
+                },
+                {
+                    "$group": {
+                        "_id": {
+                            "account_id": "$account_id",
+                            "position_id": "$frozen_position_id",
+                            "order_direction": "$order_direction",
+                        },
+                        "left_volume": {"$sum": "$left_volume"},
+                        "cost": {"$sum": "$cost"},
+                    }
+                },
+            ],
+            session=session,
+        )
+        update_position_cmds = [
+            pymongo.UpdateMany(
+                {"position_id": {"$in": modify_position_ids}}, {"$set": {"frozen": 0.0}}
+            )
+        ]
+        update_account_cmds = []
+
+        for agg_position_frozen in agg_position_frozens:
+            position_id = agg_position_frozen["_id"]["position_id"]
+            order_direction = agg_position_frozen["_id"]["order_direction"]
+
+            if order_direction == "Buy":
+                update_cmd = pymongo.UpdateOne(
+                    {"position_id": position_id},
+                    {"$set": {"frozen": agg_position_frozen["cost"] * 1.003}},
+                )
+                update_account_cmd = pymongo.UpdateOne(
+                    {"accountt_id": agg_position_frozen["_id"]["account_id"]},
+                    {"$set": {"frozen": agg_position_frozen["cost"] * 1.003}},
+                )
+                update_account_cmds.append(update_account_cmd)
+                logger.info(f"更新SQL accounts: {update_account_cmd}")
+
+            else:
+                update_cmd = pymongo.UpdateOne(
+                    {"position_id": position_id},
+                    {"$set": {"frozen": agg_position_frozen["left_volume"]}},
+                )
+
+            update_position_cmds.append(update_cmd)
+            logger.info(f"更新SQL positions: {update_cmd}")
+
+        self._database.positions.bulk_write(
+            update_position_cmds, ordered=True, session=session
+        )
+        if update_account_cmds:
+            self._database.accounts.bulk_write(
+                update_account_cmds,
+                ordered=True,
+            )
+            logger.warning(f"更新SQL accounts: {update_account_cmds}")
+        return modify_position_ids
+
+    def _update_order_filled_volumes(self, account_ids, session=None):
+        """重新计算委托订单成交信息"""
+        unfinished_order_ids = self._database.distinct(
+            "orders",
+            "order_id",
+            {
+                "status": {"$in": ["New", "PendingNew", "PartiallyFilled", "Unknown"]},
+                "account_id": {"$in": account_ids},
+            },
+            session=session,
+        )
+        logger.info(f"共有{len(unfinished_order_ids)}个未完成订单.")
+        agg_filled_volumes = self._database.trades.aggregate(
+            [
+                {"$match": {"order_id": {"$in": unfinished_order_ids}}},
+                {
+                    "$group": {
+                        "_id": {
+                            "order_id": "$order_id",
+                            "order_direction": "$order_direction",
+                        },
+                        "volume": {"$max": "$volume"},
+                        "filled_volume": {"$sum": "$volume"},
+                        "commission": {"$sum": "$commission"},
+                        "cost": {"$sum": {"$multiply": ["$price", "$volume"]}},
+                    }
+                },
+                {"$match": {"filled_volume": {"$gt": 0}}},
+            ],
+            session=session,
+        )
+
+        update_order_cmds = []
+        modify_order_ids = []
+        for agg_filled_volume in agg_filled_volumes:
+            order_id = agg_filled_volume["_id"]["order_id"]
+            order_direction = agg_filled_volume["_id"]["order_direction"]
+            filled_amount = (
+                (agg_filled_volume["cost"] + agg_filled_volume["cost"])
+                if order_direction == "Buy"
+                else (agg_filled_volume["cost"] - agg_filled_volume["cost"])
+            )
+            filled_vwap = filled_amount / agg_filled_volume["filled_volume"]
+            logger.info(
+                f"订单{order_id} {order_direction} filled_amount={filled_amount} filled_vwap={filled_vwap}."
+            )
+
+            update_order_cmd = pymongo.UpdateOne(
+                {"order_id": order_id},
+                {
+                    "$set": {
+                        "filled_volume": agg_filled_volume["filled_volume"],
+                        "filled_amount": filled_amount,
+                        "filled_vwap": filled_vwap,
+                        "status": (
+                            "Filled"
+                            if agg_filled_volume["filled_volume"]
+                            >= agg_filled_volume["volume"]
+                            else "PartiallyFilled"
+                        ),
+                    }
+                },
+            )
+            update_order_cmds.append(update_order_cmd)
+            modify_order_ids.append(order_id)
+        if update_order_cmds:
+            self._database.accounts.bulk_write(update_order_cmds, session=session)
+        return modify_order_ids
+
+    def get_account(self, account_id: str, session=None) -> vxAccountInfo:
+        """获取账户信息
+
+        Arguments:
+            account_id {str} -- 账户id
+
+        Returns:
+            vxAccountInfo -- 账户信息
+        """
+        logger.info(f"account_id({account_id}) session: {session}")
+        item = self._database.accounts.find_one(
+            {"account_id": account_id}, session=session
+        )
+
+        return vxAccountInfo(item)
+
+    def get_positions(self, account_id: str, symbol: str = None) -> Dict:
+        """获取相应的持仓信息
+
+        Arguments:
+            account_id {str} -- account_id 账户id
+            symbol {str} -- 持仓信息 (default: {None})
+
+        Returns:
+            Dict -- Dict['account_id': vxAccountInfo]
+        """
+        filter_ = {"account_id": account_id}
+        if symbol:
+            filter_["symbol"] = symbol
+        cur = self._database.query("positions", filter_)
+        return {position.symbol: position for position in cur}
+
+    def get_orders(
+        self,
+        account_id: str,
+        order_id: str = None,
+        exchange_order_id: str = None,
+        is_unfinished=False,
+    ) -> Dict:
+        """获取成交订单信息
+
+        Arguments:
+            account_id {str} -- 账户id
+
+        Keyword Arguments:
+            order_id {str} -- 委托订单id (default: {None})
+            exchange_order_id {str} -- 交易所委托订单id (default: {None})
+            is_unfinished {bool} -- 是否未完成 (default: {False})
+
+        Returns:
+            Dict -- Dict['order_id': vxOrder]
+        """
+        filter_ = {"account_id": account_id}
+        if order_id:
+            filter_["order_id"] = order_id
+        if exchange_order_id:
+            filter_["exchange_order_id"] = exchange_order_id
+        if is_unfinished:
+            filter_["status"] = {"$in": ["New", "PendingNew", "PartiallyFilled"]}
+
+        cur = self._database.query("orders", filter_)
+        return {o.order_id: o for o in cur}
+
+    def get_trades(
+        self,
+        account_id: str,
+        order_id: str = None,
+        trade_id: str = None,
+        exchange_order_id: str = None,
+    ) -> Dict:
+        """获取成交信息
+
+        Arguments:
+            account_id {str} -- 账户id
+
+        Keyword Arguments:
+            order_id {str} -- 委托订单id (default: {None})
+            trade_id {str} -- 成交回报id (default: {None})
+            exchange_order_id {str} -- 交易所委托订单id (default: {None})
+
+        Returns:
+            Dict -- Dict['trade_id':vxTrade]
+        """
+        filter_ = {"account_id": account_id}
+        if order_id:
+            filter_["order_id"] = order_id
+
+        if trade_id:
+            filter_["trade_id"] = trade_id
+
+        if exchange_order_id:
+            filter_["exchange_order_id"] = exchange_order_id
+
+        cur = self._database.query("trades", filter_)
+        return {t.trade_id: t for t in cur}
+
+    def _update_ticks(self, *symbols) -> Dict:
+        """更新ticks数据
+
+        Returns:
+            Dict -- Dict['symbol':vxTick]
+        """
+        now = vxtime.now()
+        cached_symbols = self._database.distinct(
+            "current",
+            "symbol",
+            {"symbol": {"$in": symbols}, "created_dt": {"$gt": now - 3}},
+        )
+        missing_symbols = set(symbols) - set(cached_symbols)
+        if len(missing_symbols) > 0:
+            vxticks = self._hqfetcher(*missing_symbols)
+
+            self._database.save_many("current", vxticks.values())
+        cur = self._database.query("current", {"symbol": {"$in": symbols}})
+        return {vxtick.symbol: vxtick for vxtick in cur}
+
+    def order_volume(
+        self,
+        account_id: str,
+        symbol: str,
+        volume: int,
+        price: float = 0.0,
+        algo_order_id: str = "",
+    ) -> vxOrder:
+        """委托交易volume的symbol证券
+
+        Arguments:
+            account_id {str} -- 交易账号
+            symbol {str} -- 目标证券代码
+            volume {int} -- volume> 0时，表示买入，volume < 0时，表示卖出
+            price {float} -- price 为0 时，则表示市价单，price > 0 时，表示限价单 (default: {0.0})
+
+        Returns:
+            vxOrder -- 委托订单号
+        """
+        with self._database.start_session(
+            causal_consistency=True, lock=True
+        ) as session:
+            order = vxOrder(
+                account_id=account_id,
+                algo_order_id=algo_order_id,
+                symbol=symbol,
+                status="PendingNew",
+            )
+
+            if price < 0.0:
+                raise ValueError(f"委托价格({price})必须大于等于0.")
+            elif price == 0:
+                order.order_type = "Market"
+                tick = self._update_ticks(order.symbol)
+
+                order.price = (
+                    tick[order.symbol].bid1_p
+                    if volume < 0
+                    else tick[order.symbol].ask1_p
+                )
+            else:
+                order.order_type = "Limit"
+                order.price = price
+
+            if volume == 0:
+                raise ValueError("委托volume 不可以为0.")
+
+            elif volume > 0:
+                order.order_direction = "Buy"
+                order.order_offset = "Open"
+                order.volume = volume
+                frozen_position = self._database.query_one(
+                    "positions",
+                    {"account_id": account_id, "symbol": "CNY"},
+                    session=session,
+                )
+                frozen_position = vxCashPosition(frozen_position)
+                frozen_amount = order.volume * order.price * 1.003
+                if frozen_amount > frozen_position.available:
+                    raise NoEnoughCash(
+                        f"Buy {symbol} volume({order.volume}) on price({order.price})"
+                        f" frozen {frozen_amount} > {frozen_position.available}"
+                    )
+                order.frozen_position_id = frozen_position.position_id
+                frozen_position.frozen += frozen_amount
+            else:
+                order.order_direction = "Sell"
+                order.order_offset = "Close"
+                order.volume = abs(volume)
+                frozen_position = self._database.query_one(
+                    "positions",
+                    {"account_id": account_id, "symbol": symbol},
+                    session=session,
+                )
+                if not frozen_position or frozen_position.available < order.volume:
+                    raise NoEnoughPosition(
+                        f"Sell {symbol} volume({order.volume})"
+                        f" 可用持仓:({frozen_position.available if frozen_position else 0})."
+                    )
+                order.frozen_position_id = frozen_position.position_id
+                frozen_position.available += order.volume
+
+            self._database.save("orders", order, session=session)
+            self._database.save("positions", frozen_position, session=session)
+
+            self._update_frozens([account_id], session=session)
+            self._update_account_info([account_id], session=session)
+
+            channel = self._agent_map.get(account_id, "simtest")
+            self._publisher("on_submit_broker_order", data=order, channel=channel)
+            logger.warning(
+                f"account({account_id}) 通过channel({channel}) 发送"
+                f" on_submit_broker_order 委托订单: {order}"
+            )
+            return order
+
+    def order_cancel(self, *orders):
+        """取消委托订单"""
+
+        cancel_order_ids = [order.order_id for order in orders]
+
+        cur = self._database.query(
+            "orders",
+            {
+                "order_id": {"$in": cancel_order_ids},
+                "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
+                "exchange_order_id": {"$ne": ""},
+            },
+        )
+        for order in cur:
+            channel = self._agent_map.get(order.account_id, "simtest")
+            self._publisher("on_submit_broker_order_cancel", order, channel=channel)
+            logger.warning(
+                f"account({order.account_id})通过 {channel} 发送 on_submit_broker_cancel"
+                f" 取消委托订单: {order}"
+            )
+        return
+
+    def on_order_status(self, context, event) -> None:
+        """订单状态更新"""
+        with self._database.start_session(causal_consistency=True) as session:
+            # 1. 更新order 状态信息
+            broker_order = event.data
+            if broker_order.status not in [
+                OrderStatus.PartiallyFilled,
+                OrderStatus.New,
+                OrderStatus.PendingNew,
+            ]:
+                # 已终结订单，根据返回信息更新数据库订单
+                self._database.orders.update_one(
+                    {
+                        "order_id": broker_order.order_id,
+                        "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
+                    },
+                    {
+                        "$set": {
+                            "filled_volume": broker_order.filled_volume,
+                            "filled_amount": broker_order.filled_amount,
+                            "filled_vwap": broker_order.filled_vwap,
+                            "status": broker_order.status.name,
+                            "exchange_order_id": broker_order.exchange_order_id,
+                            "updated_dt": broker_order.updated_dt,
+                        }
+                    },
+                    upsert=True,
+                    session=session,
+                )
+            else:
+                self._database.orders.update_one(
+                    {
+                        "order_id": broker_order.order_id,
+                        "status": {"$in": ["New", "PendingNew", "PartiallyFilled"]},
+                    },
+                    {
+                        "$set": {
+                            "filled_volume": broker_order.filled_volume,
+                            "filled_amount": broker_order.filled_amount,
+                            "filled_vwap": broker_order.filled_vwap,
+                            "status": broker_order.status.name,
+                            "exchange_order_id": broker_order.exchange_order_id,
+                            "updated_dt": broker_order.updated_dt,
+                        }
+                    },
+                    session=session,
+                )
+            self._update_frozens([broker_order.account_id], session=session)
+            self._update_account_info([broker_order.account_id], session=session)
+
+    def on_trade_status(self, context, event) -> None:
+        """收到成交回报信息"""
+
+        with self._database.start_session(
+            causal_consistency=True, lock=True
+        ) as session:
+            broker_trade = event.data
+            # 保存trades 层数据
+            self._database.save("trades", broker_trade, session=session)
+
+            # 处理order filled_volumes
+            self._update_order_filled_volumes(
+                [broker_trade.account_id], session=session
+            )
+
+            # 处理 position volume数据
+            if broker_trade.order_direction == OrderDirection.Buy:
+                self._update_position_buy(broker_trade, session)
+            else:
+                self._update_position_sell(broker_trade, session)
+            self._update_frozens([broker_trade.account_id], session=session)
+            self._update_account_info([broker_trade.account_id], session=session)
+
+            # *cash = self._database.positions.find_one(
+            # *    {"account_id": broker_trade.account_id, "symbol": "CNY"},
+            # *    {"_id": 0},
+            # *    session=session,
+            # *)
+            # *cash = vxCashPosition(cash)
+            # *
+            # *symbol_position = self._database.query_one(
+            # *    "positions",
+            # *    {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
+            # *    session=session,
+            # *)
+            # *if not symbol_position:
+            # *    preset = vxMarketPreset(broker_trade.symbol)
+            # *    symbol_position = vxPosition(
+            # *        account_id=broker_trade.account_id,
+            # *        symbol=broker_trade.symbol,
+            # *        security_type=preset.security_type,
+            # *        allow_t0=preset.allow_t0,
+            # *    )
+            # *
+            # *filled_amount = broker_trade.price * broker_trade.volume
+            # *commission = broker_trade.commission
+            # *
+            # *if broker_trade.order_direction == OrderDirection.Buy:
+            # *    delta = cash.volume_his - filled_amount - commission
+            # *    cash.volume_his = max(delta, 0)
+            # *    cash.volume_today = cash.volume_today + min(delta, 0)
+            # *    cash.frozen = max(cash.frozen - filled_amount - commission, 0)
+            # *
+            # *    symbol_position.volume_today += broker_trade.volume
+            # *    symbol_position.lasttrade = broker_trade.price
+            # *    symbol_position.cost += filled_amount + commission
+            # *
+            # *else:
+            # *    delta = symbol_position.volume_his - broker_trade.volume
+            # *    symbol_position.volume_his = max(delta, 0)
+            # *    symbol_position.volume_today = symbol_position.volume_today + min(
+            # *        delta, 0
+            # *    )
+            # *    symbol_position.frozen = max(
+            # *        symbol_position.frozen - broker_trade.volume, 0
+            # *    )
+            # *    symbol_position.lasttrade = broker_trade.price
+            # *    symbol_position.cost += commission - filled_amount
+            # *    cash.volume_today += filled_amount - commission
+            # *self._database.save_many(
+            # *    "positions", [cash, symbol_position], session=session
+            # *)
+            # *self._update_account_info([broker_trade.account_id], session=session)
+
+    def _update_position_buy(self, broker_trade, session=None):
+        filled_amount = broker_trade.price * broker_trade.volume
+        commission = broker_trade.commission
+
+        item = self._database.positions.find_one(
+            {
+                "account_id": broker_trade.account_id,
+                "symbol": "CNY",
+            },
+            {"_id": 0},
+        )
+
+        cash = vxCashPosition(item)
+        delta = cash.volume_his - filled_amount - commission
+        cash.volume_his = max(delta, 0)
+        cash.volume_today += min(delta, 0)
+        self._database.save("positions", cash, session=session)
+
+        preset = vxMarketPreset(broker_trade.symbol)
+        # * item = (
+        # *     self._database.positions.find_one(
+        # *         {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
+        # *         {"_id": 0},
+        # *     )
+        # *     or {}
+        # * )
+
+        self._database.positions.update_one(
+            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
+            {
+                "$set": {
+                    "lasttrade": broker_trade.price,
+                },
+                "$inc": {
+                    "volume_today": broker_trade.volume,
+                    "cost": filled_amount + commission,
+                },
+                "$setOnInsert": {
+                    "position_id": str(uuid.uuid4()),
+                    "position_side": "Long",
+                    "volume_his": 0,
+                    "volume": broker_trade.volume,
+                    "security_type": preset.security_type.name,
+                    "allow_t0": preset.allow_t0,
+                    "frozen": 0,
+                    "available": broker_trade.volume if preset.allow_t0 else 0,
+                    "fnl": -commission,
+                    "benchmark_marketvalue": -1,
+                    "uplimit_marketvalue": -1,
+                    "downlimit_marketvalue": -1,
+                },
+            },
+            upsert=True,
+            session=session,
+        )
+
+        return
+
+    def _update_position_sell(self, broker_trade, session=None):
+        filled_amount = broker_trade.price * broker_trade.volume
+        commission = broker_trade.commission
+        item = self._database.positions.find_one(
+            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol}
+        )
+        symbol_position = vxPosition(item)
+        delta = symbol_position.volume_his - symbol_position.volume
+        symbol_position.volume_his = max(delta, 0)
+        symbol_position.volume_today += min(delta, 0)
+        symbol_position.lasttrade = broker_trade.price
+        symbol_position.cost = symbol_position.cost - filled_amount + commission
+
+        self._database.positions.update_one(
+            {"account_id": broker_trade.account_id, "symbol": broker_trade.symbol},
+            {"$set": symbol_position.message},
+        )
+
+        self._database.positions.update_one(
+            {"account_id": broker_trade.account_id, "symbol": "CNY"},
+            {
+                "$inc": {
+                    "volume_today": +filled_amount - commission,
+                    "volume": +filled_amount - commission,
+                    "available": +filled_amount - commission,
+                    "marketvalue": +filled_amount - commission,
+                    "cost": +filled_amount - commission,
+                }
+            },
+        )
+
+
+if __name__ == "__main__":
+    publisher = vxZMQPublisher(
+        "simtest",
+        "tcp://uat.vxquant.com:12307",
+        "/Users/libao/src/git/all/vxquantlib/etc/frontend.key",
+    )
+    subscriber = vxZMQSubscriber(
+        "gateway",
+        "tcp://uat.vxquant.com:12309",
+        "/Users/libao/src/git/all/vxquantlib/examples/backend.key",
+    )
+
+    m = vxAccountsManager("mongodb://uat:uat@localhost:27017/uat", "uat", publisher)
+    m.create_account("test", if_exists="delete", channel_name="simtest")
+    # m.deposit("test", 1000)
+    # m.withdraw("test", 1000)
+    # logger.info(m.get_account("test"))
+    # logger.info(m.get_positions("test"))
+    # logger.info(m.get_orders("test"))
+    # logger.info(m.get_trades("test"))
+    order = m.order_volume("test", "SHSE.600000", 1000, 0)
+    # print(order)
+    # account = m.get_account("test")
+
+    # cash = m.get_positions("test", "CNY")
+    # print(cash)
+    # orders = m.get_orders("test")
+    # print(orders)
+    update_trade = False
+    update_order = False
+
+    while True:
+        reply_events = subscriber()
+        for reply_event in reply_events:
+            if reply_event.type == "on_execution_report":
+                reply_trade = reply_event.data
+                logger.info(
+                    f"{reply_trade.exchange_order_id},"
+                    f"{reply_trade.volume},"
+                    f"{reply_trade.price},"
+                )
+                m.on_trade_status(1, reply_event)
+                update_trade = True
+
+            elif reply_event.type == "on_order_status":
+                reply_order = reply_event.data
+                logger.info(
+                    f"{reply_order.exchange_order_id},"
+                    f"{reply_order.filled_volume},"
+                    f"{reply_order.status},"
+                )
+
+                m.on_order_status(None, reply_event)
+
+                if reply_order.status in (
+                    OrderStatus.Filled,
+                    OrderStatus.Canceled,
+                    OrderStatus.Rejected,
+                    OrderStatus.Expired,
+                ):
+                    update_order = True
+
+        if update_order and update_trade:
+            logger.info(f"订单已结束: {reply_order}")
+            a = input("wait ...")
+            trades = m.get_trades("test", order_id=order.order_id)
+            logger.info(f"trades: {trades}")
+
+            a = input("wait ...")
+            orders = m.get_orders("test", order_id=order.order_id)
+            logger.info(f"orders: {orders}")
+
+            a = input("wait ...")
+            positions = m.get_positions("test")
+            logger.info(f"positions:{positions}")
+
+            a = input("wait ...")
+            account = m.get_account("test")
+            logger.info(f"account:{account}")
+
+            break
+
+        vxtime.sleep(1)
+
+    # * while True:
+    # *     vxticks = m._update_ticks(
+    # *         "SHSE.600000",
+    # *         "SZSE.000001",
+    # *         "SHSE.000001",
+    # *         "SZSE.399001",
+    # *         "SZSE.300059",
+    # *         "SHSE.000001",
+    # *         "SHSE.000688",
+    # *         "SHSE.511880",
+    # *         "SHSE.510300",
+    # *         "SHSE.511990",
+    # *         "SHSE.511660",
+    # *         "SHSE.204001",
+    # *         "SZSE.399001",
+    # *         "SZSE.399673",
+    # *         "SZSE.159001",
+    # *         "SZSE.159919",
+    # *         "SZSE.159915",
+    # *         "SZSE.159937",
+    # *         "SZSE.131810",
+    # *     )
+    # *     logger.info("=" * 60)
+    # *     for symbol, tick in vxticks.items():
+    # *         logger.info(
+    # *             f"更新时间:{to_timestring(tick.created_dt,'%X.%f')}"
+    # *             f" {symbol} : 最新: {tick.lasttrade} 涨幅(%):"
+    # *             f" {tick.lasttrade*100/tick.yclose-100:.2f}%"
+    # *         )
+
+    # *     vxtime.sleep(3)
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/preset.py` & `vxquant-2023.4.1/src/vxquant/model/preset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,369 +1,388 @@
-# encoding=utf8
-""" 市场预设值清单 """
-
-from vxquant.model.contants import SecType
-
-__all__ = ["vxMarketPreset"]
-
-_DEFULAT_SYMBOL_MAP = {
-    "SHSE.204": {
-        "security_type": SecType.REPO,
-        "commission_coeff_peramount": 0.00,
-        "commission_coeff_today_peramount": 0.0,
-        "tax_coeff_peramount": 0.00,
-        "price_tick": 0.0001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 10000,
-        "down_limit_ratio": 0.0,
-        "allow_t0": False,
-    },
-    "SZSE.131": {
-        "security_type": SecType.REPO,
-        "commission_coeff_peramount": 0.00,
-        "commission_coeff_today_peramount": 0.0,
-        "tax_coeff_peramount": 0.00,
-        "price_tick": 0.0001,
-        "volume_unit": 10,
-        "upper_limit_ratio": 10000,
-        "down_limit_ratio": 0.0,
-        "allow_t0": False,
-    },
-    "SHSE.60": {
-        "security_type": SecType.STOCK,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SHSE.68": {
-        "security_type": SecType.STOCK,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.2,
-        "down_limit_ratio": 0.8,
-        "allow_t0": False,
-    },
-    "SHSE.00": {
-        "security_type": SecType.INDEX,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 1,
-        "upper_limit_ratio": 100,
-        "down_limit_ratio": 0,
-        "allow_t0": True,
-    },
-    "SZSE.39": {
-        "security_type": SecType.INDEX,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 1,
-        "upper_limit_ratio": 100,
-        "down_limit_ratio": 0,
-        "allow_t0": True,
-    },
-    "SHSE.50": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SHSE.51": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SHSE.58": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SHSE.56": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SHSE.10": {
-        "security_type": SecType.BOND,
-        "commission_coeff_peramount": 0.0008,
-        "commission_coeff_today_peramount": 0.0008,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.0001,
-        "volume_unit": 10,
-        "upper_limit_ratio": 1.3,
-        "down_limit_ratio": 0.7,
-        "allow_t0": True,
-    },
-    "SHSE.11": {
-        "security_type": SecType.BOND_CONVERTIBLE,
-        "commission_coeff_peramount": 0.0008,
-        "commission_coeff_today_peramount": 0.0008,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.01,
-        "volume_unit": 10,
-        "upper_limit_ratio": 1.3,
-        "down_limit_ratio": 0.7,
-        "allow_t0": True,
-    },
-    "SZSE.00": {
-        "security_type": SecType.STOCK,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SZSE.30": {
-        "security_type": SecType.STOCK,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.001,
-        "price_tick": 0.01,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SZSE.12": {
-        "security_type": SecType.BOND_CONVERTIBLE,
-        "commission_coeff_peramount": 0.0008,
-        "commission_coeff_today_peramount": 0.0008,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.01,
-        "volume_unit": 10,
-        "upper_limit_ratio": 1.3,
-        "down_limit_ratio": 0.7,
-        "allow_t0": True,
-    },
-    "SZSE.15": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SZSE.16": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-    "SZSE.18": {
-        "security_type": SecType.ETFLOF,
-        "commission_coeff_peramount": 0.001,
-        "commission_coeff_today_peramount": 0.001,
-        "tax_coeff_peramount": 0.0,
-        "price_tick": 0.001,
-        "volume_unit": 100,
-        "upper_limit_ratio": 1.1,
-        "down_limit_ratio": 0.9,
-        "allow_t0": False,
-    },
-}
-
-# T0的ETF产品
-_T0_ETFLOF = [
-    "SZSE.161129",
-    "SZSE.160723",
-    "SZSE.160216",
-    "SHSE.501018",
-    "SZSE.165513",
-    "SZSE.161116",
-    "SZSE.161815",
-    "SZSE.162719",
-    "SZSE.163208",
-    "SZSE.164701",
-    "SZSE.160416",
-    "SZSE.162411",
-    "SZSE.160719",
-    "SHSE.513500",
-    "SHSE.513030",
-    "SHSE.513080",
-    "SHSE.513100",
-    "SZSE.159941",
-    "SHSE.513300",
-    "SZSE.161128",
-    "SZSE.161125",
-    "SZSE.161130",
-    "SZSE.161126",
-    "SZSE.162415",
-    "SZSE.161127",
-    "SHSE.513050",
-    "SZSE.159822",
-    "SZSE.159607",
-    "SZSE.159605",
-    "SZSE.164906",
-    "SZSE.164824",
-    "SZSE.159740",
-    "SZSE.159741",
-    "SZSE.159742",
-    "SZSE.159823",
-    "SZSE.159850",
-    "SZSE.159892",
-    "SZSE.159920",
-    "SZSE.159954",
-    "SZSE.159960",
-    "SZSE.160322",
-    "SZSE.160717",
-    "SZSE.160922",
-    "SZSE.160924",
-    "SZSE.161124",
-    "SZSE.161831",
-    "SZSE.162416",
-    "SZSE.164705",
-    "SHSE.501021",
-    "SHSE.501025",
-    "SHSE.501301",
-    "SHSE.501302",
-    "SHSE.501303",
-    "SHSE.501305",
-    "SHSE.501306",
-    "SHSE.501307",
-    "SHSE.501309",
-    "SHSE.501310",
-    "SHSE.501311",
-    "SHSE.510900",
-    "SHSE.513000",
-    "SHSE.513010",
-    "SHSE.513060",
-    "SHSE.513090",
-    "SHSE.513130",
-    "SHSE.513180",
-    "SHSE.513330",
-    "SHSE.513520",
-    "SHSE.513550",
-    "SHSE.513580",
-    "SHSE.513600",
-    "SHSE.513660",
-    "SHSE.513680",
-    "SHSE.513880",
-    "SHSE.513900",
-    "SHSE.513990",
-    "SHSE.518880",
-    "SZSE.159934",
-    "SHSE.518800",
-    "SZSE.159937",
-    "SHSE.518680",
-    "SHSE.518850",
-    "SHSE.518600",
-    "SHSE.518660",
-    "SHSE.518890",
-    "SZSE.159812",
-    "SHSE.518860",
-]
-# 现金管理产品
-_CASH_SECURITIES = [
-    "SHSE.511990",
-    "SHSE.511880",
-    "SHSE.511660",
-    "SHSE.511850",
-    "SHSE.511810",
-    "SZSE.159001",
-    "SHSE.511690",
-    "SZSE.159003",
-    "SHSE.511800",
-    "SHSE.511700",
-    "SHSE.511820",
-    "SHSE.511650",
-    "SHSE.511900",
-    "SHSE.511860",
-    "SHSE.511620",
-    "SZSE.159005",
-    "SHSE.511980",
-    "SHSE.511600",
-    "SHSE.511830",
-    "SHSE.511950",
-    "SHSE.511670",
-    "SHSE.511920",
-    "SHSE.511960",
-    "SHSE.511970",
-    "SHSE.511910",
-    "SHSE.511770",
-    "SHSE.511930",
-]
-
-_DEFAULT_RESET = {
-    "security_type": SecType.OTHER,
-    "commission_coeff_peramount": 0.001,
-    "commission_coeff_today_peramount": 0.001,
-    "tax_coeff_peramount": 0.001,
-    "price_tick": 0.01,
-    "volume_unit": 100,
-    "upper_limit_ratio": 100,
-    "down_limit_ratio": 0.0,
-    "allow_t0": False,
-}
-
-
-class vxMarketPreset:
-    """交易所预设"""
-
-    def __init__(self, symbol) -> None:
-        preset = _DEFAULT_RESET.copy()
-        if symbol[:8] in _DEFULAT_SYMBOL_MAP:
-            self.__dict__.update(**_DEFULAT_SYMBOL_MAP[symbol[:8]])
-
-        elif symbol[:7] in _DEFULAT_SYMBOL_MAP:
-            self.__dict__.update(**_DEFULAT_SYMBOL_MAP[symbol[:7]])
-        else:
-            self.__dict__.update(**preset)
-
-        if symbol in _CASH_SECURITIES:
-            self.allow_t0 = True
-            self.security_type = SecType.CASH
-            self.commission_coeff_peramount = 0.0
-            self.commission_coeff_today_peramount = 0.0
-            self.tax_coeff_peramount = 0.0
-        elif symbol in _T0_ETFLOF:
-            self.allow_t0 = True
-
-    def __getitem__(self, key):
-        try:
-            return self.__dict__[key]
-        except KeyError as e:
-            raise AttributeError from e
+# encoding=utf8
+""" 市场预设值清单 """
+
+from vxquant.model.contants import SecType
+
+__all__ = ["vxMarketPreset"]
+
+_DEFULAT_SYMBOL_MAP = {
+    "SHSE.204": {
+        "security_type": SecType.REPO,
+        "commission_coeff_peramount": 0.00,
+        "commission_coeff_today_peramount": 0.0,
+        "tax_coeff_peramount": 0.00,
+        "price_tick": 0.0001,
+        "volume_unit": 10,
+        "volume_min": 10,
+        "upper_limit_ratio": 10000,
+        "down_limit_ratio": 0.0,
+        "allow_t0": False,
+    },
+    "SZSE.131": {
+        "security_type": SecType.REPO,
+        "commission_coeff_peramount": 0.00,
+        "commission_coeff_today_peramount": 0.0,
+        "tax_coeff_peramount": 0.00,
+        "price_tick": 0.0001,
+        "volume_unit": 10,
+        "volume_min": 10,
+        "upper_limit_ratio": 10000,
+        "down_limit_ratio": 0.0,
+        "allow_t0": False,
+    },
+    "SHSE.60": {
+        "security_type": SecType.STOCK,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SHSE.68": {
+        "security_type": SecType.STOCK,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 100,
+        "volume_min": 200,
+        "upper_limit_ratio": 1.2,
+        "down_limit_ratio": 0.8,
+        "allow_t0": False,
+    },
+    "SHSE.00": {
+        "security_type": SecType.INDEX,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 1,
+        "volume_min": 1,
+        "upper_limit_ratio": 100,
+        "down_limit_ratio": 0,
+        "allow_t0": True,
+    },
+    "SZSE.39": {
+        "security_type": SecType.INDEX,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 1,
+        "volume_min": 1,
+        "upper_limit_ratio": 100,
+        "down_limit_ratio": 0,
+        "allow_t0": True,
+    },
+    "SHSE.50": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SHSE.51": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SHSE.58": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SHSE.56": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SHSE.10": {
+        "security_type": SecType.BOND,
+        "commission_coeff_peramount": 0.0008,
+        "commission_coeff_today_peramount": 0.0008,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.0001,
+        "volume_unit": 10,
+        "volume_min": 10,
+        "upper_limit_ratio": 1.3,
+        "down_limit_ratio": 0.7,
+        "allow_t0": True,
+    },
+    "SHSE.11": {
+        "security_type": SecType.BOND_CONVERTIBLE,
+        "commission_coeff_peramount": 0.0008,
+        "commission_coeff_today_peramount": 0.0008,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.01,
+        "volume_unit": 10,
+        "volume_min": 10,
+        "upper_limit_ratio": 1.3,
+        "down_limit_ratio": 0.7,
+        "allow_t0": True,
+    },
+    "SZSE.00": {
+        "security_type": SecType.STOCK,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SZSE.30": {
+        "security_type": SecType.STOCK,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.001,
+        "price_tick": 0.01,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SZSE.12": {
+        "security_type": SecType.BOND_CONVERTIBLE,
+        "commission_coeff_peramount": 0.0008,
+        "commission_coeff_today_peramount": 0.0008,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.01,
+        "volume_unit": 10,
+        "volume_min": 10,
+        "upper_limit_ratio": 1.3,
+        "down_limit_ratio": 0.7,
+        "allow_t0": True,
+    },
+    "SZSE.15": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SZSE.16": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+    "SZSE.18": {
+        "security_type": SecType.ETFLOF,
+        "commission_coeff_peramount": 0.001,
+        "commission_coeff_today_peramount": 0.001,
+        "tax_coeff_peramount": 0.0,
+        "price_tick": 0.001,
+        "volume_unit": 100,
+        "volume_min": 100,
+        "upper_limit_ratio": 1.1,
+        "down_limit_ratio": 0.9,
+        "allow_t0": False,
+    },
+}
+
+# T0的ETF产品
+_T0_ETFLOF = [
+    "SZSE.161129",
+    "SZSE.160723",
+    "SZSE.160216",
+    "SHSE.501018",
+    "SZSE.165513",
+    "SZSE.161116",
+    "SZSE.161815",
+    "SZSE.162719",
+    "SZSE.163208",
+    "SZSE.164701",
+    "SZSE.160416",
+    "SZSE.162411",
+    "SZSE.160719",
+    "SHSE.513500",
+    "SHSE.513030",
+    "SHSE.513080",
+    "SHSE.513100",
+    "SZSE.159941",
+    "SHSE.513300",
+    "SZSE.161128",
+    "SZSE.161125",
+    "SZSE.161130",
+    "SZSE.161126",
+    "SZSE.162415",
+    "SZSE.161127",
+    "SHSE.513050",
+    "SZSE.159822",
+    "SZSE.159607",
+    "SZSE.159605",
+    "SZSE.164906",
+    "SZSE.164824",
+    "SZSE.159740",
+    "SZSE.159741",
+    "SZSE.159742",
+    "SZSE.159823",
+    "SZSE.159850",
+    "SZSE.159892",
+    "SZSE.159920",
+    "SZSE.159954",
+    "SZSE.159960",
+    "SZSE.160322",
+    "SZSE.160717",
+    "SZSE.160922",
+    "SZSE.160924",
+    "SZSE.161124",
+    "SZSE.161831",
+    "SZSE.162416",
+    "SZSE.164705",
+    "SHSE.501021",
+    "SHSE.501025",
+    "SHSE.501301",
+    "SHSE.501302",
+    "SHSE.501303",
+    "SHSE.501305",
+    "SHSE.501306",
+    "SHSE.501307",
+    "SHSE.501309",
+    "SHSE.501310",
+    "SHSE.501311",
+    "SHSE.510900",
+    "SHSE.513000",
+    "SHSE.513010",
+    "SHSE.513060",
+    "SHSE.513090",
+    "SHSE.513130",
+    "SHSE.513180",
+    "SHSE.513330",
+    "SHSE.513520",
+    "SHSE.513550",
+    "SHSE.513580",
+    "SHSE.513600",
+    "SHSE.513660",
+    "SHSE.513680",
+    "SHSE.513880",
+    "SHSE.513900",
+    "SHSE.513990",
+    "SHSE.518880",
+    "SZSE.159934",
+    "SHSE.518800",
+    "SZSE.159937",
+    "SHSE.518680",
+    "SHSE.518850",
+    "SHSE.518600",
+    "SHSE.518660",
+    "SHSE.518890",
+    "SZSE.159812",
+    "SHSE.518860",
+]
+# 现金管理产品
+_CASH_SECURITIES = [
+    "SHSE.511990",
+    "SHSE.511880",
+    "SHSE.511660",
+    "SHSE.511850",
+    "SHSE.511810",
+    "SZSE.159001",
+    "SHSE.511690",
+    "SZSE.159003",
+    "SHSE.511800",
+    "SHSE.511700",
+    "SHSE.511820",
+    "SHSE.511650",
+    "SHSE.511900",
+    "SHSE.511860",
+    "SHSE.511620",
+    "SZSE.159005",
+    "SHSE.511980",
+    "SHSE.511600",
+    "SHSE.511830",
+    "SHSE.511950",
+    "SHSE.511670",
+    "SHSE.511920",
+    "SHSE.511960",
+    "SHSE.511970",
+    "SHSE.511910",
+    "SHSE.511770",
+    "SHSE.511930",
+]
+
+_DEFAULT_RESET = {
+    "security_type": SecType.OTHER,
+    "commission_coeff_peramount": 0.001,
+    "commission_coeff_today_peramount": 0.001,
+    "tax_coeff_peramount": 0.001,
+    "price_tick": 0.01,
+    "volume_unit": 100,
+    "volume_min": 100,
+    "upper_limit_ratio": 100,
+    "down_limit_ratio": 0.0,
+    "allow_t0": False,
+}
+
+
+class vxMarketPreset:
+    """交易所预设"""
+
+    def __init__(self, symbol) -> None:
+        preset = _DEFAULT_RESET.copy()
+        if symbol[:8] in _DEFULAT_SYMBOL_MAP:
+            self.__dict__.update(**_DEFULAT_SYMBOL_MAP[symbol[:8]])
+
+        elif symbol[:7] in _DEFULAT_SYMBOL_MAP:
+            self.__dict__.update(**_DEFULAT_SYMBOL_MAP[symbol[:7]])
+        else:
+            self.__dict__.update(**preset)
+
+        if symbol in _CASH_SECURITIES:
+            self.allow_t0 = True
+            self.security_type = SecType.CASH
+            self.commission_coeff_peramount = 0.0
+            self.commission_coeff_today_peramount = 0.0
+            self.tax_coeff_peramount = 0.0
+        elif symbol in _T0_ETFLOF:
+            self.allow_t0 = True
+
+    def __getitem__(self, key):
+        try:
+            return self.__dict__[key]
+        except KeyError as e:
+            raise AttributeError from e
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/tools/gmData.py` & `vxquant-2023.4.1/src/vxquant/model/tools/gmData.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-""" 掘金量化数据转换至vxFinDataModel数据的转换器 """
-
-
-from vxutils import combine_datetime, to_timestring, vxtime, vxDataConvertor, to_text
-from vxquant.model.contants import PositionSide
-from vxquant.model.exchange import (
-    vxCashPosition,
-    vxTick,
-    vxBar,
-    vxPosition,
-    vxOrder,
-    vxTrade,
-    vxAccountInfo,
-)
-from vxquant.model.preset import vxMarketPreset
-
-__all__ = [
-    "gmTickConvter",
-    "gmBarConvter",
-    "gmAccountinfoConvter",
-    "update_gmcredit_cash",
-    "gmCashPositionConvter",
-    "gmPositionConvter",
-    "gmOrderConvter",
-    "gmTradeConvter",
-]
-
-# * #####################################################################
-# * gmTick的转换器
-# * #####################################################################
-
-GM_TICK_CONVERTORS = {
-    # 证券标的
-    "symbol": "symbol",
-    # 开盘价
-    "open": "open",
-    # 最高价
-    "high": "high",
-    # 最低价
-    "low": "low",
-    # 最近成交价
-    "lasttrade": "price",
-    # 昨日收盘价
-    "yclose": lambda x: 0,
-    # 成交量
-    "volume": "cum_volume",
-    # 成交金额
-    "amount": "cum_amount",
-    # 换手率
-    "turnoverratio": lambda x: 0,
-    # 卖1量
-    "bid1_v": lambda x: x["quotes"][0]["bid_v"],
-    # 卖1价
-    "bid1_p": lambda x: x["quotes"][0]["bid_p"],
-    # 卖2量
-    "bid2_v": lambda x: x["quotes"][1]["bid_v"],
-    # 卖2价
-    "bid2_p": lambda x: x["quotes"][1]["bid_p"],
-    # 卖3量
-    "bid3_v": lambda x: x["quotes"][2]["bid_v"],
-    # 卖3价
-    "bid3_p": lambda x: x["quotes"][2]["bid_p"],
-    # 卖4量
-    "bid4_v": lambda x: x["quotes"][3]["bid_v"],
-    # 卖4价
-    "bid4_p": lambda x: x["quotes"][3]["bid_p"],
-    # 卖5量
-    "bid5_v": lambda x: x["quotes"][4]["bid_v"],
-    # 卖5价
-    "bid5_p": lambda x: x["quotes"][4]["bid_p"],
-    # 买1量
-    "ask1_v": lambda x: x["quotes"][0]["ask_v"],
-    # 买1价
-    "ask1_p": lambda x: x["quotes"][0]["ask_p"],
-    # 买2量
-    "ask2_v": lambda x: x["quotes"][1]["ask_v"],
-    # 买2价
-    "ask2_p": lambda x: x["quotes"][1]["ask_p"],
-    # 买3量
-    "ask3_v": lambda x: x["quotes"][2]["ask_v"],
-    # 买3价
-    "ask3_p": lambda x: x["quotes"][2]["ask_p"],
-    # 买4量
-    "ask4_v": lambda x: x["quotes"][3]["ask_v"],
-    # 买4价
-    "ask4_p": lambda x: x["quotes"][3]["ask_p"],
-    # 买5量
-    "ask5_v": lambda x: x["quotes"][4]["ask_v"],
-    # 买5价
-    "ask5_p": lambda x: x["quotes"][4]["ask_p"],
-    # 持仓量
-    "interest": lambda x: 0,
-    # 停牌状态
-    "status": lambda x: "NORMAL",
-    # 发生事件
-    "created_dt": "created_at",
-    # 更新时间
-    "updated_dt": "created_at",
-}
-
-gmTickConvter = vxDataConvertor(vxTick, GM_TICK_CONVERTORS)
-
-
-# * #####################################################################
-# * gmBar的转换器
-# * #####################################################################
-BAR_TRANS = {"yclose": "pre_close", "created_dt": "eob"}
-gmBarConvter = vxDataConvertor(vxBar, BAR_TRANS)
-
-# * #####################################################################
-# * vxAccountInfo 的转换器
-# * #####################################################################
-
-GM_ACCOUNTINFO_CONVERTORS = {
-    # 组合ID
-    "portfolio_id": lambda x: "",
-    # 账户id
-    "account_id": "account_id",
-    # 账户币种
-    "currency": lambda x: "CNY",
-    # 今日转入金额
-    "deposit": lambda x: 0.0,
-    # 今日转出金额
-    "withdraw": lambda x: 0.0,
-    # 总资产
-    "asset": "nav",
-    # 净资产
-    "nav": "nav",
-    # 总负债
-    "debt": lambda x: 0.0,
-    # 资金余额
-    "balance": lambda x: x.order_frozen + x.available,
-    # 冻结金额
-    "frozen": "order_frozen",
-    # 可用金额
-    "available": lambda x: 0.0,
-    # 融资融券可用
-    "margin_available": lambda x: 0.0,
-    # 总市值
-    "marketvalue": "market_value",
-    # 今日盈利
-    "today_profit": lambda x: 0.0,
-    # 浮动盈亏
-    "fnl": "fpnl",
-}
-
-
-gmAccountinfoConvter = vxDataConvertor(vxAccountInfo, GM_ACCOUNTINFO_CONVERTORS)
-
-
-def update_gmcredit_cash(vxdatadict, gmCreditCash):
-    """更新负债信息"""
-    vxdatadict["marketvalue_short"] = gmCreditCash["dealfmktavl"]
-    vxdatadict["debt_long"] = gmCreditCash["ftotaldebts"]
-    vxdatadict["debt_short"] = gmCreditCash["dtotaldebts"]
-    vxdatadict["margin_available"] = gmCreditCash["marginavl"]
-    vxdatadict["balance"] = (
-        vxdatadict["asset"] - gmCreditCash["ftotaldebts"] - gmCreditCash["dtotaldebts"]
-    )
-    return vxdatadict
-
-
-# * #####################################################################
-# * gmPosition的转换器
-# * #####################################################################
-GM_POSITIONS_CONVERTORS = {
-    # 账户id
-    "account_id": "account_id",
-    # 证券类型
-    "security_type": lambda x: vxMarketPreset(x["symbol"]).security_type,
-    # 持仓方向
-    "position_side": lambda x: PositionSide.Long,
-    # 昨日持仓数量
-    "volume_his": lambda x: x["volume"] - x["volume_today"],
-    # 冻结数量
-    "frozen": "frozen",
-    # 持仓市值
-    "marketvalue": "market_value",
-    # 持仓成本
-    "cost": "amount",
-    # 浮动盈利
-    "fnl": "fnl",
-    # 最近成交价
-    "lasttrade": "price",
-    # 是否T0
-    "allow_t0": lambda x: vxMarketPreset(x["symbol"]).allow_t0,
-}
-
-gmPositionConvter = vxDataConvertor(vxPosition, GM_POSITIONS_CONVERTORS)
-
-
-# * #####################################################################
-# * gmCashPosition的转换器
-# * #####################################################################
-
-CASH_POSITION_CONVERTORS = {
-    "frozen": "order_frozen",
-    "volume_his": lambda x: x["order_frozen"] + x["available"],
-    "created_dt": "created_at",
-    "updated_dt": "updated_at",
-    "allow_t0": lambda x: True,
-}
-gmCashPositionConvter = vxDataConvertor(vxCashPosition, CASH_POSITION_CONVERTORS)
-
-# * #####################################################################
-# * gmOrder的转化器
-# * #####################################################################
-
-
-def _make_due_dt(obj):
-    created_date = to_timestring(obj["created_at"] or vxtime.now(), "%Y-%m-%d")
-    return combine_datetime(created_date, "15:00:00")
-
-
-GM_ORDER_CONVERTORS = {
-    "exchange_order_id": "cl_ord_id",
-    "order_id": "cl_ord_id",
-    "order_direction": "side",
-    "order_offset": "position_effect",
-    "reject_code": "ord_rej_reason",
-    "rej_reason_detail": lambda x: to_text(x["ord_rej_reason_detail"]),
-    "due_dt": _make_due_dt,
-    "created_dt": "created_at",
-    "updated_dt": "created_at",
-}
-gmOrderConvter = vxDataConvertor(vxOrder, GM_ORDER_CONVERTORS)
-
-# * #####################################################################
-# * gmTrade的转化器
-# * #####################################################################
-
-GM_TRADE_CONVERTORS = {
-    "trade_id": "exec_id",
-    "exchange_order_id": "cl_ord_id",
-    "order_id": "cl_ord_id",
-    "reject_code": "ord_rej_reason",
-    "reject_reason": lambda x: to_text(x["ord_rej_reason_detail"]),
-    "created_dt": "created_at",
-    "updated_dt": "created_at",
-    "status": "exec_type",
-    "order_direction": "side",
-    "order_offset": "position_effect",
-}
-
-gmTradeConvter = vxDataConvertor(vxTrade, GM_TRADE_CONVERTORS)
+""" 掘金量化数据转换至vxFinDataModel数据的转换器 """
+
+
+from vxutils import combine_datetime, to_timestring, vxtime, vxDataConvertor, to_text
+from vxquant.model.contants import PositionSide
+from vxquant.model.exchange import (
+    vxCashPosition,
+    vxTick,
+    vxBar,
+    vxPosition,
+    vxOrder,
+    vxTrade,
+    vxAccountInfo,
+)
+from vxquant.model.preset import vxMarketPreset
+
+__all__ = [
+    "gmTickConvter",
+    "gmBarConvter",
+    "gmAccountinfoConvter",
+    "update_gmcredit_cash",
+    "gmCashPositionConvter",
+    "gmPositionConvter",
+    "gmOrderConvter",
+    "gmTradeConvter",
+]
+
+# * #####################################################################
+# * gmTick的转换器
+# * #####################################################################
+
+GM_TICK_CONVERTORS = {
+    # 证券标的
+    "symbol": "symbol",
+    # 开盘价
+    "open": "open",
+    # 最高价
+    "high": "high",
+    # 最低价
+    "low": "low",
+    # 最近成交价
+    "lasttrade": "price",
+    # 昨日收盘价
+    "yclose": lambda x: 0,
+    # 成交量
+    "volume": "cum_volume",
+    # 成交金额
+    "amount": "cum_amount",
+    # 换手率
+    "turnoverratio": lambda x: 0,
+    # 卖1量
+    "bid1_v": lambda x: x["quotes"][0]["bid_v"],
+    # 卖1价
+    "bid1_p": lambda x: x["quotes"][0]["bid_p"],
+    # 卖2量
+    "bid2_v": lambda x: x["quotes"][1]["bid_v"],
+    # 卖2价
+    "bid2_p": lambda x: x["quotes"][1]["bid_p"],
+    # 卖3量
+    "bid3_v": lambda x: x["quotes"][2]["bid_v"],
+    # 卖3价
+    "bid3_p": lambda x: x["quotes"][2]["bid_p"],
+    # 卖4量
+    "bid4_v": lambda x: x["quotes"][3]["bid_v"],
+    # 卖4价
+    "bid4_p": lambda x: x["quotes"][3]["bid_p"],
+    # 卖5量
+    "bid5_v": lambda x: x["quotes"][4]["bid_v"],
+    # 卖5价
+    "bid5_p": lambda x: x["quotes"][4]["bid_p"],
+    # 买1量
+    "ask1_v": lambda x: x["quotes"][0]["ask_v"],
+    # 买1价
+    "ask1_p": lambda x: x["quotes"][0]["ask_p"],
+    # 买2量
+    "ask2_v": lambda x: x["quotes"][1]["ask_v"],
+    # 买2价
+    "ask2_p": lambda x: x["quotes"][1]["ask_p"],
+    # 买3量
+    "ask3_v": lambda x: x["quotes"][2]["ask_v"],
+    # 买3价
+    "ask3_p": lambda x: x["quotes"][2]["ask_p"],
+    # 买4量
+    "ask4_v": lambda x: x["quotes"][3]["ask_v"],
+    # 买4价
+    "ask4_p": lambda x: x["quotes"][3]["ask_p"],
+    # 买5量
+    "ask5_v": lambda x: x["quotes"][4]["ask_v"],
+    # 买5价
+    "ask5_p": lambda x: x["quotes"][4]["ask_p"],
+    # 持仓量
+    "interest": lambda x: 0,
+    # 停牌状态
+    "status": lambda x: "NORMAL",
+    # 发生事件
+    "created_dt": "created_at",
+    # 更新时间
+    "updated_dt": "created_at",
+}
+
+gmTickConvter = vxDataConvertor(vxTick, GM_TICK_CONVERTORS)
+
+
+# * #####################################################################
+# * gmBar的转换器
+# * #####################################################################
+BAR_TRANS = {"yclose": "pre_close", "created_dt": "eob"}
+gmBarConvter = vxDataConvertor(vxBar, BAR_TRANS)
+
+# * #####################################################################
+# * vxAccountInfo 的转换器
+# * #####################################################################
+
+GM_ACCOUNTINFO_CONVERTORS = {
+    # 组合ID
+    "portfolio_id": lambda x: "",
+    # 账户id
+    "account_id": "account_id",
+    # 账户币种
+    "currency": lambda x: "CNY",
+    # 今日转入金额
+    "deposit": lambda x: 0.0,
+    # 今日转出金额
+    "withdraw": lambda x: 0.0,
+    # 总资产
+    "asset": "nav",
+    # 净资产
+    "nav": "nav",
+    # 总负债
+    "debt": lambda x: 0.0,
+    # 资金余额
+    "balance": lambda x: x.order_frozen + x.available,
+    # 冻结金额
+    "frozen": "order_frozen",
+    # 可用金额
+    "available": lambda x: 0.0,
+    # 融资融券可用
+    "margin_available": lambda x: 0.0,
+    # 总市值
+    "marketvalue": "market_value",
+    # 今日盈利
+    "today_profit": lambda x: 0.0,
+    # 浮动盈亏
+    "fnl": "fpnl",
+}
+
+
+gmAccountinfoConvter = vxDataConvertor(vxAccountInfo, GM_ACCOUNTINFO_CONVERTORS)
+
+
+def update_gmcredit_cash(vxdatadict, gmCreditCash):
+    """更新负债信息"""
+    vxdatadict["marketvalue_short"] = gmCreditCash["dealfmktavl"]
+    vxdatadict["debt_long"] = gmCreditCash["ftotaldebts"]
+    vxdatadict["debt_short"] = gmCreditCash["dtotaldebts"]
+    vxdatadict["margin_available"] = gmCreditCash["marginavl"]
+    vxdatadict["balance"] = (
+        vxdatadict["asset"] - gmCreditCash["ftotaldebts"] - gmCreditCash["dtotaldebts"]
+    )
+    return vxdatadict
+
+
+# * #####################################################################
+# * gmPosition的转换器
+# * #####################################################################
+GM_POSITIONS_CONVERTORS = {
+    # 账户id
+    "account_id": "account_id",
+    # 证券类型
+    "security_type": lambda x: vxMarketPreset(x["symbol"]).security_type,
+    # 持仓方向
+    "position_side": lambda x: PositionSide.Long,
+    # 昨日持仓数量
+    "volume_his": lambda x: x["volume"] - x["volume_today"],
+    # 冻结数量
+    "frozen": "frozen",
+    # 持仓市值
+    "marketvalue": "market_value",
+    # 持仓成本
+    "cost": "amount",
+    # 浮动盈利
+    "fnl": "fnl",
+    # 最近成交价
+    "lasttrade": "price",
+    # 是否T0
+    "allow_t0": lambda x: vxMarketPreset(x["symbol"]).allow_t0,
+}
+
+gmPositionConvter = vxDataConvertor(vxPosition, GM_POSITIONS_CONVERTORS)
+
+
+# * #####################################################################
+# * gmCashPosition的转换器
+# * #####################################################################
+
+CASH_POSITION_CONVERTORS = {
+    "frozen": "order_frozen",
+    "volume_his": lambda x: x["order_frozen"] + x["available"],
+    "created_dt": "created_at",
+    "updated_dt": "updated_at",
+    "allow_t0": lambda x: True,
+}
+gmCashPositionConvter = vxDataConvertor(vxCashPosition, CASH_POSITION_CONVERTORS)
+
+# * #####################################################################
+# * gmOrder的转化器
+# * #####################################################################
+
+
+def _make_due_dt(obj):
+    created_date = to_timestring(obj["created_at"] or vxtime.now(), "%Y-%m-%d")
+    return combine_datetime(created_date, "15:00:00")
+
+
+GM_ORDER_CONVERTORS = {
+    "exchange_order_id": "cl_ord_id",
+    "order_id": "cl_ord_id",
+    "order_direction": "side",
+    "order_offset": "position_effect",
+    "reject_code": "ord_rej_reason",
+    "rej_reason_detail": lambda x: to_text(x["ord_rej_reason_detail"]),
+    "due_dt": _make_due_dt,
+    "created_dt": "created_at",
+    "updated_dt": "created_at",
+}
+gmOrderConvter = vxDataConvertor(vxOrder, GM_ORDER_CONVERTORS)
+
+# * #####################################################################
+# * gmTrade的转化器
+# * #####################################################################
+
+GM_TRADE_CONVERTORS = {
+    "trade_id": "exec_id",
+    "exchange_order_id": "cl_ord_id",
+    "order_id": "cl_ord_id",
+    "reject_code": "ord_rej_reason",
+    "reject_reason": lambda x: to_text(x["ord_rej_reason_detail"]),
+    "created_dt": "created_at",
+    "updated_dt": "created_at",
+    "status": "exec_type",
+    "order_direction": "side",
+    "order_offset": "position_effect",
+}
+
+gmTradeConvter = vxDataConvertor(vxTrade, GM_TRADE_CONVERTORS)
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/tools/qmtData.py` & `vxquant-2023.4.1/src/vxquant/model/tools/qmtData.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-""" QMT量化数据转换至vxFinDataModel数据的转换器 """
-
-import uuid
-from vxutils import combine_datetime, to_timestring, vxtime, vxDataConvertor, to_text
-
-from vxquant.model.exchange import (
-    vxCashPosition,
-    vxTick,
-    vxBar,
-    vxPosition,
-    vxOrder,
-    vxTrade,
-    vxAccountInfo,
-)
-from vxquant.model.preset import vxMarketPreset
-from vxquant.model.nomalize import to_symbol
-
-__all__ = [
-    "qmtTickConvter",
-    # "qmtBarConvter",
-    "qmtAccountInfoConvter",
-    "qmtCashPositionConvter",
-    "qmtPositionConvter",
-    "qmtOrderConvter",
-    "qmtTradeConvter",
-]
-
-
-TICK_CONVERTORS = {
-    # 证券标的
-    "symbol": "symbol",
-    # 开盘价
-    "open": "open",
-    # 最高价
-    "high": "high",
-    # 最低价
-    "low": "low",
-    # 最近成交价
-    "lasttrade": "lastPrice",
-    # 昨日收盘价
-    "yclose": "lastClose",
-    # 成交量
-    "volume": "volume",
-    # 成交金额
-    "amount": "amount",
-    # 换手率
-    "turnoverratio": lambda x: 0.0,
-    # 卖1量
-    "bid1_v": lambda x: x["bidVol"][0],
-    # 卖1价
-    "bid1_p": lambda x: x["bidPrice"][0],
-    # 卖2量
-    "bid2_v": lambda x: x["bidVol"][1],
-    # 卖2价
-    "bid2_p": lambda x: x["bidPrice"][1],
-    # 卖3量
-    "bid3_v": lambda x: x["bidVol"][2],
-    # 卖3价
-    "bid3_p": lambda x: x["bidPrice"][2],
-    # 卖4量
-    "bid4_v": lambda x: x["bidVol"][3],
-    # 卖4价
-    "bid4_p": lambda x: x["bidPrice"][3],
-    # 卖5量
-    "bid5_v": lambda x: x["bidVol"][4],
-    # 卖5价
-    "bid5_p": lambda x: x["bidPrice"][4],
-    # 买1量
-    "ask1_v": lambda x: x["askVol"][0],
-    # 买1价
-    "ask1_p": lambda x: x["askPrice"][0],
-    # 买2量
-    "ask2_v": lambda x: x["askVol"][1],
-    # 买2价
-    "ask2_p": lambda x: x["askPrice"][1],
-    # 买3量
-    "ask3_v": lambda x: x["askVol"][2],
-    # 买3价
-    "ask3_p": lambda x: x["askPrice"][2],
-    # 买4量
-    "ask4_v": lambda x: x["askVol"][3],
-    # 买4价
-    "ask4_p": lambda x: x["askPrice"][3],
-    # 买5量
-    "ask5_v": lambda x: x["askVol"][4],
-    # 买5价
-    "ask5_p": lambda x: x["askPrice"][4],
-    # 持仓量
-    "interest": "openInt",
-    # 停牌状态
-    "status": lambda x: "NORMAL",
-    # 创建时间
-    "created_dt": "timetag",
-    # 更新时间
-    "updated_dt": "timetag",
-}
-
-qmtTickConvter = vxDataConvertor(vxTick, TICK_CONVERTORS)
-
-
-def _to_order_direction(other_data):
-    return "Buy" if other_data.order_type in (23, 27, 40) else "Sell"
-
-
-def _to_order_offset(other_data):
-    return "Open" if other_data.order_type in (23, 27, 40) else "Close"
-
-
-def _to_order_type(other_data):
-    return "Limit" if other_data.price_type in (11,) else "Market"
-
-
-def _to_order_status(other_data):
-    order_code = other_data.order_status
-    if order_code in (48, 49):
-        return "PendingNew"
-    elif order_code in (50, 51):
-        return "New"
-    elif order_code in (52, 55):
-        return "PartiallyFilled"
-    elif order_code in (53, 54):
-        return "Canceled"
-    elif order_code in (56,):
-        return "Filled"
-    elif order_code in (57,):
-        return "Rejected"
-    else:
-        return "Unknown"
-
-
-ORDER_CONVERTORS = {
-    # 账号id
-    "account_id": "account_id",
-    # 委托id
-    "order_id": "order_remark",
-    # 算法委托id
-    "algo_order_id": "strategy_name",
-    # 交易所委托id
-    "exchange_order_id": "order_id",
-    # 冻结持仓id
-    "frozen_position_id": lambda x: "",
-    # 证券代码
-    "symbol": "stock_code",
-    # 买卖方向
-    "order_direction": _to_order_direction,
-    # 开平仓标志
-    "order_offset": _to_order_offset,
-    # 订单类型
-    "order_type": _to_order_type,
-    # 委托数量
-    "volume": "volume",
-    # 委托价格
-    "price": "price",
-    # 成交数量
-    "filled_volume": "traded_volume",
-    # 成交均价
-    "filled_vwap": "trade_price",
-    # 成交总额（含手续费）
-    "filled_amount": lambda x: x.traded_volume * x.traded_price,
-    # 订单状态
-    "status": _to_order_status,
-    # 订单超时时间
-    "due_dt": lambda x: combine_datetime(x.order_time, "15:00:00"),
-    # 拒绝代码
-    "reject_code": "status_msg",
-    # 拒绝原因
-    "reject_reason": "status_msg",
-    # 创建时间
-    "created_dt": "order_time",
-    # 更新时间
-    "updated_dt": "order_time",
-}
-
-
-qmtOrderConvter = vxDataConvertor(vxOrder, ORDER_CONVERTORS)
-
-
-TRADE_CONVERTORS = {
-    # 账户id
-    "account_id": "account_id",
-    # 委托id
-    "order_id": "order_remark",
-    # 交易所委托id
-    "exchange_order_id": "order_id",
-    # 成交id
-    "trade_id": "traded_id",
-    # 证券代码
-    "symbol": "stock_code",
-    # 买卖方向
-    "order_direction": _to_order_direction,
-    # 开平仓标志
-    "order_offset": _to_order_offset,
-    # 成交价格
-    "price": "traded_price",
-    # 成交数量
-    "volume": "traded_volume",
-    # 交易佣金
-    "commission": lambda x: x.traded_amount - x.traded_price * x.traded_volume,
-    # 成交状态
-    "status": lambda x: "Trade" if x.traded_volume > 0 else "Unknown",
-    # 拒绝代码
-    "reject_code": lambda x: "Unkown",
-    # 拒绝原因
-    "reject_reason": lambda x: "",
-    # 成交时间
-    "created_dt": "trade_time",
-    # 更新时间
-    "updated_dt": "trade_time",
-}
-
-qmtTradeConvter = vxDataConvertor(vxTrade, TRADE_CONVERTORS)
-
-
-POSITION_CONVERTORS = {
-    # 组合ID
-    "portfolio_id": lambda x: "",
-    # 账户id
-    "account_id": "account_id",
-    # 仓位id
-    "position_id": lambda x: str(uuid.uuid4()),
-    # 证券类型
-    "security_type": lambda x: vxMarketPreset(to_symbol(x.stock_code)).security_type,
-    # 证券代码
-    "symbol": "stock_code",
-    # 持仓方向
-    "position_side": lambda x: "Long",
-    # 今日持仓数量
-    "volume_today": lambda x: x.volume - x.can_use_volume,
-    # 昨日持仓数量
-    "volume_his": "can_use_volume",
-    # 持仓数量 --- 自动计算字段，由 volume_today + volume_his 计算所得
-    "volume": "volume",
-    # 冻结数量
-    "frozen": lambda x: x.volume - x.can_use_volume,
-    # 可用数量  --- 自动计算字段，由 volume - frozen计算
-    "available": "can_use_volume",
-    # 持仓市值
-    "marketvalue": "market_value",
-    # 持仓成本
-    "cost": lambda x: x.open_price * x.volume,
-    # 浮动盈利
-    "fnl": lambda x: x.market_value - x.open_price * x.volume,
-    # 持仓成本均价
-    "vwap": "open_price",
-    # 最近成交价
-    "lasttrade": lambda x: x.market_value / x.volume,
-    # 是否T0
-    "allow_t0": lambda x: vxMarketPreset(to_symbol(x.stock_code)).allow_t0,
-}
-
-qmtPositionConvter = vxDataConvertor(vxPosition, POSITION_CONVERTORS)
-
-CASHPOSITION_CONVERTORS = {
-    # 组合ID
-    "portfolio_id": lambda x: "",
-    # 账户id
-    "account_id": "account_id",
-    # 仓位id
-    "position_id": lambda x: str(uuid.uuid4()),
-    # 证券类型
-    "security_type": lambda x: "CASH",
-    # 证券代码
-    "symbol": lambda x: "CNY",
-    # 持仓方向
-    "position_side": lambda x: "Long",
-    # 今日持仓数量
-    "volume_today": "frozen_cash",
-    # 昨日持仓数量
-    "volume_his": "cash",
-    # 持仓数量
-    "volume": lambda x: x.frozen_cash + x.cash,
-    # 冻结数量
-    "frozen": "frozen_cash",
-    # 可用数量
-    "available": "cash",
-    # 持仓市值
-    "marketvalue": lambda x: x.frozen_cash + x.cash,
-    # 持仓成本
-    "cost": lambda x: x.frozen_cash + x.cash,
-    # 浮动盈利
-    "fnl": lambda x: 0.0,
-    # 持仓成本均价
-    "vwap": lambda x: 1.0,
-    # 最近成交价
-    "lasttrade": lambda x: 1.0,
-    # 是否T0
-    "allow_t0": lambda x: True,
-}
-
-qmtCashPositionConvter = vxDataConvertor(vxCashPosition, CASHPOSITION_CONVERTORS)
-
-ACCOUNTINFO_CONVERTORS = {
-    # 组合ID
-    "portfolio_id": lambda x: "",
-    # 账户id
-    "account_id": "account_id",
-    # 账户币种
-    "currency": lambda x: "CNY",
-    # 今日转入金额
-    "deposit": lambda x: 0.0,
-    # 今日转出金额
-    "withdraw": lambda x: 0.0,
-    # 总资产
-    "asset": "total_asset",
-    # 净资产
-    "nav": "total_asset",
-    # 总负债
-    "debt": lambda x: 0.0,
-    # 资金余额
-    "balance": lambda x: x.cash + x.frozen_cash,
-    # 冻结金额
-    "frozen": "frozen_cash",
-    # 可用金额
-    "available": "cash",
-    # 融资融券可用
-    "margin_available": lambda x: 0.0,
-    # 总市值
-    "marketvalue": "market_value",
-    # 今日盈利
-    "today_profit": lambda x: 0.0,
-    # 浮动盈亏
-    "fnl": lambda x: 0.0,
-    # 基金份额
-    "fund_shares": "total_asset",
-    # 基金净值估算
-    "fund_nav": lambda x: 1.0,
-    # 昨日总资产
-    "asset_yd": "total_asset",
-    # 昨日净资产
-    "nav_yd": "total_asset",
-    # 昨日基金金额
-    "fund_nav_yd": lambda x: 1.0,
-    # 最近结算日
-    "settle_day": lambda: vxtime.today("23:59:59") - 24 * 60 * 60,
-    # 下单channel
-    "channel": lambda x: "",
-}
-
-qmtAccountInfoConvter = vxDataConvertor(vxAccountInfo, ACCOUNTINFO_CONVERTORS)
+""" QMT量化数据转换至vxFinDataModel数据的转换器 """
+
+import uuid
+from vxutils import combine_datetime, to_timestring, vxtime, vxDataConvertor, to_text
+
+from vxquant.model.exchange import (
+    vxCashPosition,
+    vxTick,
+    vxBar,
+    vxPosition,
+    vxOrder,
+    vxTrade,
+    vxAccountInfo,
+)
+from vxquant.model.preset import vxMarketPreset
+from vxquant.model.nomalize import to_symbol
+
+__all__ = [
+    "qmtTickConvter",
+    # "qmtBarConvter",
+    "qmtAccountInfoConvter",
+    "qmtCashPositionConvter",
+    "qmtPositionConvter",
+    "qmtOrderConvter",
+    "qmtTradeConvter",
+]
+
+
+TICK_CONVERTORS = {
+    # 证券标的
+    "symbol": "symbol",
+    # 开盘价
+    "open": "open",
+    # 最高价
+    "high": "high",
+    # 最低价
+    "low": "low",
+    # 最近成交价
+    "lasttrade": "lastPrice",
+    # 昨日收盘价
+    "yclose": "lastClose",
+    # 成交量
+    "volume": "volume",
+    # 成交金额
+    "amount": "amount",
+    # 换手率
+    "turnoverratio": lambda x: 0.0,
+    # 卖1量
+    "bid1_v": lambda x: x["bidVol"][0],
+    # 卖1价
+    "bid1_p": lambda x: x["bidPrice"][0],
+    # 卖2量
+    "bid2_v": lambda x: x["bidVol"][1],
+    # 卖2价
+    "bid2_p": lambda x: x["bidPrice"][1],
+    # 卖3量
+    "bid3_v": lambda x: x["bidVol"][2],
+    # 卖3价
+    "bid3_p": lambda x: x["bidPrice"][2],
+    # 卖4量
+    "bid4_v": lambda x: x["bidVol"][3],
+    # 卖4价
+    "bid4_p": lambda x: x["bidPrice"][3],
+    # 卖5量
+    "bid5_v": lambda x: x["bidVol"][4],
+    # 卖5价
+    "bid5_p": lambda x: x["bidPrice"][4],
+    # 买1量
+    "ask1_v": lambda x: x["askVol"][0],
+    # 买1价
+    "ask1_p": lambda x: x["askPrice"][0],
+    # 买2量
+    "ask2_v": lambda x: x["askVol"][1],
+    # 买2价
+    "ask2_p": lambda x: x["askPrice"][1],
+    # 买3量
+    "ask3_v": lambda x: x["askVol"][2],
+    # 买3价
+    "ask3_p": lambda x: x["askPrice"][2],
+    # 买4量
+    "ask4_v": lambda x: x["askVol"][3],
+    # 买4价
+    "ask4_p": lambda x: x["askPrice"][3],
+    # 买5量
+    "ask5_v": lambda x: x["askVol"][4],
+    # 买5价
+    "ask5_p": lambda x: x["askPrice"][4],
+    # 持仓量
+    "interest": "openInt",
+    # 停牌状态
+    "status": lambda x: "NORMAL",
+    # 创建时间
+    "created_dt": "timetag",
+    # 更新时间
+    "updated_dt": "timetag",
+}
+
+qmtTickConvter = vxDataConvertor(vxTick, TICK_CONVERTORS)
+
+
+def _to_order_direction(other_data):
+    return "Buy" if other_data.order_type in (23, 27, 40) else "Sell"
+
+
+def _to_order_offset(other_data):
+    return "Open" if other_data.order_type in (23, 27, 40) else "Close"
+
+
+def _to_order_type(other_data):
+    return "Limit" if other_data.price_type in (11,) else "Market"
+
+
+def _to_order_status(other_data):
+    order_code = other_data.order_status
+    if order_code in (48, 49):
+        return "PendingNew"
+    elif order_code in (50, 51):
+        return "New"
+    elif order_code in (52, 55):
+        return "PartiallyFilled"
+    elif order_code in (53, 54):
+        return "Canceled"
+    elif order_code in (56,):
+        return "Filled"
+    elif order_code in (57,):
+        return "Rejected"
+    else:
+        return "Unknown"
+
+
+ORDER_CONVERTORS = {
+    # 账号id
+    "account_id": "account_id",
+    # 委托id
+    "order_id": lambda x: x.order_remark + x.strategy_name,
+    # 算法委托id
+    "algo_order_id": "",
+    # 交易所委托id
+    "exchange_order_id": lambda x: f"qmt_{x.order_id}",
+    # 冻结持仓id
+    "frozen_position_id": lambda x: "",
+    # 证券代码
+    "symbol": "stock_code",
+    # 买卖方向
+    "order_direction": _to_order_direction,
+    # 开平仓标志
+    "order_offset": _to_order_offset,
+    # 订单类型
+    "order_type": _to_order_type,
+    # 委托数量
+    "volume": "order_volume",
+    # 委托价格
+    "price": "price",
+    # 成交数量
+    "filled_volume": "traded_volume",
+    # 成交均价
+    "filled_vwap": "trade_price",
+    # 成交总额（含手续费）
+    "filled_amount": lambda x: x.traded_volume * x.traded_price,
+    # 订单状态
+    "status": _to_order_status,
+    # 订单超时时间
+    "due_dt": lambda x: combine_datetime(x.order_time, "15:00:00"),
+    # 拒绝代码
+    "reject_code": "status_msg",
+    # 拒绝原因
+    "reject_reason": "status_msg",
+    # 创建时间
+    "created_dt": "order_time",
+    # 更新时间
+    "updated_dt": "order_time",
+}
+
+
+qmtOrderConvter = vxDataConvertor(vxOrder, ORDER_CONVERTORS)
+
+
+TRADE_CONVERTORS = {
+    # 账户id
+    "account_id": "account_id",
+    # 委托id
+    "order_id": lambda x: x.order_remark + x.strategy_name,
+    # 交易所委托id
+    "exchange_order_id": lambda x: f"qmt_{x.order_id}",
+    # 成交id
+    "trade_id": "traded_id",
+    # 证券代码
+    "symbol": "stock_code",
+    # 买卖方向
+    "order_direction": _to_order_direction,
+    # 开平仓标志
+    "order_offset": _to_order_offset,
+    # 成交价格
+    "price": "traded_price",
+    # 成交数量
+    "volume": "traded_volume",
+    # 交易佣金
+    "commission": lambda x: x.traded_amount - x.traded_price * x.traded_volume,
+    # 成交状态
+    "status": lambda x: "Trade" if x.traded_volume > 0 else "Unknown",
+    # 拒绝代码
+    "reject_code": lambda x: "Unkown",
+    # 拒绝原因
+    "reject_reason": lambda x: "",
+    # 成交时间
+    "created_dt": "trade_time",
+    # 更新时间
+    "updated_dt": "trade_time",
+}
+
+qmtTradeConvter = vxDataConvertor(vxTrade, TRADE_CONVERTORS)
+
+
+POSITION_CONVERTORS = {
+    # 组合ID
+    "portfolio_id": lambda x: "",
+    # 账户id
+    "account_id": "account_id",
+    # 仓位id
+    "position_id": lambda x: str(uuid.uuid4()),
+    # 证券类型
+    "security_type": lambda x: vxMarketPreset(to_symbol(x.stock_code)).security_type,
+    # 证券代码
+    "symbol": "stock_code",
+    # 持仓方向
+    "position_side": lambda x: "Long",
+    # 今日持仓数量
+    "volume_today": lambda x: x.volume - x.frozen_volume - x.can_use_volume,
+    # 昨日持仓数量
+    "volume_his": lambda x: x.frozen_volume + x.can_use_volume,
+    # 持仓数量 --- 自动计算字段，由 volume_today + volume_his 计算所得
+    "volume": "volume",
+    # 冻结数量
+    "frozen": lambda x: x.volume - x.can_use_volume,
+    # 可用数量  --- 自动计算字段，由 volume - frozen计算
+    "available": "can_use_volume",
+    # 持仓市值
+    "marketvalue": "market_value",
+    # 持仓成本
+    "cost": lambda x: x.open_price * x.volume,
+    # 浮动盈利
+    "fnl": lambda x: x.market_value - x.open_price * x.volume,
+    # 持仓成本均价
+    "vwap": "open_price",
+    # 最近成交价
+    "lasttrade": lambda x: x.market_value / x.volume,
+    # 是否T0
+    "allow_t0": lambda x: vxMarketPreset(to_symbol(x.stock_code)).allow_t0,
+}
+
+qmtPositionConvter = vxDataConvertor(vxPosition, POSITION_CONVERTORS)
+
+CASHPOSITION_CONVERTORS = {
+    # 组合ID
+    "portfolio_id": lambda x: "",
+    # 账户id
+    "account_id": "account_id",
+    # 仓位id
+    "position_id": lambda x: str(uuid.uuid4()),
+    # 证券类型
+    "security_type": lambda x: "CASH",
+    # 证券代码
+    "symbol": lambda x: "CNY",
+    # 持仓方向
+    "position_side": lambda x: "Long",
+    # 今日持仓数量
+    "volume_today": "frozen_cash",
+    # 昨日持仓数量
+    "volume_his": "cash",
+    # 持仓数量
+    "volume": lambda x: x.frozen_cash + x.cash,
+    # 冻结数量
+    "frozen": "frozen_cash",
+    # 可用数量
+    "available": "cash",
+    # 持仓市值
+    "marketvalue": lambda x: x.frozen_cash + x.cash,
+    # 持仓成本
+    "cost": lambda x: x.frozen_cash + x.cash,
+    # 浮动盈利
+    "fnl": lambda x: 0.0,
+    # 持仓成本均价
+    "vwap": lambda x: 1.0,
+    # 最近成交价
+    "lasttrade": lambda x: 1.0,
+    # 是否T0
+    "allow_t0": lambda x: True,
+}
+
+qmtCashPositionConvter = vxDataConvertor(vxCashPosition, CASHPOSITION_CONVERTORS)
+
+ACCOUNTINFO_CONVERTORS = {
+    # 组合ID
+    "portfolio_id": lambda x: "",
+    # 账户id
+    "account_id": "account_id",
+    # 账户币种
+    "currency": lambda x: "CNY",
+    # 今日转入金额
+    "deposit": lambda x: 0.0,
+    # 今日转出金额
+    "withdraw": lambda x: 0.0,
+    # 总资产
+    "asset": "total_asset",
+    # 净资产
+    "nav": "total_asset",
+    # 总负债
+    "debt": lambda x: 0.0,
+    # 资金余额
+    "balance": lambda x: x.cash + x.frozen_cash,
+    # 冻结金额
+    "frozen": "frozen_cash",
+    # 可用金额
+    "available": "cash",
+    # 融资融券可用
+    "margin_available": lambda x: 0.0,
+    # 总市值
+    "marketvalue": "market_value",
+    # 今日盈利
+    "today_profit": lambda x: 0.0,
+    # 浮动盈亏
+    "fnl": lambda x: 0.0,
+    # 基金份额
+    "fund_shares": "total_asset",
+    # 基金净值估算
+    "fund_nav": lambda x: 1.0,
+    # 昨日总资产
+    "asset_yd": "total_asset",
+    # 昨日净资产
+    "nav_yd": "total_asset",
+    # 昨日基金金额
+    "fund_nav_yd": lambda x: 1.0,
+    # 最近结算日
+    "settle_day": lambda: vxtime.today("23:59:59") - 24 * 60 * 60,
+    # 下单channel
+    "channel": lambda x: "",
+}
+
+qmtAccountInfoConvter = vxDataConvertor(vxAccountInfo, ACCOUNTINFO_CONVERTORS)
```

### Comparing `vxquant-2023.3.1/src/vxquant/model/tools/tdxData.py` & `vxquant-2023.4.1/src/vxquant/model/tools/tdxData.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,166 @@
-# encoding=utf8
-""" 通达信数据转换 """
-import datetime
-from enum import Enum
-from pytdx.hq import TDXParams
-from vxutils.dataclass import vxDataConvertor
-from vxquant.model.exchange import vxTick, vxBar
-from vxquant.model.preset import vxMarketPreset
-from vxquant.model.contants import SecType
-
-
-class TdxExchange(Enum):
-    """通达信交易所代码"""
-
-    SHSE = TDXParams.MARKET_SH
-    SZSE = TDXParams.MARKET_SZ
-    BJSE = 2
-
-
-# * #####################################################################
-# * tdxTick的转换器
-# * #####################################################################
-TICK_TRANS = {
-    "volume": "vol",
-}
-
-
-def tdx_to_timestamp(tdx_timestamp, trade_day=None):
-    """通达信时间戳转换为时间戳"""
-    if trade_day is None:
-        trade_day = datetime.datetime.now()
-
-    tdx_timestamp = f"{tdx_timestamp:0>8}"
-    hour = int(tdx_timestamp[:2])
-    if hour < 0 or hour > 23:
-        tdx_timestamp = f"0{tdx_timestamp}"
-        hour = int(tdx_timestamp[:2])
-
-    minute = int(tdx_timestamp[2:4])
-    percent = float(f"0.{tdx_timestamp[2:]}")
-    if minute < 60:
-        second = int(percent * 60)
-        microsecond = int((percent * 60 - second) * 1000)
-    else:
-        minute = int(percent * 60)
-        second = int((percent * 60 - minute) * 60)
-        microsecond = int(((percent * 60 - minute) * 60 - second) * 1000)
-    return datetime.datetime(
-        trade_day.year,
-        trade_day.month,
-        trade_day.day,
-        hour,
-        minute,
-        second,
-        microsecond,
-    ).timestamp()
-
-
-def _quote_convter(cnt, volunit, price_unit=None):
-    if price_unit is None:
-        price_unit = volunit
-    return {
-        f"bid{cnt}_v": lambda x: x[f"bid_vol{cnt}"] * volunit,
-        f"bid{cnt}_p": lambda x: x[f"bid{cnt}"] / 100 * price_unit,
-        f"ask{cnt}_v": lambda x: x[f"ask_vol{cnt}"] * volunit,
-        f"ask{cnt}_p": lambda x: x[f"ask{cnt}"] / 100 * price_unit,
-    }
-
-
-# 非可转债转化
-TDX_STOCK_TICK_CONVERTORS = {
-    "volume": lambda x: x["vol"] * 100,
-    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
-    "yclose": lambda x: round(x["last_close"], 4),
-    "open": lambda x: round(x["open"], 4),
-    "high": lambda x: round(x["high"], 4),
-    "low": lambda x: round(x["low"], 4),
-    "lasttrade": lambda x: round(x["price"], 4) or round(x["last_close"], 4),
-    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
-}
-
-tdxStockTickConvter = vxDataConvertor(vxTick, TDX_STOCK_TICK_CONVERTORS)
-
-
-for i in range(1, 6):
-    for k, v in _quote_convter(i, 100).items():
-        tdxStockTickConvter.add_convertors(k, v)
-
-
-# 可转债转化
-TDX_CBOND_TICK_CONVERTORS = {
-    "volume": lambda x: x["vol"] * 100,
-    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
-    "yclose": lambda x: round(x["last_close"] / 100, 4),
-    "open": lambda x: round(x["open"] / 100, 4),
-    "high": lambda x: round(x["high"] / 100, 4),
-    "low": lambda x: round(x["low"] / 100, 4),
-    "lasttrade": lambda x: round(x["price"] / 100, 4)
-    or round(x["last_close"] / 100, 4),
-    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
-}
-
-tdxConBondTickConvter = vxDataConvertor(vxTick, TDX_CBOND_TICK_CONVERTORS)
-
-for i in range(1, 6):
-    for k, v in _quote_convter(i, 1).items():
-        tdxConBondTickConvter.add_convertors(k, v)
-
-
-# ETFLOF
-TDX_ETFLOF_TICK_CONVERTORS = {
-    "volume": lambda x: x["vol"] * 100,
-    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
-    "yclose": lambda x: round(x["last_close"] / 10, 4),
-    "open": lambda x: round(x["open"] / 10, 4),
-    "high": lambda x: round(x["high"] / 10, 4),
-    "low": lambda x: round(x["low"] / 10, 4),
-    "lasttrade": lambda x: round(x["price"] / 10, 4) or round(x["last_close"] / 100, 4),
-    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
-}
-tdxETFLOFTickConvter = vxDataConvertor(vxTick, TDX_ETFLOF_TICK_CONVERTORS)
-
-for i in range(1, 6):
-    for k, v in _quote_convter(i, 100, 10).items():
-        tdxETFLOFTickConvter.add_convertors(k, v)
-
-
-def tdxTickConvter(tdxtick, key=""):
-    """转化为vxtick格式
-
-    Arguments:
-        tdxtick {_type_} -- tdx tick格式
-    """
-
-    symbol = f"{TdxExchange(tdxtick['market']).name}.{tdxtick['code']}"
-    _preset = vxMarketPreset(symbol)
-
-    if _preset.security_type in (
-        SecType.BOND_CONVERTIBLE,
-        SecType.BOND,
-        SecType.REPO,
-    ):
-        return tdxConBondTickConvter(tdxtick, key="symbol")
-    elif _preset.security_type in (SecType.ETFLOF, SecType.CASH):
-        return tdxETFLOFTickConvter(tdxtick, key="symbol")
-    else:
-        return tdxStockTickConvter(tdxtick, key="symbol")
-
-
-# * #####################################################################
-# * tdxBar的转换器
-# * #####################################################################
-BAR_TRANS = {
-    "close": "price",
-    "volume": "vol",
-    "created_dt": "created_at",
-}
-
-
-# TDXParams.KLINE_TYPE_1MIN
-# TDXParams.KLINE_TYPE_DAILY
-
-tdxBarConvter = vxDataConvertor(vxBar, BAR_TRANS)
-# tdxBarConvter.add_convertors('created_at', lambda x: time.strptime(x['datetime'],'%Y-%m-%d %H:%M:%S')
-# tdxBarConvter.add_convertors('created_at', conveter_func)
+# encoding=utf8
+""" 通达信数据转换 """
+import datetime
+from enum import Enum
+from pytdx.hq import TDXParams
+from vxutils.dataclass import vxDataConvertor
+from vxquant.model.exchange import vxTick, vxBar
+from vxquant.model.preset import vxMarketPreset
+from vxquant.model.contants import SecType
+
+
+class TdxExchange(Enum):
+    """通达信交易所代码"""
+
+    SHSE = TDXParams.MARKET_SH
+    SZSE = TDXParams.MARKET_SZ
+    BJSE = 2
+
+
+# * #####################################################################
+# * tdxTick的转换器
+# * #####################################################################
+TICK_TRANS = {
+    "volume": "vol",
+}
+
+
+def tdx_to_timestamp(tdx_timestamp, trade_day=None):
+    """通达信时间戳转换为时间戳"""
+    if trade_day is None:
+        trade_day = datetime.datetime.now()
+
+    tdx_timestamp = f"{tdx_timestamp:0>8}"
+    hour = int(tdx_timestamp[:2])
+    if hour < 0 or hour > 23:
+        tdx_timestamp = f"0{tdx_timestamp}"
+        hour = int(tdx_timestamp[:2])
+
+    minute = int(tdx_timestamp[2:4])
+    percent = float(f"0.{tdx_timestamp[2:]}")
+    if minute < 60:
+        second = int(percent * 60)
+        microsecond = int((percent * 60 - second) * 1000)
+    else:
+        minute = int(percent * 60)
+        second = int((percent * 60 - minute) * 60)
+        microsecond = int(((percent * 60 - minute) * 60 - second) * 1000)
+    return datetime.datetime(
+        trade_day.year,
+        trade_day.month,
+        trade_day.day,
+        hour,
+        minute,
+        second,
+        microsecond,
+    ).timestamp()
+
+
+def _quote_convter(cnt, volunit, price_unit=None):
+    if price_unit is None:
+        price_unit = volunit
+    return {
+        f"bid{cnt}_v": lambda x: x[f"bid_vol{cnt}"] * volunit,
+        f"bid{cnt}_p": lambda x: x[f"bid{cnt}"] / 100 * price_unit,
+        f"ask{cnt}_v": lambda x: x[f"ask_vol{cnt}"] * volunit,
+        f"ask{cnt}_p": lambda x: x[f"ask{cnt}"] / 100 * price_unit,
+    }
+
+
+# 非可转债转化
+TDX_STOCK_TICK_CONVERTORS = {
+    "volume": lambda x: x["vol"] * 100,
+    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
+    "yclose": lambda x: round(x["last_close"], 4),
+    "open": lambda x: round(x["open"], 4),
+    "high": lambda x: round(x["high"], 4),
+    "low": lambda x: round(x["low"], 4),
+    "lasttrade": lambda x: round(x["price"], 4) or round(x["last_close"], 4),
+    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
+}
+
+tdxStockTickConvter = vxDataConvertor(vxTick, TDX_STOCK_TICK_CONVERTORS)
+
+
+for i in range(1, 6):
+    for k, v in _quote_convter(i, 100).items():
+        tdxStockTickConvter.add_convertors(k, v)
+
+
+# 可转债转化
+TDX_CBOND_TICK_CONVERTORS = {
+    "volume": lambda x: x["vol"] * 100,
+    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
+    "yclose": lambda x: round(x["last_close"] / 100, 4),
+    "open": lambda x: round(x["open"] / 100, 4),
+    "high": lambda x: round(x["high"] / 100, 4),
+    "low": lambda x: round(x["low"] / 100, 4),
+    "lasttrade": lambda x: round(x["price"] / 100, 4) or round(
+        x["last_close"] / 100, 4
+    ),
+    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
+}
+
+tdxConBondTickConvter = vxDataConvertor(vxTick, TDX_CBOND_TICK_CONVERTORS)
+
+for i in range(1, 6):
+    for k, v in _quote_convter(i, 1).items():
+        tdxConBondTickConvter.add_convertors(k, v)
+
+
+# ETFLOF
+TDX_ETFLOF_TICK_CONVERTORS = {
+    "volume": lambda x: x["vol"] * 100,
+    "symbol": lambda x: f"{TdxExchange(x['market']).name}.{x['code']}",
+    "yclose": lambda x: round(x["last_close"] / 10, 4),
+    "open": lambda x: round(x["open"] / 10, 4),
+    "high": lambda x: round(x["high"] / 10, 4),
+    "low": lambda x: round(x["low"] / 10, 4),
+    "lasttrade": lambda x: round(x["price"] / 10, 4) or round(x["last_close"] / 100, 4),
+    "created_dt": lambda x: tdx_to_timestamp(x["reversed_bytes0"]),
+}
+tdxETFLOFTickConvter = vxDataConvertor(vxTick, TDX_ETFLOF_TICK_CONVERTORS)
+
+for i in range(1, 6):
+    for k, v in _quote_convter(i, 100, 10).items():
+        tdxETFLOFTickConvter.add_convertors(k, v)
+
+
+def tdxTickConvter(tdxtick, key=""):
+    """转化为vxtick格式
+
+    Arguments:
+        tdxtick {_type_} -- tdx tick格式
+    """
+
+    symbol = f"{TdxExchange(tdxtick['market']).name}.{tdxtick['code']}"
+    _preset = vxMarketPreset(symbol)
+
+    if _preset.security_type in (
+        SecType.BOND_CONVERTIBLE,
+        SecType.BOND,
+        SecType.REPO,
+    ):
+        return tdxConBondTickConvter(tdxtick, key="symbol")
+    elif _preset.security_type in (SecType.ETFLOF, SecType.CASH):
+        return tdxETFLOFTickConvter(tdxtick, key="symbol")
+    else:
+        return tdxStockTickConvter(tdxtick, key="symbol")
+
+
+# * #####################################################################
+# * tdxBar的转换器
+# * #####################################################################
+BAR_TRANS = {
+    "close": "price",
+    "volume": "vol",
+    "created_dt": "created_at",
+}
+
+
+# TDXParams.KLINE_TYPE_1MIN
+# TDXParams.KLINE_TYPE_DAILY
+
+tdxBarConvter = vxDataConvertor(vxBar, BAR_TRANS)
+# tdxBarConvter.add_convertors('created_at', lambda x: time.strptime(x['datetime'],'%Y-%m-%d %H:%M:%S')
+# tdxBarConvter.add_convertors('created_at', conveter_func)
```

### Comparing `vxquant-2023.3.1/src/vxquant/modules/agent/__main__.py` & `vxquant-2023.4.1/src/vxquant/modules/agent/__main__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""各类组件启动程序"""
-
-import os
-import sys
-import subprocess
-import argparse
-from vxsched import vxContext
-from vxutils import storage, vxtime, logger
-
-
-@storage("agent", "gmagent")
-def run_gmagent(config: str, mod_path: str) -> None:
-    """启动gmagent
-
-    Arguments:
-        config {str} -- 配置文件
-        mod_path {str} -- 模块地址
-    """
-    os.makedirs("etc/", exist_ok=True)
-    context = vxContext.load_json(config)
-    _ENV = os.environ.copy()
-    _ENV.update(
-        {
-            "GMCONFIGFILE": config,
-            "STRATEGYMOD": mod_path,
-            "gm_strategyid": context.settings.gm_strategyid,
-            "gm_token": context.settings.gm_token,
-            "mode": "LIVING",
-        }
-    )
-    while True:
-        if vxtime.now() < vxtime.today("09:09:00"):
-            logger.info("休眠等待第二天开盘时间.")
-            vxtime.sleep(vxtime.today("09:10:00") - vxtime.now())
-        elif vxtime.now() < vxtime.today("15:30:00"):
-            try:
-                subprocess.run(
-                    [sys.executable, "-m", "vxquant.agent.gmagent"],
-                    env=_ENV,
-                    shell=True,
-                    check=True,
-                )
-
-                vxtime.sleep(1)
-            except subprocess.CalledProcessError as e:
-                logger.warning(f"运行时错误: {e}")
-
-        else:
-            logger.info("休眠等待第二天开盘时间.")
-            vxtime.sleep(vxtime.today("09:10:00") + 60 * 60 * 24 - vxtime.now())
-
-
-@storage("agent", "gmsimagent")
-def run_gmsimagent(config: str, mod_path: str) -> None:
-    """启动gmsimagent"""
-    os.makedirs("etc/", exist_ok=True)
-    context = vxContext.load_json(config)
-    _ENV = os.environ.copy()
-    _ENV.update(
-        {
-            "GMCONFIGFILE": config,
-            "STRATEGYMOD": mod_path,
-            "gm_strategyid": context.settings.gm_strategyid,
-            "gm_token": context.settings.gm_token,
-            "mode": "SIM24",
-        }
-    )
-
-    subprocess.run(
-        [sys.executable, "-m", "vxquant.agent.gmagent"],
-        env=_ENV,
-        shell=True,
-        check=True,
-    )
-
-
-@storage("agent", "qmtagent")
-def run_qmtagent(config: str, mod_path: str) -> None:
-    """启动qmtagent"""
-    from vxquant.agent.qmtagent import run_qmtagent
-
-    while True:
-        if vxtime.now() < vxtime.today("09:09:00"):
-            logger.info("休眠等待第二天开盘时间.")
-            vxtime.sleep(vxtime.today("09:10:00") - vxtime.now())
-        elif vxtime.now() < vxtime.today("15:30:00"):
-            try:
-                subprocess.run(
-                    [
-                        sys.executable,
-                        "-m",
-                        "vxquant.agent.qmtagent",
-                        "-c",
-                        config,
-                        "-m",
-                        mod_path,
-                    ],
-                    shell=True,
-                    check=True,
-                )
-                vxtime.sleep(1)
-            except subprocess.CalledProcessError as e:
-                logger.warning(f"运行时错误: {e}")
-
-        else:
-            logger.info("休眠等待第二天开盘时间.")
-            vxtime.sleep(vxtime.today("09:10:00") + 60 * 60 * 24 - vxtime.now())
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="""trade agent server""")
-    parser.add_argument("-s", "--script", help="启动组件", default="gmagent")
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="path to config json file",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    func = storage.get("agent", args.script)
-
-    if callable(func):
-        func(args.config, args.mod)
+"""各类组件启动程序"""
+
+import os
+import sys
+import subprocess
+import argparse
+from vxsched import vxContext
+from vxutils import storage, vxtime, logger
+
+
+@storage("agent", "gmagent")
+def run_gmagent(config: str, mod_path: str) -> None:
+    """启动gmagent
+
+    Arguments:
+        config {str} -- 配置文件
+        mod_path {str} -- 模块地址
+    """
+    os.makedirs("etc/", exist_ok=True)
+    context = vxContext.load_json(config)
+    _ENV = os.environ.copy()
+    _ENV.update(
+        {
+            "GMCONFIGFILE": config,
+            "STRATEGYMOD": mod_path,
+            "gm_strategyid": context.settings.gm_strategyid,
+            "gm_token": context.settings.gm_token,
+            "mode": "LIVING",
+        }
+    )
+    while True:
+        if vxtime.now() < vxtime.today("09:09:00"):
+            logger.info("休眠等待第二天开盘时间.")
+            vxtime.sleep(vxtime.today("09:10:00") - vxtime.now())
+        elif vxtime.now() < vxtime.today("15:30:00"):
+            try:
+                subprocess.run(
+                    [sys.executable, "-m", "vxquant.agent.gmagent"],
+                    env=_ENV,
+                    shell=True,
+                    check=True,
+                )
+
+                vxtime.sleep(1)
+            except subprocess.CalledProcessError as e:
+                logger.warning(f"运行时错误: {e}")
+
+        else:
+            logger.info("休眠等待第二天开盘时间.")
+            vxtime.sleep(vxtime.today("09:10:00") + 60 * 60 * 24 - vxtime.now())
+
+
+@storage("agent", "gmsimagent")
+def run_gmsimagent(config: str, mod_path: str) -> None:
+    """启动gmsimagent"""
+    os.makedirs("etc/", exist_ok=True)
+    context = vxContext.load_json(config)
+    _ENV = os.environ.copy()
+    _ENV.update(
+        {
+            "GMCONFIGFILE": config,
+            "STRATEGYMOD": mod_path,
+            "gm_strategyid": context.settings.gm_strategyid,
+            "gm_token": context.settings.gm_token,
+            "mode": "SIM24",
+        }
+    )
+
+    subprocess.run(
+        [sys.executable, "-m", "vxquant.agent.gmagent"],
+        env=_ENV,
+        shell=True,
+        check=True,
+    )
+
+
+@storage("agent", "qmtagent")
+def run_qmtagent(config: str, mod_path: str) -> None:
+    """启动qmtagent"""
+    from vxquant.agent.qmtagent import run_qmtagent
+
+    while True:
+        if vxtime.now() < vxtime.today("09:09:00"):
+            logger.info("休眠等待第二天开盘时间.")
+            vxtime.sleep(vxtime.today("09:10:00") - vxtime.now())
+        elif vxtime.now() < vxtime.today("15:30:00"):
+            try:
+                subprocess.run(
+                    [
+                        sys.executable,
+                        "-m",
+                        "vxquant.agent.qmtagent",
+                        "-c",
+                        config,
+                        "-m",
+                        mod_path,
+                    ],
+                    shell=True,
+                    check=True,
+                )
+                vxtime.sleep(1)
+            except subprocess.CalledProcessError as e:
+                logger.warning(f"运行时错误: {e}")
+
+        else:
+            logger.info("休眠等待第二天开盘时间.")
+            vxtime.sleep(vxtime.today("09:10:00") + 60 * 60 * 24 - vxtime.now())
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="""trade agent server""")
+    parser.add_argument("-s", "--script", help="启动组件", default="gmagent")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="path to config json file",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    func = storage.get("agent", args.script)
+
+    if callable(func):
+        func(args.config, args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxquant/modules/broker/__main__.py` & `vxquant-2023.4.1/src/vxquant/scripts/broker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,266 +1,255 @@
-""" run zmq broker"""
-
-import zmq
-import argparse
-import pathlib
-
-from itertools import chain
-from vxutils import logger
-from concurrent.futures import ThreadPoolExecutor
-from multiprocessing import Lock
-from vxquant.broker.utils import init_socket, frontend_reply, backend_publish
-from vxutils.zmqsocket import zmq_pipe
-from vxsched import vxscheduler, vxContext, vxEvent
-
-
-_default_broker_config = {
-    "settings": {
-        "frontend": {
-            "addr": "tcp://127.0.0.1:5555",
-            "public_key": "",
-            "connect_mode": "bind",
-        },
-        "backend": {
-            "addr": "tcp://127.0.0.1:6666",
-            "public_key": "",
-            "connect_mode": "bind",
-        },
-        "events": {},
-    },
-    "params": {},
-    "rpc_methods": {},
-}
-
-
-def on_recv_frontend_msgs(context, msgs):
-    """处理前端消息
-
-    Arguments:
-        context {vxContext} -- context上下文
-        msgs {[client_addr, b'',packed_event]} -- 收到前端消息清单
-
-    前端消息: channel 为：__BROKER__/gateway ————> vxscheduler.submit_event(event)
-             channel为: __RPC__  ----> vxscheduler.submit
-    """
-    client_addr, empty, packed_event = msgs
-    assert empty == b""
-    event = vxEvent.unpack(packed_event)
-    logger.debug(f"frontend 收到来自 {client_addr} 消息: {event}")
-    if event.channel == "__BROKER__":
-        event.reply_to = client_addr
-        vxscheduler.submit_event(event)
-    elif event.channel == "__RPC__":
-        if event.type not in context.rpc_methods:
-            frontend_reply(
-                context,
-                vxEvent(
-                    type="__RPC_REPLY__",
-                    data=AttributeError(f"不支持的远程调用方法: {event.type}"),
-                    channel=client_addr,
-                ),
-            )
-        event.reply_to = client_addr
-        event.channel = context.rpc_methods[event.type]
-        backend_publish(context, event)
-    elif event.type.startswith("_"):
-        frontend_reply(
-            context,
-            vxEvent(
-                type="__ACK__",
-                data=ValueError(f"not suport event.type({event.type})"),
-                channel=client_addr,
-            ),
-        )
-    else:
-        event.reply_to = ""
-        backend_publish(context, event)
-        frontend_reply(context, vxEvent(type="__ACK__", data="OK", channel=client_addr))
-
-
-def on_recv_backend_msgs(context, msgs):
-    try:
-        if msgs[0].startswith(b"\x01"):
-            vxscheduler.submit_event(
-                vxEvent(
-                    type="__ON_SUBSCRIBE__",
-                    data=msgs[0][1:].decode("ascii"),
-                    channel="__BROKER__",
-                )
-            )
-            return
-
-        if msgs[0].startswith(b"\x00"):
-            vxscheduler.submit_event(
-                vxEvent(
-                    type="__ON_UNSUBSCRIBE__",
-                    data=msgs[0][1:].decode("ascii"),
-                    channel="__BROKER__",
-                )
-            )
-            return
-
-        _, packed_event = msgs
-        event = vxEvent.unpack(packed_event)
-        if event.channel == "__BROKER__":
-            vxscheduler.submit_event(event)
-        elif event.channel:
-            frontend_reply(context, event)
-        else:
-            logger.warning(f"收到错误消息: {event}")
-
-    except Exception as e:
-        logger.error(f"error: {e}", exc_info=True)
-
-
-def on_recv_frontend_recver_msgs(context, msgs):
-    context.frontend.send_multipart(msgs)
-
-
-def on_recv_backend_recver_msgs(context, msgs):
-    context.backend.send_multipart(msgs)
-
-
-def run_broker(config: str = "etc/broker.json", mod_path: str = "mod/"):
-    if pathlib.Path(config).is_file():
-        context = vxContext.load_json(config, _default_broker_config)
-        logger.info(f"加载配置文件: {config} 完成")
-    else:
-        context = vxContext(_default_broker_config)
-        logger.info("使用缺省的配置项")
-
-    context.lock = Lock()
-    context.rpc_methods = {}
-
-    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
-        vxscheduler.load_modules(
-            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
-        )
-
-    if mod_path and pathlib.Path(mod_path).is_dir():
-        vxscheduler.load_modules(mod_path)
-
-    vxscheduler.start(
-        context=context, executor=ThreadPoolExecutor(thread_name_prefix="broker")
-    )
-
-    poller = zmq.Poller()
-
-    frontend = init_socket(zmq.ROUTER, context.settings.frontend)
-    context.frontend = frontend
-    recv_msg_handlers = {frontend: on_recv_frontend_msgs}
-    poller.register(frontend, zmq.POLLIN)
-
-    backend = init_socket(zmq.XPUB, context.settings.backend)
-    context.backend = backend
-    recv_msg_handlers[backend] = on_recv_backend_msgs
-    poller.register(backend, zmq.POLLIN)
-
-    context.frontend_sender, frontend_recver = zmq_pipe()
-    recv_msg_handlers[frontend_recver] = on_recv_frontend_recver_msgs
-    poller.register(frontend_recver, zmq.POLLIN)
-
-    context.backend_sender, backend_recver = zmq_pipe()
-    recv_msg_handlers[backend_recver] = on_recv_backend_recver_msgs
-    poller.register(backend_recver, zmq.POLLIN)
-
-    while vxscheduler.is_alive():
-        flags = dict(poller.poll(1000))
-        for s in flags:
-            try:
-                msgs = s.recv_multipart()
-                recv_msg_handlers[s](context, msgs)
-            except Exception as err:
-                logger.error(f"socket ({s}) handler msg ({msgs}) error: {err}")
-
-
-@vxscheduler.event_handler("__ON_SUBSCRIBE__")
-def backend_on_subscribe(context, event) -> None:
-    """订阅事件触发"""
-    logger.error(f"收到订阅信息: {event.data} =====")
-    if event.data.startswith("rpc_"):
-        context.backend_queue.put_nowait(
-            vxEvent(
-                type="__GET_RPCMETHODS__", channel=event.data, reply_to="__BROKER__"
-            )
-        )
-
-
-@vxscheduler.event_handler("__ON_UNSUBSCRIBE__")
-def backend_on_unsubscribe(context, event) -> None:
-    logger.warning(f"取消订阅信息: {event.data}")
-    if event.data.startswith("rpc_"):
-        context.rpc_methods = {
-            method: channel
-            for method, channel in context.rpc_methods.items()
-            if channel != event.data
-        }
-
-
-def handle_subscribers(context, event) -> None:
-    """处理外部获取的消息"""
-
-    # logger.debug(f"开始抓取subscriber ({context.subscribers})中的消息")
-    if not context.subscribers:
-        return
-
-    events = [subscriber() for subscriber in context.subscribers]
-    for event in chain(*events):
-        context.event_queue.put_nowait(event)
-        logger.info(f"internal: 收到外部event : ({event.type})")
-
-    return
-
-
-@vxscheduler.event_handler("__GET_RPCMETHODS__")
-def frontend_handle_get_rpc_method(context, event):
-    """前端或许rpc methods"""
-    reply_event = vxEvent(
-        type="__GET_RPCMETHODS__",
-        data=context.rpc_methods,
-        channel=event.reply_to,
-    )
-    context.frontend_queue.put_nowait(reply_event)
-
-
-@vxscheduler.event_handler("__RPC_METHODS__")
-def backend_on_update_methods(context, event):
-    """更新rpc methods"""
-
-    if isinstance(event.data, Exception):
-        logger.warning(f"更新rpc methods 错误: {event.data}")
-    else:
-        logger.warning(f"更新rpc method: {event.data}")
-        context.rpc_methods.update(event.data)
-
-
-@vxscheduler.event_handler("__READY__")
-def frontend_ready_event(context, event):
-    """处理前端的ready消息"""
-    reply_event = vxEvent(
-        type="__ACK__",
-        data="OK",
-        channel=event.reply_to,
-    )
-    context.frontend_queue.put_nowait(reply_event)
-    logger.debug(f"发送frontend 消息: {reply_event}")
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="""broker server""")
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="path to config json file",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    run_broker(args.config, args.mod)
+""" run zmq broker"""
+
+import zmq
+import argparse
+
+import contextlib
+from collections.abc import Mapping
+
+from itertools import chain
+from queue import Queue, Empty
+from vxutils import logger, vxZMQContext, to_binary, storage, vxtime, vxWrapper
+
+from vxsched.core import vxengine
+from vxsched.triggers import vxDailyTrigger
+from vxsched.event import vxEvent, vxEventQueue
+
+
+def init_socket(socket_type, settings):
+    ctx = vxZMQContext().instance()
+    socket_ = ctx.socket(socket_type)
+    if settings["connect_mode"].lower() == "connect":
+        socket_.connect(settings["addr"], settings["public_key"])
+    else:
+        socket_.bind(settings["addr"], settings["public_key"])
+    return socket_
+
+
+def on_recv_frontend_msg(engine, msgs):
+    client_addr, empty, packed_event = msgs
+    assert empty == b""
+    event = vxEvent.unpack(packed_event)
+
+    context = engine.context
+    logger.debug(f"frontend 收到来自 {client_addr} 消息: {event}")
+    if event.channel == "__BROKER__":
+        event.reply_to = client_addr
+        engine.submit_event(event)
+    elif event.channel == "__RPC__":
+        if event.type in context.rpc_methods:
+            event.reply_to = client_addr
+            event.channel = context.rpc_methods[event.type]
+            context.backend_queue.put_nowait(event)
+        else:
+            context.frontend_queue.put_nowait(
+                vxEvent(
+                    type="__RPC_REPLY__",
+                    data=AttributeError(f"不支持的远程调用方法: {event.type}"),
+                    channel=client_addr,
+                )
+            )
+    elif event.type.startswith("_"):
+        context.frontend_queue.put_nowait(
+            vxEvent(
+                type="__ACK__",
+                data=ValueError(f"not suport event.type({event.type})"),
+                channel=client_addr,
+            )
+        )
+    else:
+        event.reply_to = ""
+        context.backend_queue.put_nowait(event)
+        context.frontend_queue.put_nowait(
+            vxEvent(type="__ACK__", data="OK", channel=client_addr)
+        )
+
+
+def on_recv_backend_msg(engine, msgs):
+    context = engine.context
+    try:
+        if msgs[0].startswith(b"\x01"):
+            engine.submit_event(
+                vxEvent(
+                    type="__ON_SUBSCRIBE__",
+                    data=msgs[0][1:].decode("ascii"),
+                    channel="__BROKER__",
+                )
+            )
+            return
+
+        if msgs[0].startswith(b"\x00"):
+            engine.submit_event(
+                vxEvent(
+                    type="__ON_UNSUBSCRIBE__",
+                    data=msgs[0][1:].decode("ascii"),
+                    channel="__BROKER__",
+                )
+            )
+            return
+
+        _, packed_event = msgs
+        event = vxEvent.unpack(packed_event)
+        if event.channel == "__BROKER__":
+            engine.submit_event(event)
+        elif event.channel:
+            context.frontend_queue.put(event)
+        else:
+            logger.warning(f"收到错误消息: {event}")
+
+    except Exception as e:
+        logger.error(f"error: {e}", exc_info=True)
+
+
+@vxengine.backend
+def run_broker_backend(engine):
+    context = engine.context
+    context.backend_queue = vxEventQueue()
+    context.frontend_queue = Queue()
+    context.rpc_methods = {}
+
+    for event_type, trigger_params in context.settings.events.items():
+        if isinstance(trigger_params, Mapping):
+            trigger = vxWrapper.init_by_config(trigger_params)
+        elif isinstance(trigger_params, str):
+            trigger = vxDailyTrigger(run_time=trigger_params)
+        else:
+            logger.error(f"不符合设置: {event_type} == {trigger_params}. ")
+        preset_event = vxEvent(type=event_type, trigger=trigger, channel="__BROKER__")
+        context.backend_queue.put(preset_event)
+        logger.info(f"提交预设事件: {preset_event}")
+
+    frontend = init_socket(zmq.ROUTER, context.settings.frontend)
+    backend = init_socket(zmq.XPUB, context.settings.backend)
+
+    poller = zmq.Poller()
+    poller.register(frontend, zmq.POLLIN | zmq.POLLOUT)
+    poller.register(backend, zmq.POLLIN | zmq.POLLOUT)
+
+    while engine.is_alive():
+        flags = dict(poller.poll(1000))
+
+        if frontend in flags and flags[frontend] & zmq.POLLIN != 0:
+            msgs = frontend.recv_multipart()
+            logger.debug(f"frontend msgs: {msgs}")
+            on_recv_frontend_msg(engine, msgs)
+
+        if backend in flags and flags[backend] & zmq.POLLIN != 0:
+            msgs = backend.recv_multipart()
+            logger.debug(f"backend msgs: {msgs}")
+            on_recv_backend_msg(engine, msgs)
+
+        if frontend in flags and flags[frontend] & zmq.POLLOUT != 0:
+            with contextlib.suppress(Empty):
+                event = context.frontend_queue.get(timeout=0.05)
+                frontend.send_multipart(
+                    [to_binary(event.channel), b"", vxEvent.pack(event)]
+                )
+                logger.debug(
+                    f"fronend 发送消息 {event.type} ({event.data})--> {event.channel}"
+                )
+
+        if backend in flags and flags[backend] & zmq.POLLOUT != 0:
+            with contextlib.suppress(Empty):
+                event = context.backend_queue.get(timeout=0.05)
+                backend.send_multipart([to_binary(event.channel), vxEvent.pack(event)])
+                logger.debug(
+                    f"backend 发送消息: {event.type} ({event.data}) --> {event.channel}"
+                )
+        # vxtime.sleep(0.1)
+
+
+@vxengine.event_handler("__ON_SUBSCRIBE__")
+def backend_on_subscribe(context, event) -> None:
+    """订阅事件触发"""
+    logger.error(f"收到订阅信息: {event.data} =====")
+    if event.data.startswith("rpc_"):
+        context.backend_queue.put_nowait(
+            vxEvent(
+                type="__GET_RPCMETHODS__", channel=event.data, reply_to="__BROKER__"
+            )
+        )
+
+
+@vxengine.event_handler("__ON_UNSUBSCRIBE__")
+def backend_on_unsubscribe(context, event) -> None:
+    logger.warning(f"取消订阅信息: {event.data}")
+    if event.data.startswith("rpc_"):
+        context.rpc_methods = {
+            method: channel
+            for method, channel in context.rpc_methods.items()
+            if channel != event.data
+        }
+
+
+def handle_subscribers(context, event) -> None:
+    """处理外部获取的消息"""
+
+    # logger.debug(f"开始抓取subscriber ({context.subscribers})中的消息")
+    if not context.subscribers:
+        return
+
+    events = [subscriber() for subscriber in context.subscribers]
+    for event in chain(*events):
+        context.event_queue.put_nowait(event)
+        logger.info(f"internal: 收到外部event : ({event.type})")
+
+    return
+
+
+@vxengine.event_handler("__GET_RPCMETHODS__")
+def frontend_handle_get_rpc_method(context, event):
+    """前端或许rpc methods"""
+    reply_event = vxEvent(
+        type="__GET_RPCMETHODS__",
+        data=context.rpc_methods,
+        channel=event.reply_to,
+    )
+    context.frontend_queue.put_nowait(reply_event)
+
+
+@vxengine.event_handler("__RPC_METHODS__")
+def backend_on_update_methods(context, event):
+    """更新rpc methods"""
+
+    if isinstance(event.data, Exception):
+        logger.warning(f"更新rpc methods 错误: {event.data}")
+    else:
+        logger.warning(f"更新rpc method: {event.data}")
+        context.rpc_methods.update(event.data)
+
+
+@vxengine.event_handler("__READY__")
+def frontend_ready_event(context, event):
+    """处理前端的ready消息"""
+    reply_event = vxEvent(
+        type="__ACK__",
+        data="OK",
+        channel=event.reply_to,
+    )
+    context.frontend_queue.put_nowait(reply_event)
+    logger.info(f"发送frontend 消息: {reply_event}")
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="""scheduler server""")
+    parser.add_argument("-s", "--script", help="启动组件", default="broker")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="path to config json file",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    func = storage.get("scheduler", args.script)
+
+    if callable(func):
+        func(args.config, args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxquant/modules/broker/mod/system.py` & `vxquant-2023.4.1/src/vxquant/modules/broker/mod/system.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from collections.abc import Mapping
-
-from vxsched.event import vxEvent
-from vxsched.core import vxscheduler
-from vxsched.triggers import vxDailyTrigger
-from vxutils import vxWrapper, logger, to_binary
-
-
-@vxscheduler.event_handler("__init__")
-def install_preset_event(context, event):
-    for event_type, trigger_params in context.settings.events.items():
-        if isinstance(trigger_params, Mapping):
-            trigger = vxWrapper.init_by_config(trigger_params)
-        elif isinstance(trigger_params, str):
-            trigger = vxDailyTrigger(run_time=trigger_params)
-        else:
-            logger.error(f"不符合设置: {event_type} == {trigger_params}. ")
-        preset_event = vxEvent(
-            type=send_backend_event,
-            data=event_type,
-            trigger=trigger,
-            channel="__BROKER__",
-        )
-        vxscheduler.submit_event(preset_event)
-        logger.info(f"提交预设事件: {preset_event.type} trigger dt {preset_event.trigger_dt}")
-
-
-@vxscheduler.event_handler("send_backend_event")
-def send_backend_event(context, event):
-    backend_event = vxEvent(type=event.data, channel="__BROKER__")
-    context.backend_sender.send_multipart(
-        [to_binary(backend_event.channel), vxEvent.pack(backend_event)]
-    )
+from collections.abc import Mapping
+
+from vxsched.event import vxEvent
+from vxsched.core import vxscheduler
+from vxsched.triggers import vxDailyTrigger
+from vxutils import vxWrapper, logger, to_binary
+
+
+@vxscheduler.event_handler("__init__")
+def install_preset_event(context, event):
+    for event_type, trigger_params in context.settings.events.items():
+        if isinstance(trigger_params, Mapping):
+            trigger = vxWrapper.init_by_config(trigger_params)
+        elif isinstance(trigger_params, str):
+            trigger = vxDailyTrigger(run_time=trigger_params)
+        else:
+            logger.error(f"不符合设置: {event_type} == {trigger_params}. ")
+        preset_event = vxEvent(
+            type=send_backend_event,
+            data=event_type,
+            trigger=trigger,
+            channel="__BROKER__",
+        )
+        vxscheduler.submit_event(preset_event)
+        logger.info(f"提交预设事件: {preset_event.type} trigger dt {preset_event.trigger_dt}")
+
+
+@vxscheduler.event_handler("send_backend_event")
+def send_backend_event(context, event):
+    backend_event = vxEvent(type=event.data, channel="__BROKER__")
+    context.backend_sender.send_multipart(
+        [to_binary(backend_event.channel), vxEvent.pack(backend_event)]
+    )
```

### Comparing `vxquant-2023.3.1/src/vxquant/modules/broker/utils.py` & `vxquant-2023.4.1/src/vxquant/modules/broker/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from vxutils import to_binary
-from vxutils.zmqsocket import vxZMQContext
-from vxsched import vxEvent
-
-
-def init_socket(socket_type, settings):
-    ctx = vxZMQContext().instance()
-    socket_ = ctx.socket(socket_type)
-    if settings["connect_mode"].lower() == "connect":
-        socket_.connect(settings["addr"], settings["public_key"])
-    else:
-        socket_.bind(settings["addr"], settings["public_key"])
-    return socket_
-
-
-def frontend_reply(context, reply_event):
-    with context.lock:
-        context.frontend_sender.send_multipart(
-            [to_binary(reply_event.channel), b"", vxEvent.pack(reply_event)]
-        )
-
-
-def backend_publish(context, publish_event):
-    with context.lock:
-        context.backend_sender.send_multipart(
-            [to_binary(publish_event.channel), vxEvent.pack(publish_event)]
-        )
+from vxutils import to_binary
+from vxutils.zmqsocket import vxZMQContext
+from vxsched import vxEvent
+
+
+def init_socket(socket_type, settings):
+    ctx = vxZMQContext().instance()
+    socket_ = ctx.socket(socket_type)
+    if settings["connect_mode"].lower() == "connect":
+        socket_.connect(settings["addr"], settings["public_key"])
+    else:
+        socket_.bind(settings["addr"], settings["public_key"])
+    return socket_
+
+
+def frontend_reply(context, reply_event):
+    with context.lock:
+        context.frontend_sender.send_multipart(
+            [to_binary(reply_event.channel), b"", vxEvent.pack(reply_event)]
+        )
+
+
+def backend_publish(context, publish_event):
+    with context.lock:
+        context.backend_sender.send_multipart(
+            [to_binary(publish_event.channel), vxEvent.pack(publish_event)]
+        )
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/ftp.py` & `vxquant-2023.4.1/src/vxquant/providers/ftp.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-"""ftp消息通道"""
-
-
-import io
-import pathlib
-from typing import List, Union, Optional
-
-from vxutils import logger, vxFTPConnector, vxtime
-from vxsched.event import vxEvent, vxTrigger
-from .base import vxPublisherProvider, vxSubscriberProvider
-
-
-def _to_event_rank(filename: str) -> tuple:
-    """转换为 (timestamp, filename)的组合"""
-    return float(pathlib.Path(filename).name.split("||")[0]), filename
-
-
-__all__ = ["vxFTPPublisherProvider", "vxFTPSubscriberProvider"]
-
-
-class vxFTPPublisherProvider(vxPublisherProvider):
-    """FTP发布器"""
-
-    _connections = {}
-
-    def __init__(
-        self,
-        channel_name="",
-        host: str = "",
-        port: int = 21,
-        user: str = "",
-        passwd: str = "",
-        root_dir="/",
-    ) -> None:
-        super().__init__(channel_name)
-
-        key = hash(f"ftp://{user}:{passwd}@{host}:{port}")
-        if key not in self.__class__._connections:
-            self.__class__._connections[key] = vxFTPConnector(host, port, user, passwd)
-            logger.info(f"创建FTP连接：{self.__class__._connections[key]}")
-        self._ftp_conn = self.__class__._connections[key]
-
-        self._remote_dir = pathlib.Path(root_dir, channel_name).as_posix()
-        self._root_dir = root_dir
-        logger.info(f"远程ftp目录: {self._remote_dir}")
-
-        self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
-        if self._remote_dir not in self._exists_remote_dirs:
-            logger.info(f"创建远程ftp目录: {self._remote_dir}")
-            self._ftp_conn.mkdir(self._remote_dir)
-            self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
-
-    @property
-    def channel_name(self) -> str:
-        """消息渠道名称"""
-        return self._channel_name
-
-    def __str__(self) -> str:
-        return (
-            f"< {self.__class__.__name__}({self.channel_name}) with {self._ftp_conn} on"
-            f" remote_dir: {self._remote_dir}"
-        )
-
-    def __eq__(self, __o: object) -> bool:
-        return (
-            self._channel_name == __o._channel_name
-            and self._ftp_conn == __o._ftp_conn
-            and self._remote_dir == __o._remote_dir
-            if isinstance(__o, self.__class__)
-            else False
-        )
-
-    def __call__(
-        self,
-        event: Union[str, vxEvent],
-        data="",
-        trigger: Optional[vxTrigger] = None,
-        priority: float = 10,
-        channel: str = None,
-        **kwargs,
-    ) -> None:
-        """发布消息
-
-        Arguments:
-            event {Union[str, vxEvent]} -- 要推送消息或消息类型
-            data {Any} -- 消息数据信息 (default: {None})
-            trigger {Optional[vxTrigger]} -- 消息触发器 (default: {None})
-            priority {int} -- 优先级，越小优先级越高 (default: {10})
-        """
-
-        if isinstance(event, str):
-            send_event = vxEvent(
-                type=event,
-                data=data,
-                trigger=trigger,
-                priority=priority,
-                **kwargs,
-            )
-
-        else:
-            send_event = event
-        send_event.channel = channel or self.channel_name
-        picked_event = vxEvent.pack(send_event)
-
-        remote_dir = pathlib.Path(self._root_dir, send_event.channel).as_posix()
-
-        if remote_dir not in self._exists_remote_dirs:
-            self._ftp_conn.mkdir(remote_dir)
-            logger.info(f"创建远程ftp目录: {remote_dir}")
-            self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
-
-        remote_file = pathlib.Path(
-            remote_dir,
-            f"{send_event.next_trigger_dt}____{send_event.id.replace('-','')}.pkl",
-        ).as_posix()
-
-        try:
-            with io.BytesIO(picked_event) as bfp:
-                self._ftp_conn.upload(bfp, remote_file)
-                logger.debug(
-                    f"{self} put event.type({send_event.type}) to"
-                    f" remote({remote_file}). {send_event}"
-                )
-
-        except Exception as err:
-            logger.error(
-                (
-                    f"{self} put event.type({send_event.type}) to"
-                    f" remote({remote_file}). error: {err}"
-                ),
-                exc_info=True,
-            )
-
-
-class vxFTPSubscriberProvider(vxSubscriberProvider):
-    """FTP消息订阅器"""
-
-    _connections = {}
-
-    def __init__(
-        self,
-        channel_name: str = "",
-        host: str = "",
-        port: int = 21,
-        user: str = "",
-        passwd: str = "",
-        root_dir="/",
-    ) -> None:
-        super().__init__(channel_name)
-
-        key = hash(f"ftp://{user}:{passwd}@{host}:{port}")
-        if key not in self.__class__._connections:
-            self.__class__._connections[key] = vxFTPConnector(host, port, user, passwd)
-            logger.info(f"创建FTP连接：{self.__class__._connections[key]}")
-        self._ftp_conn = self.__class__._connections[key]
-        self._remote_dir = pathlib.Path(root_dir, channel_name).as_posix()
-        self._ftp_conn.mkdir(self._remote_dir)
-        self._next_fetch_dt = 0
-        self._interval = 1
-
-    @property
-    def channel_name(self) -> str:
-        """消息渠道名称"""
-        return self._channel_name
-
-    def __str__(self) -> str:
-        return (
-            f"< {self.__class__.__name__}({self.channel_name}) with {self._ftp_conn} on"
-            f" remote_dir: {self._remote_dir}"
-        )
-
-    def __eq__(self, __o: object) -> bool:
-        return (
-            self._channel_name == __o._channel_name
-            and self._ftp_conn == __o._ftp_conn
-            and self._remote_dir == __o._remote_dir
-            if isinstance(__o, self.__class__)
-            else False
-        )
-
-    def __call__(self) -> List[vxEvent]:
-        now = vxtime.now()
-        if now > self._next_fetch_dt:
-            event_files = self._ftp_conn.list(self._remote_dir)
-            self._next_fetch_dt = now + self._interval
-            return [event for event in map(self._fetch_event, event_files) if event]
-
-        return []
-
-    def _fetch_event(self, event_file: str) -> vxEvent:
-        """获取单个event
-
-        Arguments:
-            event_file {str} -- event_file文件名称
-
-        Raises:
-            ConnectionError: 连接出错
-
-        Returns:
-            vxEvent -- vxEvent实例
-        """
-        with io.BytesIO() as bfp:
-            ftp_event_file = pathlib.Path(self._remote_dir, event_file).as_posix()
-
-            is_download = self._ftp_conn.download(ftp_event_file, bfp)
-            if is_download is False:
-                logger.error(f"ConnectionError: 下载{event_file}发生错误")
-                return None
-            event = vxEvent.unpack(bfp.getvalue())
-            self._ftp_conn.delete(ftp_event_file)
-            return event
+"""ftp消息通道"""
+
+
+import io
+import pathlib
+from typing import List, Union, Optional
+
+from vxutils import logger, vxFTPConnector, vxtime
+from vxsched.event import vxEvent, vxTrigger
+from .base import vxPublisherProvider, vxSubscriberProvider
+
+
+def _to_event_rank(filename: str) -> tuple:
+    """转换为 (timestamp, filename)的组合"""
+    return float(pathlib.Path(filename).name.split("||")[0]), filename
+
+
+__all__ = ["vxFTPPublisherProvider", "vxFTPSubscriberProvider"]
+
+
+class vxFTPPublisherProvider(vxPublisherProvider):
+    """FTP发布器"""
+
+    _connections = {}
+
+    def __init__(
+        self,
+        channel_name="",
+        host: str = "",
+        port: int = 21,
+        user: str = "",
+        passwd: str = "",
+        root_dir="/",
+    ) -> None:
+        super().__init__(channel_name)
+
+        key = hash(f"ftp://{user}:{passwd}@{host}:{port}")
+        if key not in self.__class__._connections:
+            self.__class__._connections[key] = vxFTPConnector(host, port, user, passwd)
+            logger.info(f"创建FTP连接：{self.__class__._connections[key]}")
+        self._ftp_conn = self.__class__._connections[key]
+
+        self._remote_dir = pathlib.Path(root_dir, channel_name).as_posix()
+        self._root_dir = root_dir
+        logger.info(f"远程ftp目录: {self._remote_dir}")
+
+        self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
+        if self._remote_dir not in self._exists_remote_dirs:
+            logger.info(f"创建远程ftp目录: {self._remote_dir}")
+            self._ftp_conn.mkdir(self._remote_dir)
+            self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
+
+    @property
+    def channel_name(self) -> str:
+        """消息渠道名称"""
+        return self._channel_name
+
+    def __str__(self) -> str:
+        return (
+            f"< {self.__class__.__name__}({self.channel_name}) with {self._ftp_conn} on"
+            f" remote_dir: {self._remote_dir}"
+        )
+
+    def __eq__(self, __o: object) -> bool:
+        return (
+            self._channel_name == __o._channel_name
+            and self._ftp_conn == __o._ftp_conn
+            and self._remote_dir == __o._remote_dir
+            if isinstance(__o, self.__class__)
+            else False
+        )
+
+    def __call__(
+        self,
+        event: Union[str, vxEvent],
+        data="",
+        trigger: Optional[vxTrigger] = None,
+        priority: float = 10,
+        channel: str = None,
+        **kwargs,
+    ) -> None:
+        """发布消息
+
+        Arguments:
+            event {Union[str, vxEvent]} -- 要推送消息或消息类型
+            data {Any} -- 消息数据信息 (default: {None})
+            trigger {Optional[vxTrigger]} -- 消息触发器 (default: {None})
+            priority {int} -- 优先级，越小优先级越高 (default: {10})
+        """
+
+        if isinstance(event, str):
+            send_event = vxEvent(
+                type=event,
+                data=data,
+                trigger=trigger,
+                priority=priority,
+                **kwargs,
+            )
+
+        else:
+            send_event = event
+        send_event.channel = channel or self.channel_name
+        picked_event = vxEvent.pack(send_event)
+
+        remote_dir = pathlib.Path(self._root_dir, send_event.channel).as_posix()
+
+        if remote_dir not in self._exists_remote_dirs:
+            self._ftp_conn.mkdir(remote_dir)
+            logger.info(f"创建远程ftp目录: {remote_dir}")
+            self._exists_remote_dirs = self._ftp_conn.list(self._root_dir)
+
+        remote_file = pathlib.Path(
+            remote_dir,
+            f"{send_event.next_trigger_dt}____{send_event.id.replace('-','')}.pkl",
+        ).as_posix()
+
+        try:
+            with io.BytesIO(picked_event) as bfp:
+                self._ftp_conn.upload(bfp, remote_file)
+                logger.debug(
+                    f"{self} put event.type({send_event.type}) to"
+                    f" remote({remote_file}). {send_event}"
+                )
+
+        except Exception as err:
+            logger.error(
+                (
+                    f"{self} put event.type({send_event.type}) to"
+                    f" remote({remote_file}). error: {err}"
+                ),
+                exc_info=True,
+            )
+
+
+class vxFTPSubscriberProvider(vxSubscriberProvider):
+    """FTP消息订阅器"""
+
+    _connections = {}
+
+    def __init__(
+        self,
+        channel_name: str = "",
+        host: str = "",
+        port: int = 21,
+        user: str = "",
+        passwd: str = "",
+        root_dir="/",
+    ) -> None:
+        super().__init__(channel_name)
+
+        key = hash(f"ftp://{user}:{passwd}@{host}:{port}")
+        if key not in self.__class__._connections:
+            self.__class__._connections[key] = vxFTPConnector(host, port, user, passwd)
+            logger.info(f"创建FTP连接：{self.__class__._connections[key]}")
+        self._ftp_conn = self.__class__._connections[key]
+        self._remote_dir = pathlib.Path(root_dir, channel_name).as_posix()
+        self._ftp_conn.mkdir(self._remote_dir)
+        self._next_fetch_dt = 0
+        self._interval = 1
+
+    @property
+    def channel_name(self) -> str:
+        """消息渠道名称"""
+        return self._channel_name
+
+    def __str__(self) -> str:
+        return (
+            f"< {self.__class__.__name__}({self.channel_name}) with {self._ftp_conn} on"
+            f" remote_dir: {self._remote_dir}"
+        )
+
+    def __eq__(self, __o: object) -> bool:
+        return (
+            self._channel_name == __o._channel_name
+            and self._ftp_conn == __o._ftp_conn
+            and self._remote_dir == __o._remote_dir
+            if isinstance(__o, self.__class__)
+            else False
+        )
+
+    def __call__(self) -> List[vxEvent]:
+        now = vxtime.now()
+        if now > self._next_fetch_dt:
+            event_files = self._ftp_conn.list(self._remote_dir)
+            self._next_fetch_dt = now + self._interval
+            return [event for event in map(self._fetch_event, event_files) if event]
+
+        return []
+
+    def _fetch_event(self, event_file: str) -> vxEvent:
+        """获取单个event
+
+        Arguments:
+            event_file {str} -- event_file文件名称
+
+        Raises:
+            ConnectionError: 连接出错
+
+        Returns:
+            vxEvent -- vxEvent实例
+        """
+        with io.BytesIO() as bfp:
+            ftp_event_file = pathlib.Path(self._remote_dir, event_file).as_posix()
+
+            is_download = self._ftp_conn.download(ftp_event_file, bfp)
+            if is_download is False:
+                logger.error(f"ConnectionError: 下载{event_file}发生错误")
+                return None
+            event = vxEvent.unpack(bfp.getvalue())
+            self._ftp_conn.delete(ftp_event_file)
+            return event
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/local.py` & `vxquant-2023.4.1/src/vxquant/providers/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,77 @@
-"""本地文件接口"""
-import polars as pl
-from pathlib import Path
-from typing import List, Union
-from vxquant.providers.base import vxInstrumentsProvider, vxFeaturesProvider
-from vxquant.model.instruments import vxInstruments
-from vxquant.model.typehint import InstrumentType, DateTimeType
-from vxutils import logger, to_datetime, vxtime
-
-
-class vxLocalInstrumentsProvider(vxInstrumentsProvider):
-    def __init__(self) -> None:
-        self.instruments_dir = Path(
-            self.context.get("data_dir", Path.home().joinpath(".data"))
-        ).joinpath("instruments/")
-        self.instruments_dir.mkdir(parents=True, exist_ok=True)
-        logger.info(f"{self.__class__.__name__} 使用文件目录: {self.instruments_dir}")
-
-    def __call__(self, instruments_name: str = "all") -> vxInstruments:
-        registrations = pl.read_csv(
-            self.instruments_dir.joinpath(f"{instruments_name}.csv")
-        )
-        if "weight" not in registrations.columns:
-            registrations = registrations.select(
-                [pl.col("*"), pl.lit(1).alias("weight")]
-            )
-        return vxInstruments(instruments_name, registrations)
-
-
-class vxLocalFeaturesProvider(vxFeaturesProvider):
-    def __init__(
-        self, date_col: str = "trade_date", symbol_col: str = "symbol"
-    ) -> None:
-        self._features_dir = Path(
-            self.context.get("data_dir", Path.home().joinpath(".data"))
-        ).joinpath("features")
-        self._features_dir.mkdir(parents=True, exist_ok=True)
-        self._date_col = date_col
-        self._symbol_col = symbol_col
-
-    def __call__(
-        self,
-        instruments: Union[List[InstrumentType], vxInstruments],
-        start_date: DateTimeType = None,
-        end_date: DateTimeType = None,
-        freq: str = "1d",
-        fields: List[str] = None,
-    ) -> pl.DataFrame:
-        start_date = to_datetime(start_date or "2005-01-01")
-        end_date = to_datetime(end_date or vxtime.today())
-        if isinstance(instruments, vxInstruments):
-            instruments = instruments.all_instruments()
-        freq = "day" if freq == "1d" else "min"
-
-        if fields is not None:
-            fields = set(fields)
-            fields.add(self._date_col)
-            fields.add(self._symbol_col)
-            fields = pl.col(list(fields))
-        else:
-            fields = pl.col("*")
-
-        data = pl.scan_parquet(Path(self._features_dir, f"features_{freq}.parquet"))
-
-        return (
-            data.filter(
-                (pl.col(self._symbol_col).is_in(instruments))
-                & (pl.col(self._date_col).is_between(start_date, end_date))
-            )
-            .sort([self._date_col, self._symbol_col])
-            .collect()
-            .select(fields)
-        )
+"""本地文件接口"""
+import polars as pl
+from pathlib import Path
+from typing import List, Union
+from vxquant.providers.base import vxInstrumentsProvider, vxFeaturesProvider
+from vxquant.model.instruments import vxInstruments
+from vxquant.model.typehint import InstrumentType, DateTimeType
+from vxutils import logger, to_datetime, vxtime
+
+
+class vxLocalInstrumentsProvider(vxInstrumentsProvider):
+    def __init__(self, data_dir: Union[str, Path] = None) -> None:
+        self.instruments_dir = (
+            Path(data_dir) if data_dir else Path.home().joinpath(".data")
+        ).joinpath("instruments/")
+        self.instruments_dir.mkdir(parents=True, exist_ok=True)
+        logger.info(f"{self.__class__.__name__} 使用文件目录: {self.instruments_dir}")
+
+    def __call__(self, instruments_name: str = "all") -> vxInstruments:
+        registrations = pl.read_csv(
+            self.instruments_dir.joinpath(f"{instruments_name}.csv")
+        )
+        if "weight" not in registrations.columns:
+            registrations = registrations.select(
+                [pl.col("*"), pl.lit(1).alias("weight")]
+            )
+        return vxInstruments(instruments_name, registrations)
+
+
+class vxLocalFeaturesProvider(vxFeaturesProvider):
+    def __init__(
+        self,
+        data_dir: Union[str, Path] = None,
+        date_col: str = "trade_date",
+        symbol_col: str = "symbol",
+    ) -> None:
+        self._features_dir = (
+            Path(data_dir) if data_dir else Path.home().joinpath(".data")
+        ).joinpath("features")
+        self._features_dir.mkdir(parents=True, exist_ok=True)
+        logger.info(f"{self.__class__.__name__} 使用文件目录: {self._features_dir}")
+        self._date_col = date_col
+        self._symbol_col = symbol_col
+
+    def __call__(
+        self,
+        instruments: Union[List[InstrumentType], vxInstruments],
+        start_date: DateTimeType = None,
+        end_date: DateTimeType = None,
+        freq: str = "1d",
+        fields: List[str] = None,
+    ) -> pl.DataFrame:
+        start_date = to_datetime(start_date or "2005-01-01")
+        end_date = to_datetime(end_date or vxtime.today())
+        if isinstance(instruments, vxInstruments):
+            instruments = instruments.all_instruments()
+        freq = "day" if freq == "1d" else "min"
+
+        if fields is not None:
+            fields = set(fields)
+            fields.add(self._date_col)
+            fields.add(self._symbol_col)
+            fields = pl.col(list(fields))
+        else:
+            fields = pl.col("*")
+
+        data = pl.scan_parquet(Path(self._features_dir, f"features_{freq}.parquet"))
+
+        return (
+            data.filter(
+                (pl.col(self._symbol_col).is_in(instruments))
+                & (pl.col(self._date_col).is_between(start_date, end_date))
+            )
+            .sort([self._date_col, self._symbol_col])
+            .collect()
+            .select(fields)
+        )
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/miniqmt.py` & `vxquant-2023.4.1/src/vxquant/providers/miniqmt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """MINI QMT Providers"""
 
 from pathlib import Path
 from typing import List, Dict, Union
-from multiprocessing import Lock
 from enum import Enum
-from vxsched import vxContext
-from vxquant.model.contants import OrderStatus, TradeStatus
-from vxquant.model.typehint import InstrumentType
+from vxquant.accountdb.sqlitedb import vxSQLiteAccountDB
+from vxquant.model.contants import OrderStatus, TradeStatus, OrderRejectReason
+from vxquant.model.typehint import InstrumentType, DateTimeType
 from vxquant.model.exchange import (
     vxCashPosition,
     vxPosition,
     vxTick,
     vxOrder,
     vxTrade,
     vxAccountInfo,
@@ -23,65 +22,73 @@
     qmtTradeConvter,
     qmtCashPositionConvter,
     qmtAccountInfoConvter,
 )
 from vxquant.model.preset import vxMarketPreset
 from vxquant.providers.base import (
     vxHQProvider,
+    vxCalendarProvider,
+    vxFeaturesProvider,
     vxGetAccountProvider,
     vxGetPositionsProvider,
     vxOrderBatchProvider,
     vxOrderCancelProvider,
     vxGetExecutionReportsProvider,
     vxGetOrdersProvider,
     ProviderContext,
 )
-
-from vxsched import vxscheduler
-from vxutils import vxtime, logger
+from vxsched import vxScheduler, vxContext, vxscheduler
+from vxutils import vxtime, logger, to_timestring
 
 try:
     from xtquant import xtdata
     from xtquant.xttype import StockAccount
     from xtquant.xttrader import XtQuantTrader, XtQuantTraderCallback
+    from xtquant import xtconstant
 except ImportError as e:
     raise ImportError("xtquant未安装，请将QMT安装目录")
 
 
 def to_qmt_symbol(symbol: InstrumentType):
     """将symbol(SHSE.600000) --> QMT的symbol格式(600000.SH)"""
     return f"{symbol[-6:]}.{symbol[:2]}"
 
 
 class vxMiniQMTHQProvider(vxHQProvider):
+    """Mini QMT行情接口"""
+
     def _hq(self, *symbols: List[InstrumentType]) -> Dict[InstrumentType, vxTick]:
         if len(symbols) == 1 and isinstance(symbols[0], list):
             symbols = symbols[0]
 
         qmt_symbols = [to_qmt_symbol(symbol) for symbol in symbols]
         qmt_ticks = xtdata.get_full_tick(qmt_symbols)
         for k, v in qmt_ticks.items():
             v["symbol"] = k
         return dict(map(lambda x: qmtTickConvter(x, "symbol"), qmt_ticks.values()))
 
 
 class vxMiniQMTGetAccountProvider(vxGetAccountProvider):
+    """Mini QMT账户接口"""
+
     def __call__(self, account_id: str = None) -> vxAccountInfo:
-        acc_info = self.context.trader.query_stock_asset(self._account)
+        acc_info = self.context.trader.query_stock_asset(self.context.account)
         if not acc_info:
             raise ConnectionError(f"无法获取账户信息，请检查连接. {acc_info}")
 
-        qmt_positions = self.context.trader.query_stock_positions(self._account)
-        fnl = sum(p.marketvalue - p.open_price * p.volume for p in qmt_positions)
+        qmt_positions = self.context.trader.query_stock_positions(self.context.account)
+        fnl = sum(p.market_value - p.open_price * p.volume for p in qmt_positions)
         return qmtAccountInfoConvter(acc_info, fnl=fnl)
 
 
 class vxMiniQMTGetPositionsProvider(vxGetPositionsProvider):
+    """Mini QMT持仓接口"""
+
     def __call__(
-        self, symbol: InstrumentType = None, acccount_id: str = None
+        self, symbol: InstrumentType = None, account_id: str = None
     ) -> Dict[InstrumentType, Union[vxPosition, vxCashPosition]]:
         qmt_positions = self.context.trader.query_stock_positions(self.context.account)
         positions = dict(map(lambda x: qmtPositionConvter(x, "symbol"), qmt_positions))
         if symbol:
             return positions.pop(symbol, {})
 
         acc_info = self.context.trader.query_stock_asset(self.context.account)
@@ -90,15 +97,15 @@
         cash_position = qmtCashPositionConvter(acc_info)
         positions["CNY"] = cash_position
         return positions
 
 
 class vxMiniQMTGetOrdersProvider(vxGetOrdersProvider):
     def __call__(
-        self, account_id: str = None, filter_finished: bool = True
+        self, account_id: str = None, filter_finished: bool = False
     ) -> Dict[str, vxOrder]:
         qmt_orders = self.context.trader.query_stock_orders(
             self.context.account, filter_finished
         )
         return dict(
             map(lambda order: qmtOrderConvter(order, "exchange_order_id"), qmt_orders)
         )
@@ -110,65 +117,90 @@
     ) -> Dict[str, vxTrade]:
         qmt_trades = self.context.trader.query_stock_trades(self.context.account)
         return dict(map(lambda x: qmtTradeConvter(x, "trade_id"), qmt_trades))
 
 
 class vxMiniQMTOrderBatchProvider(vxOrderBatchProvider):
     def __call__(self, *vxorders) -> List[vxOrder]:
-        if len(vxorders) == 1 and isinstance(vxorders[0], list):
+        if len(vxorders) == 1 and isinstance(vxorders[0], (list, tuple, set)):
             vxorders = vxorders[0]
 
         for vxorder in vxorders:
             price_type = (
-                11
+                xtconstant.FIX_PRICE
                 if vxorder.order_type.name == "Limit"
-                else 42
-                if vxorder.symbol[:2] == "SH"
-                else 47
+                else (
+                    xtconstant.MARKET_SH_CONVERT_5_CANCEL
+                    if vxorder.symbol[:2] == "SH"
+                    else xtconstant.MARKET_SZ_CONVERT_5_CANCEL
+                )
             )
-            exchange_order_id = self.context.trader.order_stock(
+
+            order_type = (
+                xtconstant.STOCK_BUY
+                if vxorder.order_direction.name == "Buy"
+                else xtconstant.STOCK_SELL
+            )
+
+            seq_no = self.context.trader.order_stock(
                 account=self.context.account,
                 stock_code=to_qmt_symbol(vxorder.symbol),
-                order_type=23 if vxorder.order_direction.name == "Buy" else 24,
+                order_type=order_type,
                 order_volume=vxorder.volume,
                 price_type=price_type,
                 price=vxorder.price,
-                strategy_name=vxorder.algo_order_id,
-                order_remark=vxorder.order_id,
+                strategy_name=vxorder.order_id[16:],
+                order_remark=vxorder.order_id[:16],
             )
-            if exchange_order_id <= 0:
+            exchange_order_id = f"qmt_{seq_no}"
+
+            if seq_no <= 0:
                 vxorder.status = "Rejected"
-                continue
+                vxorder.reject_code = OrderRejectReason.UnknownOrder
+                vxorder.reject_reason = f"错误代码: {exchange_order_id}"
+            else:
+                vxorder.exchange_order_id = str(exchange_order_id)
+                vxorder.status = "New"
 
-            vxorder.exchange_order_id = exchange_order_id
-            vxorder.status = "New"
-            self.context.broker_orders[exchange_order_id] = vxorder
+            # self.context.broker_orders[vxorder.exchange_order_id] = vxorder
 
         return vxorders
 
 
 class vxMiniQMTOrderCancelProvider(vxOrderCancelProvider):
     def __call__(self, *vxorders) -> None:
         if len(vxorders) == 1 and isinstance(vxorders[0], list):
             vxorders = vxorders[0]
 
         for vxorder in vxorders:
             if not vxorder.exchange_order_id:
                 continue
 
             seq = self.context.trader.cancel_order_stock_async(
-                self._account, vxorder.exchange_order_id
+                self.context.account, int(vxorder.exchange_order_id.replace("qmt_", ""))
             )
             if seq <= 0:
                 logger.error(
                     f"委托订单:{vxorder.order_id} 撤单失败{vxorder.symbol} {vxorder.order_direction} {vxorder.volume}"
                 )
         return
 
 
+class vxMiniQMTCalendarProvider(vxCalendarProvider):
+    def get_trade_dates(
+        self,
+        market: str = "cn",
+        start_date: DateTimeType = None,
+        end_date: DateTimeType = None,
+    ):
+        start_date = to_timestring(start_date or "19900101", "%Y%m%d")
+        end_date = to_timestring(end_date or "20991231", "%Y%m%d")
+        return xtdata.get_trading_calendar("SH", start_date, end_date)
+
+
 class QMTAccountStatus(Enum):
     INVALID = -1
     OK = 0
     WAITING_LOGIN = 1
     STATUSING = 2
     FAIL = 3
     INITING = 4
@@ -176,54 +208,50 @@
     CLOSED = 6
     ASSIS_FAIL = 7
     DISABLEBYSYS = 8
     DISABLEBYUSER = 9
 
 
 class vxQMTTraderCallback(XtQuantTraderCallback):
-    lock = Lock()
-
-    def __init__(self, context: vxContext = None) -> None:
+    def __init__(
+        self,
+        context: vxContext,
+    ) -> None:
         self._context = context
-        if "broker_orders" not in self._context:
-            self._context["broker_orders"] = {}
-
-        if "broker_trades" not in self._context:
-            self._context["broker_trades"] = {}
-
-    @property
-    def context(self) -> vxContext:
-        return self._context
+        if "sched" not in self._context:
+            self._context.sched = vxscheduler
+        if "accountdb" not in self._context:
+            self._context.accountdb = vxSQLiteAccountDB()
 
     def on_connected(self):
         """
         连接成功推送
         """
         logger.info("连接成功")
-        vxscheduler.submit_events("on_connected")
+        self._context.sched.submit_events("on_connected")
 
     def on_disconnected(self):
         """
         连接状态回调
         :return:
         """
         logger.warning("连接断开")
-        vxscheduler.submit_events("on_disconnected")
+        self._context.sched.submit_events("on_disconnected")
 
     def on_account_status(self, status):
         """
         账号状态信息推送
         :param response: XtAccountStatus 对象
         :return:
         """
         logger.info(
             "账户状态变更为:"
             f" {status.account_id} {status.account_type} {QMTAccountStatus(status.status)}"
         )
-        vxscheduler.submit_event(
+        self._context.sched.submit_event(
             "on_account_status",
             (status.account_id, status.account_type, QMTAccountStatus(status.status)),
         )
 
     def on_stock_asset(self, asset):
         """
         资金信息推送
@@ -236,76 +264,40 @@
 
     def on_stock_order(self, order):
         """
         委托信息推送
         :param order: XtOrder对象
         :return:
         """
-        logger.debug(
-            f"收到成交更新: {order.stock_code} {order.order_status} {order.order_sysid}"
+        broker_order = qmtOrderConvter(order)
+        logger.info(
+            f"收到来自broker委托订单 {broker_order.exchange_order_id} 更新为:"
+            f" {broker_order}"
         )
-        vxorder = qmtOrderConvter(order)
-
-        if vxorder.exchange_order_id not in self.context.broker_orders:
-            with self.lock:
-                self.context.broker_orders[vxorder.exchange_order_id] = vxorder
-                logger.info(f"[新增] 委托订单{vxorder.exchange_order_id} 更新为: {vxorder}")
-            vxscheduler.submit_event("on_broker_order_status", vxorder)
-            return
-
-        broker_order = self.context.broker_orders[vxorder.exchange_order_id]
-        if broker_order.status in [
-            OrderStatus.Filled,
-            OrderStatus.Expired,
-            OrderStatus.Rejected,
-            OrderStatus.Canceled,
-            OrderStatus.Suspended,
-        ]:
-            logger.debug(
-                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} "
-                f" 当前状态:{broker_order.status} 须更新状态: {vxorder.status}"
-            )
-            return
-
-        if broker_order.filled_volume > vxorder.filled_volume:
-            logger.debug(
-                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} 当前已成交:"
-                f" {broker_order.filled_volume} > 更新状态:{vxorder.filled_volume}"
-            )
-            return
-
-        # 更新委托订单状态
-        with self.lock:
-            broker_order.status = vxorder.status
-            broker_order.filled_volume = vxorder.filled_volume
-            broker_order.filled_amount = vxorder.filled_amount
-            broker_order.updated_dt = vxorder.updated_dt
-            self.context.broker_orders[broker_order.exchange_order_id] = broker_order
-            logger.info(f"[更新] 委托订单{vxorder.exchange_order_id} 更新为: {broker_order}")
-        vxscheduler.submit_event("on_broker_order_status", broker_order)
+        with self._context.accountdb.start_session() as session:
+            order = session.update_order(broker_order)
+        if order:
+            self._context.sched.submit_event("on_order_status", order)
 
     def on_stock_trade(self, trade):
         """
         成交信息推送
         :param trade: XtTrade对象
         :return:
         """
-        logger.debug(
+        logger.info(
             f"收到成交信息: {trade.account_id}, {trade.stock_code}, {trade.order_id}"
         )
+
         vxtrade = qmtTradeConvter(trade)
 
         if vxtrade.status != TradeStatus.Trade:
             logger.warning(f"收到非成交的回报信息: {vxtrade}")
             return
 
-        if vxtrade.trade_id in self.context.broker_trades:
-            logger.warning("收到重复的委托订单信息")
-            return
-
         # 调整当日手续费
         if vxtrade.commission == 0:
             _preset = vxMarketPreset(vxtrade.symbol)
             vxtrade.commission = max(
                 (
                     vxtrade.price
                     * vxtrade.volume
@@ -314,108 +306,100 @@
                         if vxtrade.order_direction.name == "Buy"
                         else (
                             _preset.commission_coeff_peramount
                             + _preset.tax_coeff_peramount
                         )
                     )
                 ),
-                5,
+                0.5,
             )
+        with self._context.accountdb.start_session() as session:
+            trade = session.update_trade(vxtrade)
+        if trade:
+            self._context.sched.submit_event("on_execution_report", vxtrade)
+        # logger.info(
+        #    f"收到来自broker成交回报信息 {vxtrade.exchange_order_id}: {vxtrade}"
+        # )
 
-        with self.lock:
-            self.context.broker_trades[vxtrade.trade_id] = vxtrade
-            logger.info(f"收到成交回报信息: {vxtrade}")
-        vxscheduler.submit_event("on_broker_execution_report", vxtrade)
-
-    def on_stock_position(self, position):
+    def on_stock_position(self, xtposition):
         """
         持仓信息推送
         :param position: XtPosition对象
         :return:
         """
-        logger.info(f"持仓信息推送: {position.stock_code}, {position.volume}")
+        logger.info(f"持仓信息推送: {xtposition.stock_code}, {xtposition.volume}")
+        position = qmtPositionConvter(xtposition)
+        self._context.sched.submit_event("on_position_update", data=position)
 
     def on_order_error(self, order_error):
+        # sourcery skip: use-named-expression
         """
         下单失败信息推送
         :param order_error:XtOrderError 对象
         :return:
         """
+        # order_error.order_id = f"qmt_{order_error.order_id}"
+        logger.warning(
+            "收到委托订单错误反馈:"
+            f" {order_error.order_id},"
+            f" {order_error.error_id}, {order_error.error_msg}"
+        )
 
-        if order_error.order_id not in self.context.broker_orders:
-            logger.warning(
-                f"下单失败: {order_error.order_id}, {order_error.error_id},"
-                f" {order_error.error_msg}"
-            )
-            return
-
-        with self.lock:
-            broker_order = self.context.broker_orders[order_error.order_id]
-            if broker_order.status in [
-                OrderStatus.Filled,
-                OrderStatus.Expired,
-                OrderStatus.Rejected,
-                OrderStatus.Canceled,
-                OrderStatus.Suspended,
-            ]:
-                logger.debug(
-                    f"[忽略更新] 委托订单 {order_error.exchange_order_id} "
-                    f" 当前状态:{broker_order.status} 须更新状态: {order_error.error_msg}"
+        try:
+            with self._context.accountdb.start_session() as session:
+                vxorder = session.findone(
+                    "orders", exchange_order_id=f"qmt_{order_error.order_id}"
                 )
-                return
+                if not vxorder:
+                    logger.warning(
+                        f"收到来自broker委托订单 qmt_{order_error.order_id} 未找到"
+                    )
+                    return
+                vxorder.status = OrderStatus.Rejected
+                vxorder.reject_code = OrderRejectReason.UnknownOrder
+                vxorder.reject_reason = order_error.error_msg
+                order = self._context.accountdb.update_order(vxorder)
+                if order:
+                    self._context.sched.submit_event("on_order_status", order)
 
-            broker_order.status = "Rejected"
-            broker_order.reject_code = "UnknownOrder"
-            broker_order.reject_reason = order_error.error_msg
-        vxscheduler.submit_event("on_broker_order_status", broker_order)
+        except Exception as e:
+            logger.error(f"发生异常错误：{e}")
 
     def on_order_stock_async_response(self, response):
         """
         :param response: XtOrderResponse 对象
         :return:
         """
         # with self.lock:
         #    vxorder = self.seq_mapping.get(response.seq, None)
         #    vxorder.exchange_order_id = response.order_id
         #    self.broker_orders[vxorder.exchange_order_id] = vxorder
-        pass
 
     def on_smt_appointment_async_response(self, response):
         """
         :param response: XtAppointmentResponse 对象
         :return:
         """
-        pass
 
 
 def init_provider_context(
+    context: vxContext,
     miniqmt_path: Union[str, Path],
     account_id: str = None,
     account_type: str = "STOCK",
-    callback: vxQMTTraderCallback = None,
 ) -> None:
-    ProviderContext.account = StockAccount(account_id, account_type)
-    ProviderContext.trader = XtQuantTrader(miniqmt_path, int(vxtime.now()))
-    ProviderContext.trader.start()
-    connect_result = ProviderContext.trader.connect()
+    context.account = StockAccount(account_id, account_type)
+    context.trader = XtQuantTrader(miniqmt_path, int(vxtime.now()))
+    callback = vxQMTTraderCallback(context)
+
+    context.trader.start()
+    connect_result = context.trader.connect()
     if connect_result != 0:
         raise ConnectionError(f"连接失败: {connect_result}")
-    logger.info(f"trader 连接成功. {ProviderContext.trader}")
+    logger.info(f"trader 连接成功. {context.trader}")
 
-    ProviderContext.trader.register_callback(callback)
-    subscribe_result = ProviderContext.trader.subscribe(ProviderContext.account)
+    context.trader.register_callback(callback)
+    subscribe_result = context.trader.subscribe(context.account)
     if subscribe_result != 0:
         raise ConnectionError(f"订阅失败: {subscribe_result}")
-    logger.info(f"订阅账号回调信息: {ProviderContext.account}")
-
-    with vxQMTTraderCallback.lock:
-        qmt_orders = ProviderContext.trader.query_stock_orders(
-            ProviderContext.account, False
-        )
-        callback.context.broker_orders = dict(
-            map(lambda order: qmtOrderConvter(order, "exchange_order_id"), qmt_orders)
-        )
-        qmt_trades = ProviderContext.trader.query_stock_trades(ProviderContext.account)
-        callback.context.broker_trades = dict(
-            map(lambda x: qmtTradeConvter(x, "trade_id"), qmt_trades)
-        )
-        logger.info(f"更新委托订单{len(qmt_orders)}个, 更新成交回报:{len(qmt_trades)}个.")
+    logger.info(f"订阅账号回调信息: {context.account}")
+    return context
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/mongo.py` & `vxquant-2023.4.1/src/vxquant/providers/mongo.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-"""mongodb providers"""
-
-from typing import Dict, Union, List
-from multiprocessing import Lock
-from vxsched import vxscheduler
-from vxquant.model.typehint import InstrumentType
-from vxquant.model.contants import (
-    OrderDirection,
-    OrderType,
-    OrderStatus,
-    OrderOffset,
-    OrderRejectReason,
-)
-from vxquant.providers.base import (
-    vxGetAccountProvider,
-    vxGetOrdersProvider,
-    vxGetPositionsProvider,
-    vxGetExecutionReportsProvider,
-    vxOrderBatchProvider,
-    vxOrderCancelProvider,
-)
-from vxquant.model.exchange import (
-    vxAccountInfo,
-    vxOrder,
-    vxPosition,
-    vxCashPosition,
-    vxTrade,
-)
-from vxutils import logger
-from vxutils.dbproxy import vxMongoProxy
-
-_mongodb_lock = Lock()
-
-
-class vxMongoGetAccountProvider(vxGetAccountProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._accounts = self.context.dbconn["accounts"]
-        self._positions = self.context.dbconn["positions"]
-
-    def __call__(self, account_id: str = None) -> vxAccountInfo:
-        item = self._accounts.find_one({"account_id": account_id}, {"_id": 0})
-        accountinfo = vxAccountInfo(dict(item))
-        item = self._positions.find_one({"account_id": account_id, "symbol": "CNY"})
-        accountinfo.balance = item["volume"]
-        accountinfo.frozen = item["frozen"]
-
-        items = list(
-            self._positions.aggreate(
-                [
-                    {"$match": {"account_id": account_id, "symbol": {"$ne": "CNY"}}},
-                    {
-                        "$group": {
-                            "marketvalue": {"$sum": "marketvalue"},
-                            "fnl": {"$sum": "fnl"},
-                        }
-                    },
-                ]
-            )
-        )
-        if items:
-            accountinfo.marketvalue = items[0]["marketvalue"]
-            accountinfo.fnl = item[0]["fnl"]
-        else:
-            accountinfo.marketvalue = 0
-            accountinfo.fnl = 0
-        return accountinfo
-
-
-class vxMongoGetPositionsProvider(vxGetPositionsProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._positions = self.context.dbconn["positions"]
-
-    def __call__(
-        self, symbol: InstrumentType = None, acccount_id: str = None
-    ) -> Dict[InstrumentType, Union[vxPosition, vxCashPosition]]:
-        if acccount_id is None:
-            raise ValueError("未指定account_id")
-
-        query = {"account_id": acccount_id}
-        if symbol:
-            query["symbol"] = symbol
-
-        cur = self._positions.find(query, {"_id": 0})
-        return {
-            item["symbol"]: vxPosition(item)
-            if item["symbol"] != "CNY"
-            else vxCashPosition(item)
-            for item in cur
-        }
-
-
-class vxMongoGetOrdersProvider(vxGetOrdersProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._orders = self.context.dbconn["orders"]
-
-    def __call__(
-        self, account_id: str = None, filter_finished: bool = False
-    ) -> Dict[str, vxOrder]:
-        if account_id is None:
-            raise ValueError("未指定account_id")
-
-        query = {"account_id": account_id}
-        if filter_finished:
-            query["status"] = {"$in": ["PendingNew", "New", "PartiallyFilled"]}
-        cur = self._orders.find(query, {"_id": 0})
-        return {item["order_id"]: vxOrder(item) for item in cur}
-
-
-class vxMongoGetExecutionReportsProvider(vxGetExecutionReportsProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._trades = self.context.dbconn["trades"]
-
-    def __call__(
-        self, account_id: str = None, order_id: str = None, trade_id: str = None
-    ) -> Dict[str, vxTrade]:
-        query = {"account_id": account_id}
-        if order_id:
-            query["order_id"] = order_id
-        if trade_id:
-            query["trade_id"] = trade_id
-
-        cur = self._db.trades.find(query, {"_id": 0})
-        return {item["trade_id"]: vxTrade(item) for item in cur}
-
-
-def _frozen_position(dbconn, vxorder) -> bool:
-    """冻结仓位"""
-    if vxorder.order_direction == OrderDirection.Buy:
-        frozen_symbol = "CNY"
-        frozen_volume = vxorder.volume * vxorder.price * 1.003
-    else:
-        frozen_symbol = vxorder.symbol
-        frozen_volume = vxorder.volume
-
-    with dbconn.start_session(lock=_mongodb_lock) as session:
-        ret_cur = dbconn.positions.update_one(
-            {
-                "account_id": vxorder.account_id,
-                "symbol": frozen_symbol,
-                "available": {"$gte": frozen_volume},
-            },
-            {"$inc": {"frozen": frozen_volume, "available": -frozen_volume}},
-            session=session,
-        )
-        if ret_cur.matched_count == 0:
-            vxorder.status = OrderStatus.Rejected
-            vxorder.reject_code = (
-                OrderRejectReason.NoEnoughCash
-                if frozen_symbol == "CNY"
-                else OrderRejectReason.NoEnoughPosition
-            )
-            vxorder.reject_reason = (
-                f"账户({vxorder.account_id}) 冻结{frozen_symbol}资金 :{frozen_volume} 失败。"
-            )
-        else:
-            vxorder.status = OrderStatus.PendingNew
-
-        dbconn.orders.update_one(
-            {"order_id": vxorder.order_id}, {"$set": vxorder.message}, session=session
-        )
-
-    return vxorder
-
-
-def _update_frozen(self, account_id, symbol, volume, session) -> bool:
-    ret_cur = self._db.positions.update_one(
-        {"account_id": account_id, "symbol": symbol, "frozen": {"$get": volume}},
-        {"$inc": {"frozen": -volume, "available": volume}},
-        session=session,
-    )
-    if ret_cur.matched_count == 0:
-        raise ValueError(f"账号({account_id}) 解冻{symbol}仓位 {volume} 失败.")
-    if symbol == "CNY":
-        self._db.accounts.update_one(
-            {
-                "account_id": account_id,
-            },
-            {"$inc": {"frozen": -volume, "available": volume}},
-            session=session,
-        )
-    return True
-
-
-class vxMongoOrderBatchProvider(vxOrderBatchProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._dbconn = self.context.dbconn
-
-    def __call__(self, *vxorders) -> List[vxOrder]:
-        submit_orders = []
-
-        for order in vxorders:
-            if not isinstance(order, vxOrder):
-                logger.warning(f"order 类型不正确 : {type(order)}")
-                continue
-
-            frozen_order = _frozen_position(self._dbconn, order)
-
-            if frozen_order.status == OrderStatus.Rejected:
-                vxscheduler.submit_event("on_order_status", data=frozen_order)
-            submit_orders.append(order)
-        vxscheduler.submit_event("on_submit_order_batch", data=submit_orders)
-        return submit_orders
-
-
-class vxMongoOrderCancelProvider(vxOrderCancelProvider):
-    def __init__(self) -> None:
-        if "dbconn" not in self.context.keys():
-            db_params = self.context.settings.get("db_params", {})
-            self.context.dbconn = vxMongoProxy(**db_params)
-        self._dbconn = self.context.dbconn
-
-    def __call__(self, *vxorders) -> None:
-        vxscheduler.submit_event("on_submit_order_cancel", data=vxorders)
-
-
-@vxscheduler.event_handler("on_order_status")
-def on_order_status(context, event):
-    vxorder = event.data
-    if vxorder.status in [OrderStatus.Rejected,OrderStatus.Suspended,OrderStatus.Filled,OrderStatus.Canceled]:
+"""mongodb providers"""
+
+from typing import Dict, Union, List
+from multiprocessing import Lock
+from vxsched import vxscheduler
+from vxquant.model.typehint import InstrumentType
+from vxquant.model.contants import (
+    OrderDirection,
+    OrderType,
+    OrderStatus,
+    OrderOffset,
+    OrderRejectReason,
+)
+from vxquant.providers.base import (
+    vxGetAccountProvider,
+    vxGetOrdersProvider,
+    vxGetPositionsProvider,
+    vxGetExecutionReportsProvider,
+    vxOrderBatchProvider,
+    vxOrderCancelProvider,
+)
+from vxquant.model.exchange import (
+    vxAccountInfo,
+    vxOrder,
+    vxPosition,
+    vxCashPosition,
+    vxTrade,
+)
+from vxutils import logger
+from vxutils.dbproxy import vxMongoProxy
+
+_mongodb_lock = Lock()
+
+
+class vxMongoGetAccountProvider(vxGetAccountProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._accounts = self.context.dbconn["accounts"]
+        self._positions = self.context.dbconn["positions"]
+
+    def __call__(self, account_id: str = None) -> vxAccountInfo:
+        item = self._accounts.find_one({"account_id": account_id}, {"_id": 0})
+        accountinfo = vxAccountInfo(dict(item))
+        item = self._positions.find_one({"account_id": account_id, "symbol": "CNY"})
+        accountinfo.balance = item["volume"]
+        accountinfo.frozen = item["frozen"]
+
+        items = list(
+            self._positions.aggreate(
+                [
+                    {"$match": {"account_id": account_id, "symbol": {"$ne": "CNY"}}},
+                    {
+                        "$group": {
+                            "marketvalue": {"$sum": "marketvalue"},
+                            "fnl": {"$sum": "fnl"},
+                        }
+                    },
+                ]
+            )
+        )
+        if items:
+            accountinfo.marketvalue = items[0]["marketvalue"]
+            accountinfo.fnl = item[0]["fnl"]
+        else:
+            accountinfo.marketvalue = 0
+            accountinfo.fnl = 0
+        return accountinfo
+
+
+class vxMongoGetPositionsProvider(vxGetPositionsProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._positions = self.context.dbconn["positions"]
+
+    def __call__(
+        self, symbol: InstrumentType = None, acccount_id: str = None
+    ) -> Dict[InstrumentType, Union[vxPosition, vxCashPosition]]:
+        if acccount_id is None:
+            raise ValueError("未指定account_id")
+
+        query = {"account_id": acccount_id}
+        if symbol:
+            query["symbol"] = symbol
+
+        cur = self._positions.find(query, {"_id": 0})
+        return {
+            item["symbol"]: vxPosition(item)
+            if item["symbol"] != "CNY"
+            else vxCashPosition(item)
+            for item in cur
+        }
+
+
+class vxMongoGetOrdersProvider(vxGetOrdersProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._orders = self.context.dbconn["orders"]
+
+    def __call__(
+        self, account_id: str = None, filter_finished: bool = False
+    ) -> Dict[str, vxOrder]:
+        if account_id is None:
+            raise ValueError("未指定account_id")
+
+        query = {"account_id": account_id}
+        if filter_finished:
+            query["status"] = {"$in": ["PendingNew", "New", "PartiallyFilled"]}
+        cur = self._orders.find(query, {"_id": 0})
+        return {item["order_id"]: vxOrder(item) for item in cur}
+
+
+class vxMongoGetExecutionReportsProvider(vxGetExecutionReportsProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._trades = self.context.dbconn["trades"]
+
+    def __call__(
+        self, account_id: str = None, order_id: str = None, trade_id: str = None
+    ) -> Dict[str, vxTrade]:
+        query = {"account_id": account_id}
+        if order_id:
+            query["order_id"] = order_id
+        if trade_id:
+            query["trade_id"] = trade_id
+
+        cur = self._db.trades.find(query, {"_id": 0})
+        return {item["trade_id"]: vxTrade(item) for item in cur}
+
+
+def _frozen_position(dbconn, vxorder) -> bool:
+    """冻结仓位"""
+    if vxorder.order_direction == OrderDirection.Buy:
+        frozen_symbol = "CNY"
+        frozen_volume = vxorder.volume * vxorder.price * 1.003
+    else:
+        frozen_symbol = vxorder.symbol
+        frozen_volume = vxorder.volume
+
+    with dbconn.start_session(lock=_mongodb_lock) as session:
+        ret_cur = dbconn.positions.update_one(
+            {
+                "account_id": vxorder.account_id,
+                "symbol": frozen_symbol,
+                "available": {"$gte": frozen_volume},
+            },
+            {"$inc": {"frozen": frozen_volume, "available": -frozen_volume}},
+            session=session,
+        )
+        if ret_cur.matched_count == 0:
+            vxorder.status = OrderStatus.Rejected
+            vxorder.reject_code = (
+                OrderRejectReason.NoEnoughCash
+                if frozen_symbol == "CNY"
+                else OrderRejectReason.NoEnoughPosition
+            )
+            vxorder.reject_reason = (
+                f"账户({vxorder.account_id}) 冻结{frozen_symbol}资金 :{frozen_volume} 失败。"
+            )
+        else:
+            vxorder.status = OrderStatus.PendingNew
+
+        dbconn.orders.update_one(
+            {"order_id": vxorder.order_id}, {"$set": vxorder.message}, session=session
+        )
+
+    return vxorder
+
+
+def _update_frozen(self, account_id, symbol, volume, session) -> bool:
+    ret_cur = self._db.positions.update_one(
+        {"account_id": account_id, "symbol": symbol, "frozen": {"$get": volume}},
+        {"$inc": {"frozen": -volume, "available": volume}},
+        session=session,
+    )
+    if ret_cur.matched_count == 0:
+        raise ValueError(f"账号({account_id}) 解冻{symbol}仓位 {volume} 失败.")
+    if symbol == "CNY":
+        self._db.accounts.update_one(
+            {
+                "account_id": account_id,
+            },
+            {"$inc": {"frozen": -volume, "available": volume}},
+            session=session,
+        )
+    return True
+
+
+class vxMongoOrderBatchProvider(vxOrderBatchProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._dbconn = self.context.dbconn
+
+    def __call__(self, *vxorders) -> List[vxOrder]:
+        submit_orders = []
+
+        for order in vxorders:
+            if not isinstance(order, vxOrder):
+                logger.warning(f"order 类型不正确 : {type(order)}")
+                continue
+
+            frozen_order = _frozen_position(self._dbconn, order)
+
+            if frozen_order.status == OrderStatus.Rejected:
+                vxscheduler.submit_event("on_order_status", data=frozen_order)
+            submit_orders.append(order)
+        vxscheduler.submit_event("on_submit_order_batch", data=submit_orders)
+        return submit_orders
+
+
+class vxMongoOrderCancelProvider(vxOrderCancelProvider):
+    def __init__(self) -> None:
+        if "dbconn" not in self.context.keys():
+            db_params = self.context.settings.get("db_params", {})
+            self.context.dbconn = vxMongoProxy(**db_params)
+        self._dbconn = self.context.dbconn
+
+    def __call__(self, *vxorders) -> None:
+        vxscheduler.submit_event("on_submit_order_cancel", data=vxorders)
+
+
+@vxscheduler.event_handler("on_order_status")
+def on_order_status(context, event):
+    vxorder = event.data
+    if vxorder.status in [OrderStatus.Rejected,OrderStatus.Suspended,OrderStatus.Filled,OrderStatus.Canceled]:
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/spiders/calendar_sse.py` & `vxquant-2023.4.1/src/vxquant/providers/spiders/calendar_sse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-"""交易日期基础接口"""
-
-import requests
-import random
-import datetime
-from itertools import product
-from typing import List
-from tqdm import tqdm
-from vxutils import vxtime, logger
-from vxquant.providers.base import vxCalendarProvider
-
-SSE_CALENDAR_LIST = "http://www.szse.cn/api/report/exchange/onepersistenthour/monthList?month={year}-{month}&random={timestamp}"
-
-
-class CNCalenderProvider(vxCalendarProvider):
-    def get_trade_dates(self, market: str = "cn") -> List:
-        if market != "cn":
-            raise NotImplementedError(f"暂不支持 {market}类型")
-
-        start_date = datetime.datetime(2005, 1, 1)
-        end_date = datetime.datetime.now().replace(
-            month=12, day=31, hour=0, minute=0, second=0
-        )
-
-        cals = []
-
-        for year, month in tqdm(
-            product(range(start_date.year, end_date.year + 1), range(1, 13)),
-            desc="获取交易日历...",
-        ):
-            url = SSE_CALENDAR_LIST.format(
-                year=year, month=month, timestamp=random.randint(100000, 10000000)
-            )
-            resp = requests.get(url, timeout=1)
-            resp.raise_for_status()
-            reply = resp.json()
-            if "data" in reply and reply["data"]:
-                try:
-                    cals.extend(
-                        [
-                            trade_date["jyrq"]
-                            for trade_date in reply["data"]
-                            if trade_date["jybz"] == "1"
-                        ]
-                    )
-                except Exception as e:
-                    logger.error(f"{year}-{month} get calendar {reply} error: {e}")
-                vxtime.sleep(0.1)
-        return sorted(cals)
+"""交易日期基础接口"""
+
+import requests
+import random
+import datetime
+from itertools import product
+from typing import List
+from tqdm import tqdm
+from vxutils import vxtime, logger, to_datetime
+from vxquant.model.typehint import DateTimeType
+from vxquant.providers.base import vxCalendarProvider
+
+SSE_CALENDAR_LIST = "http://www.szse.cn/api/report/exchange/onepersistenthour/monthList?month={year}-{month}&random={timestamp}"
+
+
+class CNCalenderProvider(vxCalendarProvider):
+    def get_trade_dates(
+        self,
+        market: str = "cn",
+        start_date: DateTimeType = None,
+        end_date: DateTimeType = None,
+    ) -> List:
+        if market != "cn":
+            raise NotImplementedError(f"暂不支持 {market}类型")
+
+        start_date = to_datetime(start_date) or datetime.datetime(2005, 1, 1)
+        end_date = to_datetime(end_date) or datetime.datetime.now().replace(
+            month=12, day=31, hour=0, minute=0, second=0
+        )
+
+        cals = []
+
+        for year, month in tqdm(
+            product(range(start_date.year, end_date.year + 1), range(1, 13)),
+            desc=f"获取{start_date.year}年交易日历...",
+        ):
+            url = SSE_CALENDAR_LIST.format(
+                year=year, month=month, timestamp=random.randint(100000, 10000000)
+            )
+            resp = requests.get(url, timeout=1)
+            resp.raise_for_status()
+            reply = resp.json()
+            if "data" in reply and reply["data"]:
+                try:
+                    cals.extend(
+                        [
+                            trade_date["jyrq"]
+                            for trade_date in reply["data"]
+                            if trade_date["jybz"] == "1"
+                        ]
+                    )
+                except Exception as e:
+                    logger.error(f"{year}-{month} get calendar {reply} error: {e}")
+                vxtime.sleep(0.1)
+        return sorted(cals)
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/spiders/hq_tencent.py` & `vxquant-2023.4.1/src/vxquant/providers/spiders/hq_tencent.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-"""实时行情获取"""
-
-import re
-import itertools
-import requests
-from typing import Dict, List
-from functools import reduce
-from vxutils import logger, vxtime
-from vxquant.model.exchange import vxTick
-
-
-_TENCENT_HQ_URL = "https://qt.gtimg.cn/q=%s&timestamp=%s"
-_HEADERS = {
-    "Accept-Encoding": "gzip, deflate, sdch",
-    "User-Agent": (
-        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
-        "(KHTML, like Gecko) Chrome/54.0.2840.100 "
-        "Safari/537.36"
-    ),
-}
-
-
-def _to_tencent_symbol(symbol: str) -> str:
-    """转换成tencent格式的证券代码"""
-    exchange, code = symbol.split(".")
-    if exchange == "SHSE":
-        return f"sh{code}"
-    elif exchange == "SZSE":
-        return f"sz{code}"
-    else:
-        raise ValueError(f"{symbol} 格式不正确.")
-
-
-def _update_dict(source, target):
-    source.update(target)
-    return source
-
-
-class vxTencentHQ:
-    def __init__(self, worker_cnt=2):
-        self._grep_stock_code = re.compile(r"(?<=_)\w+")
-        self._session = requests.Session()
-        self._session.headers.update(_HEADERS)
-        resq = self._session.get("https://stockapp.finance.qq.com/mstats/#", timeout=1)
-        resq.raise_for_status()
-        logger.debug(f"网络连通成功{resq.status_code}...")
-
-    def __call__(self, *symbols) -> Dict[str, vxTick]:
-        """获取最新的ticks 数据
-
-        Returns:
-            Dict[str,vxTick] -- 返回最新的tick数据
-        """
-        if isinstance(symbols[0], list):
-            symbols = symbols[0]
-
-        # print(symbols)
-        stock_lines = map(
-            self.fetch_tencent_ticks,
-            [symbols[i:800] for i in range(0, len(symbols), 800)],
-        )
-        data = map(self.parser, itertools.chain(*stock_lines))
-        ret_ticks = {}
-        reduce(_update_dict, data, ret_ticks)
-        return ret_ticks
-
-    def fetch_tencent_ticks(self, symbols: List[str]) -> List[str]:
-        """抓取tick数据
-
-        Arguments:
-            symbols {List} -- 证券代码s
-
-        Returns:
-            Dict[str, vxTick] -- _description_
-        """
-
-        url = _TENCENT_HQ_URL % (
-            ",".join(map(_to_tencent_symbol, symbols)),
-            vxtime.now(),
-        )
-        try:
-            resq = self._session.get(url, timeout=0.5)
-            resq.raise_for_status()
-            text = resq.text.strip()
-            return text.split(";")[:-1]
-
-        except requests.exceptions.HTTPError as e:
-            logger.error(f"获取{url}数据出错: {e}.")
-            return {}
-
-    def parser(self, stock_line: str) -> Dict[str, vxTick]:
-        """解析程序
-
-        Arguments:
-            stock_line {str} -- 股票信息行
-
-        Returns:
-            Dict[str, vxTick] -- vxticks data
-        """
-
-        stock = stock_line.split("~")
-        if len(stock) <= 49:
-            logger.warning(f"skip stock line: {len(stock_line)}")
-            return {}
-
-        tencent_symbol = self._grep_stock_code.search(stock[0]).group()
-        if tencent_symbol[:2].lower() == "sh":
-            symbol = f"SHSE.{tencent_symbol[2:]}"
-        elif tencent_symbol[:2].lower() == "sz":
-            symbol = f"SZSE.{tencent_symbol[2:]}"
-        else:
-            logger.warniing(
-                f"wrong format tencent_symbol{tencent_symbol} ==== {stock[0]}"
-            )
-            return {}
-
-        return {
-            symbol: vxTick(
-                symbol=symbol,
-                open=stock[5],
-                high=stock[33],
-                low=stock[34],
-                lasttrade=stock[3],
-                yclose=float(stock[3]) - float(stock[31]),
-                volume=int(stock[36]) * 100,
-                amount=float(stock[37]) * 10000,
-                bid1_v=int(stock[10]) * 100,
-                bid1_p=stock[9],
-                bid2_v=int(stock[12]) * 100,
-                bid2_p=stock[11],
-                bid3_v=int(stock[14]) * 100,
-                bid3_p=stock[13],
-                bid4_v=int(stock[16]) * 100,
-                bid4_p=stock[15],
-                bid5_v=int(stock[18]) * 100,
-                bid5_p=stock[17],
-                ask1_v=int(stock[20]) * 100,
-                ask1_p=stock[19],
-                ask2_v=int(stock[22]) * 100,
-                ask2_p=stock[21],
-                ask3_v=int(stock[24]) * 100,
-                ask3_p=stock[23],
-                ask4_v=int(stock[26]) * 100,
-                ask4_p=stock[25],
-                ask5_v=int(stock[28]) * 100,
-                ask5_p=stock[27],
-                interest=0,
-                status="NORMAL",
-                created_dt=stock[30],
-                updated_dt=stock[30],
-            )
-        }
-
-
-if __name__ == "__main__":
-    hq = vxTencentHQ()
-    print(hq("SHSE.600000", "SZSE.000001", "SZSE.300059"))
+"""实时行情获取"""
+
+import re
+import itertools
+import requests
+from typing import Dict, List
+from functools import reduce
+from vxutils import logger, vxtime
+from vxquant.model.exchange import vxTick
+
+
+_TENCENT_HQ_URL = "https://qt.gtimg.cn/q=%s&timestamp=%s"
+_HEADERS = {
+    "Accept-Encoding": "gzip, deflate, sdch",
+    "User-Agent": (
+        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
+        "(KHTML, like Gecko) Chrome/54.0.2840.100 "
+        "Safari/537.36"
+    ),
+}
+
+
+def _to_tencent_symbol(symbol: str) -> str:
+    """转换成tencent格式的证券代码"""
+    exchange, code = symbol.split(".")
+    if exchange == "SHSE":
+        return f"sh{code}"
+    elif exchange == "SZSE":
+        return f"sz{code}"
+    else:
+        raise ValueError(f"{symbol} 格式不正确.")
+
+
+def _update_dict(source, target):
+    source.update(target)
+    return source
+
+
+class vxTencentHQ:
+    def __init__(self, worker_cnt=2):
+        self._grep_stock_code = re.compile(r"(?<=_)\w+")
+        self._session = requests.Session()
+        self._session.headers.update(_HEADERS)
+        resq = self._session.get("https://stockapp.finance.qq.com/mstats/#", timeout=1)
+        resq.raise_for_status()
+        logger.debug(f"网络连通成功{resq.status_code}...")
+
+    def __call__(self, *symbols) -> Dict[str, vxTick]:
+        """获取最新的ticks 数据
+
+        Returns:
+            Dict[str,vxTick] -- 返回最新的tick数据
+        """
+        if isinstance(symbols[0], list):
+            symbols = symbols[0]
+
+        # print(symbols)
+        stock_lines = map(
+            self.fetch_tencent_ticks,
+            [symbols[i:800] for i in range(0, len(symbols), 800)],
+        )
+        data = map(self.parser, itertools.chain(*stock_lines))
+        ret_ticks = {}
+        reduce(_update_dict, data, ret_ticks)
+        return ret_ticks
+
+    def fetch_tencent_ticks(self, symbols: List[str]) -> List[str]:
+        """抓取tick数据
+
+        Arguments:
+            symbols {List} -- 证券代码s
+
+        Returns:
+            Dict[str, vxTick] -- _description_
+        """
+
+        url = _TENCENT_HQ_URL % (
+            ",".join(map(_to_tencent_symbol, symbols)),
+            vxtime.now(),
+        )
+        try:
+            resq = self._session.get(url, timeout=0.5)
+            resq.raise_for_status()
+            text = resq.text.strip()
+            return text.split(";")[:-1]
+
+        except requests.exceptions.HTTPError as e:
+            logger.error(f"获取{url}数据出错: {e}.")
+            return {}
+
+    def parser(self, stock_line: str) -> Dict[str, vxTick]:
+        """解析程序
+
+        Arguments:
+            stock_line {str} -- 股票信息行
+
+        Returns:
+            Dict[str, vxTick] -- vxticks data
+        """
+
+        stock = stock_line.split("~")
+        if len(stock) <= 49:
+            logger.warning(f"skip stock line: {len(stock_line)}")
+            return {}
+
+        tencent_symbol = self._grep_stock_code.search(stock[0]).group()
+        if tencent_symbol[:2].lower() == "sh":
+            symbol = f"SHSE.{tencent_symbol[2:]}"
+        elif tencent_symbol[:2].lower() == "sz":
+            symbol = f"SZSE.{tencent_symbol[2:]}"
+        else:
+            logger.warniing(
+                f"wrong format tencent_symbol{tencent_symbol} ==== {stock[0]}"
+            )
+            return {}
+
+        return {
+            symbol: vxTick(
+                symbol=symbol,
+                open=stock[5],
+                high=stock[33],
+                low=stock[34],
+                lasttrade=stock[3],
+                yclose=float(stock[3]) - float(stock[31]),
+                volume=int(stock[36]) * 100,
+                amount=float(stock[37]) * 10000,
+                bid1_v=int(stock[10]) * 100,
+                bid1_p=stock[9],
+                bid2_v=int(stock[12]) * 100,
+                bid2_p=stock[11],
+                bid3_v=int(stock[14]) * 100,
+                bid3_p=stock[13],
+                bid4_v=int(stock[16]) * 100,
+                bid4_p=stock[15],
+                bid5_v=int(stock[18]) * 100,
+                bid5_p=stock[17],
+                ask1_v=int(stock[20]) * 100,
+                ask1_p=stock[19],
+                ask2_v=int(stock[22]) * 100,
+                ask2_p=stock[21],
+                ask3_v=int(stock[24]) * 100,
+                ask3_p=stock[23],
+                ask4_v=int(stock[26]) * 100,
+                ask4_p=stock[25],
+                ask5_v=int(stock[28]) * 100,
+                ask5_p=stock[27],
+                interest=0,
+                status="NORMAL",
+                created_dt=stock[30],
+                updated_dt=stock[30],
+            )
+        }
+
+
+if __name__ == "__main__":
+    hq = vxTencentHQ()
+    print(hq("SHSE.600000", "SZSE.000001", "SZSE.300059"))
```

### Comparing `vxquant-2023.3.1/src/vxquant/providers/tdx.py` & `vxquant-2023.4.1/src/vxquant/providers/tdx.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 except ImportError as e:
     raise ImportError("pytdx包未安装，请运行: pip install pytdx 安装。") from e
 
 __TDXHOSTS__ = "__TDXHOSTS__"
 
 
 class TDXExchange(Enum):
+    """通达信市场转换"""
+
     SHSE = TDXParams.MARKET_SH
     SZSE = TDXParams.MARKET_SZ
     BJSE = 2
 
 
 def to_tdx_symbol(symbol):
     """转成tdx的symbol格式: (market,code)
@@ -52,14 +54,16 @@
         market {_type_} -- tdx 的market代码
         code {_type_} -- 证券代码
     """
     return f"{TDXExchange(market).name}.{code}"
 
 
 class TdxHq_APIPool:
+    """tdx行情接口池"""
+
     _hosts = PriorityQueue()
     _apis = Queue()
     _lock = Lock()
 
     def __init__(self):
         self._cost = None
         self._api = None
@@ -85,15 +89,15 @@
                 with suppress(TimeoutError):
                     if tdxapi.connect(host, port, time_out=1):
                         cost = (time.perf_counter() - start) * 1000
                         tdxapi.disconnect()
                         data.append((cost, host, port))
 
             if data:
-                diskcache.set(__TDXHOSTS__, data, 24 * 60 * 60)
+                diskcache.set(__TDXHOSTS__, data, ttl=24 * 60 * 60)
 
         [cls._hosts.put(item) for item in data]
 
     def __enter__(self):
         with self._lock:
             self.reflash_hosts()
```

### Comparing `vxquant-2023.3.1/src/vxquant/scripts/broker.py` & `vxquant-2023.4.1/src/vxquant/modules/broker/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,255 +1,266 @@
-""" run zmq broker"""
-
-import zmq
-import argparse
-
-import contextlib
-from collections.abc import Mapping
-
-from itertools import chain
-from queue import Queue, Empty
-from vxutils import logger, vxZMQContext, to_binary, storage, vxtime, vxWrapper
-
-from vxsched.core import vxengine
-from vxsched.triggers import vxDailyTrigger
-from vxsched.event import vxEvent, vxEventQueue
-
-
-def init_socket(socket_type, settings):
-    ctx = vxZMQContext().instance()
-    socket_ = ctx.socket(socket_type)
-    if settings["connect_mode"].lower() == "connect":
-        socket_.connect(settings["addr"], settings["public_key"])
-    else:
-        socket_.bind(settings["addr"], settings["public_key"])
-    return socket_
-
-
-def on_recv_frontend_msg(engine, msgs):
-    client_addr, empty, packed_event = msgs
-    assert empty == b""
-    event = vxEvent.unpack(packed_event)
-
-    context = engine.context
-    logger.debug(f"frontend 收到来自 {client_addr} 消息: {event}")
-    if event.channel == "__BROKER__":
-        event.reply_to = client_addr
-        engine.submit_event(event)
-    elif event.channel == "__RPC__":
-        if event.type in context.rpc_methods:
-            event.reply_to = client_addr
-            event.channel = context.rpc_methods[event.type]
-            context.backend_queue.put_nowait(event)
-        else:
-            context.frontend_queue.put_nowait(
-                vxEvent(
-                    type="__RPC_REPLY__",
-                    data=AttributeError(f"不支持的远程调用方法: {event.type}"),
-                    channel=client_addr,
-                )
-            )
-    elif event.type.startswith("_"):
-        context.frontend_queue.put_nowait(
-            vxEvent(
-                type="__ACK__",
-                data=ValueError(f"not suport event.type({event.type})"),
-                channel=client_addr,
-            )
-        )
-    else:
-        event.reply_to = ""
-        context.backend_queue.put_nowait(event)
-        context.frontend_queue.put_nowait(
-            vxEvent(type="__ACK__", data="OK", channel=client_addr)
-        )
-
-
-def on_recv_backend_msg(engine, msgs):
-    context = engine.context
-    try:
-        if msgs[0].startswith(b"\x01"):
-            engine.submit_event(
-                vxEvent(
-                    type="__ON_SUBSCRIBE__",
-                    data=msgs[0][1:].decode("ascii"),
-                    channel="__BROKER__",
-                )
-            )
-            return
-
-        if msgs[0].startswith(b"\x00"):
-            engine.submit_event(
-                vxEvent(
-                    type="__ON_UNSUBSCRIBE__",
-                    data=msgs[0][1:].decode("ascii"),
-                    channel="__BROKER__",
-                )
-            )
-            return
-
-        _, packed_event = msgs
-        event = vxEvent.unpack(packed_event)
-        if event.channel == "__BROKER__":
-            engine.submit_event(event)
-        elif event.channel:
-            context.frontend_queue.put(event)
-        else:
-            logger.warning(f"收到错误消息: {event}")
-
-    except Exception as e:
-        logger.error(f"error: {e}", exc_info=True)
-
-
-@vxengine.backend
-def run_broker_backend(engine):
-    context = engine.context
-    context.backend_queue = vxEventQueue()
-    context.frontend_queue = Queue()
-    context.rpc_methods = {}
-
-    for event_type, trigger_params in context.settings.events.items():
-        if isinstance(trigger_params, Mapping):
-            trigger = vxWrapper.init_by_config(trigger_params)
-        elif isinstance(trigger_params, str):
-            trigger = vxDailyTrigger(run_time=trigger_params)
-        else:
-            logger.error(f"不符合设置: {event_type} == {trigger_params}. ")
-        preset_event = vxEvent(type=event_type, trigger=trigger, channel="__BROKER__")
-        context.backend_queue.put(preset_event)
-        logger.info(f"提交预设事件: {preset_event}")
-
-    frontend = init_socket(zmq.ROUTER, context.settings.frontend)
-    backend = init_socket(zmq.XPUB, context.settings.backend)
-
-    poller = zmq.Poller()
-    poller.register(frontend, zmq.POLLIN | zmq.POLLOUT)
-    poller.register(backend, zmq.POLLIN | zmq.POLLOUT)
-
-    while engine.is_alive():
-        flags = dict(poller.poll(1000))
-
-        if frontend in flags and flags[frontend] & zmq.POLLIN != 0:
-            msgs = frontend.recv_multipart()
-            logger.debug(f"frontend msgs: {msgs}")
-            on_recv_frontend_msg(engine, msgs)
-
-        if backend in flags and flags[backend] & zmq.POLLIN != 0:
-            msgs = backend.recv_multipart()
-            logger.debug(f"backend msgs: {msgs}")
-            on_recv_backend_msg(engine, msgs)
-
-        if frontend in flags and flags[frontend] & zmq.POLLOUT != 0:
-            with contextlib.suppress(Empty):
-                event = context.frontend_queue.get(timeout=0.05)
-                frontend.send_multipart(
-                    [to_binary(event.channel), b"", vxEvent.pack(event)]
-                )
-                logger.debug(
-                    f"fronend 发送消息 {event.type} ({event.data})--> {event.channel}"
-                )
-
-        if backend in flags and flags[backend] & zmq.POLLOUT != 0:
-            with contextlib.suppress(Empty):
-                event = context.backend_queue.get(timeout=0.05)
-                backend.send_multipart([to_binary(event.channel), vxEvent.pack(event)])
-                logger.debug(
-                    f"backend 发送消息: {event.type} ({event.data}) --> {event.channel}"
-                )
-        # vxtime.sleep(0.1)
-
-
-@vxengine.event_handler("__ON_SUBSCRIBE__")
-def backend_on_subscribe(context, event) -> None:
-    """订阅事件触发"""
-    logger.error(f"收到订阅信息: {event.data} =====")
-    if event.data.startswith("rpc_"):
-        context.backend_queue.put_nowait(
-            vxEvent(
-                type="__GET_RPCMETHODS__", channel=event.data, reply_to="__BROKER__"
-            )
-        )
-
-
-@vxengine.event_handler("__ON_UNSUBSCRIBE__")
-def backend_on_unsubscribe(context, event) -> None:
-    logger.warning(f"取消订阅信息: {event.data}")
-    if event.data.startswith("rpc_"):
-        context.rpc_methods = {
-            method: channel
-            for method, channel in context.rpc_methods.items()
-            if channel != event.data
-        }
-
-
-def handle_subscribers(context, event) -> None:
-    """处理外部获取的消息"""
-
-    # logger.debug(f"开始抓取subscriber ({context.subscribers})中的消息")
-    if not context.subscribers:
-        return
-
-    events = [subscriber() for subscriber in context.subscribers]
-    for event in chain(*events):
-        context.event_queue.put_nowait(event)
-        logger.info(f"internal: 收到外部event : ({event.type})")
-
-    return
-
-
-@vxengine.event_handler("__GET_RPCMETHODS__")
-def frontend_handle_get_rpc_method(context, event):
-    """前端或许rpc methods"""
-    reply_event = vxEvent(
-        type="__GET_RPCMETHODS__",
-        data=context.rpc_methods,
-        channel=event.reply_to,
-    )
-    context.frontend_queue.put_nowait(reply_event)
-
-
-@vxengine.event_handler("__RPC_METHODS__")
-def backend_on_update_methods(context, event):
-    """更新rpc methods"""
-
-    if isinstance(event.data, Exception):
-        logger.warning(f"更新rpc methods 错误: {event.data}")
-    else:
-        logger.warning(f"更新rpc method: {event.data}")
-        context.rpc_methods.update(event.data)
-
-
-@vxengine.event_handler("__READY__")
-def frontend_ready_event(context, event):
-    """处理前端的ready消息"""
-    reply_event = vxEvent(
-        type="__ACK__",
-        data="OK",
-        channel=event.reply_to,
-    )
-    context.frontend_queue.put_nowait(reply_event)
-    logger.info(f"发送frontend 消息: {reply_event}")
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="""scheduler server""")
-    parser.add_argument("-s", "--script", help="启动组件", default="broker")
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="path to config json file",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    func = storage.get("scheduler", args.script)
-
-    if callable(func):
-        func(args.config, args.mod)
+""" run zmq broker"""
+
+import zmq
+import argparse
+import pathlib
+
+from itertools import chain
+from vxutils import logger
+from concurrent.futures import ThreadPoolExecutor
+from multiprocessing import Lock
+from vxquant.broker.utils import init_socket, frontend_reply, backend_publish
+from vxutils.zmqsocket import zmq_pipe
+from vxsched import vxscheduler, vxContext, vxEvent
+
+
+_default_broker_config = {
+    "settings": {
+        "frontend": {
+            "addr": "tcp://127.0.0.1:5555",
+            "public_key": "",
+            "connect_mode": "bind",
+        },
+        "backend": {
+            "addr": "tcp://127.0.0.1:6666",
+            "public_key": "",
+            "connect_mode": "bind",
+        },
+        "events": {},
+    },
+    "params": {},
+    "rpc_methods": {},
+}
+
+
+def on_recv_frontend_msgs(context, msgs):
+    """处理前端消息
+
+    Arguments:
+        context {vxContext} -- context上下文
+        msgs {[client_addr, b'',packed_event]} -- 收到前端消息清单
+
+    前端消息: channel 为：__BROKER__/gateway ————> vxscheduler.submit_event(event)
+             channel为: __RPC__  ----> vxscheduler.submit
+    """
+    client_addr, empty, packed_event = msgs
+    assert empty == b""
+    event = vxEvent.unpack(packed_event)
+    logger.debug(f"frontend 收到来自 {client_addr} 消息: {event}")
+    if event.channel == "__BROKER__":
+        event.reply_to = client_addr
+        vxscheduler.submit_event(event)
+    elif event.channel == "__RPC__":
+        if event.type not in context.rpc_methods:
+            frontend_reply(
+                context,
+                vxEvent(
+                    type="__RPC_REPLY__",
+                    data=AttributeError(f"不支持的远程调用方法: {event.type}"),
+                    channel=client_addr,
+                ),
+            )
+        event.reply_to = client_addr
+        event.channel = context.rpc_methods[event.type]
+        backend_publish(context, event)
+    elif event.type.startswith("_"):
+        frontend_reply(
+            context,
+            vxEvent(
+                type="__ACK__",
+                data=ValueError(f"not suport event.type({event.type})"),
+                channel=client_addr,
+            ),
+        )
+    else:
+        event.reply_to = ""
+        backend_publish(context, event)
+        frontend_reply(context, vxEvent(type="__ACK__", data="OK", channel=client_addr))
+
+
+def on_recv_backend_msgs(context, msgs):
+    try:
+        if msgs[0].startswith(b"\x01"):
+            vxscheduler.submit_event(
+                vxEvent(
+                    type="__ON_SUBSCRIBE__",
+                    data=msgs[0][1:].decode("ascii"),
+                    channel="__BROKER__",
+                )
+            )
+            return
+
+        if msgs[0].startswith(b"\x00"):
+            vxscheduler.submit_event(
+                vxEvent(
+                    type="__ON_UNSUBSCRIBE__",
+                    data=msgs[0][1:].decode("ascii"),
+                    channel="__BROKER__",
+                )
+            )
+            return
+
+        _, packed_event = msgs
+        event = vxEvent.unpack(packed_event)
+        if event.channel == "__BROKER__":
+            vxscheduler.submit_event(event)
+        elif event.channel:
+            frontend_reply(context, event)
+        else:
+            logger.warning(f"收到错误消息: {event}")
+
+    except Exception as e:
+        logger.error(f"error: {e}", exc_info=True)
+
+
+def on_recv_frontend_recver_msgs(context, msgs):
+    context.frontend.send_multipart(msgs)
+
+
+def on_recv_backend_recver_msgs(context, msgs):
+    context.backend.send_multipart(msgs)
+
+
+def run_broker(config: str = "etc/broker.json", mod_path: str = "mod/"):
+    if pathlib.Path(config).is_file():
+        context = vxContext.load_json(config, _default_broker_config)
+        logger.info(f"加载配置文件: {config} 完成")
+    else:
+        context = vxContext(_default_broker_config)
+        logger.info("使用缺省的配置项")
+
+    context.lock = Lock()
+    context.rpc_methods = {}
+
+    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
+        vxscheduler.load_modules(
+            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
+        )
+
+    if mod_path and pathlib.Path(mod_path).is_dir():
+        vxscheduler.load_modules(mod_path)
+
+    vxscheduler.start(
+        context=context, executor=ThreadPoolExecutor(thread_name_prefix="broker")
+    )
+
+    poller = zmq.Poller()
+
+    frontend = init_socket(zmq.ROUTER, context.settings.frontend)
+    context.frontend = frontend
+    recv_msg_handlers = {frontend: on_recv_frontend_msgs}
+    poller.register(frontend, zmq.POLLIN)
+
+    backend = init_socket(zmq.XPUB, context.settings.backend)
+    context.backend = backend
+    recv_msg_handlers[backend] = on_recv_backend_msgs
+    poller.register(backend, zmq.POLLIN)
+
+    context.frontend_sender, frontend_recver = zmq_pipe()
+    recv_msg_handlers[frontend_recver] = on_recv_frontend_recver_msgs
+    poller.register(frontend_recver, zmq.POLLIN)
+
+    context.backend_sender, backend_recver = zmq_pipe()
+    recv_msg_handlers[backend_recver] = on_recv_backend_recver_msgs
+    poller.register(backend_recver, zmq.POLLIN)
+
+    while vxscheduler.is_alive():
+        flags = dict(poller.poll(1000))
+        for s in flags:
+            try:
+                msgs = s.recv_multipart()
+                recv_msg_handlers[s](context, msgs)
+            except Exception as err:
+                logger.error(f"socket ({s}) handler msg ({msgs}) error: {err}")
+
+
+@vxscheduler.event_handler("__ON_SUBSCRIBE__")
+def backend_on_subscribe(context, event) -> None:
+    """订阅事件触发"""
+    logger.error(f"收到订阅信息: {event.data} =====")
+    if event.data.startswith("rpc_"):
+        context.backend_queue.put_nowait(
+            vxEvent(
+                type="__GET_RPCMETHODS__", channel=event.data, reply_to="__BROKER__"
+            )
+        )
+
+
+@vxscheduler.event_handler("__ON_UNSUBSCRIBE__")
+def backend_on_unsubscribe(context, event) -> None:
+    logger.warning(f"取消订阅信息: {event.data}")
+    if event.data.startswith("rpc_"):
+        context.rpc_methods = {
+            method: channel
+            for method, channel in context.rpc_methods.items()
+            if channel != event.data
+        }
+
+
+def handle_subscribers(context, event) -> None:
+    """处理外部获取的消息"""
+
+    # logger.debug(f"开始抓取subscriber ({context.subscribers})中的消息")
+    if not context.subscribers:
+        return
+
+    events = [subscriber() for subscriber in context.subscribers]
+    for event in chain(*events):
+        context.event_queue.put_nowait(event)
+        logger.info(f"internal: 收到外部event : ({event.type})")
+
+    return
+
+
+@vxscheduler.event_handler("__GET_RPCMETHODS__")
+def frontend_handle_get_rpc_method(context, event):
+    """前端或许rpc methods"""
+    reply_event = vxEvent(
+        type="__GET_RPCMETHODS__",
+        data=context.rpc_methods,
+        channel=event.reply_to,
+    )
+    context.frontend_queue.put_nowait(reply_event)
+
+
+@vxscheduler.event_handler("__RPC_METHODS__")
+def backend_on_update_methods(context, event):
+    """更新rpc methods"""
+
+    if isinstance(event.data, Exception):
+        logger.warning(f"更新rpc methods 错误: {event.data}")
+    else:
+        logger.warning(f"更新rpc method: {event.data}")
+        context.rpc_methods.update(event.data)
+
+
+@vxscheduler.event_handler("__READY__")
+def frontend_ready_event(context, event):
+    """处理前端的ready消息"""
+    reply_event = vxEvent(
+        type="__ACK__",
+        data="OK",
+        channel=event.reply_to,
+    )
+    context.frontend_queue.put_nowait(reply_event)
+    logger.debug(f"发送frontend 消息: {reply_event}")
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="""broker server""")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="path to config json file",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    run_broker(args.config, args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxquant/scripts/gmagent.py` & `vxquant-2023.4.1/src/vxquant/scripts/gmagent.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-"""gmagent"""
-
-
-try:
-    from gm import api as gm_api
-    from vxquant.tdapi.gm import gmTdAPI
-except ImportError:
-    gm_api = None
-    gmTdAPI = None
-
-
-import os
-import pathlib
-from vxutils import logger, vxtime, to_timestamp, to_enum, to_timestring
-from vxsched.triggers import vxDailyTrigger, vxOnceTrigger
-from vxsched import vxscheduler, vxContext
-from vxquant.model.exchange import OrderStatus, TradeStatus
-from vxquant.model.contants import AccountType
-from vxquant.model.preset import vxMarketPreset
-from vxquant.model.tools.gmData import gmOrderConvter, gmTradeConvter
-
-
-__all__ = ["init", "on_tick", "on_order_status", "on_execution_report"]
-
-_default_gmagent_config = {
-    "settings": {
-        "account_type": "NORMAL",
-        "gm_strategyid": "",
-        "gm_token": "",
-        "tick_symbols": [
-            "SHSE.000001",
-            "SHSE.000688",
-            "SHSE.511880",
-            "SHSE.510300",
-            "SHSE.511990",
-            "SHSE.511660",
-            "SHSE.204001",
-            "SZSE.399001",
-            "SZSE.399673",
-            "SZSE.159001",
-            "SZSE.159919",
-            "SZSE.159915",
-            "SZSE.159937",
-            "SZSE.131810",
-        ],
-        "events": {
-            "before_trade": "09:15:00",
-            "on_trade": "09:30:00",
-            "noon_break_start": "11:30:00",
-            "noon_break_end": "13:00:00",
-            "before_close": "14:45:00",
-            "on_close": "14:55:00",
-            "after_close": "15:30:00",
-        },
-        "publisher": {},
-        "subscriber": {},
-    },
-    "params": {},
-    "remote_orders": {},
-    "last_subscriber_time": 0,
-    "has_remote_event": False,
-    "publisher": "",
-    "subscriber": "",
-}
-
-
-def setup_events(vxcontext):
-    # 订阅各种接口
-    tick_symbols = vxcontext.settings["tick_symbols"]
-    gm_api.subscribe(
-        tick_symbols,
-        "tick",
-    )
-    logger.info(f"订阅tick data: {tick_symbols}")
-
-    for event_type, run_time in vxcontext.settings["events"].items():
-        vxscheduler.submit_event(
-            event=event_type, trigger=vxDailyTrigger(run_time=run_time)
-        )
-        logger.info(f"订阅事件{event_type} 触发时间: {run_time}")
-
-    gm_api.schedule(quit_simtrade, "1d", "16:30:00")
-    logger.info("设置退出时间 16:30:00")
-
-
-def setup_sim_events(vxcontext):
-    # 订阅各种接口
-    start_time = int(vxtime.now() + 3)
-    end_time = start_time + 30 * 60
-    vxscheduler.submit_event("before_trade", trigger=vxOnceTrigger(start_time))
-    vxscheduler.submit_event("on_trade", trigger=vxOnceTrigger(start_time + 60))
-    vxscheduler.submit_event(
-        "before_close", trigger=vxOnceTrigger(start_time + 60 * 20)
-    )
-    vxscheduler.submit_event("on_close", trigger=vxOnceTrigger(start_time + 60 * 22))
-    vxscheduler.submit_event("after_close", trigger=vxOnceTrigger(start_time + 60 * 25))
-
-    for i in range(start_time, end_time, 3):
-        run_time = to_timestring(i, "%H:%M:%S")
-        gm_api.schedule(on_tick, "1d", run_time)
-        # logger.info(f"设定on_tick时间: {run_time}")
-
-    gm_api.schedule(quit_simtrade, "1d", to_timestring(end_time, "%H:%M:%S"))
-    logger.info("设置全天消息事件，测试市场30分钟.")
-
-
-def init_context(gmcontext, configfile):
-    vxcontext = vxContext.load_json(configfile, _default_gmagent_config)
-
-    # 拷贝context内容只gmcontext中
-    for k, v in vxcontext.items():
-        setattr(gmcontext, k, v)
-
-    # 设置gm tdapi接口
-    account_type = to_enum(
-        vxcontext.settings["account_type"], AccountType, AccountType.Normal
-    )
-    gmcontext.tdapi = gmTdAPI(gmcontext, account_type)
-
-    gmcontext.broker_orders = gmcontext.tdapi.get_orders()
-    logger.info(f"当前委托订单: {len(gmcontext.broker_orders)}个.")
-
-    gmcontext.broker_trades = gmcontext.tdapi.get_execution_reports()
-    logger.info(f"当前成交回报: {len(gmcontext.broker_trades)}个.")
-
-    account = gmcontext.tdapi.get_account()
-    logger.info(
-        f"检查下单接口是否正常: 账户({account.account_id}) 类型: {account_type} 净资产:"
-        f" {account.nav:,.2f}元."
-    )
-    return gmcontext
-
-
-def init(gmcontext):
-    """
-    掘金量化策略中必须有init方法,且策略会首先运行init定义的内容
-    """
-
-    # 设置 时间函数
-    vxtime.set_timefunc(lambda: to_timestamp(gmcontext.now))
-    logger.info("=" * 80)
-    logger.info(f"{' 初始化开始 ':=^80}")
-    logger.info("=" * 80)
-
-    configfile = os.environ.get("GMCONFIGFILE", "gmagent.json")
-    mod_path = os.environ.get("STRATEGYMOD", "mod/")
-    mode = os.environ.get("mode", "LIVING")
-    init_context(gmcontext, configfile)
-    if mode != "LIVING":
-        setup_sim_events(gmcontext)
-    else:
-        setup_events(gmcontext)
-
-    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
-        vxscheduler.load_modules(
-            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
-        )
-
-    if mod_path and pathlib.Path(mod_path).is_dir():
-        vxscheduler.load_modules(mod_path)
-
-    vxscheduler.initialize(context=gmcontext)
-
-    logger.info("=" * 80)
-    logger.info(f"{' 初始化完成 ':=^80}")
-    logger.info("=" * 80)
-
-
-def on_tick(gmcontext, gmtick=None):
-    """on tick"""
-    vxscheduler.trigger_events()
-
-
-def on_order_status(gmcontext, order):
-    """
-    委托状态更新事件. 参数order为委托信息
-    响应委托状态更新事情，下单后及委托状态更新时被触发
-    3.0.113 后增加.
-    与on_order_status 具有等同含义, 在二者都被定义时(当前函数返回类型为类，速度更快，推介使用), 只会调用 on_order_status_v2
-    """
-    logger.debug(f"gmorder: {order}")
-    vxorder = gmOrderConvter(order)
-
-    if vxorder.exchange_order_id not in gmcontext.broker_orders:
-        gmcontext.broker_orders[vxorder.exchange_order_id] = vxorder
-        logger.info(f"[新增] 委托订单{vxorder.exchange_order_id} 更新为: {vxorder}")
-        vxscheduler.submit_event("on_broker_order_status", vxorder)
-        vxscheduler.trigger_events()
-        return
-
-    broker_order = gmcontext.broker_orders[vxorder.exchange_order_id]
-
-    if broker_order.status in [
-        OrderStatus.Filled,
-        OrderStatus.Expired,
-        OrderStatus.Rejected,
-        OrderStatus.Canceled,
-        OrderStatus.Suspended,
-    ]:
-        logger.debug(
-            f"[忽略更新] 委托订单 {vxorder.exchange_order_id} "
-            f" 当前状态:{broker_order.status} 须更新状态: {vxorder.status}"
-        )
-        return
-
-    if broker_order.filled_volume > vxorder.filled_volume:
-        logger.debug(
-            f"[忽略更新] 委托订单 {vxorder.exchange_order_id} 当前已成交:"
-            f" {broker_order.filled_volume} > 更新状态:{vxorder.filled_volume}"
-        )
-        return
-
-    # 更新委托订单状态
-    broker_order.status = vxorder.status
-    broker_order.filled_volume = vxorder.filled_volume
-    broker_order.filled_amount = vxorder.filled_amount
-    broker_order.updated_dt = vxorder.updated_dt
-    gmcontext.broker_orders[broker_order.exchange_order_id] = broker_order
-    logger.info(f"[更新] 委托订单{vxorder.exchange_order_id} 更新为: {broker_order}")
-    vxscheduler.submit_event("on_broker_order_status", broker_order)
-    vxscheduler.trigger_events()
-
-
-def on_execution_report(gmcontext, execrpt):
-    """
-    委托执行回报事件. 参数 execrpt 为执行回报信息
-    响应委托被执行事件，委托成交后被触发
-    3.0.113 后增加
-    已 on_execution_report 具有等同含义, 在二者都被定义时(当前函数返回类型为类，速度更快，推介使用), 只会调用 on_execution_report_v2
-    """
-
-    logger.debug(f"gmtrade: {execrpt}")
-    vxtrade = gmTradeConvter(execrpt)
-    if vxtrade.commission == 0:
-        _preset = vxMarketPreset(vxtrade.symbol)
-        vxtrade.commission = max(
-            (
-                vxtrade.price
-                * vxtrade.volume
-                * (
-                    _preset.commission_coeff_peramount
-                    if vxtrade.order_direction.name == "Buy"
-                    else (
-                        _preset.commission_coeff_peramount + _preset.tax_coeff_peramount
-                    )
-                )
-            ),
-            5,
-        )
-
-    if vxtrade.status != TradeStatus.Trade:
-        logger.warning(f"收到非成交的回报信息: {vxtrade}")
-        return
-
-    if vxtrade.trade_id in gmcontext.broker_trades:
-        logger.warning("收到重复的委托订单信息")
-        return
-
-    gmcontext.broker_trades[vxtrade.trade_id] = vxtrade
-    vxscheduler.submit_event("on_broker_execution_report", vxtrade)
-    logger.info(f"收到成交回报信息: {vxtrade}")
-    vxscheduler.trigger_events()
-
-
-def quit_simtrade(gmcontext):
-    """退出时调用"""
-    configfile = os.environ.get("GMCONFIGFILE", "gmagent.json")
-    vxscheduler.submit_event("on_exit", data=configfile)
-    vxscheduler.trigger_events()
-    gm_api.stop()
-
-
-if __name__ == "__main__":
-    gm_strategyid = os.environ.get("gm_strategyid", None)
-    gm_token = os.environ.get("gm_token", None)
-
-    assert gm_token is not None
-    assert gm_strategyid is not None
-    logger.info(f"策略ID: {gm_strategyid} token: {gm_token}")
-
-    try:
-        gm_api.run(
-            strategy_id=gm_strategyid,
-            filename="vxquant.agent.gmagent",
-            mode=gm_api.MODE_LIVE,
-            token=gm_token,
-        )
-    finally:
-        vxtime.sleep(5)
+"""gmagent"""
+
+
+try:
+    from gm import api as gm_api
+    from vxquant.tdapi.gm import gmTdAPI
+except ImportError:
+    gm_api = None
+    gmTdAPI = None
+
+
+import os
+import pathlib
+from vxutils import logger, vxtime, to_timestamp, to_enum, to_timestring
+from vxsched.triggers import vxDailyTrigger, vxOnceTrigger
+from vxsched import vxscheduler, vxContext
+from vxquant.model.exchange import OrderStatus, TradeStatus
+from vxquant.model.contants import AccountType
+from vxquant.model.preset import vxMarketPreset
+from vxquant.model.tools.gmData import gmOrderConvter, gmTradeConvter
+
+
+__all__ = ["init", "on_tick", "on_order_status", "on_execution_report"]
+
+_default_gmagent_config = {
+    "settings": {
+        "account_type": "NORMAL",
+        "gm_strategyid": "",
+        "gm_token": "",
+        "tick_symbols": [
+            "SHSE.000001",
+            "SHSE.000688",
+            "SHSE.511880",
+            "SHSE.510300",
+            "SHSE.511990",
+            "SHSE.511660",
+            "SHSE.204001",
+            "SZSE.399001",
+            "SZSE.399673",
+            "SZSE.159001",
+            "SZSE.159919",
+            "SZSE.159915",
+            "SZSE.159937",
+            "SZSE.131810",
+        ],
+        "events": {
+            "before_trade": "09:15:00",
+            "on_trade": "09:30:00",
+            "noon_break_start": "11:30:00",
+            "noon_break_end": "13:00:00",
+            "before_close": "14:45:00",
+            "on_close": "14:55:00",
+            "after_close": "15:30:00",
+        },
+        "publisher": {},
+        "subscriber": {},
+    },
+    "params": {},
+    "remote_orders": {},
+    "last_subscriber_time": 0,
+    "has_remote_event": False,
+    "publisher": "",
+    "subscriber": "",
+}
+
+
+def setup_events(vxcontext):
+    # 订阅各种接口
+    tick_symbols = vxcontext.settings["tick_symbols"]
+    gm_api.subscribe(
+        tick_symbols,
+        "tick",
+    )
+    logger.info(f"订阅tick data: {tick_symbols}")
+
+    for event_type, run_time in vxcontext.settings["events"].items():
+        vxscheduler.submit_event(
+            event=event_type, trigger=vxDailyTrigger(run_time=run_time)
+        )
+        logger.info(f"订阅事件{event_type} 触发时间: {run_time}")
+
+    gm_api.schedule(quit_simtrade, "1d", "16:30:00")
+    logger.info("设置退出时间 16:30:00")
+
+
+def setup_sim_events(vxcontext):
+    # 订阅各种接口
+    start_time = int(vxtime.now() + 3)
+    end_time = start_time + 30 * 60
+    vxscheduler.submit_event("before_trade", trigger=vxOnceTrigger(start_time))
+    vxscheduler.submit_event("on_trade", trigger=vxOnceTrigger(start_time + 60))
+    vxscheduler.submit_event(
+        "before_close", trigger=vxOnceTrigger(start_time + 60 * 20)
+    )
+    vxscheduler.submit_event("on_close", trigger=vxOnceTrigger(start_time + 60 * 22))
+    vxscheduler.submit_event("after_close", trigger=vxOnceTrigger(start_time + 60 * 25))
+
+    for i in range(start_time, end_time, 3):
+        run_time = to_timestring(i, "%H:%M:%S")
+        gm_api.schedule(on_tick, "1d", run_time)
+        # logger.info(f"设定on_tick时间: {run_time}")
+
+    gm_api.schedule(quit_simtrade, "1d", to_timestring(end_time, "%H:%M:%S"))
+    logger.info("设置全天消息事件，测试市场30分钟.")
+
+
+def init_context(gmcontext, configfile):
+    vxcontext = vxContext.load_json(configfile, _default_gmagent_config)
+
+    # 拷贝context内容只gmcontext中
+    for k, v in vxcontext.items():
+        setattr(gmcontext, k, v)
+
+    # 设置gm tdapi接口
+    account_type = to_enum(
+        vxcontext.settings["account_type"], AccountType, AccountType.Normal
+    )
+    gmcontext.tdapi = gmTdAPI(gmcontext, account_type)
+
+    gmcontext.broker_orders = gmcontext.tdapi.get_orders()
+    logger.info(f"当前委托订单: {len(gmcontext.broker_orders)}个.")
+
+    gmcontext.broker_trades = gmcontext.tdapi.get_execution_reports()
+    logger.info(f"当前成交回报: {len(gmcontext.broker_trades)}个.")
+
+    account = gmcontext.tdapi.get_account()
+    logger.info(
+        f"检查下单接口是否正常: 账户({account.account_id}) 类型: {account_type} 净资产:"
+        f" {account.nav:,.2f}元."
+    )
+    return gmcontext
+
+
+def init(gmcontext):
+    """
+    掘金量化策略中必须有init方法,且策略会首先运行init定义的内容
+    """
+
+    # 设置 时间函数
+    vxtime.set_timefunc(lambda: to_timestamp(gmcontext.now))
+    logger.info("=" * 80)
+    logger.info(f"{' 初始化开始 ':=^80}")
+    logger.info("=" * 80)
+
+    configfile = os.environ.get("GMCONFIGFILE", "gmagent.json")
+    mod_path = os.environ.get("STRATEGYMOD", "mod/")
+    mode = os.environ.get("mode", "LIVING")
+    init_context(gmcontext, configfile)
+    if mode != "LIVING":
+        setup_sim_events(gmcontext)
+    else:
+        setup_events(gmcontext)
+
+    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
+        vxscheduler.load_modules(
+            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
+        )
+
+    if mod_path and pathlib.Path(mod_path).is_dir():
+        vxscheduler.load_modules(mod_path)
+
+    vxscheduler.initialize(context=gmcontext)
+
+    logger.info("=" * 80)
+    logger.info(f"{' 初始化完成 ':=^80}")
+    logger.info("=" * 80)
+
+
+def on_tick(gmcontext, gmtick=None):
+    """on tick"""
+    vxscheduler.trigger_events()
+
+
+def on_order_status(gmcontext, order):
+    """
+    委托状态更新事件. 参数order为委托信息
+    响应委托状态更新事情，下单后及委托状态更新时被触发
+    3.0.113 后增加.
+    与on_order_status 具有等同含义, 在二者都被定义时(当前函数返回类型为类，速度更快，推介使用), 只会调用 on_order_status_v2
+    """
+    logger.debug(f"gmorder: {order}")
+    vxorder = gmOrderConvter(order)
+
+    if vxorder.exchange_order_id not in gmcontext.broker_orders:
+        gmcontext.broker_orders[vxorder.exchange_order_id] = vxorder
+        logger.info(f"[新增] 委托订单{vxorder.exchange_order_id} 更新为: {vxorder}")
+        vxscheduler.submit_event("on_broker_order_status", vxorder)
+        vxscheduler.trigger_events()
+        return
+
+    broker_order = gmcontext.broker_orders[vxorder.exchange_order_id]
+
+    if broker_order.status in [
+        OrderStatus.Filled,
+        OrderStatus.Expired,
+        OrderStatus.Rejected,
+        OrderStatus.Canceled,
+        OrderStatus.Suspended,
+    ]:
+        logger.debug(
+            f"[忽略更新] 委托订单 {vxorder.exchange_order_id} "
+            f" 当前状态:{broker_order.status} 须更新状态: {vxorder.status}"
+        )
+        return
+
+    if broker_order.filled_volume > vxorder.filled_volume:
+        logger.debug(
+            f"[忽略更新] 委托订单 {vxorder.exchange_order_id} 当前已成交:"
+            f" {broker_order.filled_volume} > 更新状态:{vxorder.filled_volume}"
+        )
+        return
+
+    # 更新委托订单状态
+    broker_order.status = vxorder.status
+    broker_order.filled_volume = vxorder.filled_volume
+    broker_order.filled_amount = vxorder.filled_amount
+    broker_order.updated_dt = vxorder.updated_dt
+    gmcontext.broker_orders[broker_order.exchange_order_id] = broker_order
+    logger.info(f"[更新] 委托订单{vxorder.exchange_order_id} 更新为: {broker_order}")
+    vxscheduler.submit_event("on_broker_order_status", broker_order)
+    vxscheduler.trigger_events()
+
+
+def on_execution_report(gmcontext, execrpt):
+    """
+    委托执行回报事件. 参数 execrpt 为执行回报信息
+    响应委托被执行事件，委托成交后被触发
+    3.0.113 后增加
+    已 on_execution_report 具有等同含义, 在二者都被定义时(当前函数返回类型为类，速度更快，推介使用), 只会调用 on_execution_report_v2
+    """
+
+    logger.debug(f"gmtrade: {execrpt}")
+    vxtrade = gmTradeConvter(execrpt)
+    if vxtrade.commission == 0:
+        _preset = vxMarketPreset(vxtrade.symbol)
+        vxtrade.commission = max(
+            (
+                vxtrade.price
+                * vxtrade.volume
+                * (
+                    _preset.commission_coeff_peramount
+                    if vxtrade.order_direction.name == "Buy"
+                    else (
+                        _preset.commission_coeff_peramount + _preset.tax_coeff_peramount
+                    )
+                )
+            ),
+            5,
+        )
+
+    if vxtrade.status != TradeStatus.Trade:
+        logger.warning(f"收到非成交的回报信息: {vxtrade}")
+        return
+
+    if vxtrade.trade_id in gmcontext.broker_trades:
+        logger.warning("收到重复的委托订单信息")
+        return
+
+    gmcontext.broker_trades[vxtrade.trade_id] = vxtrade
+    vxscheduler.submit_event("on_broker_execution_report", vxtrade)
+    logger.info(f"收到成交回报信息: {vxtrade}")
+    vxscheduler.trigger_events()
+
+
+def quit_simtrade(gmcontext):
+    """退出时调用"""
+    configfile = os.environ.get("GMCONFIGFILE", "gmagent.json")
+    vxscheduler.submit_event("on_exit", data=configfile)
+    vxscheduler.trigger_events()
+    gm_api.stop()
+
+
+if __name__ == "__main__":
+    gm_strategyid = os.environ.get("gm_strategyid", None)
+    gm_token = os.environ.get("gm_token", None)
+
+    assert gm_token is not None
+    assert gm_strategyid is not None
+    logger.info(f"策略ID: {gm_strategyid} token: {gm_token}")
+
+    try:
+        gm_api.run(
+            strategy_id=gm_strategyid,
+            filename="vxquant.agent.gmagent",
+            mode=gm_api.MODE_LIVE,
+            token=gm_token,
+        )
+    finally:
+        vxtime.sleep(5)
```

### Comparing `vxquant-2023.3.1/src/vxquant/scripts/qmtagent.py` & `vxquant-2023.4.1/src/vxquant/scripts/qmtagent.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-"""miniQMT 交易接口"""
-import os
-import argparse
-import pathlib
-from enum import Enum
-from concurrent.futures import ThreadPoolExecutor
-from vxquant.tdapi.miniqmt import miniQMTCallback
-from vxquant.model.tools.qmtData import qmtOrderConvter, qmtTradeConvter
-from vxquant.model.contants import OrderStatus, TradeStatus
-from vxquant.model.preset import vxMarketPreset
-from vxsched import vxEngine, vxContext, vxDailyTrigger, vxscheduler
-from vxutils import vxtime, logger, vxWrapper
-
-
-_default_qmtagent_config = {
-    "settings": {
-        "tdapi": {
-            "class": "vxquant.tdapi.minqmt.vxQMTTdAPI",
-            "params": {"miniqmt_path": "", "account_id": "", "account_type": "NORMAL"},
-        },
-        "events": {
-            "before_trade": "09:15:00",
-            "on_trade": "09:30:00",
-            "noon_break_start": "11:30:00",
-            "noon_break_end": "13:00:00",
-            "before_close": "14:45:00",
-            "on_close": "14:55:00",
-            "after_close": "15:30:00",
-            "on_exit": "16:30:00",
-        },
-        "publisher": {},
-        "subscriber": {},
-    },
-    "params": {},
-    "remote_orders": {},
-    "last_subscriber_time": 0,
-    "has_remote_event": False,
-    "publisher": "",
-    "subscriber": "",
-}
-
-
-class QMTAccountStatus(Enum):
-    INVALID = -1
-    OK = 0
-    WAITING_LOGIN = 1
-    STATUSING = 2
-    FAIL = 3
-    INITING = 4
-    CORRECTING = 5
-    CLOSED = 6
-    ASSIS_FAIL = 7
-    DISABLEBYSYS = 8
-    DISABLEBYUSER = 9
-
-
-class miniQMTAgentCallback(miniQMTCallback):
-    def __init__(self, engine: vxEngine) -> None:
-        super().__init__()
-        self._engine = engine
-
-    def on_connected(self):
-        """
-        连接成功推送
-        """
-        logger.info("连接成功")
-
-    def on_disconnected(self):
-        """
-        连接状态回调
-        :return:
-        """
-        logger.warning("连接断开")
-
-    def on_account_status(self, status):
-        """
-        账号状态信息推送
-        :param response: XtAccountStatus 对象
-        :return:
-        """
-        logger.info(
-            "账户状态变更为:"
-            f" {status.account_id} {status.account_type} {QMTAccountStatus(status.status)}"
-        )
-
-    def on_stock_asset(self, asset):
-        """
-        资金信息推送
-        :param asset: XtAsset对象
-        :return:
-        """
-        logger.info(
-            f"on asset callback {asset.account_id}, {asset.cash}, {asset.total_asset}"
-        )
-
-    def on_stock_order(self, order):
-        """
-        委托信息推送
-        :param order: XtOrder对象
-        :return:
-        """
-        logger.debug(
-            f"收到成交更新: {order.stock_code} {order.order_status} {order.order_sysid}"
-        )
-        vxorder = qmtOrderConvter(order)
-
-        if vxorder.exchange_order_id not in self.broker_orders:
-            self.broker_orders[vxorder.exchange_order_id] = vxorder
-            logger.info(f"[新增] 委托订单{vxorder.exchange_order_id} 更新为: {vxorder}")
-            self._engine.submit_event("on_broker_order_status", vxorder)
-            self._engine.trigger_events()
-            return
-
-        broker_order = self.broker_orders[vxorder.exchange_order_id]
-        if broker_order.status in [
-            OrderStatus.Filled,
-            OrderStatus.Expired,
-            OrderStatus.Rejected,
-            OrderStatus.Canceled,
-            OrderStatus.Suspended,
-        ]:
-            logger.debug(
-                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} "
-                f" 当前状态:{broker_order.status} 须更新状态: {vxorder.status}"
-            )
-            return
-
-        if broker_order.filled_volume > vxorder.filled_volume:
-            logger.debug(
-                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} 当前已成交:"
-                f" {broker_order.filled_volume} > 更新状态:{vxorder.filled_volume}"
-            )
-            return
-
-        # 更新委托订单状态
-        broker_order.status = vxorder.status
-        broker_order.filled_volume = vxorder.filled_volume
-        broker_order.filled_amount = vxorder.filled_amount
-        broker_order.updated_dt = vxorder.updated_dt
-        self.broker_orders[broker_order.exchange_order_id] = broker_order
-        logger.info(f"[更新] 委托订单{vxorder.exchange_order_id} 更新为: {broker_order}")
-        self._engine.submit_event("on_broker_order_status", broker_order)
-        self._engine.trigger_events()
-
-    def on_stock_trade(self, trade):
-        """
-        成交信息推送
-        :param trade: XtTrade对象
-        :return:
-        """
-        logger.debug(
-            f"收到成交信息: {trade.account_id}, {trade.stock_code}, {trade.order_id}"
-        )
-        vxtrade = qmtTradeConvter(trade)
-        if vxtrade.trade_id in self.broker_trades:
-            logger.warning("收到重复的委托订单信息")
-            return
-
-        if vxtrade.status != TradeStatus.Trade:
-            logger.warning(f"收到非成交的回报信息: {vxtrade}")
-            return
-
-        if vxtrade.commission == 0:
-            _preset = vxMarketPreset(vxtrade.symbol)
-            vxtrade.commission = max(
-                (
-                    vxtrade.price
-                    * vxtrade.volume
-                    * (
-                        _preset.commission_coeff_peramount
-                        if vxtrade.order_direction.name == "Buy"
-                        else (
-                            _preset.commission_coeff_peramount
-                            + _preset.tax_coeff_peramount
-                        )
-                    )
-                ),
-                5,
-            )
-
-        self.broker_trades[vxtrade.trade_id] = vxtrade
-        logger.info(f"收到成交回报信息: {vxtrade}")
-        self._engine.submit_event("on_broker_execution_report", vxtrade)
-        self._engine.trigger_events()
-
-    def on_stock_position(self, position):
-        """
-        持仓信息推送
-        :param position: XtPosition对象
-        :return:
-        """
-        logger.info(f"持仓信息推送: {position.stock_code}, {position.volume}")
-
-    def on_order_error(self, order_error):
-        """
-        下单失败信息推送
-        :param order_error:XtOrderError 对象
-        :return:
-        """
-
-        if order_error.order_id not in self.broker_orders:
-            logger.warning(
-                f"下单失败: {order_error.order_id}, {order_error.error_id},"
-                f" {order_error.error_msg}"
-            )
-            return
-
-        broker_order = self.broker_orders[order_error.order_id]
-        if broker_order.status in [
-            OrderStatus.Filled,
-            OrderStatus.Expired,
-            OrderStatus.Rejected,
-            OrderStatus.Canceled,
-            OrderStatus.Suspended,
-        ]:
-            logger.debug(
-                f"[忽略更新] 委托订单 {order_error.exchange_order_id} "
-                f" 当前状态:{broker_order.status} 须更新状态: {order_error.error_msg}"
-            )
-            return
-
-        broker_order.status = "Rejected"
-        broker_order.reject_code = "UnknownOrder"
-        broker_order.reject_reason = order_error.error_msg
-        self._engine.submit_event("on_broker_order_status", broker_order)
-        self._engine.trigger_events()
-
-
-def run_qmtagent(config: str, mod_path: str = "mod/") -> None:
-    context = vxContext.load_json(config, _default_qmtagent_config)
-    context.configfile = config
-    if context.settings.tdapi:
-        context.tdapi = vxWrapper.init_by_config(context.settings.tdapi)
-        account_info = context.tdapi.get_account()
-        logger.info(
-            f"[测试下单接口] 账号 {account_info.account_id} 总资产：{account_info.nav:,.2f}元"
-        )
-        callback = miniQMTAgentCallback(vxscheduler)
-        context.tdapi.register_callback(callback)
-    else:
-        context.tdapi = None
-
-    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
-        vxscheduler.load_modules(
-            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
-        )
-
-    if mod_path and pathlib.Path(mod_path).is_dir():
-        vxscheduler.load_modules(mod_path)
-
-    for event_type, run_time in context.settings["events"].items():
-        vxscheduler.submit_event(
-            event=event_type, trigger=vxDailyTrigger(run_time=run_time)
-        )
-        logger.info(f"订阅事件{event_type} 触发时间: {run_time}")
-
-    vxscheduler.submit_event("on_exit", data=config, trigger=vxDailyTrigger("16:30:00"))
-
-    logger.info("=" * 80)
-    logger.info(f"{' 初始化完成 ':=^80}")
-    logger.info("=" * 80)
-
-    try:
-        vxscheduler.start(
-            context=context,
-            executor=ThreadPoolExecutor(thread_name_prefix="workerpool"),
-        )
-        while vxscheduler.is_alive():
-            vxtime.sleep(1)
-    finally:
-        context.tdapi.stop()
-        logger.warning("=" * 80)
-        logger.warning(f"{' 当天交易结束 ':*^80}")
-        logger.warning("=" * 80)
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="""miniqmt agent server""")
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="path to config json file",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    run_qmtagent(args.config, args.mod)
+"""miniQMT 交易接口"""
+import os
+import argparse
+import pathlib
+from enum import Enum
+from concurrent.futures import ThreadPoolExecutor
+from vxquant.tdapi.miniqmt import miniQMTCallback
+from vxquant.model.tools.qmtData import qmtOrderConvter, qmtTradeConvter
+from vxquant.model.contants import OrderStatus, TradeStatus
+from vxquant.model.preset import vxMarketPreset
+from vxsched import vxEngine, vxContext, vxDailyTrigger, vxscheduler
+from vxutils import vxtime, logger, vxWrapper
+
+
+_default_qmtagent_config = {
+    "settings": {
+        "tdapi": {
+            "class": "vxquant.tdapi.minqmt.vxQMTTdAPI",
+            "params": {"miniqmt_path": "", "account_id": "", "account_type": "NORMAL"},
+        },
+        "events": {
+            "before_trade": "09:15:00",
+            "on_trade": "09:30:00",
+            "noon_break_start": "11:30:00",
+            "noon_break_end": "13:00:00",
+            "before_close": "14:45:00",
+            "on_close": "14:55:00",
+            "after_close": "15:30:00",
+            "on_exit": "16:30:00",
+        },
+        "publisher": {},
+        "subscriber": {},
+    },
+    "params": {},
+    "remote_orders": {},
+    "last_subscriber_time": 0,
+    "has_remote_event": False,
+    "publisher": "",
+    "subscriber": "",
+}
+
+
+class QMTAccountStatus(Enum):
+    INVALID = -1
+    OK = 0
+    WAITING_LOGIN = 1
+    STATUSING = 2
+    FAIL = 3
+    INITING = 4
+    CORRECTING = 5
+    CLOSED = 6
+    ASSIS_FAIL = 7
+    DISABLEBYSYS = 8
+    DISABLEBYUSER = 9
+
+
+class miniQMTAgentCallback(miniQMTCallback):
+    def __init__(self, engine: vxEngine) -> None:
+        super().__init__()
+        self._engine = engine
+
+    def on_connected(self):
+        """
+        连接成功推送
+        """
+        logger.info("连接成功")
+
+    def on_disconnected(self):
+        """
+        连接状态回调
+        :return:
+        """
+        logger.warning("连接断开")
+
+    def on_account_status(self, status):
+        """
+        账号状态信息推送
+        :param response: XtAccountStatus 对象
+        :return:
+        """
+        logger.info(
+            "账户状态变更为:"
+            f" {status.account_id} {status.account_type} {QMTAccountStatus(status.status)}"
+        )
+
+    def on_stock_asset(self, asset):
+        """
+        资金信息推送
+        :param asset: XtAsset对象
+        :return:
+        """
+        logger.info(
+            f"on asset callback {asset.account_id}, {asset.cash}, {asset.total_asset}"
+        )
+
+    def on_stock_order(self, order):
+        """
+        委托信息推送
+        :param order: XtOrder对象
+        :return:
+        """
+        logger.debug(
+            f"收到成交更新: {order.stock_code} {order.order_status} {order.order_sysid}"
+        )
+        vxorder = qmtOrderConvter(order)
+
+        if vxorder.exchange_order_id not in self.broker_orders:
+            self.broker_orders[vxorder.exchange_order_id] = vxorder
+            logger.info(f"[新增] 委托订单{vxorder.exchange_order_id} 更新为: {vxorder}")
+            self._engine.submit_event("on_broker_order_status", vxorder)
+            self._engine.trigger_events()
+            return
+
+        broker_order = self.broker_orders[vxorder.exchange_order_id]
+        if broker_order.status in [
+            OrderStatus.Filled,
+            OrderStatus.Expired,
+            OrderStatus.Rejected,
+            OrderStatus.Canceled,
+            OrderStatus.Suspended,
+        ]:
+            logger.debug(
+                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} "
+                f" 当前状态:{broker_order.status} 须更新状态: {vxorder.status}"
+            )
+            return
+
+        if broker_order.filled_volume > vxorder.filled_volume:
+            logger.debug(
+                f"[忽略更新] 委托订单 {vxorder.exchange_order_id} 当前已成交:"
+                f" {broker_order.filled_volume} > 更新状态:{vxorder.filled_volume}"
+            )
+            return
+
+        # 更新委托订单状态
+        broker_order.status = vxorder.status
+        broker_order.filled_volume = vxorder.filled_volume
+        broker_order.filled_amount = vxorder.filled_amount
+        broker_order.updated_dt = vxorder.updated_dt
+        self.broker_orders[broker_order.exchange_order_id] = broker_order
+        logger.info(f"[更新] 委托订单{vxorder.exchange_order_id} 更新为: {broker_order}")
+        self._engine.submit_event("on_broker_order_status", broker_order)
+        self._engine.trigger_events()
+
+    def on_stock_trade(self, trade):
+        """
+        成交信息推送
+        :param trade: XtTrade对象
+        :return:
+        """
+        logger.debug(
+            f"收到成交信息: {trade.account_id}, {trade.stock_code}, {trade.order_id}"
+        )
+        vxtrade = qmtTradeConvter(trade)
+        if vxtrade.trade_id in self.broker_trades:
+            logger.warning("收到重复的委托订单信息")
+            return
+
+        if vxtrade.status != TradeStatus.Trade:
+            logger.warning(f"收到非成交的回报信息: {vxtrade}")
+            return
+
+        if vxtrade.commission == 0:
+            _preset = vxMarketPreset(vxtrade.symbol)
+            vxtrade.commission = max(
+                (
+                    vxtrade.price
+                    * vxtrade.volume
+                    * (
+                        _preset.commission_coeff_peramount
+                        if vxtrade.order_direction.name == "Buy"
+                        else (
+                            _preset.commission_coeff_peramount
+                            + _preset.tax_coeff_peramount
+                        )
+                    )
+                ),
+                5,
+            )
+
+        self.broker_trades[vxtrade.trade_id] = vxtrade
+        logger.info(f"收到成交回报信息: {vxtrade}")
+        self._engine.submit_event("on_broker_execution_report", vxtrade)
+        self._engine.trigger_events()
+
+    def on_stock_position(self, position):
+        """
+        持仓信息推送
+        :param position: XtPosition对象
+        :return:
+        """
+        logger.info(f"持仓信息推送: {position.stock_code}, {position.volume}")
+
+    def on_order_error(self, order_error):
+        """
+        下单失败信息推送
+        :param order_error:XtOrderError 对象
+        :return:
+        """
+
+        if order_error.order_id not in self.broker_orders:
+            logger.warning(
+                f"下单失败: {order_error.order_id}, {order_error.error_id},"
+                f" {order_error.error_msg}"
+            )
+            return
+
+        broker_order = self.broker_orders[order_error.order_id]
+        if broker_order.status in [
+            OrderStatus.Filled,
+            OrderStatus.Expired,
+            OrderStatus.Rejected,
+            OrderStatus.Canceled,
+            OrderStatus.Suspended,
+        ]:
+            logger.debug(
+                f"[忽略更新] 委托订单 {order_error.exchange_order_id} "
+                f" 当前状态:{broker_order.status} 须更新状态: {order_error.error_msg}"
+            )
+            return
+
+        broker_order.status = "Rejected"
+        broker_order.reject_code = "UnknownOrder"
+        broker_order.reject_reason = order_error.error_msg
+        self._engine.submit_event("on_broker_order_status", broker_order)
+        self._engine.trigger_events()
+
+
+def run_qmtagent(config: str, mod_path: str = "mod/") -> None:
+    context = vxContext.load_json(config, _default_qmtagent_config)
+    context.configfile = config
+    if context.settings.tdapi:
+        context.tdapi = vxWrapper.init_by_config(context.settings.tdapi)
+        account_info = context.tdapi.get_account()
+        logger.info(
+            f"[测试下单接口] 账号 {account_info.account_id} 总资产：{account_info.nav:,.2f}元"
+        )
+        callback = miniQMTAgentCallback(vxscheduler)
+        context.tdapi.register_callback(callback)
+    else:
+        context.tdapi = None
+
+    if pathlib.Path(__file__).parent.joinpath("mod/").is_dir():
+        vxscheduler.load_modules(
+            pathlib.Path(__file__).parent.joinpath("mod/").as_posix()
+        )
+
+    if mod_path and pathlib.Path(mod_path).is_dir():
+        vxscheduler.load_modules(mod_path)
+
+    for event_type, run_time in context.settings["events"].items():
+        vxscheduler.submit_event(
+            event=event_type, trigger=vxDailyTrigger(run_time=run_time)
+        )
+        logger.info(f"订阅事件{event_type} 触发时间: {run_time}")
+
+    vxscheduler.submit_event("on_exit", data=config, trigger=vxDailyTrigger("16:30:00"))
+
+    logger.info("=" * 80)
+    logger.info(f"{' 初始化完成 ':=^80}")
+    logger.info("=" * 80)
+
+    try:
+        vxscheduler.start(
+            context=context,
+            executor=ThreadPoolExecutor(thread_name_prefix="workerpool"),
+        )
+        while vxscheduler.is_alive():
+            vxtime.sleep(1)
+    finally:
+        context.tdapi.stop()
+        logger.warning("=" * 80)
+        logger.warning(f"{' 当天交易结束 ':*^80}")
+        logger.warning("=" * 80)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="""miniqmt agent server""")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="path to config json file",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    run_qmtagent(args.config, args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxquant/scripts/worker.py` & `vxquant-2023.4.1/src/vxquant/scripts/worker.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-""" run zmq worker"""
-
-import zmq
-import argparse
-import pathlib
-import contextlib
-from queue import Queue, Empty
-from vxutils import logger, vxZMQContext, to_binary, to_text, storage, vxtime
-from vxsched.context import vxContext
-from vxsched.core import vxengine
-from vxsched.event import vxEvent
-from vxsched.rpc import rpcwrapper
-
-
-@vxengine.event_handler("__init__")
-def init_worker(context, event):
-    context.reply_queue = Queue()
-    logger.info(f"初始化 workder: {context}")
-
-
-@vxengine.event_handler("__GET_RPCMETHODS__")
-def on_recv_msg(context, event):
-    reply_event = vxEvent(
-        type="__RPC_METHODS__",
-        data=rpcwrapper.methods,
-        channel="__BROKER__",
-    )
-    context.reply_queue.put_nowait(reply_event)
-    logger.info(f"注册rpc method: {reply_event.data}")
-
-
-@vxengine.event_handler("__RPC_CALL__")
-def handle_rpc_call(context, event):
-    rpc_event = event.data
-    args, kwargs = rpc_event.data
-    try:
-        reply_msg = rpcwrapper(rpc_event.type, *args, **kwargs)
-    except Exception as e:
-        reply_msg = e
-        logger.error(f"运行错误： {reply_msg}", exc_info=True)
-
-    context.reply_queue.put_nowait(
-        vxEvent(
-            type=rpc_event.type,
-            data=rpc_event.data,
-            channel=rpc_event.reply_to,
-        )
-    )
-
-
-def create_socket(engine):
-    zmqbackend_settings = engine.context.settings["zmqbackend"]
-
-    addr = zmqbackend_settings["addr"]
-    public_key = zmqbackend_settings["public_key"]
-    connect_mode = zmqbackend_settings["connect_mode"].lower()
-
-    ctx = vxZMQContext()
-    socket = ctx.socket(zmq.XSUB)
-
-    if connect_mode == "connect":
-        socket.connect(addr, public_key)
-    else:
-        socket.bind(addr, public_key)
-
-    socket.send(b"\x01" + to_binary("__BROKER__"))
-    logger.info("订阅缺省消息通道: __BROKER__")
-
-    channels = zmqbackend_settings["channels"]
-    for channel in channels:
-        socket.send(b"\x01" + to_binary(channel))
-        logger.info(f"订阅消息通道: {channel}")
-
-    if rpcwrapper.methods:
-        socket.send(b"\x01" + to_binary(rpcwrapper.rpc_token))
-        logger.info(f"订阅RPC通道: {rpcwrapper.rpc_token}")
-        engine.submit_event("__GET_RPCMETHODS__")
-
-    return socket
-
-
-@vxengine.backend
-def zmqbackend(engine):
-    socket = create_socket(engine)
-    while engine.is_alive():
-        flags = socket.poll(1000, zmq.POLLIN | zmq.POLLOUT)
-        try:
-            if flags & zmq.POLLIN != 0:
-                channel, packed_event = socket.recv_multipart()
-                channel = to_text(channel)
-                recv_event = vxEvent.unpack(packed_event)
-                logger.debug(f"收到来自{channel} 发送消息: {recv_event.type}")
-                if channel.startswith("rpc_"):
-                    engine.submit_event("__RPC_CALL__", recv_event)
-                else:
-                    engine.submit_event(recv_event)
-
-            if flags & zmq.POLLOUT != 0:
-                with contextlib.suppress(Empty):
-                    rpc_reply = engine.context.reply_queue.get(timeout=0.1)
-                    msgs = [to_binary(rpc_reply.channel), vxEvent.pack(rpc_reply)]
-                    socket.send_multipart(msgs)
-        except Exception as err:
-            logger.warning(f"运行时错误: {err}", exc_info=True)
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="""worker server""")
-    parser.add_argument("-s", "--script", help="启动组件", default="worker")
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="path to config json file",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    func = storage.get("scheduler", args.script)
-
-    if callable(func):
-        func(args.config, args.mod)
+""" run zmq worker"""
+
+import zmq
+import argparse
+import pathlib
+import contextlib
+from queue import Queue, Empty
+from vxutils import logger, vxZMQContext, to_binary, to_text, storage, vxtime
+from vxsched.context import vxContext
+from vxsched.core import vxengine
+from vxsched.event import vxEvent
+from vxsched.rpc import rpcwrapper
+
+
+@vxengine.event_handler("__init__")
+def init_worker(context, event):
+    context.reply_queue = Queue()
+    logger.info(f"初始化 workder: {context}")
+
+
+@vxengine.event_handler("__GET_RPCMETHODS__")
+def on_recv_msg(context, event):
+    reply_event = vxEvent(
+        type="__RPC_METHODS__",
+        data=rpcwrapper.methods,
+        channel="__BROKER__",
+    )
+    context.reply_queue.put_nowait(reply_event)
+    logger.info(f"注册rpc method: {reply_event.data}")
+
+
+@vxengine.event_handler("__RPC_CALL__")
+def handle_rpc_call(context, event):
+    rpc_event = event.data
+    args, kwargs = rpc_event.data
+    try:
+        reply_msg = rpcwrapper(rpc_event.type, *args, **kwargs)
+    except Exception as e:
+        reply_msg = e
+        logger.error(f"运行错误： {reply_msg}", exc_info=True)
+
+    context.reply_queue.put_nowait(
+        vxEvent(
+            type=rpc_event.type,
+            data=rpc_event.data,
+            channel=rpc_event.reply_to,
+        )
+    )
+
+
+def create_socket(engine):
+    zmqbackend_settings = engine.context.settings["zmqbackend"]
+
+    addr = zmqbackend_settings["addr"]
+    public_key = zmqbackend_settings["public_key"]
+    connect_mode = zmqbackend_settings["connect_mode"].lower()
+
+    ctx = vxZMQContext()
+    socket = ctx.socket(zmq.XSUB)
+
+    if connect_mode == "connect":
+        socket.connect(addr, public_key)
+    else:
+        socket.bind(addr, public_key)
+
+    socket.send(b"\x01" + to_binary("__BROKER__"))
+    logger.info("订阅缺省消息通道: __BROKER__")
+
+    channels = zmqbackend_settings["channels"]
+    for channel in channels:
+        socket.send(b"\x01" + to_binary(channel))
+        logger.info(f"订阅消息通道: {channel}")
+
+    if rpcwrapper.methods:
+        socket.send(b"\x01" + to_binary(rpcwrapper.rpc_token))
+        logger.info(f"订阅RPC通道: {rpcwrapper.rpc_token}")
+        engine.submit_event("__GET_RPCMETHODS__")
+
+    return socket
+
+
+@vxengine.backend
+def zmqbackend(engine):
+    socket = create_socket(engine)
+    while engine.is_alive():
+        flags = socket.poll(1000, zmq.POLLIN | zmq.POLLOUT)
+        try:
+            if flags & zmq.POLLIN != 0:
+                channel, packed_event = socket.recv_multipart()
+                channel = to_text(channel)
+                recv_event = vxEvent.unpack(packed_event)
+                logger.debug(f"收到来自{channel} 发送消息: {recv_event.type}")
+                if channel.startswith("rpc_"):
+                    engine.submit_event("__RPC_CALL__", recv_event)
+                else:
+                    engine.submit_event(recv_event)
+
+            if flags & zmq.POLLOUT != 0:
+                with contextlib.suppress(Empty):
+                    rpc_reply = engine.context.reply_queue.get(timeout=0.1)
+                    msgs = [to_binary(rpc_reply.channel), vxEvent.pack(rpc_reply)]
+                    socket.send_multipart(msgs)
+        except Exception as err:
+            logger.warning(f"运行时错误: {err}", exc_info=True)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="""worker server""")
+    parser.add_argument("-s", "--script", help="启动组件", default="worker")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="path to config json file",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument("-m", "--mod", help="模块存放目录", default="./mod", type=str)
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    func = storage.get("scheduler", args.script)
+
+    if callable(func):
+        func(args.config, args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxquant/tdapi/base.py` & `vxquant-2023.4.1/src/vxquant/tdapi/base.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-"""交易接口"""
-
-import pandas as pd
-from abc import ABC, abstractmethod
-from typing import Dict, List, Optional, Union
-from vxquant.model.preset import vxMarketPreset
-from vxutils import vxtime
-from vxquant.model.exchange import (
-    vxAccountInfo,
-    vxAlgoOrder,
-    vxCashPosition,
-    vxOrder,
-    vxPosition,
-    vxTick,
-    vxTrade,
-)
-from vxquant.model.contants import (
-    OrderDirection,
-    OrderOffset,
-    OrderStatus,
-    OrderType,
-    SecType,
-)
-
-
-class vxTdAPIBase(ABC):
-    """交易接口类"""
-
-    def __init__(self):
-        self._cache = {}
-        self._cached_at = 0
-
-    @abstractmethod
-    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
-        """获取最新的ticks 数据
-
-        Returns:
-            Dict[str,vxTick] -- 返回最新的tick数据
-        """
-
-    def current(self, *symbols: List[str]) -> Dict[str, vxTick]:
-        """实时行情信息
-
-        Arguments:
-            symbols {List[str]} -- 证券交易代码
-        """
-        if not symbols:
-            raise ValueError("symbols must not null.")
-
-        if isinstance(symbols[0], list):
-            symbols = symbols[0]
-
-        symbols = list(symbols)
-
-        now = vxtime.now()
-        if now > (self._cached_at + 3):
-            symbols.extend(self._cache.keys())
-            self._cache = {}
-            self._cached_at = now
-
-        target_symbols = set(symbols) - set(self._cache.keys())
-        vxticks = self.get_ticks(*target_symbols)
-        self._cache.update(vxticks)
-
-        return {
-            symbol: self._cache[symbol] for symbol in symbols if symbol in self._cache
-        }
-
-    @abstractmethod
-    def get_account(self) -> vxAccountInfo:
-        """获取账户基本信息"""
-
-    @abstractmethod
-    def get_positions(
-        self, symbol: str = None
-    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
-        """获取持仓信息
-
-        Keyword Arguments:
-            symbol {str} -- 对应的持仓信息 (default: {None})
-
-        Returns:
-            Dict[str, Union[vxCashPosition,vxPosition]] -- 返回持仓列表
-        """
-
-    @abstractmethod
-    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
-        """提交委托订单
-
-        Arguments:
-            vxorders {List[vxOrder]} -- 待提交的委托订单
-        """
-
-    def order_volume(
-        self, symbol: str, volume: int, price: Optional[float] = 0
-    ) -> vxOrder:
-        """下单
-
-        Arguments:
-            account_id {str} -- _description_
-            symbol {str} -- _description_
-            volume {int} -- _description_
-            price {Optional[float]} -- _description_ (default: {None})
-
-        Returns:
-            vxorder {vxOrder} -- 下单委托订单号
-        """
-        if volume == 0:
-            raise ValueError("volume can't be 0.")
-
-        if (
-            not price
-            and vxMarketPreset(symbol).security_type == SecType.BOND_CONVERTIBLE
-        ):
-            ticks = self.current(symbol)
-            price = ticks[symbol].ask1_p if volume > 0 else ticks[symbol].bid1_p
-
-        vxorder = vxOrder(
-            symbol=symbol,
-            volume=abs(volume),
-            price=price,
-            order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
-            order_direction=OrderDirection.Buy if volume > 0 else OrderDirection.Sell,
-            order_type=OrderType.Market if price <= 0 else OrderType.Limit,
-            status=OrderStatus.PendingNew,
-        )
-
-        ret_orders = self.order_batch(vxorder)
-        return ret_orders[0]
-
-    @abstractmethod
-    def get_orders(self) -> List[vxOrder]:
-        """获取当日委托订单列表
-
-        Returns:
-            List[vxOrder] -- 当日委托订单列表
-        """
-
-    @abstractmethod
-    def get_execution_reports(self) -> List[vxTrade]:
-        """获取当日成交回报信息
-
-        Returns:
-            List[vxTrade] -- 当日成交回报列表
-        """
-
-    @abstractmethod
-    def order_cancel(self, *orders: List[vxOrder]) -> None:
-        """撤单
-
-        Arguments:
-            orders {List[vxOrder]} -- 待撤销订单
-        """
+"""交易接口"""
+
+import pandas as pd
+from abc import ABC, abstractmethod
+from typing import Dict, List, Optional, Union
+from vxquant.model.preset import vxMarketPreset
+from vxutils import vxtime
+from vxquant.model.exchange import (
+    vxAccountInfo,
+    vxAlgoOrder,
+    vxCashPosition,
+    vxOrder,
+    vxPosition,
+    vxTick,
+    vxTrade,
+)
+from vxquant.model.contants import (
+    OrderDirection,
+    OrderOffset,
+    OrderStatus,
+    OrderType,
+    SecType,
+)
+
+
+class vxTdAPIBase(ABC):
+    """交易接口类"""
+
+    def __init__(self):
+        self._cache = {}
+        self._cached_at = 0
+
+    @abstractmethod
+    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
+        """获取最新的ticks 数据
+
+        Returns:
+            Dict[str,vxTick] -- 返回最新的tick数据
+        """
+
+    def current(self, *symbols: List[str]) -> Dict[str, vxTick]:
+        """实时行情信息
+
+        Arguments:
+            symbols {List[str]} -- 证券交易代码
+        """
+        if not symbols:
+            raise ValueError("symbols must not null.")
+
+        if isinstance(symbols[0], list):
+            symbols = symbols[0]
+
+        symbols = list(symbols)
+
+        now = vxtime.now()
+        if now > (self._cached_at + 3):
+            symbols.extend(self._cache.keys())
+            self._cache = {}
+            self._cached_at = now
+
+        target_symbols = set(symbols) - set(self._cache.keys())
+        vxticks = self.get_ticks(*target_symbols)
+        self._cache.update(vxticks)
+
+        return {
+            symbol: self._cache[symbol] for symbol in symbols if symbol in self._cache
+        }
+
+    @abstractmethod
+    def get_account(self) -> vxAccountInfo:
+        """获取账户基本信息"""
+
+    @abstractmethod
+    def get_positions(
+        self, symbol: str = None
+    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
+        """获取持仓信息
+
+        Keyword Arguments:
+            symbol {str} -- 对应的持仓信息 (default: {None})
+
+        Returns:
+            Dict[str, Union[vxCashPosition,vxPosition]] -- 返回持仓列表
+        """
+
+    @abstractmethod
+    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
+        """提交委托订单
+
+        Arguments:
+            vxorders {List[vxOrder]} -- 待提交的委托订单
+        """
+
+    def order_volume(
+        self, symbol: str, volume: int, price: Optional[float] = 0
+    ) -> vxOrder:
+        """下单
+
+        Arguments:
+            account_id {str} -- _description_
+            symbol {str} -- _description_
+            volume {int} -- _description_
+            price {Optional[float]} -- _description_ (default: {None})
+
+        Returns:
+            vxorder {vxOrder} -- 下单委托订单号
+        """
+        if volume == 0:
+            raise ValueError("volume can't be 0.")
+
+        if (
+            not price
+            and vxMarketPreset(symbol).security_type == SecType.BOND_CONVERTIBLE
+        ):
+            ticks = self.current(symbol)
+            price = ticks[symbol].ask1_p if volume > 0 else ticks[symbol].bid1_p
+
+        vxorder = vxOrder(
+            symbol=symbol,
+            volume=abs(volume),
+            price=price,
+            order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
+            order_direction=OrderDirection.Buy if volume > 0 else OrderDirection.Sell,
+            order_type=OrderType.Market if price <= 0 else OrderType.Limit,
+            status=OrderStatus.PendingNew,
+        )
+
+        ret_orders = self.order_batch(vxorder)
+        return ret_orders[0]
+
+    @abstractmethod
+    def get_orders(self) -> List[vxOrder]:
+        """获取当日委托订单列表
+
+        Returns:
+            List[vxOrder] -- 当日委托订单列表
+        """
+
+    @abstractmethod
+    def get_execution_reports(self) -> List[vxTrade]:
+        """获取当日成交回报信息
+
+        Returns:
+            List[vxTrade] -- 当日成交回报列表
+        """
+
+    @abstractmethod
+    def order_cancel(self, *orders: List[vxOrder]) -> None:
+        """撤单
+
+        Arguments:
+            orders {List[vxOrder]} -- 待撤销订单
+        """
```

### Comparing `vxquant-2023.3.1/src/vxquant/tdapi/gm.py` & `vxquant-2023.4.1/src/vxquant/tdapi/gm.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-"""掘金量化交易接口"""
-
-
-from gm import api as gmapi
-
-from functools import lru_cache
-from typing import Dict, List, Union
-from vxutils import vxtime, logger
-from vxutils.convertors import to_timestring
-from vxquant.model.exchange import (
-    vxCashPosition,
-    vxTick,
-    vxAccountInfo,
-    vxPosition,
-    vxOrder,
-    vxTrade,
-)
-from vxquant.model.contants import AccountType
-from vxquant.model.tools.gmData import (
-    gmTickConvter,
-    gmCashPositionConvter,
-    gmPositionConvter,
-    gmAccountinfoConvter,
-    gmOrderConvter,
-    gmTradeConvter,
-)
-from .base import vxTdAPIBase
-
-_BATCH_SIZE = 100
-
-
-class gmTdAPI(vxTdAPIBase):
-    """掘金量化交易接口"""
-
-    def __init__(
-        self, gmcontext, account_type: AccountType = AccountType.Normal
-    ) -> None:
-        super().__init__()
-        self._context = gmcontext
-        self._account_type = account_type
-
-    def get_ticks(self, *symbols: List) -> Dict[str, vxTick]:
-        allticks = []
-        for i in range(0, len(symbols), _BATCH_SIZE):
-            gmticks = gmapi.current(symbols=symbols[i : i + _BATCH_SIZE])
-            allticks.extend(gmticks)
-
-        return dict(map(lambda gmtick: gmTickConvter(gmtick, key="symbol"), allticks))
-
-    def get_account(self) -> vxAccountInfo:
-        gmcash = self._context.account().cash
-        return gmAccountinfoConvter(gmcash)
-
-    def get_positions(
-        self, symbol: str = None
-    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
-        if symbol:
-            gmposition = self._context.account().position(symbol)
-            return {symbol: gmPositionConvter(gmposition)} if gmposition else None
-
-        gmcash = self._context.account().cash
-        vxpositions = {"CNY": gmCashPositionConvter(gmcash)}
-        gmpositions = self._context.account().positions()
-        vxpositions.update(
-            map(
-                lambda gmposition: gmPositionConvter(gmposition, key="symbol"),
-                gmpositions,
-            )
-        )
-        return vxpositions
-
-    def get_orders(self) -> Dict[str, vxOrder]:
-        gmorders = gmapi.get_orders()
-        return dict(
-            map(
-                lambda gmorder: gmOrderConvter(gmorder, key="exchange_order_id"),
-                gmorders,
-            )
-        )
-
-    def get_execution_reports(self) -> Dict[str, vxTrade]:
-        gmtrades = gmapi.get_execution_reports()
-        return dict(
-            map(lambda gmtrade: gmTradeConvter(gmtrade, key="trade_id"), gmtrades)
-        )
-
-    @lru_cache(100)
-    def _get_borrowable_instruments(self, _) -> List[str]:
-        if self._account_type != AccountType.Credit:
-            return []
-
-        borrowable_instruments = gmapi.credit_get_borrowable_instruments(gmapi.Po)
-        return [
-            ins["symbol"]
-            for ins in borrowable_instruments
-            if ins["margin_rate_for_cash"] > 0
-        ]
-
-    def get_borrowable_instruments(self) -> List[str]:
-        """可融标的证券
-
-        Returns:
-            List[str] -- 可融标的证券
-        """
-        if self._account_type != AccountType.Credit:
-            return []
-        return self._get_borrowable_instruments(to_timestring(vxtime.now(), "%Y-%m-%d"))
-
-    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
-        """提交委托订单
-
-        Arguments:
-            vxorders {List[vxOrder]} -- 待提交的委托订单
-        """
-        orders = []
-        borrowable_instruments = self.get_borrowable_instruments()
-        for vxorder in vxorders:
-            if (
-                self._account_type == AccountType.Credit
-                and vxorder.symbol in borrowable_instruments
-            ):
-                order_business = gmapi.OrderBusiness_CREDIT_BOM
-            else:
-                order_business = gmapi.OrderBusiness_NORMAL
-
-            gmorder = {
-                "symbol": vxorder.symbol,
-                "volume": vxorder.volume,
-                "price": vxorder.price,
-                "side": vxorder.order_direction.value,
-                "order_type": vxorder.order_type.value,
-                "position_effect": vxorder.order_offset.value,
-                "order_business": order_business,
-                "position_src": gmapi.PositionSrc_L1,
-            }
-            orders.append(gmorder)
-            logger.debug(f"gmorder={gmorder}")
-        gmorders = gmapi.order_batch(orders)
-        # for gmorder in gmorders:
-        #    logger.debug(f"gmorder={gmorder}")
-        return list(map(gmOrderConvter, gmorders))
-
-    def order_cancel(self, *vxorders: List[vxOrder]) -> None:
-        wait_cancel_orders = [
-            {"cl_ord_id": vxorder.exchange_order_id, "account_id": ""}
-            for vxorder in vxorders
-            if vxorder.exchange_order_id
-        ]
-        return gmapi.order_cancel(wait_cancel_orders)
+"""掘金量化交易接口"""
+
+
+from gm import api as gmapi
+
+from functools import lru_cache
+from typing import Dict, List, Union
+from vxutils import vxtime, logger
+from vxutils.convertors import to_timestring
+from vxquant.model.exchange import (
+    vxCashPosition,
+    vxTick,
+    vxAccountInfo,
+    vxPosition,
+    vxOrder,
+    vxTrade,
+)
+from vxquant.model.contants import AccountType
+from vxquant.model.tools.gmData import (
+    gmTickConvter,
+    gmCashPositionConvter,
+    gmPositionConvter,
+    gmAccountinfoConvter,
+    gmOrderConvter,
+    gmTradeConvter,
+)
+from .base import vxTdAPIBase
+
+_BATCH_SIZE = 100
+
+
+class gmTdAPI(vxTdAPIBase):
+    """掘金量化交易接口"""
+
+    def __init__(
+        self, gmcontext, account_type: AccountType = AccountType.Normal
+    ) -> None:
+        super().__init__()
+        self._context = gmcontext
+        self._account_type = account_type
+
+    def get_ticks(self, *symbols: List) -> Dict[str, vxTick]:
+        allticks = []
+        for i in range(0, len(symbols), _BATCH_SIZE):
+            gmticks = gmapi.current(symbols=symbols[i : i + _BATCH_SIZE])
+            allticks.extend(gmticks)
+
+        return dict(map(lambda gmtick: gmTickConvter(gmtick, key="symbol"), allticks))
+
+    def get_account(self) -> vxAccountInfo:
+        gmcash = self._context.account().cash
+        return gmAccountinfoConvter(gmcash)
+
+    def get_positions(
+        self, symbol: str = None
+    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
+        if symbol:
+            gmposition = self._context.account().position(symbol)
+            return {symbol: gmPositionConvter(gmposition)} if gmposition else None
+
+        gmcash = self._context.account().cash
+        vxpositions = {"CNY": gmCashPositionConvter(gmcash)}
+        gmpositions = self._context.account().positions()
+        vxpositions.update(
+            map(
+                lambda gmposition: gmPositionConvter(gmposition, key="symbol"),
+                gmpositions,
+            )
+        )
+        return vxpositions
+
+    def get_orders(self) -> Dict[str, vxOrder]:
+        gmorders = gmapi.get_orders()
+        return dict(
+            map(
+                lambda gmorder: gmOrderConvter(gmorder, key="exchange_order_id"),
+                gmorders,
+            )
+        )
+
+    def get_execution_reports(self) -> Dict[str, vxTrade]:
+        gmtrades = gmapi.get_execution_reports()
+        return dict(
+            map(lambda gmtrade: gmTradeConvter(gmtrade, key="trade_id"), gmtrades)
+        )
+
+    @lru_cache(100)
+    def _get_borrowable_instruments(self, _) -> List[str]:
+        if self._account_type != AccountType.Credit:
+            return []
+
+        borrowable_instruments = gmapi.credit_get_borrowable_instruments(gmapi.Po)
+        return [
+            ins["symbol"]
+            for ins in borrowable_instruments
+            if ins["margin_rate_for_cash"] > 0
+        ]
+
+    def get_borrowable_instruments(self) -> List[str]:
+        """可融标的证券
+
+        Returns:
+            List[str] -- 可融标的证券
+        """
+        if self._account_type != AccountType.Credit:
+            return []
+        return self._get_borrowable_instruments(to_timestring(vxtime.now(), "%Y-%m-%d"))
+
+    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
+        """提交委托订单
+
+        Arguments:
+            vxorders {List[vxOrder]} -- 待提交的委托订单
+        """
+        orders = []
+        borrowable_instruments = self.get_borrowable_instruments()
+        for vxorder in vxorders:
+            if (
+                self._account_type == AccountType.Credit
+                and vxorder.symbol in borrowable_instruments
+            ):
+                order_business = gmapi.OrderBusiness_CREDIT_BOM
+            else:
+                order_business = gmapi.OrderBusiness_NORMAL
+
+            gmorder = {
+                "symbol": vxorder.symbol,
+                "volume": vxorder.volume,
+                "price": vxorder.price,
+                "side": vxorder.order_direction.value,
+                "order_type": vxorder.order_type.value,
+                "position_effect": vxorder.order_offset.value,
+                "order_business": order_business,
+                "position_src": gmapi.PositionSrc_L1,
+            }
+            orders.append(gmorder)
+            logger.debug(f"gmorder={gmorder}")
+        gmorders = gmapi.order_batch(orders)
+        # for gmorder in gmorders:
+        #    logger.debug(f"gmorder={gmorder}")
+        return list(map(gmOrderConvter, gmorders))
+
+    def order_cancel(self, *vxorders: List[vxOrder]) -> None:
+        wait_cancel_orders = [
+            {"cl_ord_id": vxorder.exchange_order_id, "account_id": ""}
+            for vxorder in vxorders
+            if vxorder.exchange_order_id
+        ]
+        return gmapi.order_cancel(wait_cancel_orders)
```

### Comparing `vxquant-2023.3.1/src/vxquant/tdapi/gmtrade.py` & `vxquant-2023.4.1/src/vxquant/tdapi/gmtrade.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""gmtrade 掘金量化仿真交易接口"""
-
-
-from gmtrade import api as gmtrade_api
-from vxquant.tdapi.base import vxTdAPI
-from vxquant.model.exchange import (
-    vxAccountInfo,
-    vxOrder,
-    vxCashPosition,
-    vxPosition,
-    vxTrade,
-    vxTick,
-)
-
-from vxquant.model.tools.gmData import (
-    gmAccountinfoConvter,
-    gmCashPositionConvter,
-    gmOrderConvter,
-    gmPositionConvter,
-    gmTickConvter,
-    gmTradeConvter,
-)
-
-
-class gmTradeTdAPI(vxTdAPI):
-    """gmtrade 掘金量化仿真交易接口"""
-
-    def __init__(self, token: str, account_id: str = "", endpoint: str = None) -> None:
-        super().__init__()
-
-        self._token = token
-        self._account_id = account_id
-        self._endpoint = endpoint or "api.myquant.cn:9000"
-
-        gmtrade_api.set_token(self._token)
-        gmtrade_api.set_endpoint(endpoint)
-        self._account = gmtrade_api.account(account_id=self._account_id)
-        gmtrade_api.login(self._account)
-
-    def get_account(self) -> vxAccountInfo:
-        cash = gmtrade_api.get_cash()
-        return gmAccountinfoConvter(cash)
-
-    def get_positions(
-        self, symbol: str = None
-    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
-        return super().get_positions(symbol)
-
-    def get_orders(self) -> List[vxOrder]:
-        return super().get_orders()
-
-    def get_execution_reports(self) -> List[vxTrade]:
-        return super().get_execution_reports()
-
-    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
-        return super().get_ticks(*symbols)
+"""gmtrade 掘金量化仿真交易接口"""
+
+
+from gmtrade import api as gmtrade_api
+from vxquant.tdapi.base import vxTdAPI
+from vxquant.model.exchange import (
+    vxAccountInfo,
+    vxOrder,
+    vxCashPosition,
+    vxPosition,
+    vxTrade,
+    vxTick,
+)
+
+from vxquant.model.tools.gmData import (
+    gmAccountinfoConvter,
+    gmCashPositionConvter,
+    gmOrderConvter,
+    gmPositionConvter,
+    gmTickConvter,
+    gmTradeConvter,
+)
+
+
+class gmTradeTdAPI(vxTdAPI):
+    """gmtrade 掘金量化仿真交易接口"""
+
+    def __init__(self, token: str, account_id: str = "", endpoint: str = None) -> None:
+        super().__init__()
+
+        self._token = token
+        self._account_id = account_id
+        self._endpoint = endpoint or "api.myquant.cn:9000"
+
+        gmtrade_api.set_token(self._token)
+        gmtrade_api.set_endpoint(endpoint)
+        self._account = gmtrade_api.account(account_id=self._account_id)
+        gmtrade_api.login(self._account)
+
+    def get_account(self) -> vxAccountInfo:
+        cash = gmtrade_api.get_cash()
+        return gmAccountinfoConvter(cash)
+
+    def get_positions(
+        self, symbol: str = None
+    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
+        return super().get_positions(symbol)
+
+    def get_orders(self) -> List[vxOrder]:
+        return super().get_orders()
+
+    def get_execution_reports(self) -> List[vxTrade]:
+        return super().get_execution_reports()
+
+    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
+        return super().get_ticks(*symbols)
```

### Comparing `vxquant-2023.3.1/src/vxquant/tdapi/miniqmt.py` & `vxquant-2023.4.1/src/vxquant/tdapi/miniqmt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-"""miniQMT 交易接口"""
-from typing import Dict, Union, List
-from xtquant import xtdata
-from xtquant.xttype import StockAccount
-from xtquant.xttrader import XtQuantTrader, XtQuantTraderCallback
-from vxquant.tdapi.base import vxTdAPIBase
-from vxquant.model.exchange import vxCashPosition, vxPosition, vxTick, vxOrder, vxTrade
-from vxutils import vxtime, logger
-from vxquant.model.tools.qmtData import (
-    qmtTickConvter,
-    qmtOrderConvter,
-    qmtPositionConvter,
-    qmtTradeConvter,
-    qmtCashPositionConvter,
-    qmtAccountInfoConvter,
-)
-
-
-class miniQMTCallback(XtQuantTraderCallback):
-    def __init__(self):
-        self.broker_orders = {}
-        self.broker_trades = {}
-
-
-class vxQMTTdAPI(vxTdAPIBase):
-    def __init__(self, miniqmt_path, account_id, account_type="STOCK"):
-        super().__init__()
-        self._account = StockAccount(account_id, account_type)
-        self._trader = XtQuantTrader(miniqmt_path, int(vxtime.now()))
-        self._callback = None
-
-        self._trader.start()
-        connect_result = self._trader.connect()
-        if connect_result != 0:
-            raise ConnectionError(f"连接失败: {connect_result}")
-
-    def register_callback(self, callback: miniQMTCallback) -> None:
-        self._callback = callback
-        self._callback.broker_orders = self.get_orders()
-        self._callback.broker_trades = self.get_execution_reports()
-        self._trader.register_callback(self._callback)
-        logger.info(f"注册callback类: {self._callback}")
-        subscribe_result = self._trader.subscribe(self._account)
-        if subscribe_result != 0:
-            raise ConnectionError(f"订阅失败: {subscribe_result}")
-        logger.info(f"订阅交易所回调成功: {subscribe_result}")
-
-    def get_account(self):
-        acc_info = self._trader.query_stock_asset(self._account)
-        if not acc_info:
-            raise ConnectionError(f"无法获取账户信息，请检查连接. {acc_info}")
-
-        positions = self.get_positions()
-        fnl = sum(p.fnl for p in positions.values())
-        return qmtAccountInfoConvter(acc_info, fnl=fnl)
-
-    def get_positions(
-        self, symbol: str = None
-    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
-        qmt_positions = self._trader.query_stock_positions(self._account)
-        positions = dict(map(lambda x: qmtPositionConvter(x, "symbol"), qmt_positions))
-        if symbol:
-            return positions.pop(symbol, {})
-
-        acc_info = self._trader.query_stock_asset(self._account)
-        if not acc_info:
-            raise ConnectionError(f"无法获取账户信息，请检查连接. {acc_info}")
-        cash_position = qmtCashPositionConvter(acc_info)
-        positions["CNY"] = cash_position
-        return positions
-
-    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
-        if len(symbols) == 1 and isinstance(symbols[0], list):
-            symbols = symbols[0]
-
-        qmt_symbols = [f"{symbol[-6:]}.{symbol[:2]}" for symbol in symbols]
-        qmt_ticks = xtdata.get_full_tick(qmt_symbols)
-        for k, v in qmt_ticks.items():
-            v["symbol"] = k
-        return dict(map(lambda x: qmtTickConvter(x, "symbol"), qmt_ticks.values()))
-
-    def get_orders(self) -> Dict[str, vxOrder]:
-        qmt_orders = self._trader.query_stock_orders(self._account)
-        return dict(
-            map(lambda order: qmtOrderConvter(order, "exchange_order_id"), qmt_orders)
-        )
-
-    def get_execution_reports(self) -> List[vxTrade]:
-        qmt_trades = self._trader.query_stock_trades(self._account)
-        return dict(map(lambda x: qmtTradeConvter(x, "trade_id"), qmt_trades))
-
-    def _to_qmt_symbol(self, symbol):
-        """将symbol(SHSE.600000) --> QMT的symbol格式(600000.SH)"""
-        return f"{symbol[-6:]}.{symbol[:2]}"
-
-    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
-        if len(vxorders) == 1 and isinstance(vxorders[0], list):
-            vxorders = vxorders[0]
-
-        for vxorder in vxorders:
-            exchange_order_id = self._trader.order_stock(
-                account=self._account,
-                stock_code=self._to_qmt_symbol(vxorder.symbol),
-                order_type=23 if vxorder.order_direction.name == "Buy" else 24,
-                order_volume=vxorder.volume,
-                price_type=11
-                if vxorder.order_type.name == "Limit"
-                else 42
-                if vxorder.symbol[:2] == "SH"
-                else 47,
-                price=vxorder.price,
-                strategy_name=vxorder.algo_order_id,
-                order_remark=vxorder.order_id,
-            )
-            if exchange_order_id < 0:
-                vxorder.status = "Rejected"
-                continue
-
-            vxorder.exchange_order_id = exchange_order_id
-            vxorder.status = "New"
-            if self._callback:
-                self._callback.broker_orders[exchange_order_id] = vxorder
-
-        return vxorders
-
-    def order_cancel(self, *vxorders: List[vxOrder]):
-        if len(vxorders) == 1 and isinstance(vxorders[0], list):
-            vxorders = vxorders[0]
-
-        for vxorder in vxorders:
-            if not vxorder.exchange_order_id:
-                continue
-
-            seq = self._trader.cancel_order_stock(
-                self._account, vxorder.exchange_order_id
-            )
-            if seq <= 0:
-                logger.error(
-                    f"委托订单:{vxorder.order_id} 撤单失败{vxorder.symbol} {vxorder.order_direction} {vxorder.volume}"
-                )
-        return
-
-    def stop(self):
-        self._trader.stop()
+"""miniQMT 交易接口"""
+from typing import Dict, Union, List
+from xtquant import xtdata
+from xtquant.xttype import StockAccount
+from xtquant.xttrader import XtQuantTrader, XtQuantTraderCallback
+from vxquant.tdapi.base import vxTdAPIBase
+from vxquant.model.exchange import vxCashPosition, vxPosition, vxTick, vxOrder, vxTrade
+from vxutils import vxtime, logger
+from vxquant.model.tools.qmtData import (
+    qmtTickConvter,
+    qmtOrderConvter,
+    qmtPositionConvter,
+    qmtTradeConvter,
+    qmtCashPositionConvter,
+    qmtAccountInfoConvter,
+)
+
+
+class miniQMTCallback(XtQuantTraderCallback):
+    def __init__(self):
+        self.broker_orders = {}
+        self.broker_trades = {}
+
+
+class vxQMTTdAPI(vxTdAPIBase):
+    def __init__(self, miniqmt_path, account_id, account_type="STOCK"):
+        super().__init__()
+        self._account = StockAccount(account_id, account_type)
+        self._trader = XtQuantTrader(miniqmt_path, int(vxtime.now()))
+        self._callback = None
+
+        self._trader.start()
+        connect_result = self._trader.connect()
+        if connect_result != 0:
+            raise ConnectionError(f"连接失败: {connect_result}")
+
+    def register_callback(self, callback: miniQMTCallback) -> None:
+        self._callback = callback
+        self._callback.broker_orders = self.get_orders()
+        self._callback.broker_trades = self.get_execution_reports()
+        self._trader.register_callback(self._callback)
+        logger.info(f"注册callback类: {self._callback}")
+        subscribe_result = self._trader.subscribe(self._account)
+        if subscribe_result != 0:
+            raise ConnectionError(f"订阅失败: {subscribe_result}")
+        logger.info(f"订阅交易所回调成功: {subscribe_result}")
+
+    def get_account(self):
+        acc_info = self._trader.query_stock_asset(self._account)
+        if not acc_info:
+            raise ConnectionError(f"无法获取账户信息，请检查连接. {acc_info}")
+
+        positions = self.get_positions()
+        fnl = sum(p.fnl for p in positions.values())
+        return qmtAccountInfoConvter(acc_info, fnl=fnl)
+
+    def get_positions(
+        self, symbol: str = None
+    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
+        qmt_positions = self._trader.query_stock_positions(self._account)
+        positions = dict(map(lambda x: qmtPositionConvter(x, "symbol"), qmt_positions))
+        if symbol:
+            return positions.pop(symbol, {})
+
+        acc_info = self._trader.query_stock_asset(self._account)
+        if not acc_info:
+            raise ConnectionError(f"无法获取账户信息，请检查连接. {acc_info}")
+        cash_position = qmtCashPositionConvter(acc_info)
+        positions["CNY"] = cash_position
+        return positions
+
+    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
+        if len(symbols) == 1 and isinstance(symbols[0], list):
+            symbols = symbols[0]
+
+        qmt_symbols = [f"{symbol[-6:]}.{symbol[:2]}" for symbol in symbols]
+        qmt_ticks = xtdata.get_full_tick(qmt_symbols)
+        for k, v in qmt_ticks.items():
+            v["symbol"] = k
+        return dict(map(lambda x: qmtTickConvter(x, "symbol"), qmt_ticks.values()))
+
+    def get_orders(self) -> Dict[str, vxOrder]:
+        qmt_orders = self._trader.query_stock_orders(self._account)
+        return dict(
+            map(lambda order: qmtOrderConvter(order, "exchange_order_id"), qmt_orders)
+        )
+
+    def get_execution_reports(self) -> List[vxTrade]:
+        qmt_trades = self._trader.query_stock_trades(self._account)
+        return dict(map(lambda x: qmtTradeConvter(x, "trade_id"), qmt_trades))
+
+    def _to_qmt_symbol(self, symbol):
+        """将symbol(SHSE.600000) --> QMT的symbol格式(600000.SH)"""
+        return f"{symbol[-6:]}.{symbol[:2]}"
+
+    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
+        if len(vxorders) == 1 and isinstance(vxorders[0], list):
+            vxorders = vxorders[0]
+
+        for vxorder in vxorders:
+            exchange_order_id = self._trader.order_stock(
+                account=self._account,
+                stock_code=self._to_qmt_symbol(vxorder.symbol),
+                order_type=23 if vxorder.order_direction.name == "Buy" else 24,
+                order_volume=vxorder.volume,
+                price_type=(
+                    11
+                    if vxorder.order_type.name == "Limit"
+                    else 42 if vxorder.symbol[:2] == "SH" else 47
+                ),
+                price=vxorder.price,
+                strategy_name=vxorder.algo_order_id,
+                order_remark=vxorder.order_id,
+            )
+            if exchange_order_id < 0:
+                vxorder.status = "Rejected"
+                continue
+
+            vxorder.exchange_order_id = exchange_order_id
+            vxorder.status = "New"
+            if self._callback:
+                self._callback.broker_orders[exchange_order_id] = vxorder
+
+        return vxorders
+
+    def order_cancel(self, *vxorders: List[vxOrder]):
+        if len(vxorders) == 1 and isinstance(vxorders[0], list):
+            vxorders = vxorders[0]
+
+        for vxorder in vxorders:
+            if not vxorder.exchange_order_id:
+                continue
+
+            seq = self._trader.cancel_order_stock(
+                self._account, vxorder.exchange_order_id
+            )
+            if seq <= 0:
+                logger.error(
+                    f"委托订单:{vxorder.order_id} 撤单失败{vxorder.symbol} {vxorder.order_direction} {vxorder.volume}"
+                )
+        return
+
+    def stop(self):
+        self._trader.stop()
```

### Comparing `vxquant-2023.3.1/src/vxquant/tdapi/sim.py` & `vxquant-2023.4.1/src/vxquant/tdapi/sim.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,296 +1,296 @@
-"""模拟交易"""
-
-import re
-import itertools
-from abc import abstractmethod
-from multiprocessing.dummy import Pool
-from typing import Dict, List, Optional, Union
-import uuid
-import requests
-from vxsched import vxContext, vxscheduler
-from vxutils import vxtime, logger
-from vxquant.model.exchange import (
-    vxAccountInfo,
-    vxAlgoOrder,
-    vxCashPosition,
-    vxOrder,
-    vxPosition,
-    vxTick,
-    vxTrade,
-)
-from functools import reduce
-from vxquant.model.contants import OrderDirection, OrderOffset, OrderStatus, OrderType
-from vxquant.tdapi.base import vxTdAPIBase
-
-_TENCENT_HQ_URL = "http://qt.gtimg.cn/q=%s&timestamp=%s"
-_HEADERS = {
-    "Accept-Encoding": "gzip, deflate, sdch",
-    "User-Agent": (
-        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
-        "(KHTML, like Gecko) Chrome/54.0.2840.100 "
-        "Safari/537.36"
-    ),
-}
-
-
-def to_tencent_symbol(symbol: str) -> str:
-    """转换成tencent格式的证券代码"""
-    exchange, code = symbol.split(".")
-    if exchange == "SHSE":
-        return f"sh{code}"
-    elif exchange == "SZSE":
-        return f"sz{code}"
-    else:
-        raise ValueError(f"{symbol} 格式不正确.")
-
-
-def _update_dict(source, target):
-    source.update(target)
-    return source
-
-
-class vxSIMTdAPI(vxTdAPIBase):
-    """交易接口类"""
-
-    def __init__(self, context: vxContext = None):
-        super().__init__()
-        self._context = context or vxContext()
-        self._session = requests.Session()
-        self._grep_stock_code = re.compile(r"(?<=_)\w+")
-        self._pool = Pool(5)
-        self._session.headers.update(_HEADERS)
-        resq = self._session.get("https://stockapp.finance.qq.com/mstats/#", timeout=1)
-        resq.raise_for_status()
-        logger.info(f"网络连通成功{resq.status_code}...")
-
-    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
-        """获取最新的ticks 数据
-
-        Returns:
-            Dict[str,vxTick] -- 返回最新的tick数据
-        """
-        if isinstance(symbols[0], list):
-            symbols = symbols[0]
-
-        # print(symbols)
-        stock_lines = map(
-            self.fetch_tencent_ticks,
-            [symbols[i:800] for i in range(0, len(symbols), 800)],
-        )
-        data = map(self.parser, itertools.chain(*stock_lines))
-        return reduce(_update_dict, data, self._cache)
-
-    def fetch_tencent_ticks(self, symbols: List[str]) -> List[str]:
-        """抓取tick数据
-
-        Arguments:
-            symbols {List} -- 证券代码s
-
-        Returns:
-            Dict[str, vxTick] -- _description_
-        """
-
-        url = _TENCENT_HQ_URL % (
-            ",".join(map(to_tencent_symbol, symbols)),
-            vxtime.now(),
-        )
-        try:
-            resq = self._session.get(url)
-            resq.raise_for_status()
-            text = resq.text.strip()
-            return text.split(";")[:-1]
-
-        except requests.exceptions.HTTPError as e:
-            logger.error(f"获取{url}数据出错: {e}.")
-            return {}
-
-    def parser(self, stock_line: str) -> Dict[str, vxTick]:
-        """解析程序
-
-        Arguments:
-            stock_line {str} -- 股票信息行
-
-        Returns:
-            Dict[str, vxTick] -- vxticks data
-        """
-
-        stock = stock_line.split("~")
-        if len(stock) <= 49:
-            logger.warning(f"skip stock line: {len(stock_line)}")
-            return {}
-
-        tencent_symbol = self._grep_stock_code.search(stock[0]).group()
-        if tencent_symbol[:2].lower() == "sh":
-            symbol = f"SHSE.{tencent_symbol[2:]}"
-        elif tencent_symbol[:2].lower() == "sz":
-            symbol = f"SZSE.{tencent_symbol[2:]}"
-        else:
-            logger.warniing(
-                f"wrong format tencent_symbol{tencent_symbol} ==== {stock[0]}"
-            )
-            return {}
-
-        return {
-            symbol: vxTick(
-                symbol=symbol,
-                open=stock[5],
-                high=stock[33],
-                low=stock[34],
-                lasttrade=stock[3],
-                yclose=float(stock[3]) - float(stock[31]),
-                volume=int(stock[36]) * 100,
-                amount=float(stock[37]) * 10000,
-                bid1_v=int(stock[10]) * 100,
-                bid1_p=stock[9],
-                bid2_v=int(stock[12]) * 100,
-                bid2_p=stock[11],
-                bid3_v=int(stock[14]) * 100,
-                bid3_p=stock[13],
-                bid4_v=int(stock[16]) * 100,
-                bid4_p=stock[15],
-                bid5_v=int(stock[18]) * 100,
-                bid5_p=stock[17],
-                ask1_v=int(stock[20]) * 100,
-                ask1_p=stock[19],
-                ask2_v=int(stock[22]) * 100,
-                ask2_p=stock[21],
-                ask3_v=int(stock[24]) * 100,
-                ask3_p=stock[23],
-                ask4_v=int(stock[26]) * 100,
-                ask4_p=stock[25],
-                ask5_v=int(stock[28]) * 100,
-                ask5_p=stock[27],
-                interest=0,
-                status="NORMAL",
-                created_dt=stock[30],
-                updated_dt=stock[30],
-            )
-        }
-
-    def current(self, *symbols: List[str]) -> Dict[str, vxTick]:
-        """实时行情信息
-
-        Arguments:
-            symbols {List[str]} -- 证券交易代码
-        """
-        if not symbols:
-            raise ValueError("symbols must not null.")
-
-        if isinstance(symbols[0], list):
-            symbols = symbols[0]
-        require_symbols = symbols
-
-        now = vxtime.now()
-        if now > (self._cached_at + 3):
-            require_symbols.extend(self._cache.keys())
-
-            self._cache = {}
-            self._cached_at = now
-
-        target_symbols = set(require_symbols) - set(self._cache.keys())
-        self.get_ticks(*target_symbols)
-
-        return {
-            symbol: self._cache[symbol] for symbol in symbols if symbol in self._cache
-        }
-
-    def get_account(self) -> vxAccountInfo:
-        """获取账户基本信息"""
-        return None
-
-    def get_positions(
-        self, symbol: str = None
-    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
-        """获取持仓信息
-
-        Keyword Arguments:
-            symbol {str} -- 对应的持仓信息 (default: {None})
-
-        Returns:
-            Dict[str, Union[vxCashPosition,vxPosition]] -- 返回持仓列表
-        """
-        return {}
-
-    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
-        """提交委托订单
-
-        Arguments:
-            vxorders {List[vxOrder]} -- 待提交的委托订单
-        """
-        if isinstance(vxorders[0], list):
-            vxorders = vxorders[0]
-
-        ret_orders = []
-        for vxorder in vxorders:
-            broker_order = vxOrder(**vxorder)
-            broker_order.exchange_order_id = str(uuid.uuid4())
-            ret_orders.append(broker_order)
-            self.context.sim_orderbooks[broker_order.exchange_order_id] = broker_order
-
-        return ret_orders
-
-    def order_volume(
-        self, symbol: str, volume: int, price: Optional[float] = 0
-    ) -> vxOrder:
-        """下单
-
-        Arguments:
-            account_id {str} -- _description_
-            symbol {str} -- _description_
-            volume {int} -- _description_
-            price {Optional[float]} -- _description_ (default: {None})
-
-        Returns:
-            vxorder {vxOrder} -- 下单委托订单号
-        """
-        if volume == 0:
-            raise ValueError("volume can't be 0.")
-
-        vxorder = vxOrder(
-            symbol=symbol,
-            volume=abs(volume),
-            price=price,
-            order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
-            order_direction=OrderDirection.Buy if volume > 0 else OrderDirection.Sell,
-            order_type=OrderType.Market if price <= 0 else OrderType.Limit,
-            status=OrderStatus.PendingNew,
-        )
-
-        ret_orders = self.order_batch(vxorder)
-        return ret_orders[0]
-
-    def get_orders(self) -> List[vxOrder]:
-        """获取当日委托订单列表
-
-        Returns:
-            List[vxOrder] -- 当日委托订单列表
-        """
-        return {}
-
-    def get_execution_reports(self) -> List[vxTrade]:
-        """获取当日成交回报信息
-
-        Returns:
-            List[vxTrade] -- 当日成交回报列表
-        """
-        return {}
-
-    def order_cancel(self, *orders: List[vxOrder]) -> None:
-        """撤单
-
-        Arguments:
-            orders {List[vxOrder]} -- 待撤销订单
-        """
-
-
-if __name__ == "__main__":
-    tdapi = vxSIMTdAPI()
-    start = vxtime.now()
-    ticks = tdapi.current(["SHSE.600000", "SZSE.000001"] * 1000)
-    print(f"耗时: {vxtime.now() -start}")
-
-    # print(ticks["SHSE.600000"])
-    ticks = tdapi.current(["SHSE.600036", "SZSE.000001", "SHSE.113591"] * 1000)
-    # print(ticks["SHSE.600036"])
-    print(f"耗时: {vxtime.now() -start}")
-    print(ticks["SHSE.113591"])
+"""模拟交易"""
+
+import re
+import itertools
+from abc import abstractmethod
+from multiprocessing.dummy import Pool
+from typing import Dict, List, Optional, Union
+import uuid
+import requests
+from vxsched import vxContext, vxscheduler
+from vxutils import vxtime, logger
+from vxquant.model.exchange import (
+    vxAccountInfo,
+    vxAlgoOrder,
+    vxCashPosition,
+    vxOrder,
+    vxPosition,
+    vxTick,
+    vxTrade,
+)
+from functools import reduce
+from vxquant.model.contants import OrderDirection, OrderOffset, OrderStatus, OrderType
+from vxquant.tdapi.base import vxTdAPIBase
+
+_TENCENT_HQ_URL = "http://qt.gtimg.cn/q=%s&timestamp=%s"
+_HEADERS = {
+    "Accept-Encoding": "gzip, deflate, sdch",
+    "User-Agent": (
+        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
+        "(KHTML, like Gecko) Chrome/54.0.2840.100 "
+        "Safari/537.36"
+    ),
+}
+
+
+def to_tencent_symbol(symbol: str) -> str:
+    """转换成tencent格式的证券代码"""
+    exchange, code = symbol.split(".")
+    if exchange == "SHSE":
+        return f"sh{code}"
+    elif exchange == "SZSE":
+        return f"sz{code}"
+    else:
+        raise ValueError(f"{symbol} 格式不正确.")
+
+
+def _update_dict(source, target):
+    source.update(target)
+    return source
+
+
+class vxSIMTdAPI(vxTdAPIBase):
+    """交易接口类"""
+
+    def __init__(self, context: vxContext = None):
+        super().__init__()
+        self._context = context or vxContext()
+        self._session = requests.Session()
+        self._grep_stock_code = re.compile(r"(?<=_)\w+")
+        self._pool = Pool(5)
+        self._session.headers.update(_HEADERS)
+        resq = self._session.get("https://stockapp.finance.qq.com/mstats/#", timeout=1)
+        resq.raise_for_status()
+        logger.info(f"网络连通成功{resq.status_code}...")
+
+    def get_ticks(self, *symbols) -> Dict[str, vxTick]:
+        """获取最新的ticks 数据
+
+        Returns:
+            Dict[str,vxTick] -- 返回最新的tick数据
+        """
+        if isinstance(symbols[0], list):
+            symbols = symbols[0]
+
+        # print(symbols)
+        stock_lines = map(
+            self.fetch_tencent_ticks,
+            [symbols[i:800] for i in range(0, len(symbols), 800)],
+        )
+        data = map(self.parser, itertools.chain(*stock_lines))
+        return reduce(_update_dict, data, self._cache)
+
+    def fetch_tencent_ticks(self, symbols: List[str]) -> List[str]:
+        """抓取tick数据
+
+        Arguments:
+            symbols {List} -- 证券代码s
+
+        Returns:
+            Dict[str, vxTick] -- _description_
+        """
+
+        url = _TENCENT_HQ_URL % (
+            ",".join(map(to_tencent_symbol, symbols)),
+            vxtime.now(),
+        )
+        try:
+            resq = self._session.get(url)
+            resq.raise_for_status()
+            text = resq.text.strip()
+            return text.split(";")[:-1]
+
+        except requests.exceptions.HTTPError as e:
+            logger.error(f"获取{url}数据出错: {e}.")
+            return {}
+
+    def parser(self, stock_line: str) -> Dict[str, vxTick]:
+        """解析程序
+
+        Arguments:
+            stock_line {str} -- 股票信息行
+
+        Returns:
+            Dict[str, vxTick] -- vxticks data
+        """
+
+        stock = stock_line.split("~")
+        if len(stock) <= 49:
+            logger.warning(f"skip stock line: {len(stock_line)}")
+            return {}
+
+        tencent_symbol = self._grep_stock_code.search(stock[0]).group()
+        if tencent_symbol[:2].lower() == "sh":
+            symbol = f"SHSE.{tencent_symbol[2:]}"
+        elif tencent_symbol[:2].lower() == "sz":
+            symbol = f"SZSE.{tencent_symbol[2:]}"
+        else:
+            logger.warniing(
+                f"wrong format tencent_symbol{tencent_symbol} ==== {stock[0]}"
+            )
+            return {}
+
+        return {
+            symbol: vxTick(
+                symbol=symbol,
+                open=stock[5],
+                high=stock[33],
+                low=stock[34],
+                lasttrade=stock[3],
+                yclose=float(stock[3]) - float(stock[31]),
+                volume=int(stock[36]) * 100,
+                amount=float(stock[37]) * 10000,
+                bid1_v=int(stock[10]) * 100,
+                bid1_p=stock[9],
+                bid2_v=int(stock[12]) * 100,
+                bid2_p=stock[11],
+                bid3_v=int(stock[14]) * 100,
+                bid3_p=stock[13],
+                bid4_v=int(stock[16]) * 100,
+                bid4_p=stock[15],
+                bid5_v=int(stock[18]) * 100,
+                bid5_p=stock[17],
+                ask1_v=int(stock[20]) * 100,
+                ask1_p=stock[19],
+                ask2_v=int(stock[22]) * 100,
+                ask2_p=stock[21],
+                ask3_v=int(stock[24]) * 100,
+                ask3_p=stock[23],
+                ask4_v=int(stock[26]) * 100,
+                ask4_p=stock[25],
+                ask5_v=int(stock[28]) * 100,
+                ask5_p=stock[27],
+                interest=0,
+                status="NORMAL",
+                created_dt=stock[30],
+                updated_dt=stock[30],
+            )
+        }
+
+    def current(self, *symbols: List[str]) -> Dict[str, vxTick]:
+        """实时行情信息
+
+        Arguments:
+            symbols {List[str]} -- 证券交易代码
+        """
+        if not symbols:
+            raise ValueError("symbols must not null.")
+
+        if isinstance(symbols[0], list):
+            symbols = symbols[0]
+        require_symbols = symbols
+
+        now = vxtime.now()
+        if now > (self._cached_at + 3):
+            require_symbols.extend(self._cache.keys())
+
+            self._cache = {}
+            self._cached_at = now
+
+        target_symbols = set(require_symbols) - set(self._cache.keys())
+        self.get_ticks(*target_symbols)
+
+        return {
+            symbol: self._cache[symbol] for symbol in symbols if symbol in self._cache
+        }
+
+    def get_account(self) -> vxAccountInfo:
+        """获取账户基本信息"""
+        return None
+
+    def get_positions(
+        self, symbol: str = None
+    ) -> Dict[str, Union[vxCashPosition, vxPosition]]:
+        """获取持仓信息
+
+        Keyword Arguments:
+            symbol {str} -- 对应的持仓信息 (default: {None})
+
+        Returns:
+            Dict[str, Union[vxCashPosition,vxPosition]] -- 返回持仓列表
+        """
+        return {}
+
+    def order_batch(self, *vxorders: List[vxOrder]) -> List[vxOrder]:
+        """提交委托订单
+
+        Arguments:
+            vxorders {List[vxOrder]} -- 待提交的委托订单
+        """
+        if isinstance(vxorders[0], list):
+            vxorders = vxorders[0]
+
+        ret_orders = []
+        for vxorder in vxorders:
+            broker_order = vxOrder(**vxorder)
+            broker_order.exchange_order_id = str(uuid.uuid4())
+            ret_orders.append(broker_order)
+            self.context.sim_orderbooks[broker_order.exchange_order_id] = broker_order
+
+        return ret_orders
+
+    def order_volume(
+        self, symbol: str, volume: int, price: Optional[float] = 0
+    ) -> vxOrder:
+        """下单
+
+        Arguments:
+            account_id {str} -- _description_
+            symbol {str} -- _description_
+            volume {int} -- _description_
+            price {Optional[float]} -- _description_ (default: {None})
+
+        Returns:
+            vxorder {vxOrder} -- 下单委托订单号
+        """
+        if volume == 0:
+            raise ValueError("volume can't be 0.")
+
+        vxorder = vxOrder(
+            symbol=symbol,
+            volume=abs(volume),
+            price=price,
+            order_offset=OrderOffset.Open if volume > 0 else OrderOffset.Close,
+            order_direction=OrderDirection.Buy if volume > 0 else OrderDirection.Sell,
+            order_type=OrderType.Market if price <= 0 else OrderType.Limit,
+            status=OrderStatus.PendingNew,
+        )
+
+        ret_orders = self.order_batch(vxorder)
+        return ret_orders[0]
+
+    def get_orders(self) -> List[vxOrder]:
+        """获取当日委托订单列表
+
+        Returns:
+            List[vxOrder] -- 当日委托订单列表
+        """
+        return {}
+
+    def get_execution_reports(self) -> List[vxTrade]:
+        """获取当日成交回报信息
+
+        Returns:
+            List[vxTrade] -- 当日成交回报列表
+        """
+        return {}
+
+    def order_cancel(self, *orders: List[vxOrder]) -> None:
+        """撤单
+
+        Arguments:
+            orders {List[vxOrder]} -- 待撤销订单
+        """
+
+
+if __name__ == "__main__":
+    tdapi = vxSIMTdAPI()
+    start = vxtime.now()
+    ticks = tdapi.current(["SHSE.600000", "SZSE.000001"] * 1000)
+    print(f"耗时: {vxtime.now() -start}")
+
+    # print(ticks["SHSE.600000"])
+    ticks = tdapi.current(["SHSE.600036", "SZSE.000001", "SHSE.113591"] * 1000)
+    # print(ticks["SHSE.600036"])
+    print(f"耗时: {vxtime.now() -start}")
+    print(ticks["SHSE.113591"])
```

### Comparing `vxquant-2023.3.1/src/vxsched/__main__.py` & `vxquant-2023.4.1/src/vxsched/__main__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""vxsched 主函数"""
-import argparse
-from vxutils import logger
-from vxsched import vxscheduler
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="config json file path: etc/config.json",
-        default="config.json",
-        type=str,
-    )
-    parser.add_argument(
-        "-m", "--mod", help="module directory path : mod/ ", default="mod/", type=str
-    )
-    parser.add_argument(
-        "-v", "--verbose", help="debug 模式", action="store_true", default=False
-    )
-    args = parser.parse_args()
-
-    if args.verbose:
-        logger.setLevel("DEBUG")
-
-    vxscheduler.server_forever(config=args.config, mod=args.mod)
+"""vxsched 主函数"""
+import argparse
+from vxutils import logger
+from vxsched import vxscheduler
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="config json file path: etc/config.json",
+        default="config.json",
+        type=str,
+    )
+    parser.add_argument(
+        "-m", "--mod", help="module directory path : mod/ ", default="mod/", type=str
+    )
+    parser.add_argument(
+        "-v", "--verbose", help="debug 模式", action="store_true", default=False
+    )
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel("DEBUG")
+
+    vxscheduler.server_forever(config=args.config, mod=args.mod)
```

### Comparing `vxquant-2023.3.1/src/vxsched/core.py` & `vxquant-2023.4.1/src/vxsched/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,367 +1,358 @@
-import os
-import importlib
-import contextlib
-from pathlib import Path
-import time
-from queue import Empty
-from itertools import chain
-
-from collections import defaultdict
-from typing import Any, Union, Callable
-from concurrent.futures import ThreadPoolExecutor as Executor
-from multiprocessing.dummy import Process, Lock
-from vxutils import logger, vxWrapper
-from vxsched.event import vxEvent, vxTrigger, vxEventQueue
-from vxsched.context import vxContext
-
-
-__all__ = ["vxScheduler", "vxscheduler"]
-
-_default_context = {
-    "settings": {},
-    "params": {},
-    "executor": {
-        "class": "concurrent.futures.ThreadPoolExecutor",
-        "params": {"thread_name_prefix": "vxSchedThread"},
-    },
-}
-
-
-class vxScheduler:
-    def __init__(self):
-        self._context = None
-        self._executor = None
-        self._map_func = map
-        self._queue = vxEventQueue()
-        self._handlers = defaultdict(set)
-        self._active = False
-        self._is_initialized = False
-        self._worker_threads = []
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__}(id-{id(self)})"
-
-    __repr__ = __str__
-
-    @property
-    def context(self):
-        return self._context
-
-    def initialize(
-        self,
-        context: vxContext = None,
-        executor: Executor = None,
-    ) -> None:
-        if self._is_initialized is True:
-            logger.warning("已经初始化，请勿重复初始化")
-            return
-
-        self._executor = executor
-        self._map_func = executor.map if hasattr(executor, "map") else map
-
-        self._context = context or self._context or vxContext(_default_context)
-        if context is not None:
-            self._context = context
-            logger.debug(f"更新context内容: {self.context}")
-        elif self._context is None:
-            self._context = vxContext(_default_context)
-            logger.debug(f"创建缺省context内容: {self.context}")
-
-        self.submit_event("__init__")
-        self.trigger_events()
-        self._is_initialized = True
-        logger.info(f"{self} 触发初始化完成 ... ")
-
-    def is_alive(self):
-        """是否运行中"""
-        return self._active
-
-    def trigger_events(self, *trigger_events) -> None:
-        """同步触发已到期的消息"""
-        if len(trigger_events) == 1 and isinstance(trigger_events[0], list):
-            trigger_events = trigger_events[0]
-
-        events = defaultdict(list)
-        for t_event in trigger_events:
-            events[t_event.type].append(t_event)
-
-        with contextlib.suppress(Empty):
-            while not self._queue.empty():
-                event = self._queue.get_nowait()
-                events[event.type].append(event)
-
-        handlers = chain.from_iterable(
-            self._handlers[event.type]
-            for event in map(max, events.values())
-            if self._handlers[event.type]
-        )
-
-        results = self._map_func(
-            lambda handler: self._run_handler(event=event, handler=handler),
-            handlers,
-        )
-        return list(results)
-
-    def submit_event(
-        self,
-        event: Union[vxEvent, str],
-        data: Any = None,
-        trigger: vxTrigger = None,
-        priority: float = 10,
-        **kwargs,
-    ) -> vxEvent:
-        """提交一个消息"""
-
-        if isinstance(event, str):
-            send_event = vxEvent(
-                type=event,
-                data=data,
-                trigger=trigger,
-                priority=priority,
-                **kwargs,
-            )
-
-        elif isinstance(event, vxEvent):
-            send_event = event
-        else:
-            raise ValueError(f"{self} event 类型{type(event)}错误，请检查: {event}")
-
-        logger.debug(f"提交消息: {send_event}")
-        self._queue.put_nowait(send_event)
-
-    def _run_handler(self, handler: Callable, event: vxEvent) -> None:
-        """单独运行一个handler"""
-
-        try:
-            lock = getattr(handler, "lock", None)
-            start = time.perf_counter()
-            if lock:
-                with lock:
-                    ret = handler(self.context, event)
-            else:
-                ret = handler(self.context, event)
-        except KeyboardInterrupt:
-            ret = None
-            logger.warning("用户提前终止... ")
-
-        except Exception as err:
-            ret = err
-            logger.error(f"{self} run handler error: {err}", exc_info=True)
-
-        finally:
-            cost_time = time.perf_counter() - start
-            if cost_time > getattr(handler, "time_limit", 1.0):
-                logger.warning(
-                    f"{self} {handler} 运行时间 {cost_time*1000:,.2f}s.  触发消息: {event}"
-                )
-
-            if (
-                event.type != "__handle_timerecord__"
-                and self._handlers["__handle_timerecord__"]
-            ):
-                self.submit_event(
-                    "__handle_timerecord__", (str(handler), event, cost_time)
-                )
-
-            if event.reply_to and self._handlers["__handle_reply__"]:
-                self.submit_event("__handle_reply__", (event, ret))
-
-        return ret
-
-    def register(
-        self,
-        event_type: str,
-        time_limit: float = 1.0,
-        lock: Lock = None,
-        handler: Callable = None,
-    ) -> Callable:
-        """注册一个handler"""
-
-        if handler in self._handlers[event_type]:
-            return
-
-        setattr(handler, "time_limit", time_limit)
-        setattr(handler, "lock", lock)
-        self._handlers[event_type].add(handler)
-        logger.info(
-            f"{self} register event_type:"
-            f" '{event_type}' time_limit: {time_limit*1000:,.2f}ms handler: {handler} "
-        )
-
-    def unregister(self, event_type: str, handler: Callable) -> None:
-        """取消注册handler"""
-        if handler in self._handlers[event_type]:
-            self._handlers[event_type].remove(handler)
-            logger.warning(
-                f"{self} unregister event_type: {event_type} handler: {handler}"
-            )
-
-    def event_handler(
-        self, event_type: str, time_limit: float = 1.0, lock: Lock = None
-    ) -> Callable:
-        """消息处理函数装饰器"""
-
-        def deco(handler):
-            self.register(event_type, time_limit, lock, handler=handler)
-            return handler
-
-        return deco
-
-    def run(
-        self,
-        context: vxContext = None,
-        executor: Executor = None,
-    ) -> None:
-        if self._is_initialized is False:
-            self.initialize(context, executor)
-
-        self._active = True
-
-        self._run()
-
-    def _run(self) -> None:
-        """单个线程运行"""
-        logger.info(f"{self} worker 开始运行...")
-        try:
-            while self._active:
-                with contextlib.suppress(Empty):
-                    event = self._queue.get(timeout=1.0)
-
-                    if not self._handlers[event.type]:
-                        continue
-
-                    if self._executor:
-                        [
-                            self._executor.submit(
-                                self._run_handler, handler=handler, event=event
-                            )
-                            for handler in self._handlers[event.type]
-                        ]
-                    else:
-                        [
-                            self._run_handler(handler, event)
-                            for handler in self._handlers[event.type]
-                        ]
-        finally:
-            self._active = False
-            logger.info(f"{self} worker 结束运行...")
-
-    def start(
-        self,
-        context: vxContext = None,
-        executor: Executor = None,
-        blocking: bool = False,
-    ) -> None:
-        """启动调度器"""
-        if self._active:
-            logger.info(f"{self} 已经激活运行...")
-            return
-
-        if self._is_initialized is False:
-            self.initialize(context, executor)
-
-        self._active = True
-        self._worker_threads = []
-        for i in range(5):
-            t = Process(target=self._run, name=f"vxSchedWorker{i}")
-            t.daemon = True
-            t.start()
-            self._worker_threads.append(t)
-
-        if blocking:
-            for t in self._worker_threads:
-                if t.is_alive():
-                    t.join()
-
-    def stop(self) -> None:
-        """停止调度器"""
-        self._active = False
-        for t in self._worker_threads:
-            if t.is_alive():
-                t.join()
-
-    def server_forever(
-        self, config: Union[str, Path] = None, mod: Union[str, Path] = "mod/"
-    ):
-        if isinstance(config, str):
-            config = Path(config)
-
-        context = (
-            vxContext.load_json(config.absolute(), _default_context)
-            if config.exists()
-            else vxContext(_default_context)
-        )
-        executor_settings = context.get("executor", None)
-        if executor_settings is not None:
-            executor = vxWrapper.init_by_config(executor_settings)
-        else:
-            executor = Executor(thread_name_prefix="vxSchedThread")
-        self.load_modules(mod)
-        self.start(context=context, executor=executor, blocking=True)
-
-    def load_modules(self, mod_path: Union[str, Path]) -> Any:
-        """加载策略目录"""
-        if isinstance(mod_path, Path):
-            mod_path = mod_path.absolute()
-
-        if not os.path.exists(mod_path):
-            logger.warning(msg=f"{mod_path} is not exists")
-            return
-
-        modules = os.listdir(mod_path)
-        logger.info(f"loading strategy dir: {mod_path}.")
-        logger.info("=" * 80)
-        for mod in modules:
-            if (not mod.startswith("__")) and mod.endswith(".py"):
-                try:
-                    loader = importlib.machinery.SourceFileLoader(
-                        mod, os.path.join(mod_path, mod)
-                    )
-                    spec = importlib.util.spec_from_loader(loader.name, loader)
-                    strategy_mod = importlib.util.module_from_spec(spec)
-                    loader.exec_module(strategy_mod)
-                    logger.info(f"Load Module: {strategy_mod} Sucess.")
-                    logger.info("+" * 80)
-                except Exception as err:
-                    logger.error(f"Load Module: {mod} Failed. {err}", exc_info=True)
-                    logger.error("-" * 80)
-
-
-vxscheduler = vxScheduler()
-
-
-if __name__ == "__main__":
-
-    class test:
-        def __call__(self, *args: Any, **kwds: Any) -> Any:
-            time.sleep(2)
-            logger.info("this is test")
-
-    s = vxScheduler()
-    # s.start(executor=Executor())
-
-    @s.event_handler("test", 10)
-    def test2(*args: Any, **kwds: Any):
-        time.sleep(1)
-        logger.info("this is test2")
-
-    @s.event_handler("__handle_timerecord__")
-    def test3(context, event):
-        logger.info(f"{event.type}")
-        logger.info(event.data)
-
-    s.register("test", 3, handler=test())
-    s.register("test1", 3, handler=test())
-    s.register("test", 3, handler=test())
-
-    # print(s._handlers)
-    s.submit_event("test")
-    print("=" * 60)
-
-    print("=" * 60)
-    print(s)
-    print("=" * 60)
-    # s.trigger_events()
-    time.sleep(4)
-    s.server_forever("config.json")
-    s.stop()
+import os
+import importlib
+import contextlib
+from pathlib import Path
+import time
+from queue import Empty
+from itertools import chain
+
+from collections import defaultdict
+from typing import Any, Union, Callable
+from concurrent.futures import ThreadPoolExecutor as Executor
+from multiprocessing.dummy import Process, Lock
+from vxutils import logger, vxWrapper, vxtime
+from vxsched.event import vxEvent, vxTrigger, vxEventQueue
+from vxsched.context import vxContext
+
+
+__all__ = ["vxScheduler", "vxscheduler"]
+
+_default_context = {
+    "settings": {},
+    "params": {},
+    "executor": {
+        "class": "concurrent.futures.ThreadPoolExecutor",
+        "params": {"thread_name_prefix": "vxSchedThread"},
+    },
+}
+
+
+class vxTask:
+    def __init__(
+        self, handler: Callable, time_limit: float = 1.0, lock: Lock = None
+    ) -> None:
+        self._handler = handler
+        self.time_limit = time_limit
+        self.lock = lock
+        self.cost_time = 0
+
+    def __call__(self, context: vxContext, event: vxEvent) -> Any:
+        try:
+            start = time.perf_counter()
+            if self.lock:
+                with self.lock:
+                    ret = self._handler(context, event)
+            else:
+                ret = self._handler(context, event)
+        except KeyboardInterrupt:
+            ret = None
+            logger.warning("用户提前终止... ")
+
+        except Exception as err:
+            ret = err
+            logger.error(f"{self} run handler error: {err}", exc_info=True)
+
+        finally:
+            self.cost_time = time.perf_counter() - start
+            if self.cost_time > self.time_limit:
+                logger.warning(
+                    f"{self._handler} 运行时间 {self.cost_time*1000:,.2f}ms.  触发消息:"
+                    f" {event}"
+                )
+
+        return ret
+
+    def __eq__(self, _other: object) -> bool:
+        if isinstance(_other, vxTask):
+            return self._handler == _other._handler
+        else:
+            return self._handler == _other
+
+    def __hash__(self) -> int:
+        return hash(self._handler)
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({self._handler})"
+
+    __repr__ = __str__
+
+
+class vxScheduler:
+    def __init__(self):
+        self._context = None
+        self._executor = None
+        self._map_func = map
+        self._queue = vxEventQueue()
+        self._handlers = defaultdict(set)
+        self._active = False
+        self._is_initialized = False
+        self._worker_threads = []
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}(id-{id(self)})"
+
+    __repr__ = __str__
+
+    @property
+    def context(self):
+        return self._context
+
+    def initialize(
+        self,
+        context: vxContext = None,
+        executor: Executor = None,
+    ) -> None:
+        if self._is_initialized is True:
+            logger.warning("已经初始化，请勿重复初始化")
+            return
+
+        self._executor = executor
+        self._map_func = executor.map if hasattr(executor, "map") else map
+
+        # self._context = context or self._context or vxContext(_default_context)
+        if context is not None:
+            self._context = context
+            logger.debug(f"更新context内容: {self.context}")
+        elif self._context is None:
+            self._context = vxContext(_default_context)
+            logger.debug(f"创建缺省context内容: {self.context}")
+
+        self.submit_event("__init__")
+        self.trigger_events()
+        self._is_initialized = True
+        logger.info(f"{self} 触发初始化完成 ... ")
+
+    def is_alive(self):
+        """是否运行中"""
+        return self._active
+
+    def trigger_events(self, *trigger_events) -> None:
+        """同步触发已到期的消息"""
+        if len(trigger_events) == 1 and isinstance(trigger_events[0], list):
+            trigger_events = trigger_events[0]
+
+        events = defaultdict(list)
+        for t_event in trigger_events:
+            events[t_event.id].append(t_event)
+
+        with contextlib.suppress(Empty):
+            while not self._queue.empty():
+                event = self._queue.get_nowait()
+                events[event.id].append(event)
+
+        if not events:
+            return None
+
+        handlers = chain.from_iterable(
+            self._handlers[event.type]
+            for event in map(max, events.values())
+            if self._handlers[event.type]
+        )
+
+        return list(
+            self._map_func(
+                lambda handler: self._run_handler(event=event, handler=handler),
+                handlers,
+            )
+        )
+
+    def submit_event(
+        self,
+        event: Union[vxEvent, str],
+        data: Any = None,
+        trigger: vxTrigger = None,
+        priority: float = 10,
+        **kwargs,
+    ) -> vxEvent:
+        """提交一个消息"""
+
+        if isinstance(event, str):
+            send_event = vxEvent(
+                type=event,
+                data=data,
+                trigger=trigger,
+                priority=priority,
+                **kwargs,
+            )
+
+        elif isinstance(event, vxEvent):
+            send_event = event
+        else:
+            raise ValueError(f"{self} event 类型{type(event)}错误，请检查: {event}")
+
+        logger.debug(f"提交消息: {send_event}")
+        self._queue.put_nowait(send_event)
+
+    def _run_handler(self, handler: Callable, event: vxEvent) -> None:
+        """单独运行一个handler"""
+
+        ret = handler(self.context, event)
+        if (
+            event.type != "__handle_timerecord__"
+            and self._handlers["__handle_timerecord__"]
+        ):
+            self.submit_event(
+                "__handle_timerecord__", (str(handler), event, handler.cost_time)
+            )
+
+        if event.reply_to and self._handlers["__handle_reply__"]:
+            self.submit_event("__handle_reply__", (event, ret))
+
+        return ret
+
+    def register(
+        self,
+        event_type: str,
+        time_limit: float = 1.0,
+        lock: Lock = None,
+        handler: Callable = None,
+    ) -> Callable:
+        """注册一个handler"""
+
+        if not isinstance(handler, vxTask):
+            handler = vxTask(handler, time_limit, lock)
+
+        if handler in self._handlers[event_type]:
+            return
+
+        self._handlers[event_type].add(handler)
+        logger.info(
+            f"{self} register event_type:"
+            f" '{event_type}' time_limit: {time_limit*1000:,.2f}ms "
+            f"handler: {handler} "
+        )
+
+    def unregister(self, event_type: str, handler: Callable) -> None:
+        """取消注册handler"""
+        if handler in self._handlers[event_type]:
+            self._handlers[event_type].remove(handler)
+            logger.warning(
+                f"{self} unregister event_type: {event_type} handler: {handler}"
+            )
+
+    def event_handler(
+        self, event_type: str, time_limit: float = 1.0, lock: Lock = None
+    ) -> Callable:
+        """消息处理函数装饰器"""
+
+        def deco(handler):
+            self.register(event_type, time_limit, lock, handler=handler)
+            return handler
+
+        return deco
+
+    def run(
+        self,
+        context: vxContext = None,
+        executor: Executor = None,
+    ) -> None:
+        if self._is_initialized is False:
+            self.initialize(context, executor)
+
+        self._active = True
+
+        self._run()
+
+    def _run(self) -> None:
+        """单个线程运行"""
+        logger.info(f"{self} worker 开始运行...")
+        try:
+            while self._active:
+                with contextlib.suppress(Empty):
+                    event = self._queue.get(timeout=1.0)
+
+                    if self._handlers[event.type]:
+                        list(
+                            self._map_func(
+                                lambda hdl: self._run_handler(hdl, event=event),
+                                self._handlers[event.type],
+                            )
+                        )
+
+        finally:
+            self._active = False
+            logger.info(f"{self} worker 结束运行...")
+
+    def start(
+        self,
+        context: vxContext = None,
+        executor: Executor = None,
+        blocking: bool = False,
+    ) -> None:
+        """启动调度器"""
+        if self._active:
+            logger.info(f"{self} 已经激活运行...")
+            return
+
+        if self._is_initialized is False:
+            self.initialize(context, executor)
+
+        self._active = True
+        self._worker_threads = []
+        for i in range(5):
+            t = Process(target=self._run, name=f"vxSchedWorker{i}")
+            t.daemon = True
+            t.start()
+            self._worker_threads.append(t)
+
+        if blocking:
+            for t in self._worker_threads:
+                if t.is_alive():
+                    t.join()
+        return
+
+    def stop(self) -> None:
+        """停止调度器"""
+        self._active = False
+        for t in self._worker_threads:
+            if t.is_alive():
+                t.join()
+
+    def server_forever(
+        self, config: Union[str, Path] = None, mod: Union[str, Path] = "mod/"
+    ):
+        if isinstance(config, str):
+            config = Path(config)
+
+        context = (
+            vxContext.load_json(config.absolute(), _default_context)
+            if config.exists()
+            else vxContext(_default_context)
+        )
+        executor_settings = context.get("executor", None)
+        if executor_settings is not None:
+            executor = vxWrapper.init_by_config(executor_settings)
+        else:
+            executor = Executor(thread_name_prefix="vxSchedThread")
+        self.load_modules(mod)
+        self.start(context=context, executor=executor, blocking=True)
+
+    def load_modules(self, mod_path: Union[str, Path]) -> Any:
+        """加载策略目录"""
+        if isinstance(mod_path, Path):
+            mod_path = mod_path.absolute()
+
+        if not os.path.exists(mod_path):
+            logger.warning(msg=f"{mod_path} is not exists")
+            return
+
+        modules = os.listdir(mod_path)
+        logger.info(f"loading strategy dir: {mod_path}.")
+        logger.info("=" * 80)
+        for mod in modules:
+            if (not mod.startswith("__")) and mod.endswith(".py"):
+                try:
+                    loader = importlib.machinery.SourceFileLoader(
+                        mod, os.path.join(mod_path, mod)
+                    )
+                    spec = importlib.util.spec_from_loader(loader.name, loader)
+                    strategy_mod = importlib.util.module_from_spec(spec)
+                    loader.exec_module(strategy_mod)
+                    logger.info(f"Load Module: {strategy_mod} Sucess.")
+                    logger.info("+" * 80)
+                except Exception as err:
+                    logger.error(f"Load Module: {mod} Failed. {err}", exc_info=True)
+                    logger.error("-" * 80)
+
+
+vxscheduler = vxScheduler()
```

### Comparing `vxquant-2023.3.1/src/vxsched/event.py` & `vxquant-2023.4.1/src/vxsched/event.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-"""消息类型"""
-
-from heapq import heappush, heappop
-from enum import Enum
-from queue import Queue, Empty
-from typing import Optional, Any
-from vxutils import (
-    vxDataClass,
-    vxIntField,
-    vxDatetimeField,
-    vxField,
-    vxFloatField,
-    vxUUIDField,
-    vxBoolField,
-    vxPropertyField,
-    vxtime,
-    combine_datetime,
-    logger,
-)
-
-
-__all__ = ["vxEvent", "vxEventQueue", "vxTrigger", "TriggerStatus"]
-
-
-class TriggerStatus(Enum):
-    """触发器状态
-
-    Pending : 未开始
-    Running : 已开始
-    Completed: 已完成
-    """
-
-    #  未开始
-    Pending = 1
-    #  已开始
-    Running = 2
-    #  已完成
-    Completed = 3
-
-
-def _trigger_status(trigger):
-    if trigger.next() is None:
-        return TriggerStatus.Completed
-    elif trigger.trigger_dt is None:
-        return TriggerStatus.Pending
-    return TriggerStatus.Running
-
-
-class vxTrigger(vxDataClass):
-    __sortkeys__ = ("trigger_dt",)
-
-    # 触发时间
-    trigger_dt = vxDatetimeField(None)
-    # 间隔 (单位：秒)
-    interval = vxFloatField(1, 3, 0.01, float("inf"))
-    # 是否跳过假期
-    skip_holiday = vxBoolField(True)
-    # 触发器状态
-    status = vxPropertyField(property_factory=_trigger_status)
-    # 开始时间
-    start_dt = vxDatetimeField()
-    # 结束时间
-    end_dt = vxDatetimeField(default_factory=float("inf"))
-
-    def next(self):
-        if self.trigger_dt is None:
-            now = vxtime.now()
-            trigger_dt = self.start_dt
-
-            if now > self.end_dt:
-                return None
-
-            if now > self.start_dt:
-                trigger_dt = (
-                    self.start_dt
-                    + (now - self.start_dt) // self.interval * self.interval
-                    + self.interval
-                )
-
-        else:
-            trigger_dt = self.trigger_dt + self.interval
-
-        while (
-            self.skip_holiday
-            and vxtime.is_holiday(trigger_dt)
-            and trigger_dt <= self.end_dt
-        ):
-            trigger_dt = (
-                trigger_dt
-                + (combine_datetime(trigger_dt, "23:59:59") - trigger_dt)
-                // self.interval
-                * self.interval
-                + self.interval
-            )
-
-        return trigger_dt if trigger_dt <= self.end_dt else None
-
-    def __iter__(self):
-        return self
-
-    def __next__(self) -> float:
-        if self.next() is not None:
-            self.trigger_dt = self.next()
-            return self.trigger_dt
-
-        raise StopIteration
-
-    @staticmethod
-    def once(trigger_dt):
-        return vxTrigger(
-            start_dt=trigger_dt, end_dt=trigger_dt, interval=1, skip_holiday=False
-        )
-
-    @staticmethod
-    def daily(run_time="00:00:00", freq=1, end_dt=None, skip_holiday=False):
-        start_dt = vxtime.today(run_time)
-        if start_dt < vxtime.now():
-            start_dt += 24 * 60 * 60
-
-        return vxTrigger(
-            start_dt=start_dt,
-            end_dt=end_dt,
-            interval=int(freq) * 24 * 60 * 60,
-            skip_holiday=skip_holiday,
-        )
-
-    @staticmethod
-    def every(interval=1, start_dt=None, end_dt=None, skip_holiday=False):
-        return vxTrigger(
-            start_dt=start_dt,
-            end_dt=end_dt,
-            interval=interval,
-            skip_holiday=skip_holiday,
-        )
-
-
-class vxEvent(vxDataClass):
-    """消息类型"""
-
-    __sortkeys__ = ("trigger_dt", "priority")
-
-    # 消息id
-    id: str = vxUUIDField(auto=True)
-    # 消息通道
-    channel: str = vxField("")
-    # 消息类型
-    type: str = vxField("", str)
-    # 消息内容
-    data: Any = vxField("")
-    # 定时触发器
-    trigger: Optional[vxTrigger] = vxField(default_factory="")
-    # 触发时间
-    trigger_dt: float = vxDatetimeField()
-    # 优先级
-    priority: int = vxIntField(10)
-    # rpc消息回复地址
-    reply_to: str = vxUUIDField(auto=False)
-
-
-class vxEventQueue(Queue):
-    def _init(self, maxsize=0):
-        self.queue = []
-        self._event_ids = set()
-
-    def _qsize(self):
-        now = vxtime.now()
-        return len([event for event in self.queue if event.trigger_dt <= now])
-
-    def _put(self, event):
-        if isinstance(event, str):
-            event = vxEvent(type=event)
-        elif not isinstance(event, vxEvent):
-            raise ValueError(f"Not support type(event) : {type(event)}.")
-
-        if event.id in self._event_ids:
-            raise ValueError(f"event({event.id})重复入库. {event}")
-
-        if event.trigger:
-            if event.trigger.status.name == "Pending":
-                event.trigger_dt = next(event.trigger, vxtime.now())
-            elif event.trigger.status.name == "Completed":
-                logger.warning(f"忽略已经完成的event。 {event}")
-                return
-
-        heappush(self.queue, event)
-        self._event_ids.add(event.id)
-
-    def get(self, block=True, timeout=None):
-        with self.not_empty:
-            if not block:
-                if not self._qsize():
-                    raise Empty
-            elif timeout is None:
-                while not self._qsize():
-                    remaining = 10
-                    if len(self.queue) > 0:
-                        remaining = self.queue[0].trigger_dt - vxtime.now()
-
-                    if remaining > 0:
-                        self.not_empty.wait(remaining)
-
-            elif timeout < 0:
-                raise ValueError("'timeout' must be a non-negative number")
-            else:
-                endtime = vxtime.now() + timeout
-                while not self._qsize():
-                    if len(self.queue) > 0:
-                        min_endtime = min(endtime, self.queue[0].trigger_dt)
-                    else:
-                        min_endtime = endtime
-
-                    remaining = min(min_endtime - vxtime.now(), 1)
-
-                    if remaining <= 0.0:
-                        raise Empty
-                    self.not_empty.wait(remaining)
-            event = self._get()
-            self.not_full.notify()
-            return event
-
-    def _get(self):
-        event = heappop(self.queue)
-        # 获取的event都将trigger给去掉，以免trigger在其他地方再进行传递
-        if not event.trigger or event.trigger.status.name == "Completed":
-            self.unfinished_tasks -= 1
-            self._event_ids.remove(event.id)
-            event.trigger = ""
-            return event
-
-        reply_event = vxEvent(**event.message)
-        reply_event.trigger = ""
-
-        event.trigger_dt = next(event.trigger, None)
-        heappush(self.queue, event)
-        self.not_empty.notify()
-        return reply_event
+"""消息类型"""
+
+from heapq import heappush, heappop
+from enum import Enum
+from queue import Queue, Empty
+from typing import Optional, Any
+from vxutils import (
+    vxDataClass,
+    vxIntField,
+    vxDatetimeField,
+    vxField,
+    vxFloatField,
+    vxUUIDField,
+    vxBoolField,
+    vxPropertyField,
+    vxtime,
+    combine_datetime,
+    logger,
+)
+
+
+__all__ = ["vxEvent", "vxEventQueue", "vxTrigger", "TriggerStatus"]
+
+
+class TriggerStatus(Enum):
+    """触发器状态
+
+    Pending : 未开始
+    Running : 已开始
+    Completed: 已完成
+    """
+
+    #  未开始
+    Pending = 1
+    #  已开始
+    Running = 2
+    #  已完成
+    Completed = 3
+
+
+def _trigger_status(trigger):
+    if trigger.next() is None:
+        return TriggerStatus.Completed
+    elif trigger.trigger_dt is None:
+        return TriggerStatus.Pending
+    return TriggerStatus.Running
+
+
+class vxTrigger(vxDataClass):
+    __sortkeys__ = ("trigger_dt",)
+
+    # 触发时间
+    trigger_dt = vxDatetimeField(None)
+    # 间隔 (单位：秒)
+    interval = vxFloatField(1, 3, 0.01, float("inf"))
+    # 是否跳过假期
+    skip_holiday = vxBoolField(True)
+    # 触发器状态
+    status = vxPropertyField(property_factory=_trigger_status)
+    # 开始时间
+    start_dt = vxDatetimeField()
+    # 结束时间
+    end_dt = vxDatetimeField(default_factory=float("inf"))
+
+    def next(self):
+        if self.trigger_dt is None:
+            now = vxtime.now()
+            trigger_dt = self.start_dt
+
+            if now > self.end_dt:
+                return None
+
+            if now > self.start_dt:
+                trigger_dt = (
+                    self.start_dt
+                    + (now - self.start_dt) // self.interval * self.interval
+                    + self.interval
+                )
+
+        else:
+            trigger_dt = self.trigger_dt + self.interval
+
+        while (
+            self.skip_holiday
+            and vxtime.is_holiday(trigger_dt)
+            and trigger_dt <= self.end_dt
+        ):
+            trigger_dt = (
+                trigger_dt
+                + (combine_datetime(trigger_dt, "23:59:59") - trigger_dt)
+                // self.interval
+                * self.interval
+                + self.interval
+            )
+
+        return trigger_dt if trigger_dt <= self.end_dt else None
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> float:
+        if self.next() is not None:
+            self.trigger_dt = self.next()
+            return self.trigger_dt
+
+        raise StopIteration
+
+    @staticmethod
+    def once(trigger_dt):
+        return vxTrigger(
+            start_dt=trigger_dt, end_dt=trigger_dt, interval=1, skip_holiday=False
+        )
+
+    @staticmethod
+    def daily(run_time="00:00:00", freq=1, end_dt=None, skip_holiday=False):
+        start_dt = vxtime.today(run_time)
+        if start_dt < vxtime.now():
+            start_dt += 24 * 60 * 60
+
+        return vxTrigger(
+            start_dt=start_dt,
+            end_dt=end_dt,
+            interval=int(freq) * 24 * 60 * 60,
+            skip_holiday=skip_holiday,
+        )
+
+    @staticmethod
+    def every(interval=1, start_dt=None, end_dt=None, skip_holiday=False):
+        return vxTrigger(
+            start_dt=start_dt,
+            end_dt=end_dt,
+            interval=interval,
+            skip_holiday=skip_holiday,
+        )
+
+
+class vxEvent(vxDataClass):
+    """消息类型"""
+
+    __sortkeys__ = ("trigger_dt", "priority")
+
+    # 消息id
+    id: str = vxUUIDField(auto=True)
+    # 消息通道
+    channel: str = vxField("")
+    # 消息类型
+    type: str = vxField("", str)
+    # 消息内容
+    data: Any = vxField("")
+    # 定时触发器
+    trigger: Optional[vxTrigger] = vxField(default_factory="")
+    # 触发时间
+    trigger_dt: float = vxDatetimeField()
+    # 优先级
+    priority: int = vxIntField(10)
+    # rpc消息回复地址
+    reply_to: str = vxUUIDField(auto=False)
+
+
+class vxEventQueue(Queue):
+    def _init(self, maxsize=0):
+        self.queue = []
+        self._event_ids = set()
+
+    def _qsize(self):
+        now = vxtime.now()
+        return len([event for event in self.queue if event.trigger_dt <= now])
+
+    def _put(self, event):
+        if isinstance(event, str):
+            event = vxEvent(type=event)
+        elif not isinstance(event, vxEvent):
+            raise ValueError(f"Not support type(event) : {type(event)}.")
+
+        if event.id in self._event_ids:
+            raise ValueError(f"event({event.id})重复入库. {event}")
+
+        if event.trigger:
+            if event.trigger.status.name == "Pending":
+                event.trigger_dt = next(event.trigger, vxtime.now())
+            elif event.trigger.status.name == "Completed":
+                logger.warning(f"忽略已经完成的event。 {event}")
+                return
+
+        heappush(self.queue, event)
+        self._event_ids.add(event.id)
+
+    def get(self, block=True, timeout=None):
+        with self.not_empty:
+            if not block:
+                if not self._qsize():
+                    raise Empty
+            elif timeout is None:
+                while not self._qsize():
+                    remaining = 10
+                    if len(self.queue) > 0:
+                        remaining = self.queue[0].trigger_dt - vxtime.now()
+
+                    if remaining > 0:
+                        self.not_empty.wait(remaining)
+
+            elif timeout < 0:
+                raise ValueError("'timeout' must be a non-negative number")
+            else:
+                endtime = vxtime.now() + timeout
+                while not self._qsize():
+                    if len(self.queue) > 0:
+                        min_endtime = min(endtime, self.queue[0].trigger_dt)
+                    else:
+                        min_endtime = endtime
+
+                    remaining = min(min_endtime - vxtime.now(), 1)
+
+                    if remaining <= 0.0:
+                        raise Empty
+                    self.not_empty.wait(remaining)
+            event = self._get()
+            self.not_full.notify()
+            return event
+
+    def _get(self):
+        event = heappop(self.queue)
+        # 获取的event都将trigger给去掉，以免trigger在其他地方再进行传递
+        if not event.trigger or event.trigger.status.name == "Completed":
+            self.unfinished_tasks -= 1
+            self._event_ids.remove(event.id)
+            event.trigger = ""
+            return event
+
+        reply_event = vxEvent(**event.message)
+        reply_event.trigger = ""
+
+        event.trigger_dt = next(event.trigger, None)
+        heappush(self.queue, event)
+        self.not_empty.notify()
+        return reply_event
```

### Comparing `vxquant-2023.3.1/src/vxsched/triggers/daily.py` & `vxquant-2023.4.1/src/vxsched/triggers/daily.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""每日触发器"""
-
-from typing import Any
-from vxutils import vxtime
-from vxsched.event import vxTrigger
-
-
-class vxDailyTrigger(vxTrigger):
-    """每日触发器"""
-
-    def __init__(
-        self,
-        run_time: str = "00:00:00",
-        freq: int = 1,
-        end_dt: Any = None,
-        skip_holiday: bool = False,
-    ):
-        """每日触发器
-
-        Keyword Arguments:
-            run_time {str} -- 运行时间 (default: {"00:00:00"})
-            freq {int} -- 间隔多少天 (default: {1})
-            end_dt {Any} -- 结束时间 (default: {None})
-            skip_holiday {bool} -- 是否跳过假期 (default: {False})
-        """
-        start_dt = vxtime.today(run_time)
-
-        if start_dt < vxtime.now():
-            start_dt += 24 * 60 * 60
-
-        super(vxDailyTrigger, self).__init__(
-            start_dt=start_dt,
-            end_dt=end_dt,
-            interval=freq * 24 * 60 * 60,
-            skip_holiday=skip_holiday,
-        )
+"""每日触发器"""
+
+from typing import Any
+from vxutils import vxtime
+from vxsched.event import vxTrigger
+
+
+class vxDailyTrigger(vxTrigger):
+    """每日触发器"""
+
+    def __init__(
+        self,
+        run_time: str = "00:00:00",
+        freq: int = 1,
+        end_dt: Any = None,
+        skip_holiday: bool = False,
+    ):
+        """每日触发器
+
+        Keyword Arguments:
+            run_time {str} -- 运行时间 (default: {"00:00:00"})
+            freq {int} -- 间隔多少天 (default: {1})
+            end_dt {Any} -- 结束时间 (default: {None})
+            skip_holiday {bool} -- 是否跳过假期 (default: {False})
+        """
+        start_dt = vxtime.today(run_time)
+
+        if start_dt < vxtime.now():
+            start_dt += 24 * 60 * 60
+
+        super(vxDailyTrigger, self).__init__(
+            start_dt=start_dt,
+            end_dt=end_dt,
+            interval=freq * 24 * 60 * 60,
+            skip_holiday=skip_holiday,
+        )
```

### Comparing `vxquant-2023.3.1/src/vxutils/convertors.py` & `vxquant-2023.4.1/src/vxutils/convertors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,444 +1,445 @@
-# encoding=utf-8
-"""转换器
-    将各种类型的数据转换为各种类型的数据
-"""
-
-from typing import Any, Optional, Union
-from functools import lru_cache, singledispatch, wraps
-from enum import Enum
-import time
-import datetime
-from dateutil import parser
-
-
-try:
-    import six
-except ImportError:
-    six = None
-
-
-try:
-    import simplejson as json
-except ImportError:
-    import json
-
-
-__all__ = [
-    "to_timestring",
-    "to_datetime",
-    "to_timestamp",
-    "to_enum",
-    "to_json",
-    "combine_datetime",
-    "vxJSONEncoder",
-]
-
-ZERO = datetime.timedelta(0)
-HOUR = datetime.timedelta(hours=1)
-SECOND = datetime.timedelta(seconds=1)
-
-
-STDOFFSET = datetime.timedelta(seconds=-time.timezone)
-if time.localtime(time.time()).tm_isdst and time.daylight:
-    DSTOFFSET = datetime.timedelta(seconds=-time.altzone)
-else:
-    DSTOFFSET = STDOFFSET
-
-DSTDIFF = DSTOFFSET - STDOFFSET
-
-
-class LocalTimezone(datetime.tzinfo):
-    """本地时区"""
-
-    def fromutc(self, dt):
-        assert dt.tzinfo is self
-        stamp = (dt - datetime.datetime(1970, 1, 1, tzinfo=self)) // SECOND
-        args = time.localtime(stamp)[:6]
-        dst_diff = DSTDIFF // SECOND
-        fold = args == time.localtime(stamp - dst_diff)
-        return datetime.datetime(
-            *args, microsecond=dt.microsecond, tzinfo=self, fold=fold
-        )
-
-    def utcoffset(self, dt):
-        return DSTOFFSET if self._isdst(dt) else STDOFFSET
-
-    def _utcoffset(self, dt):
-        return DSTOFFSET if self._isdst(dt) else STDOFFSET
-
-    def dst(self, dt):
-        return DSTDIFF if self._isdst(dt) else ZERO
-
-    def tzname(self, dt):
-        return time.tzname[self._isdst(dt)]
-
-    def _isdst(self, dt):
-        local_time = (
-            dt.year,
-            dt.month,
-            dt.day,
-            dt.hour,
-            dt.minute,
-            dt.second,
-            dt.weekday(),
-            0,
-            0,
-        )
-        stamp = time.mktime(local_time)
-        local_time = time.localtime(stamp)
-        return local_time.tm_isdst > 0
-
-    def __repr__(self) -> str:
-        return "Local_TZ"
-
-
-local_tzinfo = LocalTimezone()
-
-
-_ENT_TIME = "2199-12-31 23:59:59"
-_ENT_DATETIME = datetime.datetime(2199, 12, 31, 23, 59, 59, 0, tzinfo=local_tzinfo)
-_ENT_TIMESTAMP = datetime.datetime(
-    2199, 12, 31, 23, 59, 59, 0, tzinfo=local_tzinfo
-).timestamp()
-
-
-@singledispatch
-def to_timestring(date_time: Any, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """
-    将事件转换为格式化的日期字符串
-    :param date_time:
-    :return: time string
-    """
-    raise TypeError(f"Unsupported type: {type(date_time)}")
-
-
-@to_timestring.register(float)
-@to_timestring.register(int)
-def _(date_time: Union[float, int], fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理timestamp类型"""
-    if date_time == float("inf"):
-        return _ENT_TIME
-
-    date_time = datetime.datetime.fromtimestamp(date_time).astimezone(local_tzinfo)
-    return date_time.strftime(fmt)
-
-
-@to_timestring.register(datetime.time)
-def _(date_time: datetime.time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理time类型"""
-    return date_time.strftime("%H:%M:%S")
-
-
-@to_timestring.register(datetime.date)
-def _(date_time: datetime.date, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理date类型"""
-    return date_time.strftime("%Y-%m-%d")
-
-
-@to_timestring.register(datetime.datetime)
-def _(date_time: datetime.datetime, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理datetime"""
-
-    date_time = date_time.astimezone(local_tzinfo)
-
-    return date_time.strftime(fmt)
-
-
-@to_timestring.register(time.struct_time)
-def _(date_time: time.struct_time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理struct_time类型"""
-    date_time = datetime.datetime(*date_time[:6]).astimezone(local_tzinfo)
-    return date_time.strftime(fmt)
-
-
-@to_timestring.register(str)
-def _(date_time: str, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    """处理str类型"""
-    return parser.parse(date_time).strftime(fmt)
-
-
-@to_timestring.register(type(None))
-def _(date_time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
-    return ""
-
-
-@singledispatch
-def to_datetime(date_time: Any, tz=None) -> datetime.datetime:
-    """
-    将date_time转换为datetime对象
-    :param date_time:
-    :param fmt:
-    :return:
-    """
-    raise TypeError(f"Unsupported type: {type(date_time)}")
-
-
-@to_datetime.register(str)
-def _(date_time: str, tz=None) -> datetime.datetime:
-    """处理str类型"""
-
-    return parser.parse(date_time).astimezone(tz) if tz else parser.parse(date_time)
-
-
-@to_datetime.register(float)
-@to_datetime.register(int)
-def _(date_time: Union[float, int], tz=None) -> datetime.datetime:
-    """处理int类型"""
-    if date_time == float("inf"):
-        return _ENT_DATETIME
-
-    return (
-        datetime.datetime.fromtimestamp(date_time).astimezone(tz)
-        if tz
-        else datetime.datetime.fromtimestamp(date_time)
-    )
-
-
-@to_datetime.register(time.struct_time)
-def _(date_time: time.struct_time, tz=None) -> datetime.datetime:
-    """处理struct_time类型"""
-    return (
-        datetime.datetime(*date_time[:6]).astimezone(tz)
-        if tz
-        else datetime.datetime(*date_time[:6])
-    )
-
-
-@to_datetime.register(datetime.date)
-def _(date_time: datetime.date, tz=None) -> datetime.datetime:
-    """处理date类型"""
-    return (
-        datetime.datetime(
-            date_time.year,
-            date_time.month,
-            date_time.day,
-        ).astimezone(tz)
-        if tz
-        else datetime.datetime(
-            date_time.year,
-            date_time.month,
-            date_time.day,
-        )
-    )
-
-
-@to_datetime.register(datetime.datetime)
-def _(date_time: datetime.datetime, tz=None) -> datetime.datetime:
-    return date_time.astimezone(tz) if tz else date_time
-
-
-@singledispatch
-def to_timestamp(date_time: Any) -> float:
-    """
-    将date_time转换为timestamp
-    :param date_time:
-    :param fmt:
-    :return: timestamp
-    """
-    raise TypeError(f"Unsupported type: {type(date_time)}")
-
-
-@to_timestamp.register(datetime.datetime)
-def _(date_time: Any) -> float:
-    """处理datetime类型"""
-    return date_time.timestamp()
-
-
-@to_timestamp.register(time.struct_time)
-def _(date_time: time.struct_time) -> float:
-    """处理struct_time类型"""
-    return time.mktime(date_time)
-
-
-@to_timestamp.register(datetime.date)
-def _(date_time: datetime.date) -> float:
-    """处理date类型"""
-    return time.mktime(date_time.timetuple())
-
-
-@to_timestamp.register(str)
-def _(date_time: str) -> float:
-    """处理str类型"""
-    pasered_dt = parser.parse(date_time)
-    pasered_dt.astimezone(local_tzinfo)
-    return pasered_dt.timestamp()
-
-
-@to_timestamp.register(float)
-@to_timestamp.register(int)
-def _(date_time: Union[float, int], fmt: str = "") -> float:
-    """处理float类型"""
-    return _ENT_TIMESTAMP if date_time == float("inf") else date_time
-
-
-@lru_cache(100)
-def to_enum(obj: Any, enum_cls, default: Optional[Enum] = None) -> Enum:
-    """
-    将obj转换为enum_cls的枚举对象
-    :param obj: 待转换的对象
-    :param enum_cls: 枚举类型
-    :param default: 默认值
-    :return: 枚举对象
-    """
-    try:
-        if isinstance(obj, enum_cls):
-            return obj
-        elif (
-            isinstance(obj, str)
-            and obj.replace(f"{enum_cls.__name__}.", "") in enum_cls.__members__
-        ):
-            return enum_cls[obj.replace(f"{enum_cls.__name__}.", "")]
-        else:
-            return enum_cls(obj)
-    except ValueError as err:
-        if default:
-            return default
-        else:
-            raise ValueError(f"{obj} is not in {enum_cls}.") from err
-
-
-@singledispatch
-def _type_jsonencoder(obj: Any) -> str:
-    """
-    将obj转换为json字符串
-    :param obj:
-    :return:
-    """
-    try:
-        return str(obj)
-    except TypeError as err:
-        raise TypeError(f"Unsupported type: {type(obj)}") from err
-
-
-_type_jsonencoder.register(Enum, lambda obj: obj.name)
-_type_jsonencoder.register(datetime.datetime, to_timestring)
-_type_jsonencoder.register(datetime.date, lambda obj: to_timestring(obj, "%Y-%m-%d"))
-_type_jsonencoder.register(datetime.time, lambda obj: obj.strftime("%H:%M:%S"))
-_type_jsonencoder.register(datetime.timedelta, lambda obj: obj.total_seconds())
-_type_jsonencoder.register(time.struct_time, to_timestring)
-
-
-class vxJSONEncoder(json.JSONEncoder):
-    """json编码器"""
-
-    def default(self, o):
-        try:
-            return _type_jsonencoder(o)
-        except TypeError:
-            return json.JSONEncoder.default(self, o)
-
-    @staticmethod
-    def register(data_type):
-        """注册一个类型
-
-        Arguments:
-            data_type -- 数据格式
-        @vxJSONEncoder.register(datetime.datetime)
-        def _(obj):
-            return xxx_obj
-        """
-
-        def decorator(func):
-            _type_jsonencoder.register(data_type, func)
-
-            @wraps
-            def wapper(*args, **kwargs):
-                return func(*args, **kwargs)
-
-            return wapper
-
-        return decorator
-
-
-def to_json(obj: Any, indent: int = 4, ensure_ascii=True, **kwargs) -> str:
-    """转化为json格式"""
-    return json.dumps(
-        obj,
-        cls=vxJSONEncoder,
-        ensure_ascii=ensure_ascii,
-        indent=indent,
-        **kwargs,
-    )
-
-
-@lru_cache(100)
-def combine_datetime(date_: Any, time_: str = "00:00:00") -> float:
-    """组合日期和时间"""
-    date_ = to_timestring(date_, "%Y-%m-%d")
-    return to_timestamp(f"{date_} {time_}")
-
-
-if six:
-    __all__ += [
-        "to_text",
-        "to_binary",
-        "is_string",
-        "byte2int",
-    ]
-
-    string_types = (six.string_types, six.text_type, six.binary_type)
-
-    def to_text(value, encoding="utf-8"):
-        """转化为文本格式
-
-        Arguments:
-            value {_type_} -- 待转化的对象
-
-        Keyword Arguments:
-            encoding {str} -- 编码格式 (default: {"utf-8"})
-
-        Returns:
-            six.text_type -- 文件格式
-        """ """ """
-        if isinstance(value, six.text_type):
-            return value
-        if isinstance(value, six.binary_type):
-            return value.decode(encoding)
-        return six.text_type(value)
-
-    def to_binary(value, encoding="utf-8"):
-        """转换成二进制格式
-
-        Arguments:
-            value -- 待转化的对象
-
-        Keyword Arguments:
-            encoding -- 编码格式 (default: {"utf-8"})
-
-        Returns:
-            转换后二进制格式
-        """
-        if isinstance(value, six.binary_type):
-            return value
-        if isinstance(value, six.text_type):
-            return value.encode(encoding)
-        return six.binary_type(value)
-
-    def is_string(value):
-        """转换成sttring'格式
-
-        Arguments:
-            value -- 待转换的对象
-
-        Returns:
-            转换后string格式
-        """
-        return isinstance(value, string_types)
-
-    def byte2int(char_, index=0):
-        """Get the ASCII int value of a character in a string.
-        :param s: a string
-        :param index: the position of desired character
-        :return: ASCII int value
-        """
-        return ord(char_[index]) if six.PY2 else char_[index]
-
-
-class Serializer:
-    _potocols = {}
-
-    def __init__(self, name):
-        pass
-
-    def dumps(self, pyobj):
-        pass
+# encoding=utf-8
+"""转换器
+    将各种类型的数据转换为各种类型的数据
+"""
+
+from typing import Any, Optional, Union
+from functools import lru_cache, singledispatch, wraps
+from enum import Enum
+import time
+import datetime
+from dateutil import parser
+
+
+try:
+    import six
+except ImportError:
+    six = None
+
+
+try:
+    import simplejson as json
+except ImportError:
+    import json
+
+
+__all__ = [
+    "to_timestring",
+    "to_datetime",
+    "to_timestamp",
+    "to_enum",
+    "to_json",
+    "combine_datetime",
+    "vxJSONEncoder",
+]
+
+ZERO = datetime.timedelta(0)
+HOUR = datetime.timedelta(hours=1)
+SECOND = datetime.timedelta(seconds=1)
+
+
+STDOFFSET = datetime.timedelta(seconds=-time.timezone)
+if time.localtime(time.time()).tm_isdst and time.daylight:
+    DSTOFFSET = datetime.timedelta(seconds=-time.altzone)
+else:
+    DSTOFFSET = STDOFFSET
+
+DSTDIFF = DSTOFFSET - STDOFFSET
+
+
+class LocalTimezone(datetime.tzinfo):
+    """本地时区"""
+
+    def fromutc(self, dt):
+        assert dt.tzinfo is self
+        stamp = (dt - datetime.datetime(1970, 1, 1, tzinfo=self)) // SECOND
+        args = time.localtime(stamp)[:6]
+        dst_diff = DSTDIFF // SECOND
+        fold = args == time.localtime(stamp - dst_diff)
+        return datetime.datetime(
+            *args, microsecond=dt.microsecond, tzinfo=self, fold=fold
+        )
+
+    def utcoffset(self, dt):
+        return DSTOFFSET if self._isdst(dt) else STDOFFSET
+
+    def _utcoffset(self, dt):
+        return DSTOFFSET if self._isdst(dt) else STDOFFSET
+
+    def dst(self, dt):
+        return DSTDIFF if self._isdst(dt) else ZERO
+
+    def tzname(self, dt):
+        return time.tzname[self._isdst(dt)]
+
+    def _isdst(self, dt):
+        local_time = (
+            dt.year,
+            dt.month,
+            dt.day,
+            dt.hour,
+            dt.minute,
+            dt.second,
+            dt.weekday(),
+            0,
+            0,
+        )
+        stamp = time.mktime(local_time)
+        local_time = time.localtime(stamp)
+        return local_time.tm_isdst > 0
+
+    def __repr__(self) -> str:
+        return "Local_TZ"
+
+
+local_tzinfo = LocalTimezone()
+
+
+_ENT_TIME = "2199-12-31 23:59:59"
+_ENT_DATETIME = datetime.datetime(2199, 12, 31, 23, 59, 59, 0, tzinfo=local_tzinfo)
+_ENT_TIMESTAMP = datetime.datetime(
+    2199, 12, 31, 23, 59, 59, 0, tzinfo=local_tzinfo
+).timestamp()
+
+
+@singledispatch
+def to_timestring(date_time: Any, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """
+    将事件转换为格式化的日期字符串
+    :param date_time:
+    :return: time string
+    """
+    raise TypeError(f"Unsupported type: {type(date_time)}")
+
+
+@to_timestring.register(float)
+@to_timestring.register(int)
+def _(date_time: Union[float, int], fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理timestamp类型"""
+    if date_time == float("inf"):
+        return _ENT_TIME
+
+    date_time = datetime.datetime.fromtimestamp(date_time).astimezone(local_tzinfo)
+    return date_time.strftime(fmt)
+
+
+@to_timestring.register(datetime.time)
+def _(date_time: datetime.time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理time类型"""
+    return date_time.strftime("%H:%M:%S")
+
+
+@to_timestring.register(datetime.date)
+def _(date_time: datetime.date, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理date类型"""
+    return date_time.strftime("%Y-%m-%d")
+
+
+@to_timestring.register(datetime.datetime)
+def _(date_time: datetime.datetime, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理datetime"""
+
+    date_time = date_time.astimezone(local_tzinfo)
+
+    return date_time.strftime(fmt)
+
+
+@to_timestring.register(time.struct_time)
+def _(date_time: time.struct_time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理struct_time类型"""
+    date_time = datetime.datetime(*date_time[:6]).astimezone(local_tzinfo)
+    return date_time.strftime(fmt)
+
+
+@to_timestring.register(str)
+def _(date_time: str, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    """处理str类型"""
+    return parser.parse(date_time).strftime(fmt)
+
+
+@to_timestring.register(type(None))
+def _(date_time, fmt: str = "%Y-%m-%d %H:%M:%S.%f") -> str:
+    return ""
+
+
+@singledispatch
+def to_datetime(date_time: Any, tz=None) -> datetime.datetime:
+    """
+    将date_time转换为datetime对象
+    :param date_time:
+    :param fmt:
+    :return:
+    """
+    raise TypeError(f"Unsupported type: {type(date_time)}")
+
+
+@to_datetime.register(str)
+def _(date_time: str, tz=None) -> datetime.datetime:
+    """处理str类型"""
+
+    return parser.parse(date_time).astimezone(tz) if tz else parser.parse(date_time)
+
+
+@to_datetime.register(float)
+@to_datetime.register(int)
+def _(date_time: Union[float, int], tz=None) -> datetime.datetime:
+    """处理int类型"""
+    if date_time == float("inf"):
+        return _ENT_DATETIME
+
+    return (
+        datetime.datetime.fromtimestamp(date_time).astimezone(tz)
+        if tz
+        else datetime.datetime.fromtimestamp(date_time)
+    )
+
+
+@to_datetime.register(time.struct_time)
+def _(date_time: time.struct_time, tz=None) -> datetime.datetime:
+    """处理struct_time类型"""
+    return (
+        datetime.datetime(*date_time[:6]).astimezone(tz)
+        if tz
+        else datetime.datetime(*date_time[:6])
+    )
+
+
+@to_datetime.register(datetime.date)
+def _(date_time: datetime.date, tz=None) -> datetime.datetime:
+    """处理date类型"""
+    return (
+        datetime.datetime(
+            date_time.year,
+            date_time.month,
+            date_time.day,
+        ).astimezone(tz)
+        if tz
+        else datetime.datetime(
+            date_time.year,
+            date_time.month,
+            date_time.day,
+        )
+    )
+
+
+@to_datetime.register(datetime.datetime)
+def _(date_time: datetime.datetime, tz=None) -> datetime.datetime:
+    return date_time.astimezone(tz) if tz else date_time
+
+
+@singledispatch
+def to_timestamp(date_time: Any) -> float:
+    """
+    将date_time转换为timestamp
+    :param date_time:
+    :param fmt:
+    :return: timestamp
+    """
+    raise TypeError(f"Unsupported type: {type(date_time)}")
+
+
+@to_timestamp.register(datetime.datetime)
+def _(date_time: Any) -> float:
+    """处理datetime类型"""
+    return date_time.timestamp()
+
+
+@to_timestamp.register(time.struct_time)
+def _(date_time: time.struct_time) -> float:
+    """处理struct_time类型"""
+    return time.mktime(date_time)
+
+
+@to_timestamp.register(datetime.date)
+def _(date_time: datetime.date) -> float:
+    """处理date类型"""
+    return time.mktime(date_time.timetuple())
+
+
+@to_timestamp.register(str)
+@lru_cache(100)
+def _(date_time: str) -> float:
+    """处理str类型"""
+    pasered_dt = parser.parse(date_time)
+    pasered_dt.astimezone(local_tzinfo)
+    return pasered_dt.timestamp()
+
+
+@to_timestamp.register(float)
+@to_timestamp.register(int)
+def _(date_time: Union[float, int], fmt: str = "") -> float:
+    """处理float类型"""
+    return _ENT_TIMESTAMP if date_time == float("inf") else date_time
+
+
+@lru_cache(100)
+def to_enum(obj: Any, enum_cls, default: Optional[Enum] = None) -> Enum:
+    """
+    将obj转换为enum_cls的枚举对象
+    :param obj: 待转换的对象
+    :param enum_cls: 枚举类型
+    :param default: 默认值
+    :return: 枚举对象
+    """
+    try:
+        if isinstance(obj, enum_cls):
+            return obj
+        elif (
+            isinstance(obj, str)
+            and obj.replace(f"{enum_cls.__name__}.", "") in enum_cls.__members__
+        ):
+            return enum_cls[obj.replace(f"{enum_cls.__name__}.", "")]
+        else:
+            return enum_cls(obj)
+    except ValueError as err:
+        if default:
+            return default
+        else:
+            raise ValueError(f"{obj} is not in {enum_cls}.") from err
+
+
+@singledispatch
+def _type_jsonencoder(obj: Any) -> str:
+    """
+    将obj转换为json字符串
+    :param obj:
+    :return:
+    """
+    try:
+        return str(obj)
+    except TypeError as err:
+        raise TypeError(f"Unsupported type: {type(obj)}") from err
+
+
+_type_jsonencoder.register(Enum, lambda obj: obj.name)
+_type_jsonencoder.register(datetime.datetime, to_timestring)
+_type_jsonencoder.register(datetime.date, lambda obj: to_timestring(obj, "%Y-%m-%d"))
+_type_jsonencoder.register(datetime.time, lambda obj: obj.strftime("%H:%M:%S"))
+_type_jsonencoder.register(datetime.timedelta, lambda obj: obj.total_seconds())
+_type_jsonencoder.register(time.struct_time, to_timestring)
+
+
+class vxJSONEncoder(json.JSONEncoder):
+    """json编码器"""
+
+    def default(self, o):
+        try:
+            return _type_jsonencoder(o)
+        except TypeError:
+            return json.JSONEncoder.default(self, o)
+
+    @staticmethod
+    def register(data_type):
+        """注册一个类型
+
+        Arguments:
+            data_type -- 数据格式
+        @vxJSONEncoder.register(datetime.datetime)
+        def _(obj):
+            return xxx_obj
+        """
+
+        def decorator(func):
+            _type_jsonencoder.register(data_type, func)
+
+            @wraps
+            def wapper(*args, **kwargs):
+                return func(*args, **kwargs)
+
+            return wapper
+
+        return decorator
+
+
+def to_json(obj: Any, indent: int = 4, ensure_ascii=True, **kwargs) -> str:
+    """转化为json格式"""
+    return json.dumps(
+        obj,
+        cls=vxJSONEncoder,
+        ensure_ascii=ensure_ascii,
+        indent=indent,
+        **kwargs,
+    )
+
+
+@lru_cache(100)
+def combine_datetime(date_: Any, time_: str = "00:00:00") -> float:
+    """组合日期和时间"""
+    date_ = to_timestring(date_, "%Y-%m-%d")
+    return to_timestamp(f"{date_} {time_}")
+
+
+if six:
+    __all__ += [
+        "to_text",
+        "to_binary",
+        "is_string",
+        "byte2int",
+    ]
+
+    string_types = (six.string_types, six.text_type, six.binary_type)
+
+    def to_text(value, encoding="utf-8"):
+        """转化为文本格式
+
+        Arguments:
+            value {_type_} -- 待转化的对象
+
+        Keyword Arguments:
+            encoding {str} -- 编码格式 (default: {"utf-8"})
+
+        Returns:
+            six.text_type -- 文件格式
+        """ """ """
+        if isinstance(value, six.text_type):
+            return value
+        if isinstance(value, six.binary_type):
+            return value.decode(encoding)
+        return six.text_type(value)
+
+    def to_binary(value, encoding="utf-8"):
+        """转换成二进制格式
+
+        Arguments:
+            value -- 待转化的对象
+
+        Keyword Arguments:
+            encoding -- 编码格式 (default: {"utf-8"})
+
+        Returns:
+            转换后二进制格式
+        """
+        if isinstance(value, six.binary_type):
+            return value
+        if isinstance(value, six.text_type):
+            return value.encode(encoding)
+        return six.binary_type(value)
+
+    def is_string(value):
+        """转换成sttring'格式
+
+        Arguments:
+            value -- 待转换的对象
+
+        Returns:
+            转换后string格式
+        """
+        return isinstance(value, string_types)
+
+    def byte2int(char_, index=0):
+        """Get the ASCII int value of a character in a string.
+        :param s: a string
+        :param index: the position of desired character
+        :return: ASCII int value
+        """
+        return ord(char_[index]) if six.PY2 else char_[index]
+
+
+class Serializer:
+    _potocols = {}
+
+    def __init__(self, name):
+        pass
+
+    def dumps(self, pyobj):
+        pass
```

### Comparing `vxquant-2023.3.1/src/vxutils/database/mongodb.py` & `vxquant-2023.4.1/src/vxutils/database/mongodb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,306 +1,310 @@
-"""mongodb with vxDataClass and vxDict"""
-
-import contextlib
-from functools import reduce
-from multiprocessing import Lock
-import operator
-from typing import Type, List, Dict, Any
-import pymongo
-from pymongo import MongoClient
-from vxutils import vxDict, vxDataClass, logger
-from vxutils.convertors import local_tzinfo
-
-
-class vxMongoDB:
-    def __init__(
-        self,
-        db_uri: str,
-        db_name: str,
-        collection_mapping: Dict = None,
-    ) -> None:
-        self._db_conn = MongoClient(
-            db_uri, document_class=vxDict, tz_aware=True, tzinfo=local_tzinfo
-        )
-        self._lock = Lock()
-        self._db = self._db_conn.get_database(db_name)
-        self._collection_mapping = collection_mapping or {}
-        try:
-            self._db_conn.admin.command("replSetGetStatus")
-            self._is_replica_set = True
-        except pymongo.errors.OperationFailure:
-            self._is_replica_set = False
-
-    def __getitem__(self, collection_name: str):
-        return (
-            getattr(self._db_conn, collection_name)
-            if collection_name in dir(self._db_conn)
-            else self._db[collection_name]
-        )
-
-    def __getattr__(self, collection_name: str):
-        return (
-            getattr(self._db_conn, collection_name)
-            if collection_name in dir(self._db_conn)
-            else self._db[collection_name]
-        )
-
-    @contextlib.contextmanager
-    def start_session(
-        self,
-        causal_consistency=None,
-        default_transaction_options=None,
-        snapshot=None,
-        lock=True,
-    ):
-        if lock:
-            self._lock.acquire()
-        try:
-            with self._db_conn.start_session(
-                causal_consistency, default_transaction_options, snapshot
-            ) as session:
-                if self._is_replica_set:
-                    with session.start_transaction():
-                        yield session
-                else:
-                    yield session
-        finally:
-            if lock:
-                self._lock.release()
-
-    def mapping(
-        self,
-        collection_name: str,
-        doc_class: Any,
-        primary_keys: List[str] = None,
-    ) -> None:
-        """建立collection 和 vxDataClass 映射关系
-
-        Arguments:
-            collection_name {str} -- _description_
-            doc_class {Type[vxDataClass]} -- _description_
-        """
-        primary_keys = primary_keys or []
-        self._collection_mapping[collection_name] = (doc_class, primary_keys)
-        logger.info(
-            f"{self.__class__.__name__}: collection({collection_name}) mapping to"
-            f" {doc_class.__name__} primary_keys {primary_keys}"
-        )
-
-    def query(
-        self,
-        collection_name: str,
-        filter_: dict = None,
-        session=None,
-        **kwargs,
-    ):
-        """查询条件
-
-        Arguments:
-            collection_name {str} -- collection名称
-            filter_ {dict} -- 过滤条件 (default: {None})
-            session {_type_} -- db session (default: {None})
-        """
-        cur = self._db[collection_name].find(
-            filter_,
-            session=session,
-            # cursor_type=pymongo.CursorType.NON_TAILABLE,
-            **kwargs,
-        )
-        if collection_name in self._collection_mapping:
-            target_class, _ = self._collection_mapping[collection_name]
-            return map(target_class, cur)
-        else:
-            return cur
-
-    def query_one(
-        self, collection_name: str, filter_: dict = None, session=None, **kwargs
-    ):
-        """查找一个文档对象
-
-        Arguments:
-            collection_name {str} -- collection 名称
-
-        Keyword Arguments:
-            filter_ {dict} -- 过滤条件 (default: {None})
-            session {_type_} -- 数据库session (default: {None})
-        """
-        item = self._db[collection_name].find_one(filter_, {"_id": 0}, **kwargs)
-        if not item or collection_name not in self._collection_mapping:
-            return item
-
-        target_class, _ = self._collection_mapping[collection_name]
-        return target_class(item)
-
-    def save(
-        self,
-        collection_name: str,
-        vxdata_obj: vxDataClass,
-        filter_: Dict = None,
-        session=None,
-    ) -> None:
-        """保存vxdataclass obj
-
-        Arguments:
-            collection_name {str} -- 保存的数据表
-            vxdata_obj {vxDataClass} -- vxdata实例
-            filter_ {Dict} -- 过滤条件 (default: {None})
-            session {MongoClient session} -- 数据库session (default: {None})
-        """
-        if not isinstance(vxdata_obj, vxDataClass):
-            raise TypeError(f"vxdata_obj({vxdata_obj} 必须为vxDataClass格式。")
-
-        if collection_name in self._collection_mapping:
-            _, primarykey_keys = self._collection_mapping[collection_name]
-            filter_ = {key: vxdata_obj[key] for key in primarykey_keys}
-            logger.debug(f"{self.__class__.__name__} save vxdata_obj: {vxdata_obj}")
-            self._db[collection_name].update_one(
-                filter_,
-                update={
-                    "$set": vxdata_obj.message
-                    if hasattr(vxdata_obj, "message")
-                    else vxdata_obj
-                },
-                session=session,
-                upsert=True,
-            )
-        else:
-            self._db[collection_name].insert_one(
-                vxdata_obj.message if hasattr(vxdata_obj, "message") else vxdata_obj,
-                session=session,
-            )
-        return
-
-    def save_many(
-        self, collection_name: str, vxdata_objs: List[vxDataClass], session=None
-    ):
-        """保存多个对象
-
-        Arguments:
-            collection_name {str} -- 表格名称
-            vxdata_objs {List[vxDataClass]} -- 对象
-            session {_type_} -- 数据库连接对象 (default: {None})
-        """
-        if collection_name in self._collection_mapping:
-            _, primarykey_keys = self._collection_mapping[collection_name]
-        else:
-            primarykey_keys = []
-
-        commands = []
-        for vxdata_obj in vxdata_objs:
-            filter_ = {key: vxdata_obj[key] for key in primarykey_keys}
-            if filter_:
-                cmd = pymongo.UpdateOne(
-                    filter_,
-                    update={
-                        "$set": vxdata_obj.message
-                        if hasattr(vxdata_obj, "message")
-                        else vxdata_obj
-                    },
-                    upsert=True,
-                )
-            else:
-                cmd = pymongo.InsertOne(
-                    vxdata_obj.message if hasattr(vxdata_obj, "message") else vxdata_obj
-                )
-            commands.append(cmd)
-        if commands:
-            self._db[collection_name].bulk_write(
-                commands, ordered=False, session=session
-            )
-
-    def delete(self, collection_name: str, filter_: Dict, session=None):
-        """删除记录
-
-        Arguments:
-            collection_name {str} -- 表格名称
-            filter_ {Dict} -- 过滤条件
-            session {_type_} -- 数据库连接 (default: {None})
-        """
-        if not filter_:
-            raise ValueError("filter 必须指定相应条件，若删除全表内容，请使用turncate方法.")
-
-        self._db[collection_name].delete_many(filter_, session=session)
-
-    def turncate(self, collection_name: str, session=None) -> None:
-        """清空整表
-
-        Arguments:
-            collection_name {str} -- 表格名称
-            session {_type_} -- 数据库连接 (default: {None})
-        """
-        self._db[collection_name].delete_many({}, session=session)
-
-    def distinct(
-        self, collection_name: str, col_name: str, filter_: Dict = None, session=None
-    ) -> List:
-        """去重后的数值列表
-
-        Arguments:
-            collection_name {str} -- 数据表格名称
-            col_names {List[str]} -- 去重字段
-            filter_ {Dict} -- 过滤条件
-            session {_type_} -- 数据库session (default: {None})
-
-        Returns:
-            List -- 去重后列表
-        """
-        filter_ = filter_ or {}
-        return self._db[collection_name].distinct(col_name, filter_, session=session)
-
-    def disconnect(self):
-        self._db_conn.disconnect()
-
-
-if __name__ == "__main__":
-    import time
-
-    db = vxMongoDB(
-        "mongodb://writer:writer18007558228@127.0.0.1:27017/vxcollector", "vxcollector"
-    )
-
-    with db.start_session(causal_consistency=True) as session:
-        print(
-            db.test.count_documents({}),
-            db.test2.count_documents({}),
-        )
-        db.turncate("test")
-        db.turncate("test2")
-        start = time.perf_counter()
-
-        datas = [vxDict({"name": "test", "cnt": i}) for i in range(100000)]
-
-        # for i in range(100000):
-        #    data =
-        #    datas.append(data)
-        # db.save("test", data)
-        # db.test2.update_one({"cnt": i}, {"$set": data}, upsert=True)
-        # print(f"save: {data.cnt}")
-
-        print(
-            time.perf_counter() - start,
-            db.test.count_documents({}),
-        )
-
-        db.save_many("test2", datas)
-        print(
-            "save test2 datas:",
-            time.perf_counter() - start,
-            db.test2.count_documents({}),
-        )
-
-        print("=" * 60)
-
-        cur = db.query("test2", {})
-
-        print(f"total={reduce(lambda x,y: x+y.cnt, cur,0)}")
-        print(time.perf_counter() - start)
-        print("=" * 60)
-        print(f"total={reduce(operator.add, range(10000),0)}")
-        print(time.perf_counter() - start)
-        print("=" * 60)
-        cnts = db.distinct("test2", "cnt")
-        print(len(cnts))
-        print(time.perf_counter() - start)
-
-    db.close()
-    print(time.perf_counter() - start)
+"""mongodb with vxDataClass and vxDict"""
+
+import contextlib
+from functools import reduce
+from multiprocessing import Lock
+import operator
+from typing import Type, List, Dict, Any
+import pymongo
+from pymongo import MongoClient
+from vxutils import vxDict, vxDataClass, logger
+from vxutils.convertors import local_tzinfo
+
+
+class vxMongoDB:
+    def __init__(
+        self,
+        db_uri: str,
+        db_name: str,
+        collection_mapping: Dict = None,
+    ) -> None:
+        self._db_conn = MongoClient(
+            db_uri, document_class=vxDict, tz_aware=True, tzinfo=local_tzinfo
+        )
+        self._lock = Lock()
+        self._db = self._db_conn.get_database(db_name)
+        self._collection_mapping = collection_mapping or {}
+        try:
+            self._db_conn.admin.command("replSetGetStatus")
+            self._is_replica_set = True
+        except pymongo.errors.OperationFailure:
+            self._is_replica_set = False
+
+    def __getitem__(self, collection_name: str):
+        return (
+            getattr(self._db_conn, collection_name)
+            if collection_name in dir(self._db_conn)
+            else self._db[collection_name]
+        )
+
+    def __getattr__(self, collection_name: str):
+        return (
+            getattr(self._db_conn, collection_name)
+            if collection_name in dir(self._db_conn)
+            else self._db[collection_name]
+        )
+
+    @contextlib.contextmanager
+    def start_session(
+        self,
+        causal_consistency=None,
+        default_transaction_options=None,
+        snapshot=None,
+        lock=True,
+    ):
+        if lock:
+            self._lock.acquire()
+        try:
+            with self._db_conn.start_session(
+                causal_consistency, default_transaction_options, snapshot
+            ) as session:
+                if self._is_replica_set:
+                    with session.start_transaction():
+                        yield session
+                else:
+                    yield session
+        finally:
+            if lock:
+                self._lock.release()
+
+    def mapping(
+        self,
+        collection_name: str,
+        doc_class: Any,
+        primary_keys: List[str] = None,
+    ) -> None:
+        """建立collection 和 vxDataClass 映射关系
+
+        Arguments:
+            collection_name {str} -- _description_
+            doc_class {Type[vxDataClass]} -- _description_
+        """
+        primary_keys = primary_keys or []
+        self._collection_mapping[collection_name] = (doc_class, primary_keys)
+        logger.info(
+            f"{self.__class__.__name__}: collection({collection_name}) mapping to"
+            f" {doc_class.__name__} primary_keys {primary_keys}"
+        )
+
+    def query(
+        self,
+        collection_name: str,
+        filter_: dict = None,
+        session=None,
+        **kwargs,
+    ):
+        """查询条件
+
+        Arguments:
+            collection_name {str} -- collection名称
+            filter_ {dict} -- 过滤条件 (default: {None})
+            session {_type_} -- db session (default: {None})
+        """
+        cur = self._db[collection_name].find(
+            filter_,
+            session=session,
+            # cursor_type=pymongo.CursorType.NON_TAILABLE,
+            **kwargs,
+        )
+        if collection_name in self._collection_mapping:
+            target_class, _ = self._collection_mapping[collection_name]
+            return map(target_class, cur)
+        else:
+            return cur
+
+    def query_one(
+        self, collection_name: str, filter_: dict = None, session=None, **kwargs
+    ):
+        """查找一个文档对象
+
+        Arguments:
+            collection_name {str} -- collection 名称
+
+        Keyword Arguments:
+            filter_ {dict} -- 过滤条件 (default: {None})
+            session {_type_} -- 数据库session (default: {None})
+        """
+        item = self._db[collection_name].find_one(filter_, {"_id": 0}, **kwargs)
+        if not item or collection_name not in self._collection_mapping:
+            return item
+
+        target_class, _ = self._collection_mapping[collection_name]
+        return target_class(item)
+
+    def save(
+        self,
+        collection_name: str,
+        vxdata_obj: vxDataClass,
+        filter_: Dict = None,
+        session=None,
+    ) -> None:
+        """保存vxdataclass obj
+
+        Arguments:
+            collection_name {str} -- 保存的数据表
+            vxdata_obj {vxDataClass} -- vxdata实例
+            filter_ {Dict} -- 过滤条件 (default: {None})
+            session {MongoClient session} -- 数据库session (default: {None})
+        """
+        if not isinstance(vxdata_obj, vxDataClass):
+            raise TypeError(f"vxdata_obj({vxdata_obj} 必须为vxDataClass格式。")
+
+        if collection_name in self._collection_mapping:
+            _, primarykey_keys = self._collection_mapping[collection_name]
+            filter_ = {key: vxdata_obj[key] for key in primarykey_keys}
+            logger.debug(f"{self.__class__.__name__} save vxdata_obj: {vxdata_obj}")
+            self._db[collection_name].update_one(
+                filter_,
+                update={
+                    "$set": (
+                        vxdata_obj.message
+                        if hasattr(vxdata_obj, "message")
+                        else vxdata_obj
+                    )
+                },
+                session=session,
+                upsert=True,
+            )
+        else:
+            self._db[collection_name].insert_one(
+                vxdata_obj.message if hasattr(vxdata_obj, "message") else vxdata_obj,
+                session=session,
+            )
+        return
+
+    def save_many(
+        self, collection_name: str, vxdata_objs: List[vxDataClass], session=None
+    ):
+        """保存多个对象
+
+        Arguments:
+            collection_name {str} -- 表格名称
+            vxdata_objs {List[vxDataClass]} -- 对象
+            session {_type_} -- 数据库连接对象 (default: {None})
+        """
+        if collection_name in self._collection_mapping:
+            _, primarykey_keys = self._collection_mapping[collection_name]
+        else:
+            primarykey_keys = []
+
+        commands = []
+        for vxdata_obj in vxdata_objs:
+            filter_ = {key: vxdata_obj[key] for key in primarykey_keys}
+            if filter_:
+                cmd = pymongo.UpdateOne(
+                    filter_,
+                    update={
+                        "$set": (
+                            vxdata_obj.message
+                            if hasattr(vxdata_obj, "message")
+                            else vxdata_obj
+                        )
+                    },
+                    upsert=True,
+                )
+            else:
+                cmd = pymongo.InsertOne(
+                    vxdata_obj.message if hasattr(vxdata_obj, "message") else vxdata_obj
+                )
+            commands.append(cmd)
+        if commands:
+            self._db[collection_name].bulk_write(
+                commands, ordered=False, session=session
+            )
+
+    def delete(self, collection_name: str, filter_: Dict, session=None):
+        """删除记录
+
+        Arguments:
+            collection_name {str} -- 表格名称
+            filter_ {Dict} -- 过滤条件
+            session {_type_} -- 数据库连接 (default: {None})
+        """
+        if not filter_:
+            raise ValueError("filter 必须指定相应条件，若删除全表内容，请使用turncate方法.")
+
+        self._db[collection_name].delete_many(filter_, session=session)
+
+    def turncate(self, collection_name: str, session=None) -> None:
+        """清空整表
+
+        Arguments:
+            collection_name {str} -- 表格名称
+            session {_type_} -- 数据库连接 (default: {None})
+        """
+        self._db[collection_name].delete_many({}, session=session)
+
+    def distinct(
+        self, collection_name: str, col_name: str, filter_: Dict = None, session=None
+    ) -> List:
+        """去重后的数值列表
+
+        Arguments:
+            collection_name {str} -- 数据表格名称
+            col_names {List[str]} -- 去重字段
+            filter_ {Dict} -- 过滤条件
+            session {_type_} -- 数据库session (default: {None})
+
+        Returns:
+            List -- 去重后列表
+        """
+        filter_ = filter_ or {}
+        return self._db[collection_name].distinct(col_name, filter_, session=session)
+
+    def disconnect(self):
+        self._db_conn.disconnect()
+
+
+if __name__ == "__main__":
+    import time
+
+    db = vxMongoDB(
+        "mongodb://writer:writer18007558228@127.0.0.1:27017/vxcollector", "vxcollector"
+    )
+
+    with db.start_session(causal_consistency=True) as session:
+        print(
+            db.test.count_documents({}),
+            db.test2.count_documents({}),
+        )
+        db.turncate("test")
+        db.turncate("test2")
+        start = time.perf_counter()
+
+        datas = [vxDict({"name": "test", "cnt": i}) for i in range(100000)]
+
+        # for i in range(100000):
+        #    data =
+        #    datas.append(data)
+        # db.save("test", data)
+        # db.test2.update_one({"cnt": i}, {"$set": data}, upsert=True)
+        # print(f"save: {data.cnt}")
+
+        print(
+            time.perf_counter() - start,
+            db.test.count_documents({}),
+        )
+
+        db.save_many("test2", datas)
+        print(
+            "save test2 datas:",
+            time.perf_counter() - start,
+            db.test2.count_documents({}),
+        )
+
+        print("=" * 60)
+
+        cur = db.query("test2", {})
+
+        print(f"total={reduce(lambda x,y: x+y.cnt, cur,0)}")
+        print(time.perf_counter() - start)
+        print("=" * 60)
+        print(f"total={reduce(operator.add, range(10000),0)}")
+        print(time.perf_counter() - start)
+        print("=" * 60)
+        cnts = db.distinct("test2", "cnt")
+        print(len(cnts))
+        print(time.perf_counter() - start)
+
+    db.close()
+    print(time.perf_counter() - start)
```

### Comparing `vxquant-2023.3.1/src/vxutils/dataclass.py` & `vxquant-2023.4.1/src/vxutils/dataclass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,659 +1,671 @@
-# encoding=utf-8
-""" 定制的数据类型
-
-vxDataClass
-vxDict
-
-"""
-
-
-import contextlib
-from functools import singledispatch
-import zlib
-import math
-import uuid
-import pickle
-from pathlib import Path
-from enum import Enum
-from collections.abc import MutableMapping, Mapping, Sequence
-from typing import Any, Callable, Optional, List, Dict
-from operator import getitem
-from vxutils import (
-    vxtime,
-    vxJSONEncoder,
-    to_json,
-    to_enum,
-    to_timestamp,
-    to_timestring,
-)
-
-try:
-    import simplejson as json
-except ImportError:
-    import json
-
-
-__all__ = [
-    "vxField",
-    "vxUUIDField",
-    "vxEnumField",
-    "vxIntField",
-    "vxFloatField",
-    "vxPropertyField",
-    "vxDatetimeField",
-    "vxBoolField",
-    "vxDataMeta",
-    "vxDataClass",
-    "vxDataConvertor",
-    "vxDict",
-]
-
-
-class vxField:
-    """字段属性描述符
-
-    default_factory: 缺省值 或缺省值生成函数
-        ---> default_factory()
-
-    convertor_factory: 类型转换函数
-        ---> convertor_factory(input_value) -> value
-        ---> 例如: lambda x: to_timestring(x)
-
-    property_factory: 属性函数字段
-        ---> property_factory(obj)  -> value
-        ---> 例如: lambda obj: obj.x+obj.y
-
-    format_factory: 格式化输入函数
-        ---> fortmat_factory(value) ---> string
-        ---> 例如：lambda value: to_timestring(value, '%Y-%m-%d %H:%M:%S')
-
-
-    """
-
-    __slots__ = [
-        "_name",
-        "_fget",
-        "_fset",
-        "_property_factory",
-        "_default_factory",
-        "_convertor_factory",
-        "_format_factory",
-    ]
-
-    def __init__(
-        self,
-        default_factory: Any = None,
-        convertor_factory: Callable = None,
-        property_factory: Callable = None,
-        format_factory: Callable = None,
-    ):
-        self._fget = None
-        self._fset = None
-        self._property_factory = property_factory
-        self._default_factory = (
-            default_factory if callable(default_factory) else lambda: default_factory
-        )
-        self._convertor_factory = convertor_factory
-        self._format_factory: Callable = format_factory
-        self._name = None
-
-    def __set_name__(self, owner, name):
-        """设置属性名称"""
-
-        self._name = f"_{name}"
-        # 设置获取attr的方法
-        if callable(self._property_factory):
-            self._fget = lambda obj, owner: self._property_factory(obj)
-            self._fset = None
-            return
-
-        self._fget = lambda obj, owner: getattr(obj, self._name, self.default)
-
-        if self._name == "_updated_dt":
-
-            def fset(obj, value):
-                setattr(obj, "_updated_dt", self._convertor_factory(value))
-
-        elif callable(self._convertor_factory):
-
-            def fset(obj, value):
-                setattr(obj, self._name, self._convertor_factory(value))
-                setattr(obj, "_updated_dt", vxtime.now())
-
-        else:
-
-            def fset(obj, value):
-                setattr(obj, self._name, value)
-                setattr(obj, "_updated_dt", vxtime.now())
-
-        self._fset = fset
-
-    def __get__(self, obj, owner):
-        try:
-            return self._fget(obj, owner)
-        except Exception:
-            return self.default
-
-    def __set__(self, obj, value):
-        if self._fset is None:
-            return
-
-        try:
-            self._fset(obj, value)
-        except Exception:
-            setattr(obj, self._name, self.default)
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__} default: {self.default}"
-
-    __repr__ = __str__
-
-    @property
-    def default(self):
-        """缺省值"""
-
-        return self._default_factory()
-
-
-class vxUUIDField(vxField):
-    """uuid类型
-
-    auto : auto 为True,则系统初始化自动创建一个uuid，为false则默认值为: ''
-    """
-
-    def __init__(self, auto=True) -> None:
-        super().__init__(
-            default_factory=lambda: str(uuid.uuid4()) if auto else "",
-            convertor_factory=lambda value: value or "",
-        )
-
-
-class vxEnumField(vxField):
-    """Enum类型字段"""
-
-    def __init__(self, default: Enum) -> None:
-        super().__init__(
-            default_factory=lambda: default,
-            convertor_factory=lambda x: to_enum(x, default.__class__, default),
-        )
-
-
-class vxIntField(vxField):
-    """整数类型字段"""
-
-    def __init__(
-        self, default: int, _min: Optional[float] = None, _max: Optional[float] = None
-    ):
-        if _min is None:
-            _min = -math.inf
-
-        if _max is None:
-            _max = math.inf
-
-        def check_int(v: Any):
-            # 四舍五入
-            v = round(v)
-            if _min <= v <= _max:
-                return v
-            raise ValueError(f"赋值 {v} 超出取值范围: [{_min},{_max}]")
-
-        super().__init__(default_factory=default, convertor_factory=check_int)
-
-
-class vxFloatField(vxField):
-    """浮点类型字段"""
-
-    def __init__(
-        self,
-        default: float,
-        ndigits: Optional[int] = None,
-        _min: Optional[float] = None,
-        _max: Optional[float] = None,
-    ):
-        if _min is None:
-            _min = -math.inf
-
-        if _max is None:
-            _max = math.inf
-
-        def check_float(v: Any):
-            v = float(v)
-            if ndigits is not None:
-                v = round(v, ndigits)
-
-            if _min <= v <= _max:
-                return v
-            raise ValueError(f"赋值 {v} 超出取值范围: [{_min},{_max}]")
-
-        super().__init__(default_factory=default, convertor_factory=check_float)
-
-
-class vxPropertyField(vxField):
-    """函数属性类型字段"""
-
-    def __init__(
-        self, property_factory: Callable[[Any], Any], default_factory: Any = None
-    ):
-        super().__init__(
-            property_factory=property_factory, default_factory=default_factory
-        )
-
-
-class vxDatetimeField(vxField):
-    """时间类型字段"""
-
-    def __init__(self, default_factory=vxtime.now, formatter_string="%F %H:%M:%S.%f"):
-        super().__init__(
-            default_factory=default_factory,
-            convertor_factory=to_timestamp,
-            format_factory=lambda value: to_timestring(value, formatter_string),
-        )
-
-
-class vxBoolField(vxField):
-    """bool字段"""
-
-    def __init__(self, default):
-        super().__init__(default_factory=bool(default), convertor_factory=bool)
-
-
-class vxDataMeta(type):
-    """data 元类"""
-
-    def __new__(cls, name: str, bases: tuple, attrs: dict):
-        message_formater = {
-            name: var._format_factory
-            for name, var in attrs.items()
-            if isinstance(var, vxField)
-        }
-
-        for base_cls in bases:
-            message_formater.update(**base_cls.__vxfields__)
-
-        attrs["created_dt"]: float = vxDatetimeField()
-        attrs["updated_dt"]: float = vxDatetimeField()
-        message_formater["created_dt"] = attrs["created_dt"]._format_factory
-        message_formater["updated_dt"] = attrs["updated_dt"]._format_factory
-
-        if "__sortkeys__" in attrs:
-
-            def is_lower_than(self, other: "vxDataClass") -> bool:
-                """< 根据sortkeys的顺序一次对比"""
-                for k in self.__sortkeys__:
-                    if getattr(self, k) < getattr(other, k):
-                        return True
-                    elif getattr(self, k) > getattr(other, k):
-                        return False
-                return False
-
-            def is_greater_than(self, other: "vxDataClass") -> bool:
-                """> 根据sortkeys的顺序一次对比"""
-                for k in self.__sortkeys__:
-                    if getattr(self, k) < getattr(other, k):
-                        return False
-                    elif getattr(self, k) > getattr(other, k):
-                        return True
-                return False
-
-            attrs["__lt__"] = is_lower_than
-            attrs["__gt__"] = is_greater_than
-
-        attrs["__vxfields__"] = message_formater
-        attrs["__slots__"] = tuple(f"_{name}" for name in message_formater)
-
-        return type.__new__(cls, name, bases, attrs)
-
-    def __call__(cls, *args, **kwds) -> Any:
-        created_dt = kwds.pop("created_dt", vxtime.now())
-        updated_dt = kwds.pop("updated_dt", created_dt)
-        instance = super().__call__(*args, **kwds)
-        instance.created_dt = created_dt
-        instance.updated_dt = updated_dt
-
-        return instance
-
-
-class vxDataClass(metaclass=vxDataMeta):
-    """数据基类"""
-
-    __vxfields__: dict = {}
-    __sortkeys__: tuple = ()
-
-    def __init__(self, *args, **kwargs) -> None:
-        if args and isinstance(args[0], Mapping):
-            kwargs.update(args[0])
-        elif args:
-            kwargs.update(zip(self.__vxfields__, args))
-
-        for attr in self.keys():
-            value = kwargs.pop(attr, getattr(self, attr))
-            setattr(self, attr, value)
-
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key)
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        setattr(self, key, value)
-
-    def __len__(self):
-        return len(self.__vxfields__)
-
-    def __str__(self):
-        message = {}
-        try:
-            for attr, formatter in self.__vxfields__.items():
-                value = getattr(self, attr)
-                if isinstance(value, vxDataClass):
-                    value = value
-                elif formatter:
-                    value = formatter(value)
-
-                message[attr] = value
-            return f"< {self.__class__.__name__}(id-{id(self)}) : {to_json(message)} >"
-        except Exception:
-            message = {k: getattr(self, k) for k in self.keys()}
-            return f"< {self.__class__.__name__}(id-{id(self)}) : {message} >"
-
-    __repr__ = __str__
-
-    def __hash__(self):
-        return hash(self.__str__())
-
-    def __eq__(self, __o: "vxDataClass") -> bool:
-        return all(v == __o[k] for k, v in self.items())
-
-    def __contains__(self, item: str) -> bool:
-        return item in self.keys() if item else False
-
-    def __setstate__(self, state: dict):
-        self.__init__(**state)
-
-    def __getstate__(self):
-        return self.message
-
-    def __iter__(self):
-        return next(self)
-
-    def __next__(self):
-        yield from self.keys()
-
-    @property
-    def message(self) -> dict:
-        """展示数据"""
-        message = {}
-        for k, v in self.items():
-            if isinstance(v, Enum):
-                message[k] = v.name
-            elif isinstance(v, vxDataClass):
-                message[k] = v.message
-            else:
-                message[k] = v
-
-        return message
-
-    @staticmethod
-    def pack(obj):
-        """打包消息"""
-        pickled = pickle.dumps(obj)
-        return zlib.compress(pickled)
-
-    @staticmethod
-    def unpack(packed_obj):
-        """解包消息"""
-        pickled = zlib.decompress(packed_obj)
-        return pickle.loads(pickled)
-
-    def keys(self) -> Sequence:
-        """相关keys"""
-        yield from self.__vxfields__
-
-    def update(self, **kwargs):
-        """更新数据"""
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-
-    def values(self) -> Sequence:
-        """获取内部数据"""
-        yield from [getattr(self, key) for key in self.keys()]
-
-    def items(self) -> Sequence:
-        """获取相关(key,value)对"""
-        yield from [(key, getattr(self, key)) for key in self.keys()]
-
-    def get(self, key, _default=None) -> Any:
-        """获取相关"""
-        return getattr(self, key, _default)
-
-
-@vxJSONEncoder.register(vxDataClass)
-def _(obj):
-    message = {}
-
-    for attr, formatter in obj.__vxfields__.items():
-        value = getattr(obj, attr)
-        if isinstance(value, vxDataClass):
-            value = value
-        elif formatter:
-            value = formatter(value)
-
-        message[attr] = value
-
-    return message
-
-
-class vxDataConvertor:
-    """数据转换器基础类"""
-
-    def __init__(
-        self,
-        target_cls,
-        convertors_mapping: MutableMapping = None,
-        defaults: MutableMapping = None,
-    ) -> None:
-        self._target_cls = target_cls
-        self._convertors = {}
-        self._defaults_data = defaults or {}
-
-        if convertors_mapping is None:
-            return
-
-        for target_col, convertor in convertors_mapping.items():
-            if callable(convertor):
-                self.add_convertors(target_col, convertor)
-            else:
-                self.rename_columns(convertor, target_col)
-
-    def add_convertors(self, target_col, conveter_func):
-        """设置col的转换函数
-
-        target_col : 待转换的字段名
-        convertor_func(other_data) ：转换函数 或者是缺省值，其中other_data 为待转换对象内容
-        """
-        if not callable(conveter_func):
-            raise ValueError(f"func({conveter_func.__name__} is not callable")
-        self._convertors[target_col] = conveter_func
-
-    def rename_columns(self, source_col, target_col):
-        """重命名字段"""
-
-        def _rename_func(other_data):
-            """重命名转换器"""
-            if hasattr(other_data, source_col):
-                return getattr(other_data, source_col)
-            return other_data[source_col]
-
-        self._convertors[target_col] = _rename_func
-
-    def set_defaults(self, target_col, default_value):
-        """设置默认值"""
-        self._defaults_data[target_col] = default_value
-
-    def _convert_col(self, col, other_data):
-        try:
-            col_value = self._defaults_data.get(col, None)
-            if col in self._convertors:
-                col_value = self._convertors[col](other_data)
-            elif hasattr(other_data, col):
-                col_value = getattr(other_data, col)
-            else:
-                col_value = getitem(other_data, col)
-        except Exception as err:
-            from vxutils import logger
-
-            logger.debug(
-                (
-                    f"target class: {self._target_cls.__name__} Other_data load"
-                    f" col:{col} err. {err}"
-                ),
-                exc_info=True,
-            )
-            logger.debug(f"other_data={other_data}")
-
-        return col, col_value
-
-    def __call__(self, other_data, key="", **kwargs):
-        data = dict(
-            self._convert_col(col, other_data) for col in self._target_cls.__vxfields__
-        )
-        data.update(**kwargs)
-        instance = self._target_cls(data)
-        return (
-            (instance[key], instance)
-            if len(key) > 0 and key in instance.keys()
-            else instance
-        )
-
-
-class vxDict(MutableMapping):
-    """引擎上下文context类"""
-
-    _default_config: Dict[str, Any] = {}
-
-    def __init__(self, default_config: MutableMapping = None, **kwargs):
-        default_config = default_config or {}
-        default_config.update(kwargs)
-        for k, v in default_config.items():
-            self.__dict__[k] = _to_vxdict(v)
-
-    def __getitem__(self, key):
-        return self.__dict__[key]
-
-    def __setitem__(self, key, value):
-        self.__dict__[key] = value
-
-    def __delitem__(self, key):
-        self.__dict__.__delitem__(key)
-
-    def __setattr__(self, attr: str, value: Any) -> Any:
-        self.__dict__[attr] = _to_vxdict(value)
-
-    def __len__(self) -> int:
-        return len(self.__dict__)
-
-    def __eq__(self, __o: MutableMapping) -> bool:
-        if len(self) != len(__o):
-            return False
-
-        try:
-            return all(v == __o[k] for k, v in self.items())
-        except Exception:
-            return False
-
-    def __hash__(self):
-        return hash(self.__str__())
-
-    def __setstate__(self, state) -> None:
-        self.__init__(**state)
-
-    def __getstate__(self) -> dict:
-        return self.__dict__
-
-    def __str__(self):
-        try:
-            return f"< {self.__class__.__name__}(id-{id(self)}) : {to_json(self)} >"
-        except (TypeError, KeyError):
-            return f"< {self.__class__.__name__}(id-{id(self)}) : {self.__dict__} >"
-
-    __repr__ = __str__
-
-    def __iter__(self):
-        yield from self.__dict__
-
-    def keys(self):
-        yield from self.__dict__
-
-    def values(self):
-        yield from self.__dict__.values()
-
-    def update(self, config: MutableMapping = None, **kwargs):
-        """批量更新字典"""
-        config = config or kwargs
-        for k, v in config.items():
-            self.__dict__[k] = _to_vxdict(v)
-
-    def items(self):
-        """(key,value) pairs"""
-        yield from self.__dict__.items()
-
-    def pop(self, key: str, default_: Any = None) -> Any:
-        """弹出key对应的value，若无此数据，则返回default_"""
-        return self.__dict__.pop(key, default_)
-
-    def clear(self) -> None:
-        """清空context"""
-        self.__dict__ = {}
-
-    @staticmethod
-    def load_json(json_file, default_config=None) -> None:
-        """加载json file
-
-        Arguments:
-            json_file {_type_} -- 加载的json file
-
-        Raises:
-            OSError: 文件不存在
-        """
-
-        json_file = Path(json_file)
-        if not json_file.exists():
-            raise OSError(f"json_file({json_file.as_posix()}) is not exists.")
-
-        with open(json_file.as_posix(), "r", encoding="utf-8") as fp:
-            config = json.load(fp)
-
-        return vxDict(default_config, **config)
-
-    def save_json(self, json_file: str) -> None:
-        """保存json file
-
-        Arguments:
-            json_file {str} -- 待保存的json file
-
-        """
-        with open(json_file, "w", encoding="utf-8") as fp:
-            json.dump(self, fp, indent=4, cls=vxJSONEncoder)
-
-
-@singledispatch
-def _to_vxdict(self: Any):
-    """转换为vxdict obj"""
-    return self
-
-
-@_to_vxdict.register(MutableMapping)
-def _(obj: MutableMapping) -> vxDict:
-    return vxDict(**obj)
-
-
-@_to_vxdict.register(Sequence)
-def _(obj: Sequence) -> List:
-    return obj if isinstance(obj, str) else [_to_vxdict(o_) for o_ in obj]
-
-
-@vxJSONEncoder.register(vxDict)
-def _(obj):
-    return dict(obj.items())
-
-
-MutableMapping.register(vxDict)
-Mapping.register(vxDataClass)
+# encoding=utf-8
+""" 定制的数据类型
+
+vxDataClass
+vxDict
+
+"""
+
+
+import zlib
+import math
+import uuid
+import pickle
+from pathlib import Path
+from enum import Enum
+from functools import singledispatch
+from collections import UserDict
+from collections.abc import MutableMapping, Mapping, Sequence
+from typing import Any, Callable, Optional, List, Dict
+from operator import getitem
+from vxutils import (
+    vxtime,
+    vxJSONEncoder,
+    to_json,
+    to_enum,
+    to_timestamp,
+    to_timestring,
+    to_binary,
+)
+
+try:
+    import simplejson as json
+except ImportError:
+    import json
+
+
+__all__ = [
+    "vxField",
+    "vxUUIDField",
+    "vxEnumField",
+    "vxIntField",
+    "vxFloatField",
+    "vxPropertyField",
+    "vxDatetimeField",
+    "vxBoolField",
+    "vxDataMeta",
+    "vxDataClass",
+    "vxDataConvertor",
+    "vxDict",
+]
+
+
+class vxField:
+    """字段属性描述符
+
+    default_factory: 缺省值 或缺省值生成函数
+        ---> default_factory()
+
+    convertor_factory: 类型转换函数
+        ---> convertor_factory(input_value) -> value
+        ---> 例如: lambda x: to_timestring(x)
+
+    property_factory: 属性函数字段
+        ---> property_factory(obj)  -> value
+        ---> 例如: lambda obj: obj.x+obj.y
+
+    format_factory: 格式化输入函数
+        ---> fortmat_factory(value) ---> string
+        ---> 例如：lambda value: to_timestring(value, '%Y-%m-%d %H:%M:%S')
+
+
+    """
+
+    __slots__ = [
+        "_name",
+        "_fget",
+        "_fset",
+        "_property_factory",
+        "_default_factory",
+        "_convertor_factory",
+        "_format_factory",
+    ]
+
+    def __init__(
+        self,
+        default_factory: Any = None,
+        convertor_factory: Callable = None,
+        property_factory: Callable = None,
+        format_factory: Callable = None,
+    ):
+        self._fget = None
+        self._fset = None
+        self._property_factory = property_factory
+        self._default_factory = (
+            default_factory if callable(default_factory) else lambda: default_factory
+        )
+        self._convertor_factory = convertor_factory
+        self._format_factory: Callable = format_factory
+        self._name = None
+
+    def __set_name__(self, owner, name):
+        """设置属性名称"""
+
+        self._name = f"_{name}"
+        # 设置获取attr的方法
+        if callable(self._property_factory):
+            self._fget = lambda obj, owner: self._property_factory(obj)
+            self._fset = None
+            return
+
+        self._fget = lambda obj, owner: getattr(obj, self._name, self.default)
+
+        if self._name == "_updated_dt":
+
+            def fset(obj, value):
+                setattr(obj, "_updated_dt", self._convertor_factory(value))
+
+        elif callable(self._convertor_factory):
+
+            def fset(obj, value):
+                setattr(obj, self._name, self._convertor_factory(value))
+                setattr(obj, "_updated_dt", vxtime.now())
+
+        else:
+
+            def fset(obj, value):
+                setattr(obj, self._name, value)
+                setattr(obj, "_updated_dt", vxtime.now())
+
+        self._fset = fset
+
+    def __get__(self, obj, owner):
+        try:
+            return self._fget(obj, owner)
+        except Exception:
+            return self.default
+
+    def __set__(self, obj, value):
+        if self._fset is None:
+            return
+
+        try:
+            self._fset(obj, value)
+        except Exception:
+            setattr(obj, self._name, self.default)
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__} default: {self.default}"
+
+    __repr__ = __str__
+
+    @property
+    def default(self):
+        """缺省值"""
+
+        return self._default_factory()
+
+
+class vxUUIDField(vxField):
+    """uuid类型
+
+    auto : auto 为True,则系统初始化自动创建一个uuid，为false则默认值为: ''
+    """
+
+    def __init__(self, auto=True) -> None:
+        super().__init__(
+            default_factory=lambda: str(uuid.uuid4()) if auto else "",
+            convertor_factory=lambda value: value or "",
+        )
+
+
+class vxEnumField(vxField):
+    """Enum类型字段"""
+
+    def __init__(self, default: Enum) -> None:
+        super().__init__(
+            default_factory=lambda: default,
+            convertor_factory=lambda x: to_enum(x, default.__class__, default),
+            format_factory=lambda value: value.name,
+        )
+
+
+class vxIntField(vxField):
+    """整数类型字段"""
+
+    def __init__(
+        self, default: int, _min: Optional[float] = None, _max: Optional[float] = None
+    ):
+        if _min is None:
+            _min = -math.inf
+
+        if _max is None:
+            _max = math.inf
+
+        def check_int(v: Any):
+            # 四舍五入
+            v = round(v)
+            if _min <= v <= _max:
+                return v
+            raise ValueError(f"赋值 {v} 超出取值范围: [{_min},{_max}]")
+
+        super().__init__(default_factory=default, convertor_factory=check_int)
+
+
+class vxFloatField(vxField):
+    """浮点类型字段"""
+
+    def __init__(
+        self,
+        default: float,
+        ndigits: Optional[int] = None,
+        _min: Optional[float] = None,
+        _max: Optional[float] = None,
+    ):
+        if _min is None:
+            _min = -math.inf
+
+        if _max is None:
+            _max = math.inf
+
+        def check_float(v: Any):
+            v = float(v)
+            if ndigits is not None:
+                v = round(v, ndigits)
+
+            if _min <= v <= _max:
+                return v
+            raise ValueError(f"赋值 {v} 超出取值范围: [{_min},{_max}]")
+
+        super().__init__(default_factory=default, convertor_factory=check_float)
+
+
+class vxPropertyField(vxField):
+    """函数属性类型字段"""
+
+    def __init__(
+        self, property_factory: Callable[[Any], Any], default_factory: Any = None
+    ):
+        super().__init__(
+            property_factory=property_factory, default_factory=default_factory
+        )
+
+
+class vxDatetimeField(vxField):
+    """时间类型字段"""
+
+    def __init__(
+        self,
+        default_factory=vxtime.now,
+        formatter_string="%F %H:%M:%S.%f",
+        convertor_factory=to_timestamp,
+    ):
+        super().__init__(
+            default_factory=default_factory,
+            convertor_factory=convertor_factory,
+            format_factory=lambda value: to_timestring(value, formatter_string),
+        )
+
+
+class vxBoolField(vxField):
+    """bool字段"""
+
+    def __init__(self, default):
+        super().__init__(default_factory=bool(default), convertor_factory=bool)
+
+
+class vxBytesField(vxField):
+    """bytes字段"""
+
+    def __init__(self, default: bytes = b""):
+        super().__init__(default_factory=lambda: default, convertor_factory=to_binary)
+
+
+class vxDataMeta(type):
+    """data 元类"""
+
+    def __new__(cls, name: str, bases: tuple, attrs: dict):
+        message_formater = {
+            name: var._format_factory
+            for name, var in attrs.items()
+            if isinstance(var, vxField)
+        }
+
+        for base_cls in bases:
+            message_formater.update(**base_cls.__vxfields__)
+
+        attrs["created_dt"]: float = vxDatetimeField()
+        attrs["updated_dt"]: float = vxDatetimeField()
+        message_formater["created_dt"] = attrs["created_dt"]._format_factory
+        message_formater["updated_dt"] = attrs["updated_dt"]._format_factory
+
+        if "__sortkeys__" in attrs:
+
+            def is_lower_than(self, other: "vxDataClass") -> bool:
+                """< 根据sortkeys的顺序一次对比"""
+                for k in self.__sortkeys__:
+                    if getattr(self, k) < getattr(other, k):
+                        return True
+                    elif getattr(self, k) > getattr(other, k):
+                        return False
+                return False
+
+            def is_greater_than(self, other: "vxDataClass") -> bool:
+                """> 根据sortkeys的顺序一次对比"""
+                for k in self.__sortkeys__:
+                    if getattr(self, k) < getattr(other, k):
+                        return False
+                    elif getattr(self, k) > getattr(other, k):
+                        return True
+                return False
+
+            attrs["__lt__"] = is_lower_than
+            attrs["__gt__"] = is_greater_than
+
+        attrs["__vxfields__"] = message_formater
+        attrs["__slots__"] = tuple(f"_{name}" for name in message_formater)
+
+        return type.__new__(cls, name, bases, attrs)
+
+    def __call__(cls, *args, **kwds) -> Any:
+        created_dt = kwds.pop("created_dt", None)
+        updated_dt = kwds.pop("updated_dt", None)
+        instance = super().__call__(*args, **kwds)
+        if created_dt:
+            instance.created_dt = created_dt
+            instance.updated_dt = updated_dt or created_dt
+
+        return instance
+
+
+class vxDataClass(metaclass=vxDataMeta):
+    """数据基类"""
+
+    __vxfields__: dict = {}
+    __sortkeys__: tuple = ()
+
+    def __init__(self, *args, **kwargs) -> None:
+        if args and isinstance(args[0], Mapping):
+            kwargs.update(args[0])
+        elif args:
+            kwargs.update(zip(self.__vxfields__, args))
+
+        for attr in self.keys():
+            value = kwargs.pop(attr, getattr(self, attr))
+            setattr(self, attr, value)
+
+    def __getitem__(self, key: str) -> Any:
+        return getattr(self, key)
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        setattr(self, key, value)
+
+    def __len__(self):
+        return len(self.__vxfields__)
+
+    def __str__(self):
+        message = {}
+        try:
+            for attr, formatter in self.__vxfields__.items():
+                value = getattr(self, attr)
+                if isinstance(value, vxDataClass):
+                    value = value
+                elif formatter:
+                    value = formatter(value)
+
+                message[attr] = value
+            return f"< {self.__class__.__name__}(id-{id(self)}) : {to_json(message)} >"
+        except Exception:
+            message = {k: getattr(self, k) for k in self.keys()}
+            return f"< {self.__class__.__name__}(id-{id(self)}) : {message} >"
+
+    __repr__ = __str__
+
+    def __hash__(self):
+        return hash(self.__str__())
+
+    def __eq__(self, __o: "vxDataClass") -> bool:
+        return all(v == __o[k] for k, v in self.items())
+
+    def __contains__(self, item: str) -> bool:
+        return item in self.keys() if item else False
+
+    def __setstate__(self, state: dict):
+        self.__init__(**state)
+
+    def __getstate__(self):
+        return self.message
+
+    def __iter__(self):
+        return next(self)
+
+    def __next__(self):
+        yield from self.keys()
+
+    @property
+    def message(self) -> dict:
+        """展示数据"""
+        message = {}
+        for k, v in self.items():
+            if isinstance(v, Enum):
+                message[k] = v.name
+            elif isinstance(v, vxDataClass):
+                message[k] = v.message
+            else:
+                message[k] = v
+
+        return message
+
+    @staticmethod
+    def pack(obj):
+        """打包消息"""
+        pickled = pickle.dumps(obj)
+        return zlib.compress(pickled)
+
+    @staticmethod
+    def unpack(packed_obj):
+        """解包消息"""
+        pickled = zlib.decompress(packed_obj)
+        return pickle.loads(pickled)
+
+    def keys(self) -> Sequence:
+        """相关keys"""
+        yield from self.__vxfields__
+
+    def update(self, **kwargs):
+        """更新数据"""
+        for k, v in kwargs.items():
+            setattr(self, k, v)
+
+    def values(self) -> Sequence:
+        """获取内部数据"""
+        yield from [getattr(self, key) for key in self.keys()]
+
+    def items(self) -> Sequence:
+        """获取相关(key,value)对"""
+        yield from [(key, getattr(self, key)) for key in self.keys()]
+
+    def get(self, key, _default=None) -> Any:
+        """获取相关"""
+        return getattr(self, key, _default)
+
+
+@vxJSONEncoder.register(vxDataClass)
+def _(obj):
+    message = {}
+
+    for attr, formatter in obj.__vxfields__.items():
+        value = getattr(obj, attr)
+        if isinstance(value, vxDataClass):
+            value = value
+        elif formatter:
+            value = formatter(value)
+
+        message[attr] = value
+
+    return message
+
+
+class vxDataConvertor:
+    """数据转换器基础类"""
+
+    def __init__(
+        self,
+        target_cls,
+        convertors_mapping: MutableMapping = None,
+        defaults: MutableMapping = None,
+    ) -> None:
+        self._target_cls = target_cls
+        self._convertors = {}
+        self._defaults_data = defaults or {}
+
+        if convertors_mapping is None:
+            return
+
+        for target_col, convertor in convertors_mapping.items():
+            if callable(convertor):
+                self.add_convertors(target_col, convertor)
+            else:
+                self.rename_columns(convertor, target_col)
+
+    def add_convertors(self, target_col, conveter_func):
+        """设置col的转换函数
+
+        target_col : 待转换的字段名
+        convertor_func(other_data) ：转换函数 或者是缺省值，其中other_data 为待转换对象内容
+        """
+        if not callable(conveter_func):
+            raise ValueError(f"func({conveter_func.__name__} is not callable")
+        self._convertors[target_col] = conveter_func
+
+    def rename_columns(self, source_col, target_col):
+        """重命名字段"""
+
+        def _rename_func(other_data):
+            """重命名转换器"""
+            if hasattr(other_data, source_col):
+                return getattr(other_data, source_col)
+            return other_data[source_col]
+
+        self._convertors[target_col] = _rename_func
+
+    def set_defaults(self, target_col, default_value):
+        """设置默认值"""
+        self._defaults_data[target_col] = default_value
+
+    def _convert_col(self, col, other_data):
+        try:
+            col_value = self._defaults_data.get(col, None)
+            if col in self._convertors:
+                col_value = self._convertors[col](other_data)
+            elif hasattr(other_data, col):
+                col_value = getattr(other_data, col)
+            else:
+                col_value = getitem(other_data, col)
+        except Exception as err:
+            from vxutils import logger
+
+            logger.debug(
+                f"target class: {self._target_cls.__name__} Other_data load"
+                f" col:{col} err. {err}",
+                exc_info=True,
+            )
+            logger.debug(f"other_data={other_data}")
+
+        return col, col_value
+
+    def __call__(self, other_data, key="", **kwargs):
+        data = dict(
+            self._convert_col(col, other_data) for col in self._target_cls.__vxfields__
+        )
+        data.update(**kwargs)
+        instance = self._target_cls(data)
+        return (
+            (str(instance[key]), instance)
+            if len(key) > 0 and key in instance.keys()
+            else instance
+        )
+
+
+class vxDict(UserDict):
+    """引擎上下文context类"""
+
+    _default_config: Dict[str, Any] = {}
+
+    def __init__(self, *args, **kwargs):
+        default_config = dict(*args, **kwargs)
+        for k, v in default_config.items():
+            self.__dict__[k] = _to_vxdict(v)
+
+    def __getitem__(self, key):
+        return self.__dict__[key]
+
+    def __setitem__(self, key, value):
+        self.__dict__[key] = value
+
+    def __delitem__(self, key):
+        self.__dict__.__delitem__(key)
+
+    def __setattr__(self, attr: str, value: Any) -> Any:
+        self.__dict__[attr] = _to_vxdict(value)
+
+    def __len__(self) -> int:
+        return len(self.__dict__)
+
+    def __eq__(self, __o: MutableMapping) -> bool:
+        if len(self) != len(__o):
+            return False
+
+        try:
+            return all(v == __o[k] for k, v in self.items())
+        except Exception:
+            return False
+
+    def __hash__(self):
+        return hash(self.__str__())
+
+    def __setstate__(self, state) -> None:
+        self.__init__(**state)
+
+    def __getstate__(self) -> dict:
+        return self.__dict__
+
+    def __str__(self):
+        try:
+            return f"< {self.__class__.__name__}(id-{id(self)}) : {to_json(self)} >"
+        except (TypeError, KeyError):
+            return f"< {self.__class__.__name__}(id-{id(self)}) : {self.__dict__} >"
+
+    __repr__ = __str__
+
+    def __iter__(self):
+        yield from self.__dict__
+
+    def keys(self):
+        yield from self.__dict__
+
+    def values(self):
+        yield from self.__dict__.values()
+
+    def update(self, config: MutableMapping = None, **kwargs):
+        """批量更新字典"""
+        config = config or kwargs
+        for k, v in config.items():
+            self.__dict__[k] = _to_vxdict(v)
+
+    def items(self):
+        """(key,value) pairs"""
+        yield from self.__dict__.items()
+
+    def pop(self, key: str, default_: Any = None) -> Any:
+        """弹出key对应的value，若无此数据，则返回default_"""
+        return self.__dict__.pop(key, default_)
+
+    def clear(self) -> None:
+        """清空context"""
+        self.__dict__ = {}
+
+    @staticmethod
+    def load_json(json_file, default_config=None) -> None:
+        """加载json file
+
+        Arguments:
+            json_file {_type_} -- 加载的json file
+
+        Raises:
+            OSError: 文件不存在
+        """
+
+        json_file = Path(json_file)
+        if not json_file.exists():
+            raise OSError(f"json_file({json_file.as_posix()}) is not exists.")
+
+        with open(json_file.as_posix(), "r", encoding="utf-8") as fp:
+            config = json.load(fp)
+
+        return vxDict(default_config, **config)
+
+    def save_json(self, json_file: str) -> None:
+        """保存json file
+
+        Arguments:
+            json_file {str} -- 待保存的json file
+
+        """
+        with open(json_file, "w", encoding="utf-8") as fp:
+            json.dump(self, fp, indent=4, cls=vxJSONEncoder)
+
+
+@singledispatch
+def _to_vxdict(self: Any):
+    """转换为vxdict obj"""
+    return self
+
+
+@_to_vxdict.register(MutableMapping)
+def _(obj: MutableMapping) -> vxDict:
+    return vxDict(**obj)
+
+
+@_to_vxdict.register(Sequence)
+def _(obj: Sequence) -> List:
+    return obj if isinstance(obj, str) else [_to_vxdict(o_) for o_ in obj]
+
+
+@vxJSONEncoder.register(vxDict)
+def _(obj):
+    return dict(obj.items())
+
+
+MutableMapping.register(vxDict)
+Mapping.register(vxDataClass)
```

### Comparing `vxquant-2023.3.1/src/vxutils/debug.py` & `vxquant-2023.4.1/src/vxutils/debug.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# encoding=utf-8
-"""
-author : vex1023
-email :  vex1023@qq.com
-
-@debug_log
-def func(*args, **kwargs):
-    pass
-    
-"""
-
-
-import time
-import inspect
-from functools import wraps
-from typing import Any
-
-
-def debug_log(func) -> Any:
-    from vxutils import vxLogging
-
-    # 创建日志器
-    _logger = vxLogging.getLogger("__DEBUG__")
-    # 获取函数参数信息
-    sig = inspect.signature(func)
-
-    @wraps(func)
-    def debug_func(*args, **kwargs):
-        # 计算函数的参数
-        ba = sig.bind(*args, **kwargs)
-        ba.apply_defaults()
-
-        # 记录函数开始执行时间
-        start = time.perf_counter()
-
-        try:
-            # 执行函数，并记录返回值
-            ret = func(*args, **kwargs)
-        except Exception as e:
-            # 如果函数执行出错，记录异常信息
-            ret = e
-            raise
-        finally:
-            # 记录函数执行结束时间
-            end = time.perf_counter()
-
-            # 输出函数调用信息
-            if isinstance(ret, Exception):
-                _logger.error(
-                    f"func:{func.__name__}({ba.arguments}) 调用出错: {ret}", exc_info=True
-                )
-            else:
-                _logger.warning(
-                    f"func:{func.__name__}({ba.arguments}) 耗时: {(end-start)*1000:.2f}ms"
-                    f" 返回值: {ret}"
-                )
-
-            return ret
-
-    return debug_func
+# encoding=utf-8
+"""
+author : vex1023
+email :  vex1023@qq.com
+
+@debug_log
+def func(*args, **kwargs):
+    pass
+    
+"""
+
+
+import time
+import inspect
+from functools import wraps
+from typing import Any
+
+
+def debug_log(func) -> Any:
+    from vxutils import vxLogging
+
+    # 创建日志器
+    _logger = vxLogging.getLogger("__DEBUG__")
+    # 获取函数参数信息
+    sig = inspect.signature(func)
+
+    @wraps(func)
+    def debug_func(*args, **kwargs):
+        # 计算函数的参数
+        ba = sig.bind(*args, **kwargs)
+        ba.apply_defaults()
+
+        # 记录函数开始执行时间
+        start = time.perf_counter()
+
+        try:
+            # 执行函数，并记录返回值
+            ret = func(*args, **kwargs)
+        except Exception as e:
+            # 如果函数执行出错，记录异常信息
+            ret = e
+            raise
+        finally:
+            # 记录函数执行结束时间
+            end = time.perf_counter()
+
+            # 输出函数调用信息
+            if isinstance(ret, Exception):
+                _logger.error(
+                    f"func:{func.__name__}({ba.arguments}) 调用出错: {ret}", exc_info=True
+                )
+            else:
+                _logger.warning(
+                    f"func:{func.__name__}({ba.arguments}) 耗时: {(end-start)*1000:.2f}ms"
+                    f" 返回值: {ret}"
+                )
+
+            return ret
+
+    return debug_func
```

### Comparing `vxquant-2023.3.1/src/vxutils/decorators.py` & `vxquant-2023.4.1/src/vxutils/decorators.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-# endcoding = utf-8
-"""
-author : vex1023
-email :  vex1023@qq.com
-各类型的decorator
-"""
-
-
-import signal
-import time
-
-from typing import Any
-from collections import defaultdict
-from multiprocessing.pool import ThreadPool
-from multiprocessing import Lock
-from functools import wraps
-
-
-__all__ = [
-    "retry",
-    "timeit",
-    "singleton",
-    "threads",
-    "lazy_property",
-    "timeout",
-    "storage",
-]
-
-
-###################################
-# 错误重试方法实现
-# @retry(tries, CatchExceptions=(Exception,), delay=0.01, backoff=2)
-###################################
-
-
-def retry(tries, CatchExceptions=(Exception,), delay=0.1, backoff=2):
-    """
-    错误重试的修饰器
-    :param tries: 重试次数
-    :param CatchExceptions: 需要重试的exception列表
-    :param delay: 重试前等待
-    :param backoff: 重试n次后，需要等待delay * n * backoff
-    :return:
-    @retry(5,ValueError)
-    def test():
-        raise ValueError
-    """
-    if backoff <= 1:
-        raise ValueError("backoff must be greater than 1")
-
-    if tries < 0:
-        raise ValueError("tries must be 0 or greater")
-
-    if delay <= 0:
-        raise ValueError("delay must be greater than 0")
-
-    if not isinstance(CatchExceptions, (tuple, list)):
-        CatchExceptions = [CatchExceptions]
-
-    def deco_retry(f):
-        @wraps(f)
-        def f_retry(*args, **kwargs):
-            mdelay = delay
-            for i in range(1, tries):
-                try:
-                    return f(*args, **kwargs)
-                except CatchExceptions as ex:
-                    from vxutils import logger
-
-                    logger.error(
-                        f"function {f.__name__}({args}, {kwargs}) try {i} times"
-                        f" error: {str(ex)}\n"
-                    )
-                    logger.warning("Retrying in {mdelay:.4f} seconds...")
-
-                    time.sleep(mdelay)
-                    mdelay *= backoff
-
-            return f(*args, **kwargs)
-
-        return f_retry
-
-    return deco_retry
-
-
-###################################
-# 计算运行消耗时间
-# @timeit
-###################################
-
-
-def timeit(func):
-    """
-    计算运行消耗时间
-    @timeit
-    def test():
-        time.sleep(1)
-    """
-
-    def wapper(*args, **kwargs):
-        _start = time.time()
-        retval = func(*args, **kwargs)
-        _end = time.time()
-        print(f"function {func.__name__}() used : {(_end - _start):.6f)}s")
-        return retval
-
-    return wapper
-
-
-###################################
-# Singleton 实现
-# @singleton
-###################################
-
-
-class singleton(object):
-    """
-    单例
-    example::
-
-        @singleton
-        class YourClass(object):
-            def __init__(self, *args, **kwargs):
-                pass
-    """
-
-    def __init__(self, cls):
-        self._instance = None
-        self._cls = cls
-        self._lock = Lock()
-
-    def __call__(self, *args, **kwargs):
-        if self._instance is None:
-            with self._lock:
-                if self._instance is None:
-                    self._instance = self._cls(*args, **kwargs)
-        return self._instance
-
-
-###################################
-# 异步多线程
-# @thread(n,timeout=None)
-###################################
-
-
-class asyncResult:
-    """异步返回结果"""
-
-    def __init__(self, future, timeout_time):
-        self._future = future
-        self._timeout = timeout_time
-        self._result = None
-
-    def __getattr__(self, name):
-        return getattr(self.result, name)
-
-    @property
-    def result(self):
-        """获取异步返回结果
-
-        Returns:
-            返回计算结果
-        """
-        if self._result is None:
-            self._result = self._future.get(self._timeout)
-        return self._result
-
-
-def threads(n, time_limit=5):
-    """多线程装饰器
-    @thread(n,timeout=None)
-    def handler(*args, **kwargs):
-        pass
-
-    rets = map(handler , iterable)
-    for ret in rets:
-        print(ret.get())
-    """
-
-    def decorator(f):
-        pool = ThreadPool(n)
-
-        @wraps(f)
-        def warpped(*args, **kwargs):
-            return asyncResult(
-                pool.apply_async(func=f, args=args, kwds=kwargs), time_limit
-            )
-
-        return warpped
-
-    return decorator
-
-
-###################################
-# 限制超时时间
-# @timeout(seconds, error_message='Function call timed out')
-###################################
-
-
-def timeout(seconds, error_message="Function call timed out"):
-    """超时限制装饰器
-
-    Arguments:
-        seconds -- 超时秒数
-
-    Keyword Arguments:
-        error_message -- 超时返回信息 (default: {"Function call timed out"})
-    """
-
-    def decorated(func):
-        def _handle_timeout(signum, frame):
-            raise TimeoutError(
-                f"{error_message} after {seconds} seconds,{signum},{frame}"
-            )
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            signal.signal(signal.SIGALRM, _handle_timeout)
-            signal.alarm(seconds)
-            try:
-                result = func(*args, **kwargs)
-            finally:
-                signal.alarm(0)
-            return result
-
-        return wrapper
-
-    return decorated
-
-
-###################################
-# 类似@property的功能，但只执行一次
-# @lazy_property
-###################################
-
-
-class lazy_property(object):
-    """类似@property的功能，但只执行一次"""
-
-    def __init__(self, deferred):
-        self._deferred = deferred
-        self.__doc__ = deferred.__doc__
-
-    def __get__(self, obj, cls):
-        if obj is None:
-            return self
-        value = self._deferred(obj)
-        setattr(obj, self._deferred.__name__, value)
-        return value
-
-
-###################################
-# 存储器 ---- 用于收集，整理各种元素
-# @storage(type_name, element_name)
-#
-###################################
-
-
-class storage:
-    """采集器，负责收集零散在各处的元素
-
-    storage("hello", "jack","hi")
-    storage("hello", "vex1023","hi")
-    ------------------------------------
-    @storage("parser","sina"):
-    def sina_parser(content):
-        print("sina_parser",content)
-
-    @storage("parser","qq"):
-    def qq_parser(content):
-        print("qq_parser",content)
-
-    parser = storage.get("parser",'sina')
-    parser()
-
-    """
-
-    __elements = defaultdict(dict)
-
-    def __init__(self, type_name: str, element_name: str, element: Any = None) -> None:
-        self._type_name = type_name
-        self._element_name = element_name
-        self.__call__(element)
-
-    def __call__(self, element: Any) -> Any:
-        self.__class__.__elements[self._type_name][self._element_name] = element
-        return element
-
-    @classmethod
-    def get(cls, type_name: str, element_name: str) -> Any:
-        return cls.__elements[type_name][element_name]
+# endcoding = utf-8
+"""
+author : vex1023
+email :  vex1023@qq.com
+各类型的decorator
+"""
+
+
+import signal
+import time
+
+from typing import Any
+from collections import defaultdict
+from multiprocessing.pool import ThreadPool
+from multiprocessing import Lock
+from functools import wraps
+
+
+__all__ = [
+    "retry",
+    "timeit",
+    "singleton",
+    "threads",
+    "lazy_property",
+    "timeout",
+    "storage",
+]
+
+
+###################################
+# 错误重试方法实现
+# @retry(tries, CatchExceptions=(Exception,), delay=0.01, backoff=2)
+###################################
+
+
+def retry(tries, CatchExceptions=(Exception,), delay=0.1, backoff=2):
+    """
+    错误重试的修饰器
+    :param tries: 重试次数
+    :param CatchExceptions: 需要重试的exception列表
+    :param delay: 重试前等待
+    :param backoff: 重试n次后，需要等待delay * n * backoff
+    :return:
+    @retry(5,ValueError)
+    def test():
+        raise ValueError
+    """
+    if backoff <= 1:
+        raise ValueError("backoff must be greater than 1")
+
+    if tries < 0:
+        raise ValueError("tries must be 0 or greater")
+
+    if delay <= 0:
+        raise ValueError("delay must be greater than 0")
+
+    if not isinstance(CatchExceptions, (tuple, list)):
+        CatchExceptions = [CatchExceptions]
+
+    def deco_retry(f):
+        @wraps(f)
+        def f_retry(*args, **kwargs):
+            mdelay = delay
+            for i in range(1, tries):
+                try:
+                    return f(*args, **kwargs)
+                except CatchExceptions as ex:
+                    from vxutils import logger
+
+                    logger.error(
+                        f"function {f.__name__}({args}, {kwargs}) try {i} times"
+                        f" error: {str(ex)}\n"
+                    )
+                    logger.warning("Retrying in {mdelay:.4f} seconds...")
+
+                    time.sleep(mdelay)
+                    mdelay *= backoff
+
+            return f(*args, **kwargs)
+
+        return f_retry
+
+    return deco_retry
+
+
+###################################
+# 计算运行消耗时间
+# @timeit
+###################################
+
+
+def timeit(func):
+    """
+    计算运行消耗时间
+    @timeit
+    def test():
+        time.sleep(1)
+    """
+
+    def wapper(*args, **kwargs):
+        _start = time.time()
+        retval = func(*args, **kwargs)
+        _end = time.time()
+        print(f"function {func.__name__}() used : {(_end - _start):.6f)}s")
+        return retval
+
+    return wapper
+
+
+###################################
+# Singleton 实现
+# @singleton
+###################################
+
+
+class singleton(object):
+    """
+    单例
+    example::
+
+        @singleton
+        class YourClass(object):
+            def __init__(self, *args, **kwargs):
+                pass
+    """
+
+    def __init__(self, cls):
+        self._instance = None
+        self._cls = cls
+        self._lock = Lock()
+
+    def __call__(self, *args, **kwargs):
+        if self._instance is None:
+            with self._lock:
+                if self._instance is None:
+                    self._instance = self._cls(*args, **kwargs)
+        return self._instance
+
+
+###################################
+# 异步多线程
+# @thread(n,timeout=None)
+###################################
+
+
+class asyncResult:
+    """异步返回结果"""
+
+    def __init__(self, future, timeout_time):
+        self._future = future
+        self._timeout = timeout_time
+        self._result = None
+
+    def __getattr__(self, name):
+        return getattr(self.result, name)
+
+    @property
+    def result(self):
+        """获取异步返回结果
+
+        Returns:
+            返回计算结果
+        """
+        if self._result is None:
+            self._result = self._future.get(self._timeout)
+        return self._result
+
+
+def threads(n, time_limit=5):
+    """多线程装饰器
+    @thread(n,timeout=None)
+    def handler(*args, **kwargs):
+        pass
+
+    rets = map(handler , iterable)
+    for ret in rets:
+        print(ret.get())
+    """
+
+    def decorator(f):
+        pool = ThreadPool(n)
+
+        @wraps(f)
+        def warpped(*args, **kwargs):
+            return asyncResult(
+                pool.apply_async(func=f, args=args, kwds=kwargs), time_limit
+            )
+
+        return warpped
+
+    return decorator
+
+
+###################################
+# 限制超时时间
+# @timeout(seconds, error_message='Function call timed out')
+###################################
+
+
+def timeout(seconds, error_message="Function call timed out"):
+    """超时限制装饰器
+
+    Arguments:
+        seconds -- 超时秒数
+
+    Keyword Arguments:
+        error_message -- 超时返回信息 (default: {"Function call timed out"})
+    """
+
+    def decorated(func):
+        def _handle_timeout(signum, frame):
+            raise TimeoutError(
+                f"{error_message} after {seconds} seconds,{signum},{frame}"
+            )
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            signal.signal(signal.SIGALRM, _handle_timeout)
+            signal.alarm(seconds)
+            try:
+                result = func(*args, **kwargs)
+            finally:
+                signal.alarm(0)
+            return result
+
+        return wrapper
+
+    return decorated
+
+
+###################################
+# 类似@property的功能，但只执行一次
+# @lazy_property
+###################################
+
+
+class lazy_property(object):
+    """类似@property的功能，但只执行一次"""
+
+    def __init__(self, deferred):
+        self._deferred = deferred
+        self.__doc__ = deferred.__doc__
+
+    def __get__(self, obj, cls):
+        if obj is None:
+            return self
+        value = self._deferred(obj)
+        setattr(obj, self._deferred.__name__, value)
+        return value
+
+
+###################################
+# 存储器 ---- 用于收集，整理各种元素
+# @storage(type_name, element_name)
+#
+###################################
+
+
+class storage:
+    """采集器，负责收集零散在各处的元素
+
+    storage("hello", "jack","hi")
+    storage("hello", "vex1023","hi")
+    ------------------------------------
+    @storage("parser","sina"):
+    def sina_parser(content):
+        print("sina_parser",content)
+
+    @storage("parser","qq"):
+    def qq_parser(content):
+        print("qq_parser",content)
+
+    parser = storage.get("parser",'sina')
+    parser()
+
+    """
+
+    __elements = defaultdict(dict)
+
+    def __init__(self, type_name: str, element_name: str, element: Any = None) -> None:
+        self._type_name = type_name
+        self._element_name = element_name
+        self.__call__(element)
+
+    def __call__(self, element: Any) -> Any:
+        self.__class__.__elements[self._type_name][self._element_name] = element
+        return element
+
+    @classmethod
+    def get(cls, type_name: str, element_name: str) -> Any:
+        return cls.__elements[type_name][element_name]
```

### Comparing `vxquant-2023.3.1/src/vxutils/log.py` & `vxquant-2023.4.1/src/vxutils/log.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-#!encoding=utf-8
-"""
-author: vex1023
-email: vex1023@qq.com
-回测用的logger，方便观察回测中的日志
-"""
-
-
-import pathlib
-import sys
-import logging
-import logging.handlers
-
-
-__all__ = ["vxLoggerFactory"]
-
-__DEFAULT_LOG_FORMAT__ = (
-    "%(asctime)s [%(process)s:%(threadName)s - %(funcName)s@%(filename)s:%(lineno)d]"
-    " %(levelname)s === %(message)s"
-)
-
-
-class vxLoggerFactory:
-    def __init__(self, root="", level=logging.INFO, log_dir="log/"):
-        """
-        :param root_name: 基础logger的名称，默认为__vxQuant__
-        :param log_dir: log文件的存放目录，默认为当前目录
-        :param log_level: log的级别，默认为INFO
-        """
-        self._root = root
-        self._root_level = level
-        self._log_dir = log_dir
-        self._formatter = logging.Formatter(__DEFAULT_LOG_FORMAT__)
-        self._log_dir = pathlib.Path(log_dir)
-        self._log_dir.mkdir(parents=True, exist_ok=True)
-        self.reset()
-
-    def _add_filehandler(self, logger, filename, level=None):
-        if self._log_dir is None:
-            logger.warning(f"{self.__class__.__name__} 未设置log dir.")
-            return
-
-        level = level or logging.INFO
-
-        filename = self._log_dir.joinpath(filename).as_posix()
-
-        filehandler = logging.handlers.TimedRotatingFileHandler(
-            filename, when="D", backupCount=20, encoding="utf8"
-        )
-
-        filehandler.setFormatter(self._formatter)
-        filehandler.setLevel(self._root_level)
-        logger.addHandler(filehandler)
-
-    def getLogger(self, logger_name="", level=logging.INFO, filename=""):
-        """获取一个logger的实例
-
-        Keyword Arguments:
-            logger_name -- _description_ (default: {""})
-            level -- _description_ (default: {logging.INFO})
-            filename -- _description_ (default: {""})
-
-        Returns:
-            _description_
-        """
-        if not logger_name:
-            return logging.getLogger(self._root)
-
-        logger_name = f"{self._root}.{logger_name}"
-        logger = logging.getLogger(logger_name)
-        for handler in logger.handlers:
-            logger.removeHandler(handler)
-            logger.debug(f"移除 log handler: {handler}")
-
-        logger.setLevel(level)
-        if filename and self._log_dir:
-            self._add_filehandler(logger, filename, logging.DEBUG)
-        return logger
-
-    def reset(self):
-        logger = logging.getLogger(self._root)
-        logger.setLevel(self._root_level)
-        has_console = False
-        has_filehandler = False
-        for handler in logger.handlers:
-            if isinstance(handler, logging.StreamHandler):
-                handler.setLevel(logging.DEBUG)
-                handler.setFormatter(self._formatter)
-                has_console = True
-            elif isinstance(handler, logging.handlers.TimedRotatingFileHandler):
-                has_filehandler = True
-
-        if has_console is False:
-            console = logging.StreamHandler(sys.stdout)
-            console.setFormatter(self._formatter)
-            console.setLevel(logging.DEBUG)
-            logger.addHandler(console)
-
-        if self._log_dir and has_filehandler is False:
-            self._add_filehandler(logger, "vxquant.log", logging.DEBUG)
-
-        logger.debug("logger 初始化完成.")
+#!encoding=utf-8
+"""
+author: vex1023
+email: vex1023@qq.com
+回测用的logger，方便观察回测中的日志
+"""
+
+
+import pathlib
+import sys
+import logging
+import logging.handlers
+
+
+__all__ = ["vxLoggerFactory"]
+
+__DEFAULT_LOG_FORMAT__ = (
+    "%(asctime)s [%(process)s:%(threadName)s - %(funcName)s@%(filename)s:%(lineno)d]"
+    " %(levelname)s === %(message)s"
+)
+
+
+class vxLoggerFactory:
+    def __init__(self, root="", level=logging.INFO, log_dir="log/"):
+        """
+        :param root_name: 基础logger的名称，默认为__vxQuant__
+        :param log_dir: log文件的存放目录，默认为当前目录
+        :param log_level: log的级别，默认为INFO
+        """
+        self._root = root
+        self._root_level = level
+        self._log_dir = log_dir
+        self._formatter = logging.Formatter(__DEFAULT_LOG_FORMAT__)
+        self._log_dir = pathlib.Path(log_dir)
+        self._log_dir.mkdir(parents=True, exist_ok=True)
+        self.reset()
+
+    def _add_filehandler(self, logger, filename, level=None):
+        if self._log_dir is None:
+            logger.warning(f"{self.__class__.__name__} 未设置log dir.")
+            return
+
+        level = level or logging.INFO
+
+        filename = self._log_dir.joinpath(filename).as_posix()
+
+        filehandler = logging.handlers.TimedRotatingFileHandler(
+            filename, when="D", backupCount=20, encoding="utf8"
+        )
+
+        filehandler.setFormatter(self._formatter)
+        filehandler.setLevel(self._root_level)
+        logger.addHandler(filehandler)
+
+    def getLogger(self, logger_name="", level=logging.INFO, filename=""):
+        """获取一个logger的实例
+
+        Keyword Arguments:
+            logger_name -- _description_ (default: {""})
+            level -- _description_ (default: {logging.INFO})
+            filename -- _description_ (default: {""})
+
+        Returns:
+            _description_
+        """
+        if not logger_name:
+            return logging.getLogger(self._root)
+
+        logger_name = f"{self._root}.{logger_name}"
+        logger = logging.getLogger(logger_name)
+        for handler in logger.handlers:
+            logger.removeHandler(handler)
+            logger.debug(f"移除 log handler: {handler}")
+
+        logger.setLevel(level)
+        if filename and self._log_dir:
+            self._add_filehandler(logger, filename, logging.DEBUG)
+        return logger
+
+    def reset(self):
+        logger = logging.getLogger(self._root)
+        logger.setLevel(self._root_level)
+        has_console = False
+        has_filehandler = False
+        for handler in logger.handlers:
+            if isinstance(handler, logging.StreamHandler):
+                handler.setLevel(logging.DEBUG)
+                handler.setFormatter(self._formatter)
+                has_console = True
+            elif isinstance(handler, logging.handlers.TimedRotatingFileHandler):
+                has_filehandler = True
+
+        if has_console is False:
+            console = logging.StreamHandler(sys.stdout)
+            console.setFormatter(self._formatter)
+            console.setLevel(logging.DEBUG)
+            logger.addHandler(console)
+
+        if self._log_dir and has_filehandler is False:
+            self._add_filehandler(logger, "vxquant.log", logging.DEBUG)
+
+        logger.debug("logger 初始化完成.")
```

### Comparing `vxquant-2023.3.1/src/vxutils/zmqsocket.py` & `vxquant-2023.4.1/src/vxutils/zmqsocket.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,383 +1,383 @@
-"""zeromq 相关函数"""
-
-import os
-import zmq
-import secrets
-import pickle
-import asyncio
-import pathlib
-import contextlib
-from zmq.auth import CURVE_ALLOW_ANY
-from zmq.auth.thread import ThreadAuthenticator
-from zmq.asyncio import Context as AsyncContext
-from zmq.asyncio import Socket as AsyncSocket
-from zmq.auth.asyncio import AsyncioAuthenticator
-from queue import Empty, Queue
-from multiprocessing import Lock
-from multiprocessing.dummy import Process
-from typing import Callable
-from vxutils import (
-    logger,
-    to_binary,
-)
-
-__all__ = [
-    "vxZMQContext",
-    "vxSecSocket",
-    "vxAsyncSecSocket",
-    "vxAsyncZMQContext",
-    "vxZMQRequest",
-    "vxAsyncServer",
-    "vxZMQBackendThread",
-]
-
-
-class vxZMQAuthenticator:
-    _auth_thread = None
-    _auth_async = None
-
-    def __init__(self, zsocket):
-        """启动加密线程
-
-        Arguments:
-            zsocket {socket} -- zmq的socket
-
-
-        Raises:
-            FileNotFoundError: 密钥文件不存在
-        """
-
-    @classmethod
-    def start_auth(cls, is_async=False):
-        if cls._auth_thread is None and is_async is False:
-            cls._auth_thread = ThreadAuthenticator()
-            cls._auth_thread.start()
-            cls._auth_thread.configure_curve(domain="*", location=CURVE_ALLOW_ANY)
-            cls._auth_thread.allow()
-
-        elif cls._auth_async is None and is_async is True:
-            cls._auth_async = AsyncioAuthenticator()
-            cls._auth_async.start()
-            cls._auth_async.configure_curve(domain="*", location=CURVE_ALLOW_ANY)
-            cls._auth_async.allow()
-
-
-class vxSecSocket(zmq.Socket):
-    """构建加密的ZMQ socket链接工具集合"""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.__dict__["_lock"] = None
-
-    @property
-    def lock(self):
-        """锁"""
-        if self._lock is None:
-            self.__dict__["_lock"] = Lock()
-        return self.__dict__["_lock"]
-
-    def bind(self, addr: str, secret_key: str = ""):
-        if secret_key and pathlib.Path(secret_key).is_file():
-            vxZMQAuthenticator.start_auth(is_async=False)
-            public_keystr, secret_keystr = zmq.auth.load_certificate(secret_key)
-            self.curve_publickey = public_keystr
-            self.curve_secretkey = secret_keystr
-            self.curve_server = True
-            logger.info(f"启动加密模式, server public key: {public_keystr}.")
-        logger.info(f"绑定 {addr} 完成.")
-        return super().bind(addr)
-
-    def connect(self, addr: str = "", public_key: str = ""):
-        """创建连接服务器socket
-
-        Keyword Arguments:
-            addr {str} -- 服务器地址 (default: {""})
-            public_key {str} -- 服务器公钥 (default: {""})
-
-        """
-        if zmq.zmq_version_info() < (4, 0):
-            logger.warning(
-                "Security is not supported in libzmq version < 4.0. libzmq version"
-                f" {zmq.zmq_version()}"
-            )
-            public_key = None
-
-        if public_key and os.path.exists(public_key):
-            server_public, _ = zmq.auth.load_certificate(public_key)
-            self.curve_serverkey = server_public
-            self.curve_publickey, self.curve_secretkey = zmq.curve_keypair()
-            logger.info(f"启动加密模式,public server public key: {server_public}.")
-
-        ret = super().connect(addr)
-        logger.info(f"connect to {addr} ...")
-        return ret
-
-
-class vxZMQContext(zmq.Context):
-    """ZMQ context"""
-
-    _socket_class = vxSecSocket
-
-
-class vxAsyncSecSocket(AsyncSocket):
-    """构建加密的ZMQ socket链接工具集合"""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.__dict__["secret_mode"] = False
-        self.__dict__["_lock"] = None
-
-    def lock(self):
-        """锁"""
-        return self._lock
-
-    def bind(self, addr: str, secret_key: str = ""):
-        """绑定地址"""
-        if secret_key and pathlib.Path(secret_key).is_file():
-            vxZMQAuthenticator.start_auth(is_async=True)
-            public_keystr, secret_keystr = zmq.auth.load_certificate(secret_key)
-            self.curve_publickey = public_keystr
-            self.curve_secretkey = secret_keystr
-            self.curve_server = True
-            self.__dict__["secret_mode"] = True
-            logger.info(f"启动加密模式,secret key文件: {secret_key}.")
-
-        logger.info(f"绑定 {addr} 完成.")
-        return super().bind(addr)
-
-    def connect(self, addr: str = "", public_key: str = ""):
-        """创建连接服务器socket
-
-        Keyword Arguments:
-            addr {str} -- 服务器地址 (default: {""})
-            public_key {str} -- 服务器公钥 (default: {""})
-
-        """
-        if zmq.zmq_version_info() < (4, 0):
-            logger.warning(
-                "Security is not supported in libzmq version < 4.0. libzmq version"
-                f" {zmq.zmq_version()}"
-            )
-            public_key = None
-
-        if public_key and os.path.exists(public_key):
-            server_public, _ = zmq.auth.load_certificate(public_key)
-            self.curve_serverkey = server_public
-            self.curve_publickey, self.curve_secretkey = zmq.curve_keypair()
-            logger.info(f"启动加密模式,server public key文件: {public_key}.")
-
-        logger.info(f"链接 {addr} 完成.")
-        return super().connect(addr)
-
-
-class vxAsyncZMQContext(AsyncContext):
-    """ZMQ context"""
-
-    _socket_class = vxAsyncSecSocket
-
-
-class vxZMQRequest:
-    def __init__(
-        self,
-        url: str,
-        public_key: str,
-        serializer=None,
-        deserializer=None,
-        clientid=None,
-    ) -> None:
-        self._url = url
-        self._public_key = public_key
-        self._ctx = None
-        self._socket = None
-        self._serializer = serializer if callable(serializer) else pickle.dumps
-        self._deserializer = deserializer if callable(deserializer) else pickle.loads
-        self._clientid = (
-            to_binary(clientid) if clientid is not None else secrets.token_bytes(16)
-        )
-
-    @property
-    def socket(self):
-        if self._socket is None:
-            self._ctx = vxZMQContext()
-            self._socket = self._ctx.socket(zmq.REQ)
-            self._socket.setsockopt(zmq.IDENTITY, self._clientid)
-            self._socket.connect(self._url, self._public_key)
-
-        return self._socket
-
-    def reset(self) -> None:
-        """重置连接"""
-        if self._socket:
-            with self._socket.lock:
-                self._socket.setsockopt(zmq.LINGER, 0)
-                self._socket.close()
-                self._ctx.destroy(0)
-
-        self._ctx = None
-        self._socket = None
-
-    def __str__(self) -> str:
-        return f"< {self.__class__.__name__} (id-{id(self)}) connect to {self._url}."
-
-    def __call__(self, obj):
-        with self.socket.lock:
-            packed_obj = self._serializer(obj)
-            self.socket.send(packed_obj)
-            flags = self.socket.poll(3000, zmq.POLLIN)
-            if flags & zmq.POLLIN == 0:
-                raise TimeoutError("连接超时")
-
-            packed_obj = self.socket.recv()
-            return self._deserializer(packed_obj)
-
-
-class vxAsyncServer:
-    def __init__(
-        self, socket_type, url, secret_key=None, send_queue=None, bind_mode=True
-    ):
-        self._ctx = vxAsyncZMQContext().instance()
-        self._socket = self._ctx.socket(socket_type)
-        if bind_mode:
-            self._socket.bind(url, secret_key)
-        else:
-            self._socket.connect(url, secret_key)
-        self._active = False
-        self._queue = send_queue if send_queue is None else Queue()
-
-    @property
-    def socket(self):
-        """socket"""
-        return self._socket
-
-    async def receiver(self, callback) -> None:
-        """接收进程
-
-        Arguments:
-            callback {Callable} -- 回调函数
-        """
-        while self._active:
-            flags = await self._socket.poll(zmq.POLLIN)
-            if flags & zmq.POLLIN != 0:
-                msg = await self._socket.recv_multipart()
-                callback(msg)
-
-    async def sender(self, serializer=None) -> None:
-        """发送
-
-        Arguments:
-            serializer {callable} -- 序列化函数
-        """
-        while self._active:
-            try:
-                msg = self._queue.get_nowait()
-                print(msg)
-
-                if (not isinstance(msg, bytes)) and serializer:
-                    msg = serializer(msg)
-
-                await self._socket.send(msg)
-            except Empty:
-                await asyncio.sleep(0.5)
-
-    async def run(self, callback: callable, serializer: callable) -> None:
-        wait_tasks = []
-        if callable(callback):
-            wait_tasks.append(self.receiver(callback))
-
-        wait_tasks.append(self.sender(serializer))
-
-        if not wait_tasks:
-            logger.warning("callback and msg_queue 不满足条件")
-
-        self._active = True
-        logger.info(f"开始运行 {self}")
-        await asyncio.gather(*wait_tasks)
-        self._active = False
-        logger.info(f"开始结束 {self}")
-
-    def send(self, msg) -> None:
-        self._queue.put(msg)
-
-
-class vxZMQBackendThread(Process):
-    def __init__(
-        self, on_send_callback: Callable = None, on_recv_callback: Callable = None
-    ) -> None:
-        self._zmqctx = None
-        self._socket = None
-        self._active = False
-        self._queue = Queue()
-        self._on_send_callback = on_send_callback
-        self._on_recv_callback = on_recv_callback
-
-        super().__init__()
-        name = self.getName()
-        self.setName(name.replace("Thread", self.__class__.__name__))
-
-    def set_on_send_callback(self, callback: Callable = None) -> None:
-        self._on_send_callback = callback
-
-    def set_on_recv_callback(self, callback: Callable = None) -> None:
-        self._on_recv_callback = callback
-
-    def send(self, *msgs) -> None:
-        """发送消息"""
-        self._queue.put(msgs)
-
-    def bind(self, socket_type, addr: str, secret_key: str = ""):
-        if self._active is True:
-            return
-        self._active = True
-        self._zmqctx = vxZMQContext().instance()
-        self._socket = self._zmqctx.socket(socket_type)
-        self._socket.bind(addr, secret_key)
-        return self
-
-    def connect(self, socket_type, addr: str, public_key: str = ""):
-        if self._active is True:
-            return
-        self._active = True
-        self._zmqctx = vxZMQContext().instance()
-        self._socket = self._zmqctx.socket(socket_type)
-        self._socket.connect(addr, public_key)
-
-    def run(self) -> None:
-        if self._active is False:
-            logger.info("请先调用 activate(url, public_key=None)进行初始化操作. 后运行")
-            return
-
-        logger.info(f"{self.name} (id-{id(self)}) 启动运行...")
-
-        try:
-            while self._active:
-                flags = self._socket.poll(1000, zmq.POLLIN | zmq.POLLOUT)
-
-                if self._on_recv_callback and flags & zmq.POLLIN != 0:
-                    msgs = self._socket.recv_multipart()
-                    logger.debug(f"recive msgs: {msgs}")
-                    self._on_recv_callback(self, *msgs)
-
-                if flags & zmq.POLLOUT != 0:
-                    with contextlib.suppress(Empty):
-                        msgs = self._queue.get(timeout=0.1)
-                        if self._on_send_callback:
-                            msgs = self._on_send_callback(self, *msgs)
-                        self._socket.send_multipart(list(map(to_binary, msgs)))
-        finally:
-            logger.info(f"{self.name} (id-{id(self)}) 停止运行...")
-            self.stop()
-
-    def close(self) -> None:
-        if self._active is False:
-            return
-        self.stop()
-
-    def stop(self) -> None:
-        self._active = False
-        # self.join()
-        if self._socket:
-            self._socket.setsockopt(zmq.LINGER, 0)
-            self._socket.close()
-            self._socket = None
-            self._zmqctx = None
+"""zeromq 相关函数"""
+
+import os
+import zmq
+import secrets
+import pickle
+import asyncio
+import pathlib
+import contextlib
+from zmq.auth import CURVE_ALLOW_ANY
+from zmq.auth.thread import ThreadAuthenticator
+from zmq.asyncio import Context as AsyncContext
+from zmq.asyncio import Socket as AsyncSocket
+from zmq.auth.asyncio import AsyncioAuthenticator
+from queue import Empty, Queue
+from multiprocessing import Lock
+from multiprocessing.dummy import Process
+from typing import Callable
+from vxutils import (
+    logger,
+    to_binary,
+)
+
+__all__ = [
+    "vxZMQContext",
+    "vxSecSocket",
+    "vxAsyncSecSocket",
+    "vxAsyncZMQContext",
+    "vxZMQRequest",
+    "vxAsyncServer",
+    "vxZMQBackendThread",
+]
+
+
+class vxZMQAuthenticator:
+    _auth_thread = None
+    _auth_async = None
+
+    def __init__(self, zsocket):
+        """启动加密线程
+
+        Arguments:
+            zsocket {socket} -- zmq的socket
+
+
+        Raises:
+            FileNotFoundError: 密钥文件不存在
+        """
+
+    @classmethod
+    def start_auth(cls, is_async=False):
+        if cls._auth_thread is None and is_async is False:
+            cls._auth_thread = ThreadAuthenticator()
+            cls._auth_thread.start()
+            cls._auth_thread.configure_curve(domain="*", location=CURVE_ALLOW_ANY)
+            cls._auth_thread.allow()
+
+        elif cls._auth_async is None and is_async is True:
+            cls._auth_async = AsyncioAuthenticator()
+            cls._auth_async.start()
+            cls._auth_async.configure_curve(domain="*", location=CURVE_ALLOW_ANY)
+            cls._auth_async.allow()
+
+
+class vxSecSocket(zmq.Socket):
+    """构建加密的ZMQ socket链接工具集合"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.__dict__["_lock"] = None
+
+    @property
+    def lock(self):
+        """锁"""
+        if self._lock is None:
+            self.__dict__["_lock"] = Lock()
+        return self.__dict__["_lock"]
+
+    def bind(self, addr: str, secret_key: str = ""):
+        if secret_key and pathlib.Path(secret_key).is_file():
+            vxZMQAuthenticator.start_auth(is_async=False)
+            public_keystr, secret_keystr = zmq.auth.load_certificate(secret_key)
+            self.curve_publickey = public_keystr
+            self.curve_secretkey = secret_keystr
+            self.curve_server = True
+            logger.info(f"启动加密模式, server public key: {public_keystr}.")
+        logger.info(f"绑定 {addr} 完成.")
+        return super().bind(addr)
+
+    def connect(self, addr: str = "", public_key: str = ""):
+        """创建连接服务器socket
+
+        Keyword Arguments:
+            addr {str} -- 服务器地址 (default: {""})
+            public_key {str} -- 服务器公钥 (default: {""})
+
+        """
+        if zmq.zmq_version_info() < (4, 0):
+            logger.warning(
+                "Security is not supported in libzmq version < 4.0. libzmq version"
+                f" {zmq.zmq_version()}"
+            )
+            public_key = None
+
+        if public_key and os.path.exists(public_key):
+            server_public, _ = zmq.auth.load_certificate(public_key)
+            self.curve_serverkey = server_public
+            self.curve_publickey, self.curve_secretkey = zmq.curve_keypair()
+            logger.info(f"启动加密模式,public server public key: {server_public}.")
+
+        ret = super().connect(addr)
+        logger.info(f"connect to {addr} ...")
+        return ret
+
+
+class vxZMQContext(zmq.Context):
+    """ZMQ context"""
+
+    _socket_class = vxSecSocket
+
+
+class vxAsyncSecSocket(AsyncSocket):
+    """构建加密的ZMQ socket链接工具集合"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__dict__["secret_mode"] = False
+        self.__dict__["_lock"] = None
+
+    def lock(self):
+        """锁"""
+        return self._lock
+
+    def bind(self, addr: str, secret_key: str = ""):
+        """绑定地址"""
+        if secret_key and pathlib.Path(secret_key).is_file():
+            vxZMQAuthenticator.start_auth(is_async=True)
+            public_keystr, secret_keystr = zmq.auth.load_certificate(secret_key)
+            self.curve_publickey = public_keystr
+            self.curve_secretkey = secret_keystr
+            self.curve_server = True
+            self.__dict__["secret_mode"] = True
+            logger.info(f"启动加密模式,secret key文件: {secret_key}.")
+
+        logger.info(f"绑定 {addr} 完成.")
+        return super().bind(addr)
+
+    def connect(self, addr: str = "", public_key: str = ""):
+        """创建连接服务器socket
+
+        Keyword Arguments:
+            addr {str} -- 服务器地址 (default: {""})
+            public_key {str} -- 服务器公钥 (default: {""})
+
+        """
+        if zmq.zmq_version_info() < (4, 0):
+            logger.warning(
+                "Security is not supported in libzmq version < 4.0. libzmq version"
+                f" {zmq.zmq_version()}"
+            )
+            public_key = None
+
+        if public_key and os.path.exists(public_key):
+            server_public, _ = zmq.auth.load_certificate(public_key)
+            self.curve_serverkey = server_public
+            self.curve_publickey, self.curve_secretkey = zmq.curve_keypair()
+            logger.info(f"启动加密模式,server public key文件: {public_key}.")
+
+        logger.info(f"链接 {addr} 完成.")
+        return super().connect(addr)
+
+
+class vxAsyncZMQContext(AsyncContext):
+    """ZMQ context"""
+
+    _socket_class = vxAsyncSecSocket
+
+
+class vxZMQRequest:
+    def __init__(
+        self,
+        url: str,
+        public_key: str,
+        serializer=None,
+        deserializer=None,
+        clientid=None,
+    ) -> None:
+        self._url = url
+        self._public_key = public_key
+        self._ctx = None
+        self._socket = None
+        self._serializer = serializer if callable(serializer) else pickle.dumps
+        self._deserializer = deserializer if callable(deserializer) else pickle.loads
+        self._clientid = (
+            to_binary(clientid) if clientid is not None else secrets.token_bytes(16)
+        )
+
+    @property
+    def socket(self):
+        if self._socket is None:
+            self._ctx = vxZMQContext()
+            self._socket = self._ctx.socket(zmq.REQ)
+            self._socket.setsockopt(zmq.IDENTITY, self._clientid)
+            self._socket.connect(self._url, self._public_key)
+
+        return self._socket
+
+    def reset(self) -> None:
+        """重置连接"""
+        if self._socket:
+            with self._socket.lock:
+                self._socket.setsockopt(zmq.LINGER, 0)
+                self._socket.close()
+                self._ctx.destroy(0)
+
+        self._ctx = None
+        self._socket = None
+
+    def __str__(self) -> str:
+        return f"< {self.__class__.__name__} (id-{id(self)}) connect to {self._url}."
+
+    def __call__(self, obj):
+        with self.socket.lock:
+            packed_obj = self._serializer(obj)
+            self.socket.send(packed_obj)
+            flags = self.socket.poll(3000, zmq.POLLIN)
+            if flags & zmq.POLLIN == 0:
+                raise TimeoutError("连接超时")
+
+            packed_obj = self.socket.recv()
+            return self._deserializer(packed_obj)
+
+
+class vxAsyncServer:
+    def __init__(
+        self, socket_type, url, secret_key=None, send_queue=None, bind_mode=True
+    ):
+        self._ctx = vxAsyncZMQContext().instance()
+        self._socket = self._ctx.socket(socket_type)
+        if bind_mode:
+            self._socket.bind(url, secret_key)
+        else:
+            self._socket.connect(url, secret_key)
+        self._active = False
+        self._queue = send_queue if send_queue is None else Queue()
+
+    @property
+    def socket(self):
+        """socket"""
+        return self._socket
+
+    async def receiver(self, callback) -> None:
+        """接收进程
+
+        Arguments:
+            callback {Callable} -- 回调函数
+        """
+        while self._active:
+            flags = await self._socket.poll(zmq.POLLIN)
+            if flags & zmq.POLLIN != 0:
+                msg = await self._socket.recv_multipart()
+                callback(msg)
+
+    async def sender(self, serializer=None) -> None:
+        """发送
+
+        Arguments:
+            serializer {callable} -- 序列化函数
+        """
+        while self._active:
+            try:
+                msg = self._queue.get_nowait()
+                print(msg)
+
+                if (not isinstance(msg, bytes)) and serializer:
+                    msg = serializer(msg)
+
+                await self._socket.send(msg)
+            except Empty:
+                await asyncio.sleep(0.5)
+
+    async def run(self, callback: callable, serializer: callable) -> None:
+        wait_tasks = []
+        if callable(callback):
+            wait_tasks.append(self.receiver(callback))
+
+        wait_tasks.append(self.sender(serializer))
+
+        if not wait_tasks:
+            logger.warning("callback and msg_queue 不满足条件")
+
+        self._active = True
+        logger.info(f"开始运行 {self}")
+        await asyncio.gather(*wait_tasks)
+        self._active = False
+        logger.info(f"开始结束 {self}")
+
+    def send(self, msg) -> None:
+        self._queue.put(msg)
+
+
+class vxZMQBackendThread(Process):
+    def __init__(
+        self, on_send_callback: Callable = None, on_recv_callback: Callable = None
+    ) -> None:
+        self._zmqctx = None
+        self._socket = None
+        self._active = False
+        self._queue = Queue()
+        self._on_send_callback = on_send_callback
+        self._on_recv_callback = on_recv_callback
+
+        super().__init__()
+        name = self.getName()
+        self.setName(name.replace("Thread", self.__class__.__name__))
+
+    def set_on_send_callback(self, callback: Callable = None) -> None:
+        self._on_send_callback = callback
+
+    def set_on_recv_callback(self, callback: Callable = None) -> None:
+        self._on_recv_callback = callback
+
+    def send(self, *msgs) -> None:
+        """发送消息"""
+        self._queue.put(msgs)
+
+    def bind(self, socket_type, addr: str, secret_key: str = ""):
+        if self._active is True:
+            return
+        self._active = True
+        self._zmqctx = vxZMQContext().instance()
+        self._socket = self._zmqctx.socket(socket_type)
+        self._socket.bind(addr, secret_key)
+        return self
+
+    def connect(self, socket_type, addr: str, public_key: str = ""):
+        if self._active is True:
+            return
+        self._active = True
+        self._zmqctx = vxZMQContext().instance()
+        self._socket = self._zmqctx.socket(socket_type)
+        self._socket.connect(addr, public_key)
+
+    def run(self) -> None:
+        if self._active is False:
+            logger.info("请先调用 activate(url, public_key=None)进行初始化操作. 后运行")
+            return
+
+        logger.info(f"{self.name} (id-{id(self)}) 启动运行...")
+
+        try:
+            while self._active:
+                flags = self._socket.poll(1000, zmq.POLLIN | zmq.POLLOUT)
+
+                if self._on_recv_callback and flags & zmq.POLLIN != 0:
+                    msgs = self._socket.recv_multipart()
+                    logger.debug(f"recive msgs: {msgs}")
+                    self._on_recv_callback(self, *msgs)
+
+                if flags & zmq.POLLOUT != 0:
+                    with contextlib.suppress(Empty):
+                        msgs = self._queue.get(timeout=0.1)
+                        if self._on_send_callback:
+                            msgs = self._on_send_callback(self, *msgs)
+                        self._socket.send_multipart(list(map(to_binary, msgs)))
+        finally:
+            logger.info(f"{self.name} (id-{id(self)}) 停止运行...")
+            self.stop()
+
+    def close(self) -> None:
+        if self._active is False:
+            return
+        self.stop()
+
+    def stop(self) -> None:
+        self._active = False
+        # self.join()
+        if self._socket:
+            self._socket.setsockopt(zmq.LINGER, 0)
+            self._socket.close()
+            self._socket = None
+            self._zmqctx = None
```

### Comparing `vxquant-2023.3.1/PKG-INFO` & `vxquant-2023.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxquant
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: 一个简单、易用、面向中国股市实盘的python量化交易框架
 Home-page: https://gitee.com/vxquant/vxquant
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

