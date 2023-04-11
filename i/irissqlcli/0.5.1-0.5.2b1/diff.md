# Comparing `tmp/irissqlcli-0.5.1.tar.gz` & `tmp/irissqlcli-0.5.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irissqlcli-0.5.1.tar", last modified: Thu Mar 23 07:38:31 2023, max compression
+gzip compressed data, was "irissqlcli-0.5.2b1.tar", last modified: Tue Apr 11 08:29:03 2023, max compression
```

## Comparing `irissqlcli-0.5.1.tar` & `irissqlcli-0.5.2b1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.270655 irissqlcli-0.5.1/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20005 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.270655 irissqlcli-0.5.1/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94603 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12186 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.270655 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78424 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.274654 irissqlcli-0.5.1/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.274654 irissqlcli-0.5.1/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      815 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.274654 irissqlcli-0.5.1/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-03-23 07:38:22.000000 irissqlcli-0.5.1/irisnative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.274654 irissqlcli-0.5.1/irissqlcli/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-23 07:38:05.000000 irissqlcli-0.5.1/irissqlcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/clitoolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/completion_refresher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/irissqlclirc
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    35292 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/irissqlcli/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/completion_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/encodingutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/parseutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/prompt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/irissqlcli/packages/special/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/dbcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/favoritequeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/iocommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/packages/special/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/sqlcompleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/sqlexecute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/irissqlcli/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/irissqlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-23 07:38:31.000000 irissqlcli-0.5.1/irissqlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:31.278654 irissqlcli-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:38:04.000000 irissqlcli-0.5.1/tests/test_sqlcompletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.671512 irissqlcli-0.5.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-11 08:29:03.671512 irissqlcli-0.5.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.651512 irissqlcli-0.5.2b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.655512 irissqlcli-0.5.2b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.655512 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.659512 irissqlcli-0.5.2b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.663512 irissqlcli-0.5.2b1/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.663512 irissqlcli-0.5.2b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-11 08:28:53.000000 irissqlcli-0.5.2b1/irisnative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.667512 irissqlcli-0.5.2b1/irissqlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 08:28:27.000000 irissqlcli-0.5.2b1/irissqlcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/clitoolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/completion_refresher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/irissqlclirc
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35292 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.667512 irissqlcli-0.5.2b1/irissqlcli/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/completion_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/encodingutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/parseutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/prompt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.671512 irissqlcli-0.5.2b1/irissqlcli/packages/special/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/dbcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/favoritequeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/iocommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/packages/special/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/sqlcompleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/sqlexecute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/irissqlcli/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.667512 irissqlcli-0.5.2b1/irissqlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 08:29:03.000000 irissqlcli-0.5.2b1/irissqlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-11 08:29:03.671512 irissqlcli-0.5.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:29:03.671512 irissqlcli-0.5.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:28:26.000000 irissqlcli-0.5.2b1/tests/test_sqlcompletion.py
```

### Comparing `irissqlcli-0.5.1/LICENSE` & `irissqlcli-0.5.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/PKG-INFO` & `irissqlcli-0.5.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irissqlcli
-Version: 0.5.1
+Version: 0.5.2b1
 Summary: CLI for SQL of InterSystems IRIS Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/caretdev/irissqlcli
 Author: CaretDev
 Author-email: irissqlcli@caretdev.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `irissqlcli-0.5.1/README.md` & `irissqlcli-0.5.2b1/README.md`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_BufferWriter.py` & `irissqlcli-0.5.2b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_ConnectionInformation.py` & `irissqlcli-0.5.2b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_ConnectionParameters.py` & `irissqlcli-0.5.2b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_Constant.py` & `irissqlcli-0.5.2b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_DBList.py` & `irissqlcli-0.5.2b1/intersystems_iris/_DBList.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
     def _grab_oref_unicode(cls, buffer, offset, length, *args):
         return intersystems_iris._IRISOREF._IRISOREF(cls._grab_unicode_string(buffer, offset, length))
 
     @classmethod
     def _set(cls, buffer, offset, data, locale, is_unicode, compact_double):
         func = cls._set_switcher.get(type(data), None)
         if func is None:
