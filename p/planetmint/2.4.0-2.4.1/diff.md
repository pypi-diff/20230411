# Comparing `tmp/planetmint-2.4.0.tar.gz` & `tmp/planetmint-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint-2.4.0.tar", max compression
+gzip compressed data, was "planetmint-2.4.1.tar", max compression
```

## Comparing `planetmint-2.4.0.tar` & `planetmint-2.4.1.tar`

### file list

```diff
@@ -1,81 +1,80 @@
--rw-r--r--   0        0        0    34523 2023-04-05 13:51:24.199678 planetmint-2.4.0/LICENSE
--rw-r--r--   0        0        0     1614 2023-04-05 13:51:24.199678 planetmint-2.4.0/LICENSES.md
--rw-r--r--   0        0        0     3126 2023-04-05 13:51:24.199678 planetmint-2.4.0/README.md
--rw-r--r--   0        0        0     1796 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/README.md
--rw-r--r--   0        0        0      205 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/__init__.py
--rw-r--r--   0        0        0    10928 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/application_logic.py
--rw-r--r--   0        0        0      104 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/block.py
--rw-r--r--   0        0        0     4896 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/parallel_validation.py
--rw-r--r--   0        0        0     2994 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/rpc.py
--rw-r--r--   0        0        0     5291 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/abci/utils.py
--rw-r--r--   0        0        0       86 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/application/__init__.py
--rw-r--r--   0        0        0      833 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/application/basevalidationrules.py
--rw-r--r--   0        0        0    23655 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/application/validator.py
--rw-r--r--   0        0        0     2319 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/README.md
--rw-r--r--   0        0        0      705 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/__init__.py
--rw-r--r--   0        0        0     4496 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/connection.py
--rw-r--r--   0        0        0      891 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/exceptions.py
--rw-r--r--   0        0        0     1192 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/localmongodb/__init__.py
--rw-r--r--   0        0        0     6303 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/localmongodb/connection.py
--rw-r--r--   0        0        0     9891 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/localmongodb/query.py
--rw-r--r--   0        0        0     2995 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/localmongodb/schema.py
--rw-r--r--   0        0        0      438 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/__init__.py
--rw-r--r--   0        0        0      938 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/asset.py
--rw-r--r--   0        0        0      727 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/block.py
--rw-r--r--   0        0        0     3050 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/dbtransaction.py
--rw-r--r--   0        0        0      446 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/fulfills.py
--rw-r--r--   0        0        0     1971 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/input.py
--rw-r--r--   0        0        0      603 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/metadata.py
--rw-r--r--   0        0        0     4387 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/output.py
--rw-r--r--   0        0        0      600 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/models/script.py
--rw-r--r--   0        0        0    10596 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/query.py
--rw-r--r--   0        0        0     4222 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/schema.py
--rw-r--r--   0        0        0      127 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/__init__.py
--rw-r--r--   0        0        0      917 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/const.py
--rw-r--r--   0        0        0    11224 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/init.lua
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/sync_io/__init__.py
--rw-r--r--   0        0        0     2714 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/sync_io/connection.py
--rw-r--r--   0        0        0    19185 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/sync_io/query.py
--rw-r--r--   0        0        0     1046 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/sync_io/schema.py
--rw-r--r--   0        0        0      916 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/tarantool/tarantool.md
--rw-r--r--   0        0        0     1123 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/backend/utils.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/commands/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/commands/election_types.py
--rw-r--r--   0        0        0    13925 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/commands/planetmint.py
--rw-r--r--   0        0        0     4976 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/commands/utils.py
--rw-r--r--   0        0        0     6711 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/config.py
--rw-r--r--   0        0        0    12361 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/config_utils.py
--rw-r--r--   0        0        0      401 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/const.py
--rw-r--r--   0        0        0      390 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/ipc/__init__.py
--rw-r--r--   0        0        0      951 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/ipc/events.py
--rw-r--r--   0        0        0     2195 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/ipc/exchange.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/model/__init__.py
--rw-r--r--   0        0        0    11519 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/model/dataaccessor.py
--rw-r--r--   0        0        0     2889 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/model/fastquery.py
--rw-r--r--   0        0        0     3442 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/start.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/utils/lazy.py
--rw-r--r--   0        0        0     2253 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/utils/processes.py
--rw-r--r--   0        0        0      261 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/utils/python.py
--rw-r--r--   0        0        0      239 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/utils/singleton.py
--rw-r--r--   0        0        0      327 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/version.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/routes.py
--rw-r--r--   0        0        0     3671 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/server.py
--rw-r--r--   0        0        0      947 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/strip_content_type_middleware.py
--rw-r--r--   0        0        0        0 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/assets.py
--rw-r--r--   0        0        0     1525 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/base.py
--rw-r--r--   0        0        0     2345 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/blocks.py
--rw-r--r--   0        0        0     1817 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/info.py
--rw-r--r--   0        0        0     1428 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/metadata.py
--rw-r--r--   0        0        0     1455 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/outputs.py
--rw-r--r--   0        0        0     1631 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/parameters.py
--rw-r--r--   0        0        0     4785 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/transactions.py
--rw-r--r--   0        0        0      677 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/views/validators.py
--rw-r--r--   0        0        0     3548 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/websocket_dispatcher.py
--rw-r--r--   0        0        0     4906 2023-04-05 13:51:24.215678 planetmint-2.4.0/planetmint/web/websocket_server.py
--rw-r--r--   0        0        0     2664 2023-04-05 13:51:24.219678 planetmint-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-11 13:23:28.031970 planetmint-2.4.1/LICENSE
+-rw-r--r--   0        0        0     1614 2023-04-11 13:23:28.031970 planetmint-2.4.1/LICENSES.md
+-rw-r--r--   0        0        0     3126 2023-04-11 13:23:28.031970 planetmint-2.4.1/README.md
+-rw-r--r--   0        0        0     1796 2023-04-11 13:23:28.051971 planetmint-2.4.1/planetmint/README.md
+-rw-r--r--   0        0        0      205 2023-04-11 13:23:28.051971 planetmint-2.4.1/planetmint/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.051971 planetmint-2.4.1/planetmint/abci/__init__.py
+-rw-r--r--   0        0        0    10928 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/abci/application_logic.py
+-rw-r--r--   0        0        0      104 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/abci/block.py
+-rw-r--r--   0        0        0     4896 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/abci/parallel_validation.py
+-rw-r--r--   0        0        0     2994 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/abci/rpc.py
+-rw-r--r--   0        0        0     5291 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/abci/utils.py
+-rw-r--r--   0        0        0       86 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/application/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/application/basevalidationrules.py
+-rw-r--r--   0        0        0    23655 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/application/validator.py
+-rw-r--r--   0        0        0     2319 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/README.md
+-rw-r--r--   0        0        0      705 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/__init__.py
+-rw-r--r--   0        0        0     4496 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/connection.py
+-rw-r--r--   0        0        0      891 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/localmongodb/__init__.py
+-rw-r--r--   0        0        0     6303 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/localmongodb/connection.py
+-rw-r--r--   0        0        0     9498 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/localmongodb/query.py
+-rw-r--r--   0        0        0     2995 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/localmongodb/schema.py
+-rw-r--r--   0        0        0      438 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/asset.py
+-rw-r--r--   0        0        0      727 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/block.py
+-rw-r--r--   0        0        0     3050 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/dbtransaction.py
+-rw-r--r--   0        0        0      446 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/fulfills.py
+-rw-r--r--   0        0        0     1971 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/input.py
+-rw-r--r--   0        0        0      603 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/metadata.py
+-rw-r--r--   0        0        0     4387 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/output.py
+-rw-r--r--   0        0        0      600 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/models/script.py
+-rw-r--r--   0        0        0    10645 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/query.py
+-rw-r--r--   0        0        0     4222 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/schema.py
+-rw-r--r--   0        0        0      127 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/__init__.py
+-rw-r--r--   0        0        0      917 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/const.py
+-rw-r--r--   0        0        0    11502 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/init.lua
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/sync_io/__init__.py
+-rw-r--r--   0        0        0     2714 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/sync_io/connection.py
+-rw-r--r--   0        0        0    19127 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/sync_io/query.py
+-rw-r--r--   0        0        0     1046 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/sync_io/schema.py
+-rw-r--r--   0        0        0      916 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/tarantool/tarantool.md
+-rw-r--r--   0        0        0     1123 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/backend/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/commands/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/commands/election_types.py
+-rw-r--r--   0        0        0    13925 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/commands/planetmint.py
+-rw-r--r--   0        0        0     4976 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/commands/utils.py
+-rw-r--r--   0        0        0     6711 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/config.py
+-rw-r--r--   0        0        0    12361 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/config_utils.py
+-rw-r--r--   0        0        0      401 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/const.py
+-rw-r--r--   0        0        0      390 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/ipc/__init__.py
+-rw-r--r--   0        0        0      951 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/ipc/events.py
+-rw-r--r--   0        0        0     2195 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/ipc/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/model/__init__.py
+-rw-r--r--   0        0        0    14086 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/model/dataaccessor.py
+-rw-r--r--   0        0        0     3442 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/start.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/utils/lazy.py
+-rw-r--r--   0        0        0     2253 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/utils/processes.py
+-rw-r--r--   0        0        0      261 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/utils/python.py
+-rw-r--r--   0        0        0      239 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/utils/singleton.py
+-rw-r--r--   0        0        0      327 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/version.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/routes.py
+-rw-r--r--   0        0        0     3671 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/server.py
+-rw-r--r--   0        0        0      947 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/strip_content_type_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/assets.py
+-rw-r--r--   0        0        0     1525 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/base.py
+-rw-r--r--   0        0        0     2345 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/blocks.py
+-rw-r--r--   0        0        0     1817 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/info.py
+-rw-r--r--   0        0        0     1428 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/metadata.py
+-rw-r--r--   0        0        0     1455 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/outputs.py
+-rw-r--r--   0        0        0     1631 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/parameters.py
+-rw-r--r--   0        0        0     4785 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/transactions.py
+-rw-r--r--   0        0        0      677 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/views/validators.py
+-rw-r--r--   0        0        0     3548 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/websocket_dispatcher.py
+-rw-r--r--   0        0        0     4906 2023-04-11 13:23:28.055971 planetmint-2.4.1/planetmint/web/websocket_server.py
+-rw-r--r--   0        0        0     2664 2023-04-11 13:23:28.059972 planetmint-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.1/PKG-INFO
```

### Comparing `planetmint-2.4.0/LICENSE` & `planetmint-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/LICENSES.md` & `planetmint-2.4.1/LICENSES.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/README.md` & `planetmint-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/README.md` & `planetmint-2.4.1/planetmint/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/abci/application_logic.py` & `planetmint-2.4.1/planetmint/abci/application_logic.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/abci/parallel_validation.py` & `planetmint-2.4.1/planetmint/abci/parallel_validation.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/abci/rpc.py` & `planetmint-2.4.1/planetmint/abci/rpc.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/abci/utils.py` & `planetmint-2.4.1/planetmint/abci/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/application/basevalidationrules.py` & `planetmint-2.4.1/planetmint/application/basevalidationrules.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/application/validator.py` & `planetmint-2.4.1/planetmint/application/validator.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/README.md` & `planetmint-2.4.1/planetmint/backend/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/__init__.py` & `planetmint-2.4.1/planetmint/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/connection.py` & `planetmint-2.4.1/planetmint/backend/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/exceptions.py` & `planetmint-2.4.1/planetmint/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/localmongodb/__init__.py` & `planetmint-2.4.1/planetmint/backend/localmongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/localmongodb/connection.py` & `planetmint-2.4.1/planetmint/backend/localmongodb/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/localmongodb/query.py` & `planetmint-2.4.1/planetmint/backend/localmongodb/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 # TODO: pass filter/projection in function call this is not the expected behaviour for a function called get_assets
 @register_query(LocalMongoDBConnection)
 def get_assets(conn, asset_ids):
     return conn.run(conn.collection("assets").find({"id": {"$in": asset_ids}}, projection={"_id": False}))
 
 
 @register_query(LocalMongoDBConnection)