-            raise Exception("Unsupported argument type: " + str(type(data)))
+            # raise Exception("Unsupported argument type: " + str(type(data)))
+            return cls._stuff_str(buffer, offset, str(data), locale, is_unicode, compact_double)
         else:
             return func(buffer, offset, data, locale, is_unicode, compact_double)
 
     @classmethod
     def _set_undefined(cls, buffer, offset):
         buffer[offset] = 1
         return offset + 1
```

### Comparing `irissqlcli-0.5.1/intersystems_iris/_Device.py` & `irissqlcli-0.5.2b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_GatewayContext.py` & `irissqlcli-0.5.2b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_GatewayUtility.py` & `irissqlcli-0.5.2b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRIS.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISConnection.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISEmbedded.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISGlobalNode.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISGlobalNodeView.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISIterator.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISList.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISNative.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISObject.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_IRISReference.py` & `irissqlcli-0.5.2b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_InStream.py` & `irissqlcli-0.5.2b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_LegacyIterator.py` & `irissqlcli-0.5.2b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_ListReader.py` & `irissqlcli-0.5.2b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_ListWriter.py` & `irissqlcli-0.5.2b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_LogFileStream.py` & `irissqlcli-0.5.2b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_MessageHeader.py` & `irissqlcli-0.5.2b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_OutStream.py` & `irissqlcli-0.5.2b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_PrintStream.py` & `irissqlcli-0.5.2b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_PythonGateway.py` & `irissqlcli-0.5.2b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/_SharedMemorySocket.py` & `irissqlcli-0.5.2b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/__init__.py` & `irissqlcli-0.5.2b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_Column.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_DBAPI.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 
 def embedded_connect(*args, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
     connection = _IRISEmbedded()
     connection.connect(hostname, port,  namespace, username, password, **kw)
     return connection
 
 def connect(*args, embedded=False, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
-    if not embedded:
-        return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-    else:
-        return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-
+    try:
+        if not embedded:
+            return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+        else:
+            return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+    except Exception as e:
+        raise DatabaseError(e)
 
 class ServerReturnType(enum.IntEnum):
     NO_RETURN_VALUE = 0
     IGNORE_RETURN_VALUE = 1
     HAS_RETURN_VALUE = 2
     NULL_RETURN_VALUE = 3
 
@@ -56,14 +58,17 @@
 paramstyle = "qmark"
 
 class _BaseCursor:
     embedded = False
     def __init__(self, connection):
         self._connection = connection
         
+        self.statement = None
+        self._parsed_statement = None
+        
         self._columns = None
         self._rowcount = -1
         self.arraysize = 1
 
         self._result_set = None
 
         self._rsrow = None
@@ -184,15 +189,23 @@
         self._rowcount = -1
         self._exec_params = None
         self._statementType = StatementType.UPDATE
         self.statementFeatureOption = 0
         self.maxRowItemCount = 0
         self._is_batch_update = False
 
+    def _is_alive(self):
+        if self._closed:
+            raise InterfaceError("Cursor is closed")
+        if self._connection == None or self._connection.isClosed():
+            raise InterfaceError("Connection not open")
+
     def direct_execute(self, operation, *params):
+        self._is_alive()
+
         self.statement = operation
         if len(params) == 1 and (isinstance(params[0], tuple) or isinstance(params[0], list)):
             self.params = params[0]
         else:
             self.params = params
         self._params.set_input_params(self.params)
 
@@ -200,14 +213,16 @@
         self._cleanup()
         self._preparse()
 
         self._execute()
         return self._rowcount
 
     def execute(self, operation, params=()):
+        self._is_alive()
+
         self.statement = operation
         if params and not isinstance(params, list) and not isinstance(params, tuple):
             params = (params, )
         self.params = params if params is not None else ()
         self._params.set_input_params(self.params)
 
         self._cleanup()
@@ -219,16 +234,15 @@
         else:
             self._cursor_type = CursorType.DEFAULT
 
         self._execute()
         return self._rowcount
 
     def add_batch(self):
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
+        self._is_alive()
         
         if self._params._array_bound:
             if len(self._params._params_list) > 0:
                 cnt = 0
                 first = True
                 for i in range(self._params._user_parameters_size):
                     i = i + 1
@@ -249,19 +263,19 @@
                 if len(param._values) != self._parameter_sets:
                     if self._parameter_sets != 1:
                         if len(param._values) + 1 == self._parameter_sets:
                             param._values.append(param._values[len(param._values) - 1])
                             continue
 
     def executemany(self, operation, seq_of_params):
+        self._is_alive()
         self._rowcount = 0
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
-        if self._connection == None or self._connection.isClosed():
-            raise InterfaceError("Connection not open")
+
+        if not isinstance(seq_of_params, tuple) and not isinstance(seq_of_params, list):
+            seq_of_params = tuple(seq_of_params)
 
         self.statement = operation
         self.params = seq_of_params
         self._params.set_input_params(self.params)
 
         self._cursor_type = CursorType.PREPARED
         self._cleanup()
@@ -285,14 +299,22 @@
             if mode == ParameterMode.INPUT_OUTPUT or mode == ParameterMode.OUTPUT:
                 raise ValueError("INOUT/OUT parameters not permitted")
 
         self._prepared_update_execute()
 
         return self._rowcount
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        self._sqlcode = sqlcode
+        if sqlcode in [0, 100]:
+            return
+        if abs(sqlcode) in [108, 119, 121, 122]:
+            raise IntegrityError(message)
+        raise DatabaseError(message)
+
     def _preparse(self):
         csql = self._connection._pre_preparse_cache.get(self.statement)
         if csql != None:
             self._has_return_value = csql._has_return_value
             self._params = copy.deepcopy(csql._params)
             self._params.set_input_params(self.params)
             self._parsed_statement = csql._parsed_statement
@@ -305,15 +327,16 @@
             if isinstance(item, list) or isinstance(item, tuple):
                 if not self._is_batch_update:
                     raise TypeError("Unsupported argument type: " + str(type(item)))
                 for ele in item:
                     if intersystems_iris._DBList._DBList._set_switcher.get(type(ele), None) == None:
                         raise TypeError("Unsupported argument type: " + str(type(ele)))
             elif intersystems_iris._DBList._DBList._set_switcher.get(type(item), None) is None:
-                raise TypeError("Unsupported argument type: " + str(type(item)))
+                item = str(item)
+                # raise TypeError("Unsupported argument type: " + str(type(item)))
             if i == 0:
                 count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
             else:
                 curr_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
                 if count != curr_count:
                     raise Exception("Parameter count does not match")
 
@@ -364,15 +387,15 @@
                 elif item == '?':
                     unknown_count = unknown_count + 1
 
             if len(self.params) > 0:
                 item = self.params[0]
                 param_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else len(self.params)
                 if param_count != unknown_count:
-                    raise Exception("Parameter mismatch")
+                    raise Exception(f"Parameter mismatch: {param_count}/{unknown_count}")
         else:
             if self._cursor_type == CursorType.CALLABLE:
                 i = 0
                 for param in self._params._params_list:
                     if param.mode == ParameterMode.RETURN_VALUE:
                         continue
                     else:
@@ -395,15 +418,15 @@
                 for item in temp_list_data:
                     if item == 'c':
                         replaced_count = replaced_count + 1
                     elif item == '?':
                         unknown_count = unknown_count + 1
 
                 if unknown_count != len(self.params):
-                    raise Exception("Incorrect number of parameters")
+                    raise Exception(f"Incorrect number of parameters: {unknown_count}/{replaced_count}/{len(self.params)}")
 
     def _is_not_default_or_replaced(self, param):
         mode = param.mode
         if mode != ParameterMode.REPLACED_LITERAL and mode != ParameterMode.DEFAULT_PARAMETER and mode != ParameterMode.INPUT:
             raise Exception("Parameters not allowed in Cursor class")
 
     def _validate_parameters(self):
@@ -433,14 +456,15 @@
             raise InterfaceError("Cursor is closed")
         if self._connection == None or self._connection.isClosed():
             raise InterfaceError("Connection not open")
 
         exec_switcher = {
             StatementType.QUERY: self._execute_query,
             StatementType.CALL: self._execute_update,
+            StatementType.STMT_USE: self._execute_update,
             StatementType.UPDATE: self._execute_update,
             StatementType.DDL_OTHER: self._execute_update,
             StatementType.DDL_ALTER_DROP: self._execute_update
         }
         exec_func = exec_switcher.get(self._statementType, None)
         if exec_func is None:
             raise NotImplementedErrorDBAPI(f'StatementType {self._statementType.name} not implemented')
@@ -643,14 +667,19 @@
         self._fetch_done = False
         self._output_parameter_list = None
 
         self._lastrowid = None
 
         self._closed = False
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        if sqlcode in [0, 100]:
+            return
+        super()._process_sqlcode(sqlcode, self._get_error_info(sqlcode))
+
     def _get_cached_info(self):
         if not self._connection._preparedCache or not hasattr(self._connection._preparedCache, '__iter__'):
             return False
         if self._parsed_statement in self._connection._preparedCache:
             self._prepare_cached(self._connection._preparedCache[self._parsed_statement])
             return True
         else:
@@ -730,15 +759,15 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
             sqlcode = self._in_message.wire.header._get_function_code()
             if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+                raise DatabaseError(self._get_error_info(sqlcode))
 
         # process metadata
         try:
             if self._connection._isFastOption():
                 self._check_statement_feature(self._in_message.wire)
             else:
                 self.statementFeatureOption = Feature.optionNone
@@ -910,16 +939,15 @@
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
             self._handle_error_504(self._sqlcode)
             if self._sqlcode == 404:
                 return
-            if self._sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
         self._current_wire = self._in_message.wire
         self._result_set = [self._current_wire]
         self._rs_index = 0
         
         self._rowcount = -1
 
@@ -944,15 +972,15 @@
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
                 if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                    raise DatabaseError(self._get_error_info(sqlcode))
 
                 self._process_stored_procedure_metadata(self._in_message.wire, True)
                 if self._multiple_result_sets:
                     # todo
                     return
 
                 self._cache_prepared_statement()
@@ -993,30 +1021,29 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
-                if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                self._process_sqlcode(sqlcode)
 
                 if self._connection._isFastOption():
                     self._check_statement_feature(self._in_message.wire)
                 else:
                     self.statementFeatureOption = Feature.optionNone
                 self._get_column_info(self._in_message.wire)
                 self._get_parameter_info(self._in_message.wire)
                 self._cache_prepared_statement()
 
                 # retrieve data
                 self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
                 if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))
+                    raise DatabaseError(self._get_error_info(self._sqlcode))
 
             except IndexError:
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
 
         self._current_wire = self._in_message.wire
@@ -1044,22 +1071,19 @@
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
-            sqlcode = self._in_message.wire.header._get_function_code()
-            if sqlcode == 404:
+            self._sqlcode = self._in_message.wire.header._get_function_code()
+            if self._sqlcode == 404:
                 self._update404()
                 return
-            if sqlcode == 119:
-                raise IntegrityError(self._get_error_info(sqlcode))
-            if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
     def _send_direct_update_request(self):
         # send DU message
         with self._connection._lock:
             self._statement_id = self._connection._get_new_statement_id()
             # message header
             self._out_message.wire._write_header(_Message.DIRECT_UPDATE)
@@ -1078,16 +1102,15 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve response
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
-                if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))
+                self._process_sqlcode(self._sqlcode)
 
                 addToCache = self._get_parameter_info(self._in_message.wire)
                 
                 notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
                                   and self._statementType != StatementType.DDL_OTHER)
                 if notDDL and addToCache:
                     self._cache_prepared_statement()
@@ -1110,17 +1133,16 @@
             
             # send message
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
-            self._sqlcode = self._in_message.wire.header._get_function_code()
-            if self._sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            sqlcode = self._in_message.wire.header._get_function_code()
+            self._process_sqlcode(sqlcode)
 
             self._process_stored_procedure_metadata(self._in_message.wire, False)
             if self._multiple_result_sets:
                 return
         self._cache_prepared_statement()
         return
 