-def get_spent(conn, transaction_id, output):
+def get_spending_transaction(conn, transaction_id, output):
     query = {
         "inputs": {
             "$elemMatch": {"$and": [{"fulfills.transaction_id": transaction_id}, {"fulfills.output_index": output}]}
         }
     }
 
     return conn.run(conn.collection("transactions").find(query, {"_id": 0}))
@@ -164,29 +164,14 @@
 def delete_transactions(conn, txn_ids):
     conn.run(conn.collection("assets").delete_many({"id": {"$in": txn_ids}}))
     conn.run(conn.collection("metadata").delete_many({"id": {"$in": txn_ids}}))
     conn.run(conn.collection("transactions").delete_many({"id": {"$in": txn_ids}}))
 
 
 @register_query(LocalMongoDBConnection)
-def store_unspent_outputs(conn, *unspent_outputs):
-    if unspent_outputs:
-        try:
-            return conn.run(
-                conn.collection("utxos").insert_many(
-                    unspent_outputs,
-                    ordered=False,
-                )
-            )
-        except DuplicateKeyError:
-            # TODO log warning at least
-            pass
-
-
-@register_query(LocalMongoDBConnection)
 def delete_unspent_outputs(conn, *unspent_outputs):
     if unspent_outputs:
         return conn.run(
             conn.collection("utxos").delete_many(
                 {
                     "$or": [
                         {
```

### Comparing `planetmint-2.4.0/planetmint/backend/localmongodb/schema.py` & `planetmint-2.4.1/planetmint/backend/localmongodb/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/asset.py` & `planetmint-2.4.1/planetmint/backend/models/asset.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/block.py` & `planetmint-2.4.1/planetmint/backend/models/block.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/dbtransaction.py` & `planetmint-2.4.1/planetmint/backend/models/dbtransaction.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/input.py` & `planetmint-2.4.1/planetmint/backend/models/input.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/metadata.py` & `planetmint-2.4.1/planetmint/backend/models/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/output.py` & `planetmint-2.4.1/planetmint/backend/models/output.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/models/script.py` & `planetmint-2.4.1/planetmint/backend/models/script.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/query.py` & `planetmint-2.4.1/planetmint/backend/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         The result of the operation.
     """
 
     raise NotImplementedError
 
 
 @singledispatch
-def get_spent(connection, transaction_id, condition_id):
+def get_spending_transaction(connection, transaction_id, condition_id):
     """Check if a `txid` was already used as an input.
 
     A transaction can be used as an input for another transaction. Bigchain
     needs to make sure that a given `txid` is only used once.
 
     Args:
         transaction_id (str): The id of the transaction.
@@ -204,15 +204,15 @@
         block_id (int): the block id or `None`
     """
 
     raise NotImplementedError
 
 
 @singledispatch
-def store_transaction_outputs(connection, output: Output, index: int):
+def store_transaction_outputs(connection, output: Output, index: int, table: str):
     """Store the transaction outputs.
 
     Args:
         output (Output): the output to store.
         index (int): the index of the output in the transaction.
     """
     raise NotImplementedError
@@ -261,21 +261,14 @@
         The result of the operation.
     """
 
     raise NotImplementedError
 
 
 @singledispatch
-def store_unspent_outputs(connection, unspent_outputs):
-    """Store unspent outputs in ``utxo_set`` table."""
-
-    raise NotImplementedError
-
-
-@singledispatch
 def delete_unspent_outputs(connection, unspent_outputs):
     """Delete unspent outputs in ``utxo_set`` table."""
 
     raise NotImplementedError
 
 
 @singledispatch
@@ -452,10 +445,16 @@
 @singledispatch
 def get_outputs_by_tx_id(connection, tx_id: str) -> list[Output]:
     """Retrieve outputs for a transaction by its id"""
     raise NotImplementedError
 
 
 @singledispatch
+def get_outputs_by_owner(connection, public_key: str, table: str) -> list[Output]:
+    """Retrieve an owners outputs by public key"""
+    raise NotImplementedError
+
+
+@singledispatch
 def get_metadata(conn, transaction_ids):
     """Retrieve metadata for a list of transactions by their ids"""
     raise NotImplementedError
```

### Comparing `planetmint-2.4.0/planetmint/backend/schema.py` & `planetmint-2.4.1/planetmint/backend/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/const.py` & `planetmint-2.4.1/planetmint/backend/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/init.lua` & `planetmint-2.4.1/planetmint/backend/tarantool/init.lua`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,19 @@
     })
 
 
     -- UTXO
     utxos = box.schema.create_space('utxos', { if_not_exists = true })
     utxos:format({
         { name = 'id', type = 'string' },
-        { name = 'transaction_id', type = 'string' },
-        { name = 'output_index', type = 'unsigned' },
-        { name = 'utxo', type = 'map' }
+        { name = 'amount' , type = 'unsigned' },
+        { name = 'public_keys', type = 'array' },
+        { name = 'condition', type = 'map' },
+        { name = 'output_index', type = 'number' },
+        { name = 'transaction_id' , type = 'string' }
     })
     utxos:create_index('id', { 
         if_not_exists = true,
         parts = {{ field = 'id', type = 'string' }}
     })
     utxos:create_index('utxos_by_transaction_id', {
         if_not_exists = true,
@@ -185,15 +187,21 @@
         parts = {{ field = 'transaction_id', type = 'string' }}
     })
     utxos:create_index('utxo_by_transaction_id_and_output_index', { 
         if_not_exists = true,
         parts = {
             { field = 'transaction_id', type = 'string' },
             { field = 'output_index', type = 'unsigned' }
-    }})
+        }
+    })
+    utxos:create_index('public_keys', { 
+        if_not_exists = true,
+        unique = false,
+        parts = {{field = 'public_keys[*]', type  = 'string' }}
+    })
 
 
     -- Elections
     elections = box.schema.create_space('elections', { if_not_exists = true })
     elections:format({
         { name = 'id', type = 'string' },
         { name = 'height', type = 'unsigned' },
```

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/sync_io/connection.py` & `planetmint-2.4.1/planetmint/backend/tarantool/sync_io/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/sync_io/query.py` & `planetmint-2.4.1/planetmint/backend/tarantool/sync_io/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,19 +123,20 @@
         .select(TARANT_TABLE_TRANSACTION, metadata, limit=limit, index="transactions_by_metadata_cid")
         .data
     )
     tx_ids = [tx[0] for tx in txs]
     return get_complete_transactions_by_ids(connection, tx_ids)
 
 
+@register_query(TarantoolDBConnection)
 @catch_db_exception
-def store_transaction_outputs(connection, output: Output, index: int) -> str:
+def store_transaction_outputs(connection, output: Output, index: int, table=TARANT_TABLE_OUTPUT) -> str:
     output_id = uuid4().hex
     connection.connect().insert(
-        TARANT_TABLE_OUTPUT,
+        table,
         (
             output_id,
             int(output.amount),
             output.public_keys,
             output.condition.to_dict(),
             index,
             output.transaction_id,
@@ -216,15 +217,17 @@
 
     sorted_assets = sorted(_returned_data, key=lambda k: k[1], reverse=False)
     return [Asset.from_dict(asset) for asset in sorted_assets]
 
 
 @register_query(TarantoolDBConnection)
 @catch_db_exception
-def get_spent(connection, fullfil_transaction_id: str, fullfil_output_index: str) -> list[DbTransaction]:
+def get_spending_transaction(
+    connection, fullfil_transaction_id: str, fullfil_output_index: str
+) -> list[DbTransaction]:
     _inputs = (
         connection.connect()
         .select(
             TARANT_TABLE_TRANSACTION,
             [fullfil_transaction_id, fullfil_output_index],
             index=TARANT_INDEX_SPENDING_BY_ID_AND_OUTPUT_INDEX,
         )
@@ -296,15 +299,15 @@
 
 
 @register_query(TarantoolDBConnection)
 def get_spending_transactions(connection, inputs):
     _transactions = []
 
     for inp in inputs:
-        _trans_list = get_spent(
+        _trans_list = get_spending_transaction(
             fullfil_transaction_id=inp["transaction_id"],
             fullfil_output_index=inp["output_index"],
             connection=connection,
         )
         _transactions.extend(_trans_list)
 
     return _transactions
@@ -333,41 +336,25 @@
 @register_query(TarantoolDBConnection)
 @catch_db_exception
 def delete_transactions(connection, txn_ids: list):
     for _id in txn_ids:
         _outputs = get_outputs_by_tx_id(connection, _id)
         for x in range(len(_outputs)):
             connection.connect().call("delete_output", (_outputs[x].id))
+            connection.connect().delete(
+                TARANT_TABLE_UTXOS, (_id, _outputs[x].index), index="utxo_by_transaction_id_and_output_index"
+            )
     for _id in txn_ids:
         connection.connect().delete(TARANT_TABLE_TRANSACTION, _id)
         connection.connect().delete(TARANT_TABLE_GOVERNANCE, _id)
 
 
 @register_query(TarantoolDBConnection)
 @catch_db_exception
-def store_unspent_outputs(connection, *unspent_outputs: list):
-    result = []
-    if unspent_outputs:
-        for utxo in unspent_outputs:
-            try:
-                output = (
-                    connection.connect()
-                    .insert(TARANT_TABLE_UTXOS, (uuid4().hex, utxo["transaction_id"], utxo["output_index"], utxo))
-                    .data
-                )
-                result.append(output)
-            except Exception as e:
-                logger.info(f"Could not insert unspent output: {e}")
-                raise OperationDataInsertionError()
-    return result
-
-
-@register_query(TarantoolDBConnection)
-@catch_db_exception
-def delete_unspent_outputs(connection, *unspent_outputs: list):
+def delete_unspent_outputs(connection, unspent_outputs: list):
     result = []
     if unspent_outputs:
         for utxo in unspent_outputs:
             output = (
                 connection.connect()
                 .delete(
                     TARANT_TABLE_UTXOS,
@@ -379,16 +366,16 @@
             result.append(output)
     return result
 
 
 @register_query(TarantoolDBConnection)
 @catch_db_exception
 def get_unspent_outputs(connection, query=None):  # for now we don't have implementation for 'query'.
-    _utxos = connection.connect().select(TARANT_TABLE_UTXOS, []).data
-    return [utx[3] for utx in _utxos]
+    utxos = connection.connect().select(TARANT_TABLE_UTXOS, []).data
+    return [{"transaction_id": utxo[5], "output_index": utxo[4]} for utxo in utxos]
 
 
 @register_query(TarantoolDBConnection)
 @catch_db_exception
 def store_pre_commit_state(connection, state: dict):
     _precommit = connection.connect().select(TARANT_TABLE_PRE_COMMITS, [], limit=1).data
     _precommitTuple = (
@@ -518,7 +505,14 @@
 @catch_db_exception
 def get_latest_abci_chain(connection) -> Union[dict, None]:
     _all_chains = connection.connect().select(TARANT_TABLE_ABCI_CHAINS).data
     if _all_chains is None or len(_all_chains) == 0:
         return None
     _chain = sorted(_all_chains, key=itemgetter(1), reverse=True)[0]
     return {"chain_id": _chain[0], "height": _chain[1], "is_synced": _chain[2]}
+
+
+@register_query(TarantoolDBConnection)
+@catch_db_exception
+def get_outputs_by_owner(connection, public_key: str, table=TARANT_TABLE_OUTPUT) -> list[Output]:
+    outputs = connection.connect().select(table, public_key, index="public_keys")
+    return [Output.from_tuple(output) for output in outputs]
```

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/sync_io/schema.py` & `planetmint-2.4.1/planetmint/backend/tarantool/sync_io/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/tarantool/tarantool.md` & `planetmint-2.4.1/planetmint/backend/tarantool/tarantool.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/backend/utils.py` & `planetmint-2.4.1/planetmint/backend/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/commands/election_types.py` & `planetmint-2.4.1/planetmint/commands/election_types.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/commands/planetmint.py` & `planetmint-2.4.1/planetmint/commands/planetmint.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/commands/utils.py` & `planetmint-2.4.1/planetmint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/config.py` & `planetmint-2.4.1/planetmint/config.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/config_utils.py` & `planetmint-2.4.1/planetmint/config_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/ipc/events.py` & `planetmint-2.4.1/planetmint/ipc/events.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/ipc/exchange.py` & `planetmint-2.4.1/planetmint/ipc/exchange.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/model/dataaccessor.py` & `planetmint-2.4.1/planetmint/model/dataaccessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import rapidjson
 from itertools import chain
+from hashlib import sha3_256
 
 from transactions import Transaction
 from transactions.common.exceptions import DoubleSpend
 from transactions.common.crypto import public_key_from_ed25519_key
 from transactions.common.exceptions import InputDoesNotExist
 
 from planetmint import config_utils, backend
 from planetmint.const import GOVERNANCE_TRANSACTION_TYPES
-from planetmint.model.fastquery import FastQuery
-from planetmint.abci.utils import key_from_base64
+from planetmint.abci.utils import key_from_base64, merkleroot
 from planetmint.backend.connection import Connection
-from planetmint.backend.tarantool.const import TARANT_TABLE_TRANSACTION, TARANT_TABLE_GOVERNANCE
+from planetmint.backend.tarantool.const import (
+    TARANT_TABLE_TRANSACTION,
+    TARANT_TABLE_GOVERNANCE,
+    TARANT_TABLE_UTXOS,
+    TARANT_TABLE_OUTPUT,
+)
 from planetmint.backend.models.block import Block
 from planetmint.backend.models.output import Output
 from planetmint.backend.models.asset import Asset
 from planetmint.backend.models.metadata import MetaData
 from planetmint.backend.models.dbtransaction import DbTransaction
 
 
@@ -33,14 +38,15 @@
             if transaction["operation"] in GOVERNANCE_TRANSACTION_TYPES:
                 gov_txns.append(transaction)
             else:
                 txns.append(transaction)
 
         backend.query.store_transactions(self.connection, txns, TARANT_TABLE_TRANSACTION)
         backend.query.store_transactions(self.connection, gov_txns, TARANT_TABLE_GOVERNANCE)
+        [self.update_utxoset(t) for t in txns + gov_txns]
 
     def delete_transactions(self, txs):
         return backend.query.delete_transactions(self.connection, txs)
 
     def is_committed(self, transaction_id):
         transaction = backend.query.get_transaction_single(self.connection, transaction_id)
         return bool(transaction)
@@ -56,34 +62,41 @@
         txids = backend.query.get_txids_filtered(self.connection, asset_ids, operation, last_tx)
         for txid in txids:
             yield self.get_transaction(txid)
 
     def get_outputs_by_tx_id(self, txid):
         return backend.query.get_outputs_by_tx_id(self.connection, txid)
 
-    def get_outputs_filtered(self, owner, spent=None):
+    def get_outputs_filtered(self, owner, spent=None) -> list[Output]:
         """Get a list of output links filtered on some criteria
 
         Args:
             owner (str): base58 encoded public_key.
             spent (bool): If ``True`` return only the spent outputs. If
                           ``False`` return only unspent outputs. If spent is
                           not specified (``None``) return all outputs.
 
         Returns:
-            :obj:`list` of TransactionLink: list of ``txid`` s and ``output`` s
+            :obj:`list` of Output: list of ``txid`` s and ``output`` s
             pointing to another transaction's condition
         """
-        outputs = self.fastquery.get_outputs_by_public_key(owner)
-        if spent is None:
-            return outputs
-        elif spent is True:
-            return self.fastquery.filter_unspent_outputs(outputs)
+        outputs = backend.query.get_outputs_by_owner(self.connection, owner)
+        unspent_outputs = backend.query.get_outputs_by_owner(self.connection, owner, TARANT_TABLE_UTXOS)
+        if spent is True:
+            spent_outputs = []
+            for output in outputs:
+                if not any(
+                    utxo.transaction_id == output.transaction_id and utxo.index == output.index
+                    for utxo in unspent_outputs
+                ):
+                    spent_outputs.append(output)
+            return spent_outputs
         elif spent is False:
-            return self.fastquery.filter_spent_outputs(outputs)
+            return unspent_outputs
+        return outputs
 
     def store_block(self, block):
         """Create a new block."""
 
         return backend.query.store_block(self.connection, block)
 
     def get_latest_block(self) -> dict:
@@ -134,16 +147,16 @@
         for validator in self.get_validators(height):
             # NOTE: we assume that Tendermint encodes public key in base64
             public_key = public_key_from_ed25519_key(key_from_base64(validator["public_key"]["value"]))
             validators[public_key] = validator["voting_power"]
 
         return validators
 
-    def get_spent(self, txid, output, current_transactions=[]) -> DbTransaction:
-        transactions = backend.query.get_spent(self.connection, txid, output)
+    def get_spending_transaction(self, txid, output, current_transactions=[]) -> DbTransaction:
+        transactions = backend.query.get_spending_transaction(self.connection, txid, output)
 
         current_spent_transactions = []
         for ctxn in current_transactions:
             for ctxn_input in ctxn.inputs:
                 if ctxn_input.fulfills and ctxn_input.fulfills.txid == txid and ctxn_input.fulfills.output == output:
                     current_spent_transactions.append(ctxn)
 
@@ -192,15 +205,15 @@
                             Output.from_dict(output, index, ctxn.id)
                             for index, output in enumerate(ctxn_dict["outputs"])
                         ]
 
             if input_tx is None:
                 raise InputDoesNotExist("input `{}` doesn't exist".format(input_txid))
 
-            spent = self.get_spent(input_txid, input_.fulfills.output, current_transactions)
+            spent = self.get_spending_transaction(input_txid, input_.fulfills.output, current_transactions)
             if spent:
                 raise DoubleSpend("input `{}` was already spent".format(input_txid))
 
             output = _output[input_.fulfills.output]
             input_conditions.append(output)
             tx_dict = input_tx.to_dict()
             tx_dict["outputs"] = Output.list_to_dict(_output)
@@ -273,10 +286,58 @@
     def store_abci_chain(self, height, chain_id, is_synced=True):
         return backend.query.store_abci_chain(self.connection, height, chain_id, is_synced)
 
     def get_asset_tokens_for_public_key(self, transaction_id, election_pk):
         txns = backend.query.get_asset_tokens_for_public_key(self.connection, transaction_id, election_pk)
         return txns
 
-    @property
-    def fastquery(self):
-        return FastQuery(self.connection)
+    def update_utxoset(self, transaction):
+        spent_outputs = [
+            {"output_index": input["fulfills"]["output_index"], "transaction_id": input["fulfills"]["transaction_id"]}
+            for input in transaction["inputs"]
+            if input["fulfills"] != None
+        ]
+
+        if spent_outputs:
+            backend.query.delete_unspent_outputs(self.connection, spent_outputs)
+        [
+            backend.query.store_transaction_outputs(
+                self.connection, Output.outputs_dict(output, transaction["id"]), index, TARANT_TABLE_UTXOS
+            )
+            for index, output in enumerate(transaction["outputs"])
+        ]
+
+    def get_utxoset_merkle_root(self):
+        """Returns the merkle root of the utxoset. This implies that
+        the utxoset is first put into a merkle tree.
+
+        For now, the merkle tree and its root will be computed each
+        time. This obviously is not efficient and a better approach
+        that limits the repetition of the same computation when
+        unnecesary should be sought. For instance, future optimizations
+        could simply re-compute the branches of the tree that were
+        affected by a change.
+
+        The transaction hash (id) and output index should be sufficient
+        to uniquely identify a utxo, and consequently only that
+        information from a utxo record is needed to compute the merkle
+        root. Hence, each node of the merkle tree should contain the
+        tuple (txid, output_index).
+
+        .. important:: The leaves of the tree will need to be sorted in
+            some kind of lexicographical order.
+
+        Returns:
+            str: Merkle root in hexadecimal form.
+        """
+        utxoset = backend.query.get_unspent_outputs(self.connection)
+        # TODO Once ready, use the already pre-computed utxo_hash field.
+        # See common/transactions.py for details.
+
+        hashes = [
+            sha3_256("{}{}".format(utxo["transaction_id"], utxo["output_index"]).encode()).digest() for utxo in utxoset
+        ]
+
+        print(sorted(hashes))
+
+        # TODO Notice the sorted call!
+        return merkleroot(sorted(hashes))
```

### Comparing `planetmint-2.4.0/planetmint/start.py` & `planetmint-2.4.1/planetmint/start.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/utils/lazy.py` & `planetmint-2.4.1/planetmint/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/utils/processes.py` & `planetmint-2.4.1/planetmint/utils/processes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/routes.py` & `planetmint-2.4.1/planetmint/web/routes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/server.py` & `planetmint-2.4.1/planetmint/web/server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/strip_content_type_middleware.py` & `planetmint-2.4.1/planetmint/web/strip_content_type_middleware.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/assets.py` & `planetmint-2.4.1/planetmint/web/views/assets.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/base.py` & `planetmint-2.4.1/planetmint/web/views/base.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/blocks.py` & `planetmint-2.4.1/planetmint/web/views/blocks.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/info.py` & `planetmint-2.4.1/planetmint/web/views/info.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/metadata.py` & `planetmint-2.4.1/planetmint/web/views/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/outputs.py` & `planetmint-2.4.1/planetmint/web/views/outputs.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/parameters.py` & `planetmint-2.4.1/planetmint/web/views/parameters.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/transactions.py` & `planetmint-2.4.1/planetmint/web/views/transactions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/views/validators.py` & `planetmint-2.4.1/planetmint/web/views/validators.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/websocket_dispatcher.py` & `planetmint-2.4.1/planetmint/web/websocket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/planetmint/web/websocket_server.py` & `planetmint-2.4.1/planetmint/web/websocket_server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.0/pyproject.toml` & `planetmint-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint"
-version = "2.4.0"
+version = "2.4.1"
 description = "Planetmint: The Blockchain Database"
 authors = ["Planetmint contributors"]
 license = "AGPLv3"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
```

### Comparing `planetmint-2.4.0/PKG-INFO` & `planetmint-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint
-Version: 2.4.0
+Version: 2.4.1
 Summary: Planetmint: The Blockchain Database
 License: AGPLv3
 Author: Planetmint contributors
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