@@ -1276,16 +1298,15 @@
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
-            if self._sqlcode not in [0, 100,]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 404:
                 self._update404(404)
             else:
                 self._get_output_parameters(self._in_message.wire)
         return
 
     def _stored_procedure_query(self):
@@ -1315,14 +1336,15 @@
                 return
             elif self._sqlcode == 100:
                 self._handle_error_100(100)
                 return
             self._get_output_parameters(self._in_message.wire)
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 100:
                 self._handle_error_100(100)
 
             self._current_wire = self._in_message.wire
             self._result_set = [self._current_wire]
             self._rs_index = 0
 
@@ -1619,15 +1641,15 @@
         # with self._connection._lock:
         #     self._out_message.wire._write_header(_Message.GET_AUTO_GENERATED_KEYS)
         #     sequence_number = self._connection._get_new_sequence_number()
         #     self._out_message._send(sequence_number)
         #     self._in_message._read_message_sql(sequence_number)
         #     self._sqlcode = self._in_message.wire.header._get_function_code()
         #     if self._sqlcode != 100:
-        #         raise InterfaceError(self._get_error_info(self._sqlcode))
+        #         raise DatabaseError(self._get_error_info(self._sqlcode))
         #     self._get_column_info(self._in_message.wire)
         #     self._lastrowid = self._in_message.wire._get()
 
         self.execute('SELECT LAST_IDENTITY()')
         self._lastrowid = self.fetchone()[0]
         return self._lastrowid
 
@@ -1778,16 +1800,15 @@
                 intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
 
                 sequence_number = self._connection._get_new_sequence_number()
                 self._out_message._send(sequence_number)
 
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
-                if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))                
+                self._process_sqlcode(self._sqlcode)
             self._result_set.append(self._in_message.wire)
 
         if self._sqlcode == 404:
             self._query404()
             return
 
         if self._rs_index + 1 == len(self._result_set):
@@ -1892,23 +1913,24 @@
                 self._scroll_flag = False
             else:
                 if self.fetchone_helper():
                     retval = self._rsrow._offsets
 
         if retval is None:
             return retval
-        return retval[:]
+        return retval.as_tuple()
+        # return tuple(retval[:])
 
     def fetchmany(self, size = None):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if size is None:
                 size = self.arraysize
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     for i in range(size):
                         row = self._warehouse[self._cursor_ptr]
@@ -1933,24 +1955,24 @@
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.fetchone()
             if row is None:
                 break
-            rows.append(row[:])
+            rows.append(row)
         return rows
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     while 1:
                         row = self._warehouse[self._cursor_ptr]
                         rows.append(row[:])
                         if self._cursor_ptr + 1 >= len(self._warehouse):
@@ -1969,15 +1991,16 @@
                     self._cursor_ptr += 1
                 return rows
         
         rows = []
         while self._current_wire is not None:
             row = self.fetchone()
             if not row: break
-            rows.append(row[:])
+            rows.append(row)
+        
         return rows
 
 class EmbdeddedCursor(_BaseCursor):
     embedded = True
     _result_set = None
 
     def __init__(self, connection: _IRISEmbedded) -> None:
@@ -2040,20 +2063,14 @@
                 _column_info.isHidden,
                 _column_info.isIdentity,
                 _column_info.isKeyColumn,
                 _column_info.isRowId,
             ]
             self._columns.append(intersystems_iris.dbapi._Column._Column(name, odbctype, precision, scale, nullable, label, tableName, schema, catalog, additionalData, slotPosition))
 
-    def _process_sqlcode(self, sqlcode, message):
-        if sqlcode == -119:
-            raise IntegrityError(message)
-        if sqlcode not in [0, 100]:
-            raise InterfaceError(message)
-
     @property
     def lastrowid(self):
         return self._lastrowid
 
     def _prepare_new(self):
         statement = self._parsed_statement
         sqlcode = 0
@@ -2157,33 +2174,34 @@
         return self._rowcount
         
     def fetchone(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         try:
-            row = self._result_set.__next__()
+            values = self._result_set.__next__()
         except:
             return None
 
-        row = [None if v == '' else '' if v == '\x00' else v for v in row]
+        values = [None if v == '' else '' if v == '\x00' else v for v in values]
+        row = namedtuple('Row', [col.name for col in self._columns], rename=True)
 
         _types = {
             SQLType.BIGINT: int,
             SQLType.BINARY: bytes,
             SQLType.BIT: bool,
             SQLType.INTEGER: int,
             SQLType.VARCHAR: str,
             SQLType.LONGVARBINARY: IRISBinaryStream,
             SQLType.LONGVARCHAR: IRISStream,
         }
         
         if self._columns:
             for _column in self._columns:
-                value = row[_column.slotPosition - 1]
+                value = values[_column.slotPosition - 1]
 
                 ctype = _column.type
                 value_type = _types[ctype] if ctype in _types else None
                 try:
                     if type(value) == float:
                         value = decimal.Decimal(str(value))
                     elif not _column.tableName and not _column.schema:
@@ -2194,16 +2212,16 @@
                         stream = value_type(self._connection, value, embedded=True)
                         value = stream.fetch()
                     elif not isinstance(value, value_type):
                         value = value_type(value)
                 except Exception as ex:
                     raise ex
                     pass
-                row[_column.slotPosition - 1] = value
-        return row
+                values[_column.slotPosition - 1] = value
+        return row(*values)
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         rows = []
         while True:
```

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_Descriptor.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_IRISStream.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_Message.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_Parameter.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_ParameterCollection.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_ResultSetRow.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+from datetime import datetime
+from collections import namedtuple
 from ._SQLType import SQLType
 from .._DBList import _DBList
 from .._ListItem import _ListItem
 from ._IRISStream import IRISStream, IRISBinaryStream
 from ._Column import _Column
 
+def from_timestamp_posix(posix):
+    time = int(posix)
+    if time > 0:
+        time ^= 0x1000000000000000 
+    else:
+        time |= 0xF000000000000000 
+
+    time /= 1000000
+
+    value = datetime.utcfromtimestamp(time).replace(tzinfo=None)
+    return value
+
 class _ResultSetRow:
     _locale = "latin-1"
     _connection = None
 
     def __init__(self, connection, columns=None, rowcount=0, ):
         self._connection = connection
         # index from user-inputted columns to columns received from server
@@ -105,14 +119,19 @@
             self._locale = rsrow._locale
 
         def __getattr__(self, key):
             return self.__getitem__(key)
 
         def get(self):
             return self[:]
+        
+        def as_tuple(self):
+            row = namedtuple('Row', [col.name for col in self._columns], rename=True)
+            values = self[:]
+            return row(*values)
 
         def __getitem__(self, key):
             if isinstance(key, str):
                 key = key.lower()
                 if key not in self._name_dict_keys:
                     raise KeyError("Column '" + key + "' does not exist")
                 return self[self._name_dict[key][0] + 1]
@@ -134,14 +153,17 @@
                 self._list_item.next_offset = self._offsets[key]
                 _DBList._get_list_element(self._list_item)
                 item = _DBList._get(self._list_item, self._locale)
                 _column: _Column = self._columns[idx]
                 ctype = _column.type
                 value_type = self._types[ctype] if ctype in self._types else None
                 try:
+                    if ctype == SQLType.TIMESTAMP_POSIX:
+                        item = from_timestamp_posix(item)
+
                     if _column.tableName == 'None' and _column.schema == 'None':
                         # Ignore for anonymous tables
                         pass
                     elif item is None:
                         pass
                     elif issubclass(value_type, IRISStream):
                         stream = value_type(self._connection, item)
```

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/_SQLType.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_PreParser.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import functools
 import enum
 import intersystems_iris._IRISList
 import intersystems_iris.dbapi._DBAPI
 import intersystems_iris.dbapi._Parameter
 import intersystems_iris.dbapi.preparser._Token
 import intersystems_iris.dbapi.preparser._TokenList
@@ -753,15 +754,18 @@
         #  Do a table lookup to identify token
         if t_strIDUpper in self.s_KeywordTable:
             #  Found it, replace ID with specific type
             t_eToken = self.s_KeywordTable[t_strIDUpper]
             if (t_eToken == TOKEN.NOT):
                 t_strID = self.m_Scanner.checkForNotPredicates()
                 t_strIDUpper = t_strID.upper()
-        self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
+        if t_strID == '%s':
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(TOKEN.QUESTION_MARK, "?"))
+        else:
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
 
     # used for various operators
     def Tokenize_op(self, check_tokens = [ParseToken.tokEQUAL]):
         self.m_Scanner.BeginLexeme()
         if self.m_Scanner.PeekNextToken() in check_tokens:
             # Check for composite operators (e.g. <=, >=, !=, etc.)
             self.m_Scanner.NextToken()
```

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_Scanner.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_Token.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/dbapi/preparser/_TokenList.py` & `irissqlcli-0.5.2b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_BusinessHost.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_BusinessOperation.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_BusinessProcess.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_BusinessService.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_Common.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_Director.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_IRISBusinessService.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_IRISOutboundAdapter.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_InboundAdapter.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/_OutboundAdapter.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/intersystems_iris/pex/__init__.py` & `irissqlcli-0.5.2b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/iris/__init__.py` & `irissqlcli-0.5.2b1/iris/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from sys import path as __syspath
 import os
 
 # check for install dir in environment
 # environment to check is IRISINSTALLDIR
 # if not found, raise exception and exit
-installdir = os.environ.get('IRISINSTALLDIR')
+# ISC_PACKAGE_INSTALLDIR - defined by default in Docker images
+installdir = os.environ.get('IRISINSTALLDIR') or os.environ.get('ISC_PACKAGE_INSTALLDIR')
 if installdir is None:
         raise Exception("""Cannot find InterSystems IRIS installation directory
     Please set IRISINSTALLDIR environment variable to the InterSystems IRIS installation directory""")
 
 # join the install dir with the bin directory
 __syspath.append(os.path.join(installdir, 'bin'))
 # also append lib/python
```

### Comparing `irissqlcli-0.5.1/iris/irisbuiltins.py` & `irissqlcli-0.5.2b1/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/iris/irisloader.py` & `irissqlcli-0.5.2b1/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irisnative/_IRISNative.py` & `irissqlcli-0.5.2b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/clitoolbar.py` & `irissqlcli-0.5.2b1/irissqlcli/clitoolbar.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/completion_refresher.py` & `irissqlcli-0.5.2b1/irissqlcli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/config.py` & `irissqlcli-0.5.2b1/irissqlcli/config.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/irissqlclirc` & `irissqlcli-0.5.2b1/irissqlcli/irissqlclirc`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/key_bindings.py` & `irissqlcli-0.5.2b1/irissqlcli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/magic.py` & `irissqlcli-0.5.2b1/irissqlcli/magic.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/main.py` & `irissqlcli-0.5.2b1/irissqlcli/main.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/completion_engine.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/completion_engine.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/encodingutils.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/encodingutils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/filepaths.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/filepaths.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/parseutils.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/parseutils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/prompt_utils.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/special/dbcommands.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/special/dbcommands.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/special/favoritequeries.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/special/iocommands.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/special/iocommands.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/special/main.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/packages/special/utils.py` & `irissqlcli-0.5.2b1/irissqlcli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/sqlcompleter.py` & `irissqlcli-0.5.2b1/irissqlcli/sqlcompleter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/sqlexecute.py` & `irissqlcli-0.5.2b1/irissqlcli/sqlexecute.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli/style.py` & `irissqlcli-0.5.2b1/irissqlcli/style.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/irissqlcli.egg-info/PKG-INFO` & `irissqlcli-0.5.2b1/irissqlcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irissqlcli
-Version: 0.5.1
+Version: 0.5.2b1
 Summary: CLI for SQL of InterSystems IRIS Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/caretdev/irissqlcli
 Author: CaretDev
 Author-email: irissqlcli@caretdev.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `irissqlcli-0.5.1/irissqlcli.egg-info/SOURCES.txt` & `irissqlcli-0.5.2b1/irissqlcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/setup.py` & `irissqlcli-0.5.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.1/tests/test_main.py` & `irissqlcli-0.5.2b1/tests/test_main.py`

 * *Files identical despite different names*

