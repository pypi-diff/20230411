# Comparing `tmp/constellate-0.6.9-py2.py3-none-any.whl.zip` & `tmp/constellate-0.6.90-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,81 +1,163 @@
-Zip file size: 43511 bytes, number of entries: 79
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/concurrency/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/concurrency/pebble/__init__.py
--rw-r--r--  2.0 unx     2265 b- defN 21-Oct-18 17:41 constellate/concurrency/pebble/pool_cleanup.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/concurrency/std/__init__.py
--rw-r--r--  2.0 unx      591 b- defN 21-Oct-18 17:41 constellate/concurrency/std/pool.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/constant/__init__.py
--rw-r--r--  2.0 unx      195 b- defN 21-Oct-18 17:41 constellate/constant/concurrency.py
--rw-r--r--  2.0 unx       22 b- defN 21-Oct-18 17:41 constellate/constant/debug.py
--rw-r--r--  2.0 unx      102 b- defN 21-Oct-18 17:41 constellate/constant/platform.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/container/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/container/orchestration/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/container/orchestration/k8s/__init__.py
--rw-r--r--  2.0 unx      447 b- defN 21-Oct-18 17:41 constellate/container/orchestration/k8s/probe.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/cryptography/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/cryptography/digest/__init__.py
--rw-r--r--  2.0 unx      223 b- defN 21-Oct-18 17:41 constellate/cryptography/digest/hexadecimal.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/migration/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 21-Oct-18 17:41 constellate/database/migration/databasetype.py
--rw-r--r--  2.0 unx     6136 b- defN 21-Oct-18 17:41 constellate/database/migration/migrate.py
--rw-r--r--  2.0 unx      549 b- defN 21-Oct-18 17:41 constellate/database/migration/migration_step.py
--rw-r--r--  2.0 unx      114 b- defN 21-Oct-18 17:41 constellate/database/migration/migrationaction.py
--rw-r--r--  2.0 unx       46 b- defN 21-Oct-18 17:41 constellate/database/migration/migrationerror.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/__init__.py
--rw-r--r--  2.0 unx      946 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/multienginesession.py
--rw-r--r--  2.0 unx      180 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/relationshiptype.py
--rw-r--r--  2.0 unx      127 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sessiontype.py
--rw-r--r--  2.0 unx    37060 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sqlalchemy.py
--rw-r--r--  2.0 unx      944 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sqlalchemydbconfig.py
--rw-r--r--  2.0 unx      896 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
--rw-r--r--  2.0 unx     5578 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sqlalchemypostgresql.py
--rw-r--r--  2.0 unx     8610 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/sqlalchemysqlite3.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/exception/__init__.py
--rw-r--r--  2.0 unx       42 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/exception/vacumexception.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/utils/__init__.py
--rw-r--r--  2.0 unx     1320 b- defN 21-Oct-18 17:41 constellate/database/sqlalchemy/utils/sql_query.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/database/sqlite3/__init__.py
--rw-r--r--  2.0 unx     1578 b- defN 21-Oct-18 17:41 constellate/database/sqlite3/sqlite3.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/datatype/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/datatype/enum/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 21-Oct-18 17:41 constellate/datatype/enum/enum.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/debug/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/debug/packages/__init__.py
--rw-r--r--  2.0 unx       88 b- defN 21-Oct-18 17:41 constellate/debug/packages/package.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/debugger/__init__.py
--rw-r--r--  2.0 unx     1156 b- defN 21-Oct-18 17:41 constellate/debugger/debugger.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/logger/__init__.py
--rw-r--r--  2.0 unx    17919 b- defN 21-Oct-18 17:41 constellate/logger/log.py
--rw-r--r--  2.0 unx     2929 b- defN 21-Oct-18 17:41 constellate/logger/loggers.py
--rw-r--r--  2.0 unx      652 b- defN 21-Oct-18 17:41 constellate/logger/logmode.py
--rw-r--r--  2.0 unx     2453 b- defN 21-Oct-18 17:41 constellate/logger/simple.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/logger/handler/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 21-Oct-18 17:41 constellate/logger/handler/forwarderhandler.py
--rw-r--r--  2.0 unx      569 b- defN 21-Oct-18 17:41 constellate/logger/handler/stringhandler.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/network/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/network/download/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/network/url/__init__.py
--rw-r--r--  2.0 unx      249 b- defN 21-Oct-18 17:41 constellate/network/url/unshortener.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/pretty/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/pretty/log/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 21-Oct-18 17:41 constellate/pretty/log/line.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/project/__init__.py
--rw-r--r--  2.0 unx      241 b- defN 21-Oct-18 17:41 constellate/project/version.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/resource/__init__.py
--rw-r--r--  2.0 unx     1963 b- defN 21-Oct-18 17:41 constellate/resource/resource.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/storage/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/anyfs/__init__.py
--rw-r--r--  2.0 unx      127 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/anyfs/availability.py
--rw-r--r--  2.0 unx     2914 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/anyfs/path.py
--rw-r--r--  2.0 unx      250 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/anyfs/size.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/tmpfs/__init__.py
--rw-r--r--  2.0 unx      953 b- defN 21-Oct-18 17:41 constellate/storage/filesystem/tmpfs/rambacked.py
--rw-rw-rw-  2.0 unx       47 b- defN 21-Oct-18 17:41 constellate-0.6.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     1592 b- defN 21-Oct-18 17:41 constellate-0.6.9.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Oct-18 17:41 constellate-0.6.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 21-Oct-18 17:41 constellate-0.6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7457 b- defN 21-Oct-18 17:41 constellate-0.6.9.dist-info/RECORD
-79 files, 111045 bytes uncompressed, 31197 bytes compressed:  71.9%
+Zip file size: 109861 bytes, number of entries: 161
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/py.typed
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/compression/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/compression/zip/__init__.py
+-rw-r--r--  2.0 unx     2575 b- defN 23-Apr-11 18:37 constellate/compression/zip/zip.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/concurrency/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/concurrency/asyncio/__init__.py
+-rw-r--r--  2.0 unx     3009 b- defN 23-Apr-11 18:37 constellate/concurrency/asyncio/tasks.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/concurrency/pebble/__init__.py
+-rw-r--r--  2.0 unx     2695 b- defN 23-Apr-11 18:37 constellate/concurrency/pebble/pool_cleanup.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/concurrency/simple/__init__.py
+-rw-r--r--  2.0 unx     4056 b- defN 23-Apr-11 18:37 constellate/concurrency/simple/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/concurrency/std/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 23-Apr-11 18:37 constellate/concurrency/std/pool.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/constant/__init__.py
+-rw-r--r--  2.0 unx      195 b- defN 23-Apr-11 18:37 constellate/constant/concurrency.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 18:37 constellate/constant/debug.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Apr-11 18:37 constellate/constant/platform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/container/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/container/orchestration/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/container/orchestration/k8s/__init__.py
+-rw-r--r--  2.0 unx      447 b- defN 23-Apr-11 18:37 constellate/container/orchestration/k8s/probe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/cryptography/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/cryptography/digest/__init__.py
+-rw-r--r--  2.0 unx     1809 b- defN 23-Apr-11 18:37 constellate/cryptography/digest/hexadecimal.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/common/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Apr-11 18:37 constellate/database/common/databasetype.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/migration/__init__.py
+-rw-r--r--  2.0 unx      697 b- defN 23-Apr-11 18:37 constellate/database/migration/constant.py
+-rw-r--r--  2.0 unx     2220 b- defN 23-Apr-11 18:37 constellate/database/migration/metadata.py
+-rw-r--r--  2.0 unx     6720 b- defN 23-Apr-11 18:37 constellate/database/migration/migrate.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Apr-11 18:37 constellate/database/migration/migrationcontext.py
+-rw-r--r--  2.0 unx     9565 b- defN 23-Apr-11 18:37 constellate/database/migration/migrationstep.py
+-rw-r--r--  2.0 unx      372 b- defN 23-Apr-11 18:37 constellate/database/migration/tablecontext.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/migration/standard/__init__.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Apr-11 18:37 constellate/database/migration/standard/base.py
+-rw-r--r--  2.0 unx    22358 b- defN 23-Apr-11 18:37 constellate/database/migration/standard/migrate.py
+-rw-r--r--  2.0 unx     2492 b- defN 23-Apr-11 18:37 constellate/database/migration/standard/table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sparql/__init__.py
+-rw-r--r--  2.0 unx      606 b- defN 23-Apr-11 18:37 constellate/database/sparql/query.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sparql/sparqlburger/__init__.py
+-rw-r--r--  2.0 unx      553 b- defN 23-Apr-11 18:37 constellate/database/sparql/sparqlburger/triple.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/__init__.py
+-rw-r--r--  2.0 unx      180 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/relationshiptype.py
+-rw-r--r--  2.0 unx    31998 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemy.py
+-rw-r--r--  2.0 unx      810 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemydbconfig.py
+-rw-r--r--  2.0 unx     1477 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
+-rw-r--r--  2.0 unx     1004 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemyengineconfig.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
+-rw-r--r--  2.0 unx    12746 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemypostgresql.py
+-rw-r--r--  2.0 unx     9931 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sqlalchemysqlite3.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/crud/__init__.py
+-rw-r--r--  2.0 unx     6047 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/crud/cru.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/exception/__init__.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/exception/migrationexception.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/exception/vacumexception.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/execution/__init__.py
+-rw-r--r--  2.0 unx     7580 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/execution/execute.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/schema/__init__.py
+-rw-r--r--  2.0 unx     1462 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/schema/create.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/schema/drop.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/schema/setsearchpath.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/table/__init__.py
+-rw-r--r--  2.0 unx     2321 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/table/drop.py
+-rw-r--r--  2.0 unx     3585 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/table/presence.py
+-rw-r--r--  2.0 unx     1105 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/expression/table/truncate.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/__init__.py
+-rw-r--r--  2.0 unx     6092 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/multienginesession.py
+-rw-r--r--  2.0 unx     3722 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/syncmultienginesession.py
+-rw-r--r--  2.0 unx     3097 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/binder/__init__.py
+-rw-r--r--  2.0 unx     1813 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/session/binder/binderresolver.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sharding/__init__.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sharding/sharder.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sharding/shardoption.py
+-rw-r--r--  2.0 unx     2468 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sharding/simplesession.py
+-rw-r--r--  2.0 unx     2103 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/sharding/unittoshardmixin.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/typedecorator/__init__.py
+-rw-r--r--  2.0 unx      756 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/typedecorator/enuminteger.py
+-rw-r--r--  2.0 unx      755 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/typedecorator/enumstring.py
+-rw-r--r--  2.0 unx     2097 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/typedecorator/enumvalue.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/typedecorator/timestamptz.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/types/__init__.py
+-rw-r--r--  2.0 unx    16084 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/types/composite.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/utils/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/utils/sessioncommit.py
+-rw-r--r--  2.0 unx     1681 b- defN 23-Apr-11 18:37 constellate/database/sqlalchemy/utils/sql_query.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/database/sqlite3/__init__.py
+-rw-r--r--  2.0 unx     1932 b- defN 23-Apr-11 18:37 constellate/database/sqlite3/sqlite3.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/datatype/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/datatype/dictionary/__init__.py
+-rw-r--r--  2.0 unx      383 b- defN 23-Apr-11 18:37 constellate/datatype/dictionary/pop.py
+-rw-r--r--  2.0 unx      663 b- defN 23-Apr-11 18:37 constellate/datatype/dictionary/update.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/datatype/enum/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Apr-11 18:37 constellate/datatype/enum/enum.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/datetime/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/datetime/timeinterval/__init__.py
+-rw-r--r--  2.0 unx    11006 b- defN 23-Apr-11 18:37 constellate/datetime/timeinterval/timeinterval.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/debug/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/debug/packages/__init__.py
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-11 18:37 constellate/debug/packages/package.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/debugger/__init__.py
+-rw-r--r--  2.0 unx     1374 b- defN 23-Apr-11 18:37 constellate/debugger/debugger.py
+-rw-r--r--  2.0 unx      737 b- defN 23-Apr-11 18:37 constellate/debugger/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/logger/__init__.py
+-rw-r--r--  2.0 unx    18630 b- defN 23-Apr-11 18:37 constellate/logger/log.py
+-rw-r--r--  2.0 unx     3980 b- defN 23-Apr-11 18:37 constellate/logger/loggers.py
+-rw-r--r--  2.0 unx      652 b- defN 23-Apr-11 18:37 constellate/logger/logmode.py
+-rw-r--r--  2.0 unx     3050 b- defN 23-Apr-11 18:37 constellate/logger/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/logger/handler/__init__.py
+-rw-r--r--  2.0 unx      562 b- defN 23-Apr-11 18:37 constellate/logger/handler/forwarderhandler.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-11 18:37 constellate/logger/handler/stringhandler.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/network/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/network/download/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/network/url/__init__.py
+-rw-r--r--  2.0 unx      248 b- defN 23-Apr-11 18:37 constellate/network/url/unshortener.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/package/__init__.py
+-rw-r--r--  2.0 unx      173 b- defN 23-Apr-11 18:37 constellate/package/package.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/pretty/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/pretty/log/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Apr-11 18:37 constellate/pretty/log/line.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/progression/__init__.py
+-rw-r--r--  2.0 unx     1013 b- defN 23-Apr-11 18:37 constellate/progression/progres.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/project/__init__.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Apr-11 18:37 constellate/project/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/resource/__init__.py
+-rw-r--r--  2.0 unx     2206 b- defN 23-Apr-11 18:37 constellate/resource/resource.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/storage/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/anyfs/__init__.py
+-rw-r--r--  2.0 unx      127 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/anyfs/availability.py
+-rw-r--r--  2.0 unx     3186 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/anyfs/path.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/anyfs/size.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/tmpfs/__init__.py
+-rw-r--r--  2.0 unx     2029 b- defN 23-Apr-11 18:37 constellate/storage/filesystem/tmpfs/rambacked.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/__init__.py
+-rw-r--r--  2.0 unx      596 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/accessor/__init__.py
+-rw-r--r--  2.0 unx     3173 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/accessor/attribute_accessor.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/extra/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/extra/sanitize/__init__.py
+-rw-r--r--  2.0 unx    11089 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/extra/sanitize/sanitize.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/io/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/io/sql/__init__.py
+-rw-r--r--  2.0 unx     2570 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/io/sql/sqlalchemy.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/validation/__init__.py
+-rw-r--r--  2.0 unx      624 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/validation/pandera.py
+-rw-r--r--  2.0 unx     6050 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandas/validation/validation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandera/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Apr-11 18:37 constellate/thirdparty/pandera/inspector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/virtualization/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/virtualization/common/__init__.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Apr-11 18:37 constellate/virtualization/common/common.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 18:37 constellate/virtualization/docker/__init__.py
+-rw-rw-rw-  2.0 unx       47 b- defN 23-Apr-11 18:38 constellate-0.6.90.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3273 b- defN 23-Apr-11 18:38 constellate-0.6.90.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-11 18:38 constellate-0.6.90.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 18:38 constellate-0.6.90.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    16017 b- defN 23-Apr-11 18:38 constellate-0.6.90.dist-info/RECORD
+161 files, 297126 bytes uncompressed, 83321 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,19 +1,43 @@
 Filename: constellate/__init__.py
 Comment: 
 
+Filename: constellate/py.typed
+Comment: 
+
+Filename: constellate/compression/__init__.py
+Comment: 
+
+Filename: constellate/compression/zip/__init__.py
+Comment: 
+
+Filename: constellate/compression/zip/zip.py
+Comment: 
+
 Filename: constellate/concurrency/__init__.py
 Comment: 
 
+Filename: constellate/concurrency/asyncio/__init__.py
+Comment: 
+
+Filename: constellate/concurrency/asyncio/tasks.py
+Comment: 
+
 Filename: constellate/concurrency/pebble/__init__.py
 Comment: 
 
 Filename: constellate/concurrency/pebble/pool_cleanup.py
 Comment: 
 
+Filename: constellate/concurrency/simple/__init__.py
+Comment: 
+
+Filename: constellate/concurrency/simple/simple.py
+Comment: 
+
 Filename: constellate/concurrency/std/__init__.py
 Comment: 
 
 Filename: constellate/concurrency/std/pool.py
 Comment: 
 
 Filename: constellate/constant/__init__.py
@@ -48,86 +72,236 @@
 
 Filename: constellate/cryptography/digest/hexadecimal.py
 Comment: 
 
 Filename: constellate/database/__init__.py
 Comment: 
 
+Filename: constellate/database/common/__init__.py
+Comment: 
+
+Filename: constellate/database/common/databasetype.py
+Comment: 
+
 Filename: constellate/database/migration/__init__.py
 Comment: 
 
-Filename: constellate/database/migration/databasetype.py
+Filename: constellate/database/migration/constant.py
+Comment: 
+
+Filename: constellate/database/migration/metadata.py
 Comment: 
 
 Filename: constellate/database/migration/migrate.py
 Comment: 
 
-Filename: constellate/database/migration/migration_step.py
+Filename: constellate/database/migration/migrationcontext.py
 Comment: 
 
-Filename: constellate/database/migration/migrationaction.py
+Filename: constellate/database/migration/migrationstep.py
 Comment: 
 
-Filename: constellate/database/migration/migrationerror.py
+Filename: constellate/database/migration/tablecontext.py
 Comment: 
 
-Filename: constellate/database/sqlalchemy/__init__.py
+Filename: constellate/database/migration/standard/__init__.py
 Comment: 
 
-Filename: constellate/database/sqlalchemy/multienginesession.py
+Filename: constellate/database/migration/standard/base.py
 Comment: 
 
-Filename: constellate/database/sqlalchemy/relationshiptype.py
+Filename: constellate/database/migration/standard/migrate.py
+Comment: 
+
+Filename: constellate/database/migration/standard/table.py
+Comment: 
+
+Filename: constellate/database/sparql/__init__.py
+Comment: 
+
+Filename: constellate/database/sparql/query.py
+Comment: 
+
+Filename: constellate/database/sparql/sparqlburger/__init__.py
 Comment: 
 
-Filename: constellate/database/sqlalchemy/sessiontype.py
+Filename: constellate/database/sparql/sparqlburger/triple.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/relationshiptype.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/sqlalchemy.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/sqlalchemydbconfig.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/sqlalchemyengineconfig.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/sqlalchemypostgresql.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/sqlalchemysqlite3.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/crud/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/crud/cru.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/exception/__init__.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/exception/migrationexception.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/exception/vacumexception.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/execution/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/execution/execute.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/schema/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/schema/create.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/schema/drop.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/schema/setsearchpath.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/table/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/table/drop.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/table/presence.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/expression/table/truncate.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/multienginesession.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/syncmultienginesession.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/binder/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/session/binder/binderresolver.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sharding/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sharding/sharder.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sharding/shardoption.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sharding/simplesession.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/sharding/unittoshardmixin.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/typedecorator/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/typedecorator/enuminteger.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/typedecorator/enumstring.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/typedecorator/enumvalue.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/typedecorator/timestamptz.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/types/__init__.py
+Comment: 
+
+Filename: constellate/database/sqlalchemy/types/composite.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/utils/__init__.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/utils/sessioncommit.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/utils/sql_query.py
 Comment: 
 
 Filename: constellate/database/sqlite3/__init__.py
 Comment: 
 
 Filename: constellate/database/sqlite3/sqlite3.py
 Comment: 
 
 Filename: constellate/datatype/__init__.py
 Comment: 
 
+Filename: constellate/datatype/dictionary/__init__.py
+Comment: 
+
+Filename: constellate/datatype/dictionary/pop.py
+Comment: 
+
+Filename: constellate/datatype/dictionary/update.py
+Comment: 
+
 Filename: constellate/datatype/enum/__init__.py
 Comment: 
 
 Filename: constellate/datatype/enum/enum.py
 Comment: 
 
+Filename: constellate/datetime/__init__.py
+Comment: 
+
+Filename: constellate/datetime/timeinterval/__init__.py
+Comment: 
+
+Filename: constellate/datetime/timeinterval/timeinterval.py
+Comment: 
+
 Filename: constellate/debug/__init__.py
 Comment: 
 
 Filename: constellate/debug/packages/__init__.py
 Comment: 
 
 Filename: constellate/debug/packages/package.py
@@ -135,14 +309,17 @@
 
 Filename: constellate/debugger/__init__.py
 Comment: 
 
 Filename: constellate/debugger/debugger.py
 Comment: 
 
+Filename: constellate/debugger/simple.py
+Comment: 
+
 Filename: constellate/logger/__init__.py
 Comment: 
 
 Filename: constellate/logger/log.py
 Comment: 
 
 Filename: constellate/logger/loggers.py
@@ -171,23 +348,35 @@
 
 Filename: constellate/network/url/__init__.py
 Comment: 
 
 Filename: constellate/network/url/unshortener.py
 Comment: 
 
+Filename: constellate/package/__init__.py
+Comment: 
+
+Filename: constellate/package/package.py
+Comment: 
+
 Filename: constellate/pretty/__init__.py
 Comment: 
 
 Filename: constellate/pretty/log/__init__.py
 Comment: 
 
 Filename: constellate/pretty/log/line.py
 Comment: 
 
+Filename: constellate/progression/__init__.py
+Comment: 
+
+Filename: constellate/progression/progres.py
+Comment: 
+
 Filename: constellate/project/__init__.py
 Comment: 
 
 Filename: constellate/project/version.py
 Comment: 
 
 Filename: constellate/resource/__init__.py
@@ -216,23 +405,80 @@
 
 Filename: constellate/storage/filesystem/tmpfs/__init__.py
 Comment: 
 
 Filename: constellate/storage/filesystem/tmpfs/rambacked.py
 Comment: 
 
-Filename: constellate-0.6.9.dist-info/LICENSE
+Filename: constellate/thirdparty/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/accessor/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/accessor/attribute_accessor.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/extra/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/extra/sanitize/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/extra/sanitize/sanitize.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/io/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/io/sql/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/io/sql/sqlalchemy.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/validation/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/validation/pandera.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/validation/validation.py
+Comment: 
+
+Filename: constellate/thirdparty/pandera/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandera/inspector.py
+Comment: 
+
+Filename: constellate/virtualization/__init__.py
+Comment: 
+
+Filename: constellate/virtualization/common/__init__.py
+Comment: 
+
+Filename: constellate/virtualization/common/common.py
+Comment: 
+
+Filename: constellate/virtualization/docker/__init__.py
+Comment: 
+
+Filename: constellate-0.6.90.dist-info/LICENSE
 Comment: 
 
-Filename: constellate-0.6.9.dist-info/METADATA
+Filename: constellate-0.6.90.dist-info/METADATA
 Comment: 
 
-Filename: constellate-0.6.9.dist-info/WHEEL
+Filename: constellate-0.6.90.dist-info/WHEEL
 Comment: 
 
-Filename: constellate-0.6.9.dist-info/top_level.txt
+Filename: constellate-0.6.90.dist-info/top_level.txt
 Comment: 
 
-Filename: constellate-0.6.9.dist-info/RECORD
+Filename: constellate-0.6.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## constellate/concurrency/pebble/pool_cleanup.py

```diff
@@ -18,15 +18,14 @@
 def _pebble_cleanup_pool(
     force_shutdown: bool = False,
     pool: pebble.ProcessPool = None,
     futures: List[pebble.ProcessFuture] = [],
     post_cleanup: PostPebblePoolCleanup = None,
     logger: logging.Logger = None,
 ):
-
     # Cancel remaining tasks
     logger.debug(f"Cancelling tasks pool ...")
     for future in futures:
         if not future.done():
             future.cancel()
 
     if force_shutdown:
@@ -60,16 +59,25 @@
     force_shutdown: bool = False,
     logger=None,
     pool: pebble.ProcessPool = None,
     futures: List[pebble.ProcessFuture] = [],
     signals: Dict[int, str] = {signal.SIGINT: "SIGINT", signal.SIGTERM: "SIGTERM"},
     post_cleanup: PostPebblePoolCleanup = None,
 ):
-    """
-    Clean up pebble process pool on signals
+    """Clean up pebble process pool on signals
+
+    :param force_shutdown: bool:  (Default value = False)
+    :param logger:  (Default value = None)
+    :param pool: pebble.ProcessPool:  (Default value = None)
+    :param futures: List[pebble.ProcessFuture]:  (Default value = [])
+    :param signals: Dict[int:
+    :param str]:  (Default value = {signal.SIGINT: "SIGINT")
+    :param signal.SIGTERM: "SIGTERM"}:
+    :param post_cleanup: PostPebblePoolCleanup:  (Default value = None)
+
     """
 
     def _handler(signum, _frame):
         # logger.critical(f"Received {signals.get(signum, signum)} signal ...")
         _pebble_cleanup_pool(
             force_shutdown=force_shutdown,
             logger=logger,
```

## constellate/cryptography/digest/hexadecimal.py

```diff
@@ -1,11 +1,72 @@
 import hashlib
+from pathlib import Path
+from typing import Any, Union
 
+from blake3 import blake3
+from typing import Protocol
 
-def hex_sha256(value: str = None):
-    h = hashlib.sha256()
-    return _hex(value=value, hash=h)
 
+class Hasher(Protocol):
+    def hexdigest(self) -> str:
+        ...
 
-def _hex(value: str = None, hash=None):
-    hash.update(value.encode("utf-8"))
-    return hash.hexdigest()
+    def update(self, __data: Any) -> None:
+        ...
+
+
+def hasher(family: str = "sha256", **kwargs) -> Hasher:
+    """
+
+    :param family: str:  (Default value = "sha256")
+    :param **kwargs:
+
+    """
+    if family in hashlib.algorithms_available:
+        return hashlib.new(family)
+
+    family = family.lower()
+    if family == "blake3":
+        return blake3(**kwargs)
+    else:
+        raise NotImplementedError()
+
+
+_hasher_fn = hasher
+
+
+def hexadecimal(
+    family: str = None, hasher: Hasher = None, value: Union[str, bytes, Path] = None
+) -> str:
+    """
+
+    :param family: A digest algorithm supported by python standard lib (eg: sha256) or one of the custom ones: blake3.
+    :param hasher: A hasher created with `hasher(...)`
+    :param value: A value to digest
+    :param family: str:  (Default value = None)
+    :param hasher: Hasher:  (Default value = None)
+    :param value: Union[str:
+    :param bytes]:  (Default value = None)
+    :returns: s Message digest
+
+    """
+    if family is not None and isinstance(family, str):
+        hasher = _hasher_fn(family=family)
+    elif hasher is not None:
+        pass
+    else:
+        raise ValueError("Missing family or hasher")
+
+    if isinstance(value, str):
+        value = value.encode("utf-8")
+        hasher.update(value)
+    elif isinstance(value, bytes):
+        hasher.update(value)
+    elif isinstance(value, Path):
+        # Support: py38 and better
+        with open(value, "rb") as f:
+            while chunk := f.read(8192):
+                hasher.update(chunk)
+    else:
+        raise NotImplementedError()
+
+    return hasher.hexdigest()
```

## constellate/database/migration/migrate.py

```diff
@@ -1,160 +1,186 @@
+import contextlib
 import logging
-from logging import getLogger
-from pathlib import Path
-from typing import List
-
-from yoyo import read_migrations
-from yoyo import get_backend
-
-from constellate.database.migration.databasetype import DatabaseType
-from constellate.database.migration.migrationaction import MigrationAction
-from constellate.database.migration.migrationerror import MigrationException
-
-
-def _migrate_with_yoyo(
-    connection_url: str = None,
-    migration_dirs: List[Path] = [],
-    action: MigrationAction = MigrationAction.UNKNOWN,
-    logger: logging.Logger = None,
-):
-    """Run database migrations using yoyo library: https://ollycope.com/software/yoyo/latest/#migrations-as-sql-scripts"""
+import urllib
+from typing import Any
+
+from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
+from sqlalchemy.orm import sessionmaker
+
+from constellate.database.common.databasetype import DatabaseType
+from constellate.database.migration.migrationcontext import (
+    MigrationContext,
+    ConnectionContext,
+    ConnectionResolution,
+)
+from constellate.database.migration.migrationstep import migration_steps
+from constellate.database.migration.standard.migrate import migrate as migrate_standard
+
+
+def edit_connection_url_schema(url: str = None, schema: str = None):
+    # FIXME (high) Is this still useful ?
+    url_parts = list(urllib.parse.urlparse(url))
+    query = dict(urllib.parse.parse_qsl(url_parts[4]))
+
+    if schema is not None:
+        query.update({"schema": schema})
 
-    class Handler(logging.Handler):
-        def __init__(self, level: int = logging.NOTSET, target_logger: logging.Logger = None):
-            super(Handler, self).__init__(level=level)
-            self._target_logger = target_logger
-
-        def emit(self, record: logging.LogRecord) -> None:
-            if self._target_logger is not None:
-                self._target_logger.log(level=record.levelno, msg=record.getMessage())
-
-        def flush(self) -> None:
-            if self._target_logger is not None:
-                for _handler in self._target_logger.handlers:
-                    _handler.flush()
-
-    handler = Handler(level=logging.DEBUG, target_logger=logger)
-    # Append temporary Handler to yoyo's library
-    yoyo_logger = getLogger("yoyo.migrations")
-    yoyo_logger.setLevel(logging.DEBUG)
-
-    backend = None
-    try:
-        yoyo_logger.addHandler(handler)
-
-        # Run migration
-        backend = get_backend(connection_url)
-        migrations = read_migrations(*[str(path) for path in migration_dirs])
-
-        with backend.lock():
-            if action == MigrationAction.UP:
-                # Apply any outstanding migrations
-                backend.apply_migrations(backend.to_apply(migrations))
-            elif action == MigrationAction.DOWN:
-                # Rollback all migrations
-                backend.rollback_migrations(backend.to_rollback(migrations))
-    except BaseException:
-        raise
-    finally:
-        # Remove lock, regardless of migration status
-        if backend is not None:
-            backend.break_lock()
-        yoyo_logger.removeHandler(handler)
-
-
-def _migrate_unsupported(
-    connection_url: str = None,
-    migration_dirs: List[Path] = [],
-    action: MigrationAction = MigrationAction.UNKNOWN,
+    url_parts[4] = urllib.parse.urlencode(query)
+
+    return urllib.parse.urlunparse(url_parts)
+
+
+async def _migrate_standard(
+    migration_context: MigrationContext = None,
+    user_context: Any = None,
     logger: logging.Logger = None,
-):
+) -> None:
+    @contextlib.asynccontextmanager
+    async def _create_session(migration_context: MigrationContext = None) -> AsyncSession:
+        connection_context = migration_context.connection_context
+        fn_session_create = None
+
+        # Create the session making function
+        for r in connection_context.resolution:
+            if (
+                r == ConnectionResolution.SESSION_CREATE
+                and connection_context.session_create is not None
+            ):
+                fn_session_create = connection_context.session_create
+                break
+            elif r == ConnectionResolution.SESSION and connection_context.session is not None:
+
+                @contextlib.asynccontextmanager
+                async def _create_default_session():
+                    logger.debug(f"Using session: {session}")
+                    yield session
+
+                fn_session_create = _create_default_session
+                break
+            elif r == ConnectionResolution.ENGINE and connection_context.engine is not None:
+
+                @contextlib.asynccontextmanager
+                async def _create_default_session():
+                    session_maker = sessionmaker(
+                        engine=connection_context.engine, class_=AsyncSession
+                    )
+                    async with session_maker() as session:
+                        logger.debug(
+                            f"Using session: {session} from engine {connection_context.engine}"
+                        )
+                        yield session
+
+                fn_session_create = _create_default_session
+                break
+            elif (
+                r == ConnectionResolution.CONNECTION_URL
+                and connection_context.connection_url is not None
+            ):
+
+                @contextlib.asynccontextmanager
+                async def _create_default_session():
+                    engine = create_async_engine(connection_context.connection_url)
+
+                    session_maker = sessionmaker(
+                        engine=connection_context.engine, class_=AsyncSession
+                    )
+                    try:
+                        async with session_maker() as session:
+                            logger.debug(
+                                f"Using session: {session} from engine {connection_context.engine} with url {connection_context.connection_url}"
+                            )
+                            yield session
+                    except BaseException as e:
+                        raise e
+                    finally:
+                        await engine.dispose()
+
+                fn_session_create = _create_default_session
+                break
+            else:
+                NotImplementedError(f"Create session from {r}")
+
+        async with fn_session_create() as session:
+            yield session
+
+    await migrate_standard(
+        migration_context=migration_context,
+        user_context=user_context,
+        fn_create_session=_create_session,
+        logger=logger,
+    )
+
+
+def _migrate_unsupported(**kwargs):
     raise NotImplementedError()
 
 
-def migrate(
-    database_type: DatabaseType = DatabaseType.UNKNOWN,
-    connection_url: str = None,
-    migration_dirs: List[Path] = [],
-    action: MigrationAction = MigrationAction.UNKNOWN,
+async def migrate(
+    migration_context: MigrationContext = None,
+    connection_context: ConnectionContext = None,
+    user_context: Any = None,
     logger: logging.Logger = None,
-):
+) -> None:
     """Run database migrations.
-    :migration_dirs: List of directory contains SQL file scripts (or equivalent)
-                     SQL file scripts must be named with script alphabetic order:
-                     - 0001.up.foobar.sql
-                     - 0001.down.foobar.sql
-                     - 0002.up.zoobar.sql
-                     - etc ...
+
+    m = MigrationContext(directory=d)
+    where directory = 1 level tree of directories, where each directory contains .py or .sql migration scripts.
+    Example: Each directory must contain 1+ sql/py file scripts.
+             SQL file scripts must be named with script alphabetic order (executed in the alphabetic order across all directories):
+               - 0001.up.foobar.sql
+               - 0001.down.foobar.sql
+               - 0002.up.zoobar.py
+               - 0002.down.zoobar.py
+               - etc ...
+
+    Each 1 level directory can have metadata in __init__.py:
+        from constellate.database.migration.constant import MigrationKind
+        migration_dir = Path(os.path.dirname(__file__))
+        kind = MigrationKind.SCHEMA
+        schema = 'schema_1'
+
+    Each SQL file can have metadata:
+        -- kind = ????
+        -- schema = 'schema_1'
+
+    Each Python file can have metadata and functions:
+        from constellate.database.migration.constant import MigrationKind
+        migration_dir = Path(os.path.dirname(__file__))
+        kind = MigrationKind.SCHEMA
+        schema = 'schema_1'
+
+        async def upgrade(**kwargs):
+            pass
+
+        async def downgrade(**kwargs):
+            pass
+
+    @param migration_context: Migration context
+    @param connection_context: Connection context
+    @param user_context: User specific context
     :raises:
-        MigrationException When migration fails
+        BaseException When migration fails
     """
-    DB_TYPE_TO_MIGRATOR = {
-        DatabaseType.SQLITE: _migrate_with_yoyo,
-        DatabaseType.POSTGRESQL: _migrate_with_yoyo,
-    }
-
-    try:
-        migrate = DB_TYPE_TO_MIGRATOR.get(database_type, _migrate_unsupported)
-        migrate(
-            connection_url=connection_url,
-            migration_dirs=migration_dirs,
-            action=action,
-            logger=logger,
-        )
-    except BaseException as e:
-        raise MigrationException() from e
-
-
-#
-# from pkg_resources import resource_listdir, resource_string
-# def migrate2(connection=None, logger=None):
-#     """Run database migrations."""
-#
-#     def get_script_version(filename) -> int:
-#         return int(filename.split("_")[0])
-#
-#     def get_current_version(connection, default_version=9999999):
-#         try:
-#             current_version = connection.execute("pragma user_version").fetchone()[0]
-#             return current_version
-#         except BaseException:
-#             return default_version
-#
-#     migrations_parent_pkg_dir = __package__
-#     migration_dir_name = "migrations"
-#
-#     # Retrieve list of incremental migration scripts, sorted by migration number ascending
-#     migration_files = resource_listdir(migrations_parent_pkg_dir, migration_dir_name)
-#     migration_version_to_files = {get_script_version(file): file for file in migration_files}
-#
-#     migration_versions = sorted(list(migration_version_to_files.keys()))
-#     logger.info(f"{len(migration_versions)} migration scripts available")
-#
-#     # Apply incremental migration scripts strictly above current db schema version
-#     for script_version in migration_versions:
-#         script_filename = migration_version_to_files.get(script_version, None)
-#
-#         current_version = get_current_version(connection)
-#         if script_version == current_version:
-#             logger.info(f"database currently at version {current_version}")
-#
-#         if script_version > current_version:
-#             logger.debug(f"migration being applied {script_version}")
-#             sql = resource_string(
-#                 migrations_parent_pkg_dir, f"{migration_dir_name}/{script_filename}"
-#             ).decode("utf-8")
-#             connection.executescript(sql)
-#             new_current_version = get_current_version(connection)
-#
-#             if new_current_version == script_version:
-#                 logger.info(f"database now upgraded to version {script_version}")
-#             else:
-#                 raise Exception(f"database failed migrate to version {script_version}")
-#
-#     # Verify the app's db is now at the version of the very last migration script available
-#     last_available_migration_version = (
-#         migration_versions[-1] if len(migration_versions) > 0 else current_version
-#     )
-#     assert (
-#         current_version == last_available_migration_version
-#     ), f"Database not migrated to most up to date version {last_available_migration_version}"
+    _migrate = {
+        DatabaseType.SQLITE: _migrate_standard,
+        DatabaseType.POSTGRESQL: _migrate_standard,
+    }.get(migration_context.database_type, _migrate_unsupported)
+
+    migration_context.connection_context = (
+        migration_context.connection_context or connection_context
+    )
+
+    if len(migration_context.steps) == 0:
+        # Auto populate some migration context steps properties
+        # - migration steps
+        kwargs = {}
+        if migration_context.migration_context_step_name:
+            kwargs.update(
+                {"migration_context_step_file_name": migration_context.migration_context_step_name}
+            )
+        migration_steps(migration_context=migration_context, **kwargs)
+
+    await _migrate(
+        migration_context=migration_context,
+        user_context=user_context,
+        logger=logger,
+    )
```

## constellate/database/sqlalchemy/sqlalchemy.py

```diff
@@ -1,30 +1,74 @@
 import asyncio
+import itertools
 import logging
-import pprint
 import time
 import warnings
 from contextlib import asynccontextmanager
-from random import random
-from typing import Dict, Tuple, List, Iterator, AsyncGenerator, Optional
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
+from typing import (
+    Dict,
+    Tuple,
+    List,
+    Iterator,
+    AsyncGenerator,
+    Optional,
+    Any,
+    Union,
+    Callable,
+    MutableMapping,
+)
 
+from deprecated.classic import deprecated
 from sqlalchemy import event, ForeignKeyConstraint
-from sqlalchemy.engine import Engine
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, AsyncSessionTransaction
+from sqlalchemy.ext.horizontal_shard import ShardedSession
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy.sql.expression import select
+from sqlalchemy.future import Select
+from sqlalchemy.orm.session import ORMExecuteState, Session
 
+from constellate.database.sqlalchemy.exception.migrationexception import MigrationException
 from constellate.database.sqlalchemy.exception.vacumexception import VacumException
-from constellate.database.sqlalchemy.multienginesession import MultiEngineSession
+from constellate.database.sqlalchemy.execution.execute import execute_scalar
 from constellate.database.sqlalchemy.relationshiptype import RelationshipType
-from constellate.database.sqlalchemy.sessiontype import SessionType
+
+from constellate.database.sqlalchemy.session.multienginesession import MultiEngineSession
+from constellate.database.sqlalchemy.session.syncmultienginesession import SyncMultiEngineSession
+from constellate.database.sqlalchemy.session.syncmultiengineshardsession import (
+    SyncMultiEngineShardSession,
+)
+from constellate.database.sqlalchemy.sharding.sharder import Sharder
+from constellate.database.sqlalchemy.sharding.simplesession import (
+    SimpleShardSession,
+    SyncSimpleShardSession,
+    SyncSimpleSession,
+)
+from constellate.database.sqlalchemy.sharding.shardoption import SetShardEngineOption
 from constellate.database.sqlalchemy.sqlalchemydbconfig import DBConfigType, SQLAlchemyDBConfig
 from constellate.database.sqlalchemy.sqlalchemydbconfigmanager import SQLAlchemyDbConfigManager
+from constellate.database.sqlalchemy.sqlalchemyengineconfig import _EngineConfig
+from constellate.datatype.dictionary.update import dict_update, DictCondition
+
+
+class _SQLAlchemyDBConfigLogger(logging.LoggerAdapter):
+    def __init__(self, logger: logging.Logger = None, extra: Dict = None):
+        super().__init__(logger, extra or {})
+
+    def process(
+        self, msg: Any, kwargs: MutableMapping[str, Any]
+    ) -> Tuple[Any, MutableMapping[str, Any]]:
+        identifier = self.extra.get("identifier")
+        return f"({identifier}) {msg}", kwargs
+
+
+def FILTER_LOGICAL_SHARD_BY_NOTHING(storage: Any, config: SQLAlchemyDBConfig) -> bool:
+    return True
 
 
-def _warn_no_per_engine_option_found(options: Dict):
+def _warn_no_per_engine_option_found(options: Dict) -> None:
     engines = options.get("engines", None)
     if engines is None:
         warnings.warn(
             "options must be configured per engine. {engines:[{your options here}]}",
             DeprecationWarning,
         )
 
@@ -33,75 +77,51 @@
     engines = options.get("engines", [])
     engines_ids = [e.get("id", None) for e in engines]
     if None in engines_ids:
         raise ValueError("1+ engine is missing field: id")
     return engines_ids
 
 
-def _get_engine_options(options: Dict) -> List[Dict]:
-    _warn_no_per_engine_option_found(options)
+def _get_engine_options(
+    options: Dict = None, ignore_no_per_engine_option: bool = False
+) -> List[Dict]:
+    if not ignore_no_per_engine_option:
+        _warn_no_per_engine_option_found(options)
 
     engines = options.get("engines", [])
     if len(engines) == 0:
         engines = [{"id": "default", **options}]
     return engines
 
 
-async def session_scope(
-    session_maker: sessionmaker = None, config=None, **kwargs
-) -> AsyncGenerator[AsyncSession, None]:
-    """Provide a transactional scope around a series of operations."""
-    # If config manager hold max 1 engine instance, then the session default bind is to that engine.
-    # Otherwise, the session bind is project implementation specific
-    configs = [s for s in kwargs.get("config_manager", [])]
-    configs = (
-        list(filter(lambda t: t[1].type == DBConfigType.INSTANCE, configs))
-        if len(configs) < 2
-        else configs
-    )
-    if config is not None:
-        session_maker.configure(bind=config.engine)
-    elif len(configs) == 1:
-        default_config = configs[0]
-        session_maker.configure(bind=default_config[1].engine)
-
-    session = session_maker(**kwargs)
-    try:
-        yield session
-        await session.commit()
-    except BaseException:
-        await session.rollback()
-        raise
-    finally:
-        await session.close()
-
-
 class SQLAlchemy:
-    """
-    Use SQLAlchemy to interact with db
+    """Use SQLAlchemy to interact with db
     Usage 1: With context manager
         s = SQLAlchemy()
         async with s.setup(...) as db:
-            await db.reflect_schema(...)
             async with db.session_scope(...) as session:
                 result = await session.execute(select(...)...)
 
     Usage 2: Without context manager
        s = SQLAlchemy()
        setup_options = await s.setup2(...)
-       await s.reflect_schema(...)
        session = await s.session_scope2(...)
        result = await session.execute(select(...)...)
        await s.dispose2(setup_options)
+
+
     """
 
     def __init__(self):
-        self._session_type = SessionType.UNKNOWN
         self._config_manager = SQLAlchemyDbConfigManager()
 
+    @property
+    def config_manager(self):
+        return self._config_manager
+
     def _engines(
         self, engine_options: List[Dict], types: List[DBConfigType] = [DBConfigType.INSTANCE]
     ) -> Iterator[Tuple[SQLAlchemyDBConfig, Dict]]:
         engine_id_to_options = {
             engine_options.get("id"): engine_options for engine_options in engine_options
         }
         instance_id_to_instances = {k: v for k, v in self._config_manager if v.type in types}
@@ -118,611 +138,316 @@
     async def setup(self, options: Dict = {}):
         """
         :options: See each _setup_engine_XXXX method for available options in addition to the options below
         - key: engines: Per engine options
         -- Key: type: "instance" (default) => SQLAlchemy will connect to it. "template" SQLAlchemy will use the config for later
         -- Key: id:str. Any string value except "default"
         -- Key: logger:logging.Logger. Default: None
+        -- Key: Dict. engine_execution_options: Default: None.
 
         Eg:
         options = {
             "engines": [
                 {
                     "type": "instance",
                     "id": "shard_main",
                     "logger": ...
+                    "engine_execution_options: : {...}
+                    "migration_priority": 0
                 },
                 {
                     "type": "template",
                     "id": "shard_slave",
-                    "logger": ...
+                    "logger": ...,
+                    "migration_priority": 1
                 }
             ]
         }
         """
         setup_engines_options = []
         try:
             setup_engines_options = await self.setup2(options=options)
             yield self
         finally:
-            await self.dispose2(setup_engines_options=setup_engines_options)
+            await self.__dispose_wrapper(
+                setup_engines_options=setup_engines_options, ignore_no_per_engine_option=True
+            )
 
     async def setup2(self, options: Dict = {}):
         setup_engines_options = []
-        for engine_options in _get_engine_options(options):
+        for engine_options in _get_engine_options(options=options):
             db_config_type = (
                 DBConfigType.INSTANCE
                 if engine_options.get("type", "instance") == "instance"
                 else DBConfigType.TEMPLATE
             )
 
-            if self._session_type == SessionType.UNKNOWN:
-                self._session_type = SessionType.MONO_ENGINE
-            elif self._session_type == SessionType.MONO_ENGINE:
-                self._session_type = SessionType.MULTI_ENGINE
-
             instance = SQLAlchemyDBConfig()
             instance.identifier = engine_options.get("id", None)
             instance.type = db_config_type
             instance.options = engine_options
-            instance.logger = engine_options.get(
-                "logger", logging.getLogger("constellate.sqlalchemy")
+            instance.logger = _SQLAlchemyDBConfigLogger(
+                engine_options.get("logger", logging.getLogger("constellate.sqlalchemy")),
+                {"identifier": instance.identifier},
             )
             instance.logger.debug(f"setup database context: started")
             if instance.type == DBConfigType.INSTANCE:
                 await self._setup(instance=instance, options=engine_options)
             instance.logger.debug(f"setup database context: completed")
             self._config_manager.update(instance=instance)
             setup_engines_options.append(engine_options)
 
         return setup_engines_options
 
     async def _setup(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
-        (
-            instance.connection_uri,
-            instance.connection_uri_plain,
-            instance.engine,
-            instance.sync_engine,
-        ) = await self._create_engine(options=options)
+        instance.engine_config = await self._create_engine(instance=instance, options=options)
 
-        await self._setup_engine_logging(instance=instance, engine=instance.engine, options=options)
+        await self._setup_engine_logging(
+            instance=instance, engine=instance.engine_config.engine, options=options
+        )
         await self._setup_engine_before_cursor_execute(
-            instance=instance, engine=instance.engine, options=options
+            instance=instance, engine=instance.engine_config.engine, options=options
         )
         await self._setup_engine_after_cursor_execute(
-            instance=instance, engine=instance.engine, options=options
+            instance=instance, engine=instance.engine_config.engine, options=options
         )
         await self._setup_engine_connection_connect(
-            instance=instance, engine=instance.engine, options=options
+            instance=instance, engine=instance.engine_config.engine, options=options
         )
         await self._setup_engine_connection_begin(
-            instance=instance, engine=instance.engine, options=options
+            instance=instance, engine=instance.engine_config.engine, options=options
         )
         await self._setup_engine_session_maker(instance=instance)
 
-    async def _create_engine(self, options: Dict = {}) -> Tuple[str, str, AsyncEngine, Engine]:
+    async def _create_engine(
+        self, instance: SQLAlchemyDBConfig, options: Dict = {}
+    ) -> _EngineConfig:
         raise NotImplementedError("Subclass must implemented")
 
     def _get_database_driver_name(self) -> Optional[str]:
         """
-        @return: If no driver, then None. Otherwise driver name
+
+
+        :returns: If no driver, then None. Otherwise driver name
+
         """
         return None
 
     async def _setup_engine_logging(
-        self, instance: SQLAlchemyDBConfig, engine: object = None, options: Dict = None
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
     ):
-        if options.get("is_production", False):
-            severity1 = logging.INFO if options.developer else logging.WARN
-            severity2 = logging.DEBUG if options.developer else logging.INFO
+        # Note: Log levels inspired from:
+        # https://docs.sqlalchemy.org/en/14/core/engines.html#configuring-logging
+        debug = options.get("debug", None)
+        if debug is not None:
+            severity1 = logging.INFO if debug.get("developer", False) else logging.WARN
+            severity2 = logging.DEBUG if debug.get("developer", False) else logging.INFO
             # Turn on SQL Query logging
             logging.getLogger("sqlalchemy").setLevel(severity1)
+            # INFO=Log SQL query. DEBUG=Log SQL query + result
             logging.getLogger("sqlalchemy.engine").setLevel(severity1)
             logging.getLogger("sqlalchemy.dialects").setLevel(severity1)
             # Turn on Connection Pool usage logging
+            # INFO=Log connection invalidation + recycle events. DEBUG=Log all pool
+            # checkings/checkouts
             logging.getLogger("sqlalchemy.pool").setLevel(severity2)
             # Turn on other things
             logging.getLogger("sqlalchemy.orm").setLevel(severity2)
             instance.logger.setLevel(logging.DEBUG)
         else:
             instance.logger.setLevel(logging.WARN)
 
     async def _setup_engine_before_cursor_execute(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
     ):
         # Profile SQL query execution time
         @event.listens_for(engine.sync_engine, "before_cursor_execute")
-        def before_cursor_execute(conn, cursor, statement, parameters, context, executemany):
+        def profile_query_exec_time_begin(
+            conn, cursor, statement, parameters, context, executemany
+        ):
             context._query_start_time = time.time()
             instance.logger.debug("Start Query:\n%s" % statement)
             # Modification for StackOverflow answer:
             # Show parameters, which might be too verbose, depending on usage..
             instance.logger.debug("Parameters:\n%r" % (parameters,))
 
     async def _setup_engine_after_cursor_execute(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
     ):
         @event.listens_for(engine.sync_engine, "after_cursor_execute")
-        def after_cursor_execute(conn, cursor, statement, parameters, context, executemany):
+        def profile_query_exec_time_end(conn, cursor, statement, parameters, context, executemany):
             total = time.time() - context._query_start_time
-            instance.logger.debug("Query Complete!")
             # Modification for StackOverflow: times in milliseconds
-            instance.logger.debug("Total Time: %.02fms" % (total * 1000))
-
-    async def _setup_engine_connection_connect(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
-    ):
-        pass
-
-    async def _setup_engine_connection_begin(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
-    ):
-        pass
-
-    async def reflect_schema(
-        self,
-        options: Dict = {},
-        entity_base_class: object = None,
-        entity_classes: List[object] = [],
-        scalar_relation_mapping: List[Tuple] = [],
-        collection_direct_relation_mapping: List[Tuple] = [],
-        collection_indirect_relation_mapping: List[Tuple] = [],
-    ):
-        for instance, i_options in self._engines(_get_engine_options(options)):
-            try:
-                instance.logger.info(f"Reflect db schema: started")
-                await self._reflect_schema(
-                    instance=instance,
-                    entity_base_class=entity_base_class,
-                    entity_classes=entity_classes,
-                    scalar_relation_mapping=scalar_relation_mapping,
-                    collection_direct_relation_mapping=collection_direct_relation_mapping,
-                    collection_indirect_relation_mapping=collection_indirect_relation_mapping,
-                )
-                instance.logger.info(f"Reflect db schema: completed")
-            except BaseException:
-                instance.logger.error(f"Reflect db schema: failed", exc_info=1)
-                raise
+            instance.logger.debug(f"Query Complete! Total Time: %.02fms" % (total * 1000))
 
-    async def _reflect_schema(
-        self,
-        instance: SQLAlchemyDBConfig = None,
-        entity_base_class: object = None,
-        entity_classes: List[object] = [],
-        scalar_relation_mapping: List[Tuple] = [],
-        collection_direct_relation_mapping: List[Tuple] = [],
-        collection_indirect_relation_mapping: List[Tuple] = [],
-    ):
-        """
-        Reflect tables + relations
-        :entity_base_class: See example
-
-        from sqlalchemy.ext.automap import automap_base
-        Base = automap_base()
-
-        Base *is* the entity_base_class
-
-        :scalar_relation_mapping, collection_direct_relation_mapping, collection_indirect_relation_mapping: See example
-        class Table(Enum):
-            FAVORITE = "favorites"
-            FOLLOWER_NAMES = "followers_names"
-            FOLLOWER = "followers"
-            FOLLOWING = "following"
-            FOLLOWING_NAMES = "following_names"
-            QUOTEAGG = "view_quotes_aggregate"
-            REPLY = "replies"
-            RETWEET = "retweets"
-            QUOTE = "quotes"
-            TWEET = "tweets"
-            USER = "users"
-
-        scalar_relation_mapping = [
-            "FromEntity name", "entity property name", "ToEntity name", "entity property name", "relation name (stored in FromEntity)"
-            (Table.FAVORITE.value, "user_id", Table.USER.value, "id", "user") ==> "Favorite.user is the scalar relation Favorite.user_id->User.id"
-            (Table.FAVORITE.value, "tweet_id", Table.TWEET.value, "id", "tweet")
-        ]
-
-        collection_indirect_relation_mapping = [
-           ("FromEntity name", "entity property name", "ToFinalEntity nane", "entity property name", "ViaEntityStart name", "entity property name", "ViaEntityEnd", "entity property name", "Relation Name", "Reverse Relation Name")
-           ( Table.TWEET.value, "id", Table.USER.value, "id", Table.FAVORITE.value, "tweet_id", Table.FAVORITE.value, "user_id", "favorited_by", "favorited")
-                ==> Tweet.favorited_by is the collection relation Tweet.id->Favorite.tweet_id->Favorite.user_id->User.id
-                ==> User.favorited is the collection relation User.id->Favorite.user_id->Favorite.tweet_id->Tweet.id
-        ]
-
-        collection_direct_relation_mapping = [
-           ("FromEntity name", "entity property name", "ToFinalEntity nane", "entity property name", "Relation Name", "Reverse Relation Name")
-           ( Table.TWEET.value, "id", Table.USER.value, "id", "froms", "tweets")
-                ==> Tweet.froms is the collection relation Tweet.id->User.id
-                ==> User.tweets is the collection relation User.id->Tweet.id
-        ]
+    async def _setup_session_do_orm_execute(self, session=AsyncSession, options: Dict = None):
+        logger = (options or {}).get("logger", logging.getLogger("constellate.dummy.logger"))
 
-
-        """
-
-        def name_for_collection_relationship(base, local_cls, referred_cls, constraint):
-            relation_src_table_id = local_cls.__table__.name
-            relation_dst_table_id = referred_cls.__table__.name
-
-            reflexive_relation = relation_src_table_id == relation_dst_table_id
-
-            assert len(constraint.column_keys) < 2
-            assert len(constraint.elements) < 2
-
-            third_party_tables = list(
-                filter(
-                    lambda table: table.name not in [relation_src_table_id, relation_dst_table_id],
-                    [constraint.table, constraint.referred_table],
-                )
-            )
-            indirect_relation = len(third_party_tables) > 0
-
-            if indirect_relation:
-                intermediary_tables = third_party_tables
-            else:
-                intermediary_tables = [constraint.table]
-
-            def to_relation_string(
-                src_table_id,
-                src_columns_id,
-                dst_table_id,
-                dst_columns_id,
-                intermediary_relation_path=None,
-            ):
-                intermediary_relation_path = (
-                    f"=>{intermediary_relation_path}=>"
-                    if intermediary_relation_path is not None
-                    else "=>"
-                )
-                return f"{src_table_id}.{src_columns_id}{intermediary_relation_path}{dst_table_id}.{dst_columns_id}"
-
-            def via_relation_path(
-                src_table_id, src_columns_id, dst_table_id, dst_columns_id, backref
-            ):
-                if None not in [src_table_id, src_columns_id, dst_table_id, dst_columns_id]:
-                    if not backref:
-                        return f"{src_table_id}.{src_columns_id}~~~{dst_table_id}.{dst_columns_id}"
-                    else:
-                        return f"{dst_table_id}.{dst_columns_id}~~~{src_table_id}.{src_columns_id}"
-                return None
-
-            # Find transitive relation (ie intermediary table)
-            inter_table = intermediary_tables[0]
-            inter_fkcs = [
-                fk for fk in inter_table.constraints if isinstance(fk, ForeignKeyConstraint)
-            ]
-
-            # Find foreign keys constraints of the intermediary table, matching our relation start/end table
-            # - These keys will *individually* point to either the relation's source table or the relation's destination table
-            relation_to_src__inter_fkc = None
-            relation_to_dst__inter_fkc = None
-
-            for inter_fkc in inter_fkcs:
-                inter_fk_dst_table_id = inter_fkc.referred_table.name
-                if (
-                    inter_fk_dst_table_id == relation_src_table_id
-                    and relation_to_src__inter_fkc is None
-                ):
-                    relation_to_src__inter_fkc = inter_fkc
-                elif inter_fk_dst_table_id == relation_dst_table_id:
-                    relation_to_dst__inter_fkc = inter_fkc
-
-            # Sanity check:
-            #  - Indirect relations must have both variable set
-            #  - Direct relations only one. By default it will be relation_to_src__inter_fkc
-            if (
-                indirect_relation
-                and not reflexive_relation
-                and None in [relation_to_src__inter_fkc, relation_to_dst__inter_fkc]
-            ):
-                raise BaseException("What's going on here ???")
-            if indirect_relation and reflexive_relation:
-                pass
-                # else:
-                #     relation_to_src__inter_fkc = relation_to_dst__inter_fkc if relation_to_dst__inter_fkc is not None else relation_to_src__inter_fkc
-                #     relation_to_dst__inter_fkc = relation_to_src__inter_fkc if relation_to_src__inter_fkc is not None else relation_to_dst__inter_fkc
-            if not indirect_relation:
-                relation_to_src__inter_fkc = (
-                    relation_to_dst__inter_fkc
-                    if relation_to_dst__inter_fkc is not None
-                    else relation_to_src__inter_fkc
-                )
-                relation_to_dst__inter_fkc = None
-
-            # Find the starting/ending tables associated to the foreign key constraint
-            inter_fk_src_table_id = None
-            inter_fk_dst_table_id = None
-            inter_fk_src_referred_table_id = None
-            # inter_fk_dst_referred_table_id = None
-            if indirect_relation:
-                inter_fk_src_table_id = relation_to_src__inter_fkc.table.name
-                inter_fk_dst_table_id = relation_to_dst__inter_fkc.table.name
-                inter_fk_src_referred_table_id = relation_to_src__inter_fkc.referred_table.name
-                # inter_fk_dst_referred_table_id = relation_to_dst__inter_fkc.referred_table.name
-            else:
-                inter_fk_src_table_id = relation_to_src__inter_fkc.table.name
-                inter_fk_dst_table_id = relation_to_src__inter_fkc.referred_table.name
-                inter_fk_src_referred_table_id = None
-                # inter_fk_dst_referred_table_id = None
-
-            # Find the column of each matching foreign key used as either starting
-            # point or ending point of the relation's table
-            relation_src_columns_id = None
-            relation_dst_columns_id = None
-            if indirect_relation:
-                relation_src_columns_id = relation_to_src__inter_fkc.elements[0].column.key
-                relation_dst_columns_id = relation_to_dst__inter_fkc.elements[0].column.key
-            else:
-                relation_src_columns_id = relation_to_src__inter_fkc.elements[0].column.key
-                relation_dst_columns_id = relation_to_src__inter_fkc.columns[
-                    relation_to_src__inter_fkc.column_keys[0]
-                ].key
-
-            inter_fk_end0_columns_id = None
-            inter_fk_end1_columns_id = None
-            if indirect_relation:
-                inter_fk_end0_columns_id = ",".join(
-                    [
-                        relation_to_src__inter_fkc.columns[col_key].key
-                        for col_key in relation_to_src__inter_fkc.column_keys
-                    ]
-                )
-                inter_fk_end1_columns_id = ",".join(
-                    [
-                        relation_to_dst__inter_fkc.columns[col_key].key
-                        for col_key in relation_to_dst__inter_fkc.column_keys
-                    ]
-                )
-            else:
-                inter_fk_end0_columns_id = None
-                inter_fk_end1_columns_id = None
-
-            # Determine if relation is a backref
-            backref = None
-            if indirect_relation and relation_src_table_id != relation_dst_table_id:
-                # Case: A to C via B (ie non reflexive + indirect relation)
-                backref = relation_src_table_id > relation_dst_table_id
-            elif indirect_relation and relation_src_table_id == relation_dst_table_id:
-                # Case: A to A via B  (ie reflexive + indirect reflexion)
-                backref = relation_to_src__inter_fkc.name > relation_to_dst__inter_fkc.name
-            else:
-                # Case: A to B (ie direct relation)
-                backref = relation_src_table_id != inter_fk_src_table_id
-
-            def relation(
-                src_table_id, src_columns_id, dst_table_id, dst_columns_id, backref, via_path
-            ):
-                if backref:
-                    resolution_path = to_relation_string(
-                        dst_table_id, dst_columns_id, src_table_id, src_columns_id, via_path
-                    )
-                else:
-                    resolution_path = to_relation_string(
-                        src_table_id, src_columns_id, dst_table_id, dst_columns_id, via_path
-                    )
-                return resolution_path
-
-            # Swap intermediary columns if the relation is a backref and the
-            # intermediary foreign key to source association is backward
-            inter_src_table_id = inter_fk_src_table_id
-            inter_dst_table_id = inter_fk_dst_table_id
-            inter_end0_columns_id = None
-            inter_end1_columns_id = None
-            backref_inter = backref and relation_src_table_id == inter_fk_src_referred_table_id
-            if backref_inter:
-                inter_end0_columns_id = inter_fk_end0_columns_id
-                inter_end1_columns_id = inter_fk_end1_columns_id
-            else:
-                inter_end0_columns_id = inter_fk_end1_columns_id
-                inter_end1_columns_id = inter_fk_end0_columns_id
-            indirect_path = via_relation_path(
-                inter_src_table_id,
-                inter_end0_columns_id,
-                inter_dst_table_id,
-                inter_end1_columns_id,
-                not backref,
-            )
-
-            relation_path = None
-            if backref:
-                relation_path = relation(
-                    relation_dst_table_id,
-                    relation_dst_columns_id,
-                    relation_src_table_id,
-                    relation_src_columns_id,
-                    True,
-                    indirect_path,
-                )
-            else:
-                relation_path = relation(
-                    relation_src_table_id,
-                    relation_src_columns_id,
-                    relation_dst_table_id,
-                    relation_dst_columns_id,
-                    False,
-                    indirect_path,
-                )
-
-            def via_relation_path_builder(
-                src_table_id, src_column_id, dst_table_id, dst_column_id, backref
-            ):
-                if backref:
-                    return via_relation_path(
-                        dst_table_id, dst_column_id, src_table_id, src_column_id, False
-                    )
-                return via_relation_path(
-                    src_table_id, src_column_id, dst_table_id, dst_column_id, False
-                )
-
-            # Mapping such as Table.A.col_a -> Table.B.col_b MUST ALWAYS BE expressed in the same direction as in the
-            # SQL schema's defined relations. More on the relation's "order" below.
-            VIA_NONE = via_relation_path(None, None, None, None, backref)
-            mapping_indirects = {
+        def _switch_shard_engine(context: ORMExecuteState = None, shard_id: str = None):
+            logger.debug(f"Using engine with shard_id={shard_id}")
+            context.update_execution_options(_sa_shard_id=shard_id)
+
+        @event.listens_for(session.sync_session, "do_orm_execute")
+        def switch_shard_engine(context: ORMExecuteState):
+            if isinstance(context.session, ShardedSession):
                 #
-                # Indirect relations:
-                # relation(A, col_a, B, col_b, ..., via_relation_path(C, col_c0, C, col_c1))
-                #  - A < B must be lexicographically ordered true. relation definition MUST be in lexicographic order.
-                #  -- relation(A, .., B, ...) is well defined
-                #  -- relation(B, .., A, ...) is not well defined
-                #  - A > B means the relation is a backref. This is an arbitrary decision when dealing with indirect
-                #                                            relations
-                #  - reads as the relation is resolved from A.col_a -> C.col_c0 ~~~~ C.col_c1 -> B.col_b
-                # relation(Table.USER.value, 'following_id', Table.USER.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz6' if not backref else 'zoob6',
-                # relation(Table.USER.value, 'following_id', Table.USER.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz5' if not backref else 'zoob5',
-                # relation(Table.USER.value, 'id', Table.USER.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz4' if not backref else 'zoob4',
-                # relation(Table.USER.value, 'follower_id', Table.USER.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz3' if not backref else 'zoob3',
-                # relation(Table.USER.value, 'tweet_id', Table.TWEET.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz' if not backref else 'favorited_by_users',
-                relation(
-                    t[0],
-                    t[1],
-                    t[2],
-                    t[3],
-                    backref,
-                    via_relation_path_builder(t[4], t[5], t[6], t[7], backref),
-                ): t[8]
-                if not backref
-                else t[9]
-                for t in collection_indirect_relation_mapping
-            }
-
-            mapping_directs = {
+                # ShardedSession official usages
                 #
-                # Direct relations
-                # relation(A, col_a, B, col_b, ...) ==> reads as the relation
-                #  - A < B must be in the same order as the foreign key constraint defined in the table betweet A and B for the columns
-                #  -- A > B means the relation is a backref as defined by SQLAlchemy
-                #  - reads as resolved from A.col_a -> B.col_b
-                # resolution(Table.TWEET.value, 'user_id', Table.USER.value, 'id', backref, NO_INTER_RELATION):
-                # 'booz2' if not backref else 'favorited_tweets',
-                relation(t[0], [1], t[2], t[3], backref, VIA_NONE): t[4] if not backref else t[5]
-                for t in collection_direct_relation_mapping
-            }
 
-            mapping = {**mapping_indirects, **mapping_directs}
+                # Usage: session.execute(select(...), bind_arguments={"shard_id": "engine_shard_id_3"})
+                # - src: https://github.com/sqlalchemy/sqlalchemy/blob/979ea6b21f71605314dc0ac1231dd385eced98c4/lib/sqlalchemy/ext/horizontal_shard.py#L241
+                # Usage: session.execute(select(...), execution_options={"_sa_shard_id": "engine_shard_id_3"})
+                # - src: https://github.com/sqlalchemy/sqlalchemy/blob/979ea6b21f71605314dc0ac1231dd385eced98c4/lib/sqlalchemy/ext/horizontal_shard.py#L241
 
-            name = mapping.get(relation_path, None)
+                #
+                # ShardedSession unofficial usages
+                #
 
-            via_relation = "N/A" if not indirect_relation else indirect_path
-            relationship_type = None
-            if not backref:
-                if indirect_relation:
-                    relationship_type = RelationshipType.MANY_TO_MANY
-                else:
-                    relationship_type = RelationshipType.MANY_TO_ONE
-            else:
-                if indirect_relation:
-                    relationship_type = RelationshipType.MANY_TO_MANY
-                else:
-                    relationship_type = RelationshipType.ONE_TO_MANY
+                # Usage: Instruct session to use a particular engine whose shard_id is 'engine_shard_id_3' to execute THIS select(...)
+                # Sample: session.execute(select(...).options(SetShardEngineOption("engine_shard_id_3"))
+                # Conditions:
+                # - Only supported for query with .options() available, I think
+                # - Only supported for ShardedSession instances since they trigger do_orm_execute events
+                # src: #
+                # https://github.com/sqlalchemy/sqlalchemy/discussions/6885#discussioncomment-1186864
+                # NOTE:
+                # - Will be deprecated in favor of THIS ? THIS https://github.com/sqlalchemy/sqlalchemy/issues/7226#issuecomment-950440743
+                for elem in context.user_defined_options:
+                    found_shard_engine_option = isinstance(elem, SetShardEngineOption)
+                    if found_shard_engine_option:
+                        _switch_shard_engine(context=context, shard_id=elem.payload)
+                        return
+
+                # Usage: Instruct session to use a particular engine whose shard_id is 'engine_shard_id_3' for all statement by default,
+                #        unless overwritten on an individual statement basis
+                # Sample: async with self.session_scope(execution_options={'shard_id':SetShardEngineOption('engine_shard_id_3')}) as session:
+                #           ...
+                elem = context.execution_options.get("shard_id", None)
+                found_shard_engine_option = isinstance(elem, SetShardEngineOption)
+                if found_shard_engine_option:
+                    _switch_shard_engine(context=context, shard_id=elem.payload)
+                    return
 
-            name = f"RANDOMLY_ASSIGNED-{random()}" if name is None else name
+    async def _setup_engine_connection_connect(
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
+    ):
+        pass
 
-            instance.logger.debug(
-                f"---\ncollection relationship name: \nBACKREF:{backref}\nFROM({'backref' if backref else ''}): {relation_src_table_id} \nTO({'backref' if backref else ''}):{relation_dst_table_id}\nINDIRECT RELATION:{indirect_relation}\nVIA:{via_relation}\nVIA(RAW):{str(constraint)}\nBECOMES: {relationship_type} {relation_src_table_id}.{name}\nDUE TO RELATION PATH:{relation_path} \nON MAPPING:\n{pprint.PrettyPrinter(depth=4).pformat(mapping)})"
-            )
+    async def _setup_engine_connection_begin(
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
+    ):
+        pass
 
-            if name is None:
-                raise BaseException(
-                    f"key {relation_path} has no matching relationship name. Missing a case ?"
-                )
+    async def _setup_engine_session_maker(self, instance: SQLAlchemyDBConfig = None, **kwargs):
+        if instance is not None:
+            kwargs.update({"bind": instance.engine_config.engine})
 
-            return name
+        instance.session_maker = await self._create_session_maker(**kwargs)
 
-        def name_for_scalar_relationship(base, local_cls, referred_cls, constraint):
-            relation_src_table_id = local_cls.__table__.name
-            relation_dst_table_id = referred_cls.__table__.name
+    async def migrate(self, options: Dict = {}):
+        """
+        :options per engine:
+        - key: migration_context:MigrationContext, A migration context
+        - key: migration_priority: int [0, max_size]. Default: 0. Migration priority amongst all engines.
+               Engines with identical priority will be migrated concurrently. Otherwise serialized by ascending priority number
+        """
 
-            def relation(src_table_id, src_columns_name, dst_table_id, dst_columns_name):
-                return f"{src_table_id}.{src_columns_name}->{dst_table_id}.{dst_columns_name}"
+        def _get_priority(options: Dict):
+            return options.get("migration_priority", 0)
 
-            constraint_src_table_columns_name = ",".join(
-                [constraint.columns[col_key].key for col_key in constraint.column_keys]
-            )
-            constraint_dst_table_columns_name = ",".join(
-                [foreign_key.column.key for foreign_key in constraint.elements]
-            )
+        pios = [
+            (_get_priority(i_options), instance, i_options)
+            for instance, i_options in self._engines(_get_engine_options(options=options))
+        ]
 
-            relation_path = relation(
-                relation_src_table_id,
-                constraint_src_table_columns_name,
-                relation_dst_table_id,
-                constraint_dst_table_columns_name,
-            )
-            relationship_type = RelationshipType.ONE_TO_ONE
+        migration_orders = {}
+        for p, i, o in pios:
+            sub_migrations = migration_orders.get(p, [])
+            sub_migrations.append((i, o))
+            migration_orders[p] = sub_migrations
 
-            # Mapping always expressed in the same direction as in the sql schema
-            mapping = {relation(t[0], t[1], t[2], t[3]): t[4] for t in scalar_relation_mapping}
-            name = mapping.get(relation_path, None)
-
-            if name is None:
-                raise BaseException(
-                    f"key {relation_path} has no matching relationship name. Missing a case ?"
-                )
+        async def __migrate(
+            instance: SQLAlchemyDBConfig = None, options: Dict = None, concurrent: bool = None
+        ):
+            log_prefix = f"Migrating {'concurrently' if concurrent else ''}: {instance.identifier}"
+            try:
+                try:
+                    instance.logger.info(f"{log_prefix}: started")
+                    await self._migrate(instance=instance, options=options)
+                    instance.logger.info(f"{log_prefix}: completed")
+                except BaseException as e:
+                    raise MigrationException() from e
+            except BaseException as e:
+                instance.logger.error(f"{log_prefix}: failed", exc_info=1)
+                raise e
 
-            instance.logger.debug(
-                f"scalar relationship name:\nFROM:{relation_src_table_id}\nTO:{relation_dst_table_id}\nBY {str(constraint)}\nBECOMES:{relationship_type} {relation_src_table_id}.{name}\nDUE TO RESOLUTION PATH:{relation_path}"
+        for priority, migrations in migration_orders.items():
+            concurrent = len(migrations) > 0
+            await asyncio.gather(
+                *[__migrate(instance=i, options=o, concurrent=concurrent) for i, o in migrations]
             )
-            return name
-
-        async with instance.engine.connect() as conn:
 
-            def prepare(connection):
-                kwargs = {}
-                if (
-                    len(collection_direct_relation_mapping)
-                    + len(collection_indirect_relation_mapping)
-                ) > 0:
-                    kwargs.update(
-                        {"name_for_collection_relationship": name_for_collection_relationship}
-                    )
-                if len(scalar_relation_mapping) > 0:
-                    kwargs.update({"name_for_scalar_relationship": name_for_scalar_relationship})
-
-                entity_base_class.prepare(autoload_with=connection, **kwargs)
-
-            await conn.run_sync(prepare)
-
-        # Force checking db classes & relationships are automapped and/or manually mapped
-        instance.logger.debug("Table(s) relationships:")
-        from sqlalchemy.inspection import inspect
-
-        for entity_cls in entity_classes:
-            relations = inspect(entity_cls).relationships.items()
-            for relation in relations:
-                instance.logger.debug(
-                    f"Table {entity_cls.__name__} has relationship: -> {relation}"
-                )
+    async def _migrate(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
+        raise NotImplementedError("Must be implemented by the sub class")
 
-    async def migrate(self, options: Dict = {}):
-        """
-        :options per engine:
-        - key: migration_dirs:List[PurePath], list of absolute path to sql migration scripts
+    async def database_compatible(self, options: Dict = {}) -> bool:
         """
-        for instance, i_options in self._engines(_get_engine_options(options)):
-            try:
-                instance.logger.info(f"Migrating db schema: started")
-                await self._migrate(instance=instance, options=i_options)
-                instance.logger.info(f"Migrating db schema: completed")
-            except BaseException:
-                instance.logger.error(f"Migrating db schema: failed", exc_info=1)
-                raise
+        True when database is greater than the min database user version
+        Option per engine:
+        - database_user_version_compatible_query: SQLAlchemy SELECT query. To query the current database version from (incompatible with database_user_version_class_column).
+                                                                           The queur must return a scalar boolean value: True == compatible
+        - engine_execution_options: Dict. Execution options to pass on
+        - database_compatibility_check: Callable[[AsyncSession, Select], AsyncGenerator[bool,None]]. Custom function to check if the database is compatible
+        """
+
+        async def has_compatibility(
+            instance=None,
+            version_check_query=None,
+            execution_options={},
+            compatibility_check: Callable[
+                [AsyncSession, Any, Select], AsyncGenerator[bool, None]
+            ] = None,
+        ):
+            async with self.session_scope(config=instance) as session:
+                if compatibility_check is None:
 
-    async def _migrate(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
-        raise NotImplementedError("Must be implemented by the sub class")
+                    async def user_version_compatible(
+                        session: AsyncSession = None, version_check_query: Select = None
+                    ) -> bool:
+                        @execute_scalar
+                        async def _read_database_compatibility(**kwargs):
+                            return version_check_query
+
+                        compatible = await _read_database_compatibility(session=session)
+                        return compatible or False
+
+                    compatibility_check = user_version_compatible
+
+                return await compatibility_check(
+                    session=session, version_check_query=version_check_query
+                )
+
+        compatibles = [
+            has_compatibility(
+                instance=instance,
+                version_check_query=i_options.get("database_user_version_compatible_query"),
+                execution_options=i_options.get("engine_execution_options", {}),
+                compatibility_check=i_options.get("database_compatibility_check", None),
+            )
+            for instance, i_options in self._engines(_get_engine_options(options=options))
+        ]
+        compatibles = await asyncio.gather(*compatibles)
+        return len(compatibles) > 0 and all(compatibles)
 
     async def vacuum(self, options: Dict = {}):
         """
         :raises:
             VacumException when vacum fails
         """
-        for instance, i_options in self._engines(_get_engine_options(options)):
+        for instance, i_options in self._engines(_get_engine_options(options=options)):
             try:
                 instance.logger.info(f"Vacumming db: started")
                 await self._vacuum(instance=instance, options=i_options)
                 instance.logger.info(f"Vacumming db: completed")
             except BaseException as e:
                 instance.logger.error(f"Vacumming db: failed", exc_info=1)
                 raise VacumException() from e
@@ -732,91 +457,278 @@
 
     async def backup(self, options: Dict = {}):
         """
         :options:
         Key: db_file:str Source db absolute file path
         Key: db_file_backup:str Destination db absolute file path
         """
-        for instance, i_options in self._engines(_get_engine_options(options)):
+        for instance, i_options in self._engines(_get_engine_options(options=options)):
             try:
                 instance.logger.info(f"Backup db: started")
                 await self._backup(instance=instance, options=i_options)
                 instance.logger.info(f"Backup db: completed")
             except BaseException:
                 instance.logger.error(f"Backup db: failed", exc_info=1)
                 raise
 
     async def _backup(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
         raise NotImplementedError("Must be implemented by sub class")
 
     async def dispose(self, options: Dict = {}):
-        for instance, i_options in self._engines(_get_engine_options(options)):
-            if instance.engine is not None:
-                await self._dispose(engine=instance.engine)
-            self._config_manager.pop(instance.identifier)
+        await self.__dispose_wrapper(options=options)
 
     async def dispose2(self, setup_engines_options: List = []):
-        for engine_options in setup_engines_options:
-            await self.dispose(engine_options)
+        await self.__dispose_wrapper(setup_engines_options=setup_engines_options)
+
+    async def __dispose_wrapper(
+        self,
+        options: Dict = None,
+        setup_engines_options: List = None,
+        ignore_no_per_engine_option: bool = False,
+    ):
+        values = []
+        if options is not None:
+            values = self._engines(
+                _get_engine_options(
+                    options=options, ignore_no_per_engine_option=ignore_no_per_engine_option
+                )
+            )
+        elif setup_engines_options is not None:
+            values = itertools.chain(
+                *[
+                    self._engines(
+                        _get_engine_options(
+                            options=setup_engine_options,
+                            ignore_no_per_engine_option=ignore_no_per_engine_option,
+                        )
+                    )
+                    for setup_engine_options in setup_engines_options
+                ]
+            )
+        else:
+            raise ValueError()
+
+        for instance, i_options in values:
+            if instance.engine_config.engine is not None:
+                await self._dispose(engine=instance.engine_config.engine)
+            # FIXME (medium) pop will try to pop an identifier that was already poped
+            self._config_manager.pop(instance.identifier)
 
     async def _dispose(self, engine: AsyncEngine = None):
         if engine is not None:
             await engine.dispose()
 
-    async def _setup_engine_session_maker(self, instance: SQLAlchemyDBConfig = None):
-        instance.session_maker = await self._create_session_maker(
-            type=SessionType.MONO_ENGINE, bind=instance.engine, autoflush=True, future=True
+    async def _create_session_maker(self, **kwargs):
+        dict_update(map=kwargs, when=DictCondition.MISSING, key="autoflush", value=True)
+        dict_update(map=kwargs, when=DictCondition.MISSING, key="future", value=True)
+        dict_update(map=kwargs, when=DictCondition.MISSING, key="expire_on_commit", value=True)
+        dict_update(map=kwargs, when=DictCondition.MISSING, key="twophase", value=False)
+        dict_update(map=kwargs, when=DictCondition.MISSING, key="execution_options", value={})
+        # dict_update_when_missing(map=kwargs, when=DictCondition.MISSING, key='bind', value=...)
+        dict_update(
+            map=kwargs, when=DictCondition.MISSING, key="class_", value=self._get_session_class()
         )
-
-    async def _setup_multi_engine_session_maker(self, **kwargs):
-        return await self._create_session_maker(
-            type=SessionType.MULTI_ENGINE, future=True, **kwargs
+        dict_update(
+            map=kwargs,
+            when=DictCondition.MISSING,
+            key="sync_session_class",
+            value=self._get_sync_session_class(),
         )
 
-    async def _create_session_maker(self, type: SessionType = SessionType.UNKNOWN, **kwargs):
-        session_class = self._get_session_class(type=type)
-        return sessionmaker(class_=session_class, **kwargs)
+        return sessionmaker(**kwargs)
 
-    def _get_session_class(self, type: SessionType = SessionType.UNKNOWN) -> AsyncSession.__class__:
+    def _get_session_class(self) -> AsyncSession:
         return MultiEngineSession
 
+    def _get_sync_session_class(self) -> Session:
+        return SyncMultiEngineSession
+
     @asynccontextmanager
-    async def session_scope(
-        self, auto_flush=True, expire_on_commit=True
-    ) -> AsyncGenerator[AsyncSession, None]:
+    async def session_scope(self, **kwargs) -> AsyncGenerator[AsyncSession, None]:
         """Provide a transactional scope around a series of database operations."""
-        async for session in self._session_scope_generator(
-            auto_flush=auto_flush, expire_on_commit=expire_on_commit
+        kwargs, custom_kwargs = self.__pop_custom_kwargs(kwargs=kwargs)
+        session_maker = await self._create_session_maker(**kwargs)
+
+        async for session in self.__session_scope(
+            session_maker=session_maker,
+            owner=self,
+            config_manager=self._config_manager,
+            **custom_kwargs,
         ):
             yield session
             await asyncio.sleep(0)
 
-    async def _session_scope_generator(
-        self, auto_flush=True, expire_on_commit=True
+    async def session_scope2(self, **kwargs) -> AsyncSession:
+        """Provide a transactional scope around a series of database operations."""
+        kwargs, custom_kwargs = self.__pop_custom_kwargs(kwargs=kwargs)
+        session_maker = await self._create_session_maker(**kwargs)
+
+        async for session in self.__session_scope(
+            session_maker=session_maker,
+            owner=self,
+            config_manager=self._config_manager,
+            **custom_kwargs,
+        ):
+            # Note: This is not a generator function, by design
+            return session
+
+    @asynccontextmanager
+    async def __session_scope_for_shard(
+        self,
+        shard_session_class: Any = None,
+        shard_sync_session_class: Any = None,
+        unshard_session_class: Any = None,
+        unshard_sync_session_class: Any = None,
+        autoflush=True,
+        expire_on_commit=True,
+        config: SQLAlchemyDBConfig = None,
+        execution_options: Dict = None,
+        bind_arguments: Dict = None,
+        twophase: bool = False,
+        sharded: bool = True,
+        begin_explicit: bool = True,
+        horizontal_shard_chooser: Callable = None,
+        horizontal_id_chooser: Callable = None,
+        horizontal_execute_chooser: Callable = None,
+        logging_token: str = None,
     ) -> AsyncGenerator[AsyncSession, None]:
-        session_maker = await self._setup_multi_engine_session_maker(
-            autoflush=auto_flush, expire_on_commit=expire_on_commit
-        )
+        """
+        Template function to provide sharded or unsharded session
+        User should typically override `session_scope_for_shard`
+        """
+        if sharded:
+            execution_options = execution_options or {}
+            bind_arguments = bind_arguments or {}
+
+            # Prepare sharded session DEFAULT settings
+            # by selecting a database (and therefore an engine)
+            # - with database level shards
+            full_level_shards = {
+                config.identifier: config.engine_config.engine.sync_engine
+                for config in await self.for_each_engine(filter_fn=FILTER_LOGICAL_SHARD_BY_NOTHING)
+            }
+            bind_arguments.update({"shard_id": config.identifier})
+            # by selecting a schema within the selected database
+            # - with schema level shards
+            #
+            # This works for SQLAlchemy constructs supporting it such as:
+            # - select()/delete()/etc from actual table object
+            #
+            shard_schema_id = config.options.get("custom").schema_id
+            execution_options.update({"schema_translate_map": {"per_unit": shard_schema_id}})
+            if logging_token is not None:
+                # Doc: https://docs.sqlalchemy.org/en/14/core/engines.html#setting-per-connection-sub-engine-tokens
+                execution_options.update({"logging_token": logging_token})
+
+            # - with sharding choosers
+            # Instantiate a sharded session
+            async with self.session_scope(
+                class_=shard_session_class,
+                autoflush=autoflush,
+                expire_on_commit=expire_on_commit,
+                execution_options=execution_options,
+                bind_arguments=bind_arguments,
+                twophase=twophase,
+                sync_session_class=shard_sync_session_class,
+                shards=full_level_shards,
+                id_chooser=horizontal_id_chooser,
+                shard_chooser=horizontal_shard_chooser,
+                execute_chooser=horizontal_execute_chooser,
+                begin_explicit=begin_explicit,
+            ) as session:
+                yield session
+        else:
+            # Instantiate a un-sharded session
+            async with self.session_scope(
+                class_=unshard_session_class,
+                autoflush=autoflush,
+                expire_on_commit=expire_on_commit,
+                execution_options=execution_options,
+                bind_arguments=bind_arguments,
+                twophase=twophase,
+                sync_session_class=unshard_sync_session_class,
+                bind=config.engine_config.engine,
+                begin_explicit=begin_explicit,
+            ) as session:
+                yield session
 
-        async for session in self._session_scope(session_maker=session_maker):
+    @asynccontextmanager
+    async def session_scope_for_shard(
+        self,
+        shard_session_class: MultiEngineSession = SimpleShardSession,
+        shard_sync_session_class: SyncMultiEngineShardSession = SyncSimpleShardSession,
+        unshard_session_class: MultiEngineSession = SimpleShardSession,  # FIXME (high) Why is there the word SHARD in it ?
+        unshard_sync_session_class: SyncMultiEngineSession = SyncSimpleSession,
+        sharder: Sharder = None,
+        **kwargs,
+    ) -> AsyncGenerator[AsyncSession, None]:
+        """Create session using shards"""
+        sharder = sharder or Sharder(config_manager=self.config_manager)
+        async with self.__session_scope_for_shard(
+            shard_session_class=shard_session_class,
+            shard_sync_session_class=shard_sync_session_class,
+            unshard_session_class=unshard_session_class,  # FIXME (high) Why is there the word SHARD in it ?
+            unshard_sync_session_class=unshard_sync_session_class,
+            horizontal_shard_chooser=sharder.shard_chooser,
+            horizontal_id_chooser=sharder.id_chooser,
+            horizontal_execute_chooser=sharder.execute_chooser,
+            **kwargs,
+        ) as session:
             yield session
-            await asyncio.sleep(0)
 
-    async def session_scope2(self, auto_flush=True, expire_on_commit=True) -> AsyncSession:
-        """Provide a transactional scope around a series of database operations."""
-        session_maker = await self._setup_multi_engine_session_maker(
-            autoflush=auto_flush, expire_on_commit=expire_on_commit
+    def __pop_custom_kwargs(self, kwargs: Dict = {}):
+        custom_kwargs = {}
+
+        begin_explicit = kwargs.pop("begin_explicit", None)
+        if begin_explicit is not None:
+            custom_kwargs["begin_explicit"] = begin_explicit
+
+        return kwargs, custom_kwargs
+
+    async def __session_scope(
+        self,
+        session_maker: sessionmaker = None,
+        config: Any = None,
+        begin_explicit: bool = False,
+        invalidate_session_on_exception: bool = False,
+        **kwargs,
+    ) -> AsyncGenerator[Union[AsyncSession, AsyncSessionTransaction], None]:
+        """Provide a transactional scope around a series of operations."""
+        # If config manager hold max 1 engine instance, then the session default bind is to that engine.
+        # Otherwise, the session bind is project implementation specific
+        # (horizontal / vertical sharding)
+        configs = [config] if config is not None else [s for s in kwargs.get("config_manager", [])]
+        configs = (
+            list(filter(lambda t: t[1].type == DBConfigType.INSTANCE, configs))
+            if len(configs) < 2
+            else configs
         )
 
-        async for session in self._session_scope(session_maker=session_maker):
-            # Note: This is not a generator function, by design
-            return session
+        if len(configs) == 1:
+            # Case SQLALchemy's AsyncSession is provided. SQLAlchemyDBConfig is not a supported option.
+            # Fall back to binding the session to the sole engine available
+            # NOTE: This applies to SQLALchemy's AsyncSession (not constelatte's AsyncSession subclasses like MultiEngineSession)
+            # FIXME (low) config tuple is ugly. Use a proper attr enabled class
+            default_config = configs[0]
+            session_maker.configure(bind=default_config[1].engine_config.engine)
+        else:
+            # Case Constellate's AsyncSession subclasses are provided. SQLAlchemyDBConfig is a supported option.
+            pass
 
-    async def _session_scope(self, session_maker=None) -> AsyncGenerator[AsyncSession, None]:
-        """Provide a transactional scope around a series of database operations."""
-        async for session in session_scope(
-            session_maker=session_maker,
-            owner=self,
-            config_manager=self._config_manager,
-        ):
+        session = session_maker(**kwargs)
+        invalidate_session = False
+        try:
+            await self._setup_session_do_orm_execute(session=session)
+
+            if begin_explicit:
+                session.begin()
             yield session
-            await asyncio.sleep(0)
+            await session.commit()
+        except BaseException as e:
+            invalidate_session = True
+            await session.rollback()
+            raise
+        finally:
+            if invalidate_session and invalidate_session_on_exception:
+                await session.invalidate()
+            else:
+                await session.close()
```

## constellate/database/sqlalchemy/sqlalchemydbconfig.py

```diff
@@ -1,30 +1,31 @@
 import logging
 from enum import IntEnum, auto
 from typing import Dict
 
 import attr
-from sqlalchemy.engine import Engine
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
 from sqlalchemy.orm import sessionmaker
 
+from constellate.database.sqlalchemy.sqlalchemyengineconfig import _EngineConfig
+from constellate.database.sqlalchemy.sqlalchemymigrationconfig import _MigrationConfig
+
 
 class DBConfigType(IntEnum):
     INSTANCE = auto()
     TEMPLATE = auto()
 
 
 @attr.s(kw_only=True, frozen=False, eq=True, auto_attribs=True)
 class SQLAlchemyDBConfig:
+    # Generic Identification
     type: DBConfigType = None
     identifier: str = None
-    # scheme contain the database type name and optionally a driver name. Eg: postgresql+psyops2
-    connection_uri: str = None
-    # scheme only contain the database type name
-    connection_uri_plain: str = None
-    # (Async) Engine is public engine for apps
-    engine: AsyncEngine = None
-    # Sync Engine is private engine for vertical/horizanodal shard needs only
-    sync_engine: Engine = None
+    # Engine conf
+    engine_config: _EngineConfig = None
+    # Session conf
     session_maker: sessionmaker = None
+    # Logging conf
     logger: logging.Logger = None
+    # Migration
+    migration: _MigrationConfig = None
+    # Misc conf
     options: Dict = None
```

## constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py

```diff
@@ -1,27 +1,43 @@
+from typing import Optional, Callable, Iterable, Any
+
 from constellate.database.sqlalchemy.sqlalchemydbconfig import SQLAlchemyDBConfig, DBConfigType
 
 
 class SQLAlchemyDbConfigManager:
-    def __init__(self):
+    def __init__(self) -> None:
         self._instances = {}
 
-    def update(self, instance: SQLAlchemyDBConfig = None):
+    def update(self, instance: SQLAlchemyDBConfig = None) -> None:
         self._instances.update({instance.identifier: instance})
 
-    def pop(self, identifier: str = None):
+    def pop(self, identifier: str = None) -> None:
         self._instances.pop(identifier)
 
     def __iter__(self):
         return self._instances.items().__iter__()
 
     def get(self, identifier: str = None, default_value=None):
         return self._instances.get(identifier, default_value)
 
-    def find(self, type: DBConfigType = DBConfigType.INSTANCE, identifier: str = None):
+    def find(
+        self, type: DBConfigType = DBConfigType.INSTANCE, identifier: str = None, **kwargs
+    ) -> Optional[SQLAlchemyDBConfig]:
+        """Find a SQLAlchemyDBConfig by identifier, type and other application provided settings
+
+        :param type: DBConfigType:  (Default value = DBConfigType.INSTANCE)
+        :param identifier: str:  (Default value = None)
+        :param **kwargs:
+
+        """
         return next(
             filter(
                 lambda config: config.type == type and config.identifier == identifier,
                 self._instances.values(),
             ),
             None,
         )
+
+    def filter(
+        self, key: Callable[[Any, SQLAlchemyDBConfig], bool] = None
+    ) -> Iterable[SQLAlchemyDBConfig]:
+        return [v for k, v in filter(key, list(self))]
```

## constellate/database/sqlalchemy/sqlalchemypostgresql.py

```diff
@@ -1,129 +1,276 @@
-from typing import Dict, Tuple, Optional
+import asyncio
+import functools
+from typing import Dict, Optional, Tuple
 
+from sqlalchemy import create_engine, inspect
+from sqlalchemy import event
 from sqlalchemy import text
-from sqlalchemy import create_engine
+from sqlalchemy.engine.url import make_url
+from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy.pool import QueuePool
+from sqlalchemy.pool import NullPool
 from sqlalchemy_utils import database_exists
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
-from sqlalchemy.engine import Engine
 
-
-from constellate.database.migration.databasetype import DatabaseType
+from constellate.database.common.databasetype import DatabaseType
 from constellate.database.migration.migrate import migrate
-from constellate.database.migration.migrationaction import MigrationAction
+from constellate.database.migration.constant import MigrationAction
+from constellate.database.migration.migrationcontext import MigrationContext, ConnectionContext
+from constellate.database.sqlalchemy.execution.execute import execute_discard_result
+from constellate.database.sqlalchemy.expression.schema.create import CreateSchema
 from constellate.database.sqlalchemy.sqlalchemy import SQLAlchemy
 from constellate.database.sqlalchemy.sqlalchemydbconfig import SQLAlchemyDBConfig
+from constellate.database.sqlalchemy.sqlalchemyengineconfig import _EngineConfig
 
 _POOL_CONNECTION_PERMANENT_SIZE = 10
 _POOL_CONNECTION_OVERFLOW_SIZE = 5
 
 
 class SQLAlchemyPostgresql(SQLAlchemy):
     def __init__(self):
         super().__init__()
+        self._migrate_db_creation_lock = asyncio.Lock()
+        self._migrate_db_schema_creation_lock = asyncio.Lock()
 
     def _get_database_driver_name(self) -> Optional[str]:
         return "asyncpg"
 
-    async def _create_engine(self, options: Dict = {}) -> Tuple[str, str, AsyncEngine, Engine]:
+    async def _create_engine(
+        self, instance: SQLAlchemyDBConfig, options: Dict = {}
+    ) -> _EngineConfig:
         """
         :options:
-        - host:str               . DB host
-        - port:str               . DB port
-        - username:str           . DB user name
-        - password:str           . DB password
-        - db_name:str            . DB name
-        - db_name_fallback:str    . DB name to connect to if the database "db_name" does not exist (yet)
+        - server_host:str               . DB host
+        - server_port:str               . DB port
+        - database_username:str         . DB user name
+        - database_password:str         . DB user password
+        - database_name:str             . DB name
+        - database_name_fallback:str    . DB name to connect to if the database "database_name" does not exist (yet)
+        - database_schema_name:str      . DB schema name
         - pool_connection_size:int            . Max permanent connection held in the pool. Default: 10
         - pool_connection_overflow_size:int            . Max connection returned in addition to the ones in the pool. Default: 5
         - pool_connection_timeout:float . Max timeout to return a connection, in seconds. Default: 30.0 (sec)
         - pool_pre_ping: bool. Default: False
+        - application_name: str. Default: None. Set the postgres application name (visible in logs via app=%a). src: https://stackoverflow.com/a/15691283/219728
         - custom: Dict[any,any]. Dictionary of custom attribute, never used by constellate
         - asynchronous:bool . Use asyncio enabled sqlalchemy engine. Default: False
         """
         # Create engine
         # - https://docs.sqlalchemy.org/en/14/dialects/postgresql.html
         username_port = ":".join(
-            filter(None, [options.get("username", None), options.get("password", None)])
+            filter(
+                None,
+                [options.get("database_username", None), options.get("database_password", None)],
+            )
+        )
+        host_port = ":".join(
+            filter(None, [options.get("server_host", None), options.get("server_port", None)])
         )
-        host_port = ":".join(filter(None, [options.get("host", None), options.get("port", None)]))
         credential_host = f"{username_port}@{host_port}"
 
-        db_name = options.get("db_name", None)
-        db_name_default = options.get("db_name_fallback", "postgres")
+        db_name = options.get("database_name", None)
+        db_name_default = options.get("database_name_fallback", "postgres")
+        db_schema = options.get("database_schema_name", "public")
+        execution_options = options.get("engine_execution_options", None)
+        application_name = options.get("application_name", "constellate")
 
         scheme_driver = f"postgresql+{self._get_database_driver_name()}"
         connection_uri = f"{scheme_driver}://{credential_host}/{db_name}"
         connection_uri_plain = f"postgresql://{credential_host}/{db_name}"
-        if not database_exists(connection_uri_plain):
-            await self._create_database(
-                connection_uri=f"{scheme_driver}://{credential_host}/{db_name_default}",
-                db_name=db_name,
-            )
+        connection_uri_plain_schema = f"postgresql://{credential_host}/{db_name}?schema={db_schema}"
+        connection_default_uri_plain = f"{scheme_driver}://{credential_host}/{db_name_default}"
 
+        pool_class = options.get("pool_class", QueuePool)
         pool_size = options.get("pool_connection_size", 10)
         pool_overflow_size = options.get("pool_connection_overflow_size", 5)
         pool_timeout = options.get("pool_connection_timeout", 30.0)
         pool_pre_ping = options.get("pool_pre_ping", False)
 
+        kwargs = {
+            "future": True,
+            "echo": False,
+            "echo_pool": False,
+            "poolclass": pool_class,
+        }
+
+        if pool_class == QueuePool:
+            kwargs.update(
+                {
+                    "pool_size": pool_size,
+                    "max_overflow": pool_overflow_size,
+                    "pool_timeout": pool_timeout,
+                    "pool_pre_ping": pool_pre_ping,
+                }
+            )
+        elif pool_class == NullPool:
+            kwargs.update(
+                {
+                    "pool_pre_ping": pool_pre_ping,
+                }
+            )
+        else:
+            raise NotImplementedError("Unsupported pool class so far")
+
+        kwargs_async_engine = {}
+        kwargs_sync_engine = {}
+        if execution_options is not None:
+            kwargs.update({"execution_options": execution_options})
+        if application_name is not None:
+            # asyncpg driver: 'server_settings' is a special argument to pass PG's client runtime parameters
+            # src: https://magicstack.github.io/asyncpg/current/api/index.html#connection
+            kwargs_async_engine.update(
+                connect_args={"server_settings": {"application_name": application_name}}
+            )
+            # psycopg2 driver: no special argument for the driver to pass PG's client runtime parameters
+            # src: https://www.psycopg.org/docs/module.html#psycopg2.connect
+            kwargs_sync_engine.update(connect_args={"application_name": application_name})
+
         engine = create_async_engine(
             connection_uri,
-            poolclass=QueuePool,
-            pool_size=pool_size,
-            max_overflow=pool_overflow_size,
-            pool_timeout=pool_timeout,
-            pool_pre_ping=pool_pre_ping,
-            future=True,
+            **kwargs,
+            **kwargs_async_engine,
         )
 
-        sync_engine = create_engine(
-            connection_uri_plain,
-            poolclass=QueuePool,
-            pool_size=pool_size,
-            max_overflow=pool_overflow_size,
-            pool_timeout=pool_timeout,
-            pool_pre_ping=pool_pre_ping,
-            future=True,
+        sync_engine = create_engine(connection_uri_plain, **kwargs, **kwargs_sync_engine)
+        return _EngineConfig(
+            connection_uri=connection_uri,
+            connection_uri_plain=connection_uri_plain,
+            connection_uri_plain_schema=connection_uri_plain_schema,
+            connection_default_uri=connection_default_uri_plain,
+            engine=engine,
+            sync_engine=sync_engine,
         )
-        return connection_uri, connection_uri_plain, engine, sync_engine
 
     async def _create_database(
         self, connection_uri: str = None, db_name: str = None, encoding="UTF8"
     ):
+        @execute_discard_result
+        async def __create_database(**kargs):
+            return text(f"CREATE DATABASE {db_name} ENCODING {encoding};")
+
         async with create_async_engine(
             connection_uri, isolation_level="AUTOCOMMIT"
         ).connect() as connection:
-            query = text(f"CREATE DATABASE {db_name} ENCODING {encoding};")
-            await connection.execute(query)
+            await __create_database(session=connection)
 
-    async def _migrate(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
-        migrate(
-            database_type=DatabaseType.POSTGRESQL,
-            connection_url=instance.connection_uri_plain,
-            migration_dirs=options.get("migration_dirs", []),
-            action=MigrationAction.UP,
-            logger=instance.logger,
+    async def __database_schema_create(self, connection_uri: str = None, name: str = None):
+        @execute_discard_result
+        async def __create_database_schema(**kargs):
+            return CreateSchema(name, if_not_exists=True)
+
+        async with create_async_engine(connection_uri).connect() as connection:
+            try:
+                await __create_database_schema(session=connection)
+                await connection.commit()
+            except BaseException:
+                await connection.rollback()
+                raise
+
+    async def _setup_engine_before_cursor_execute(
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
+    ):
+        await super()._setup_engine_before_cursor_execute(
+            instance=instance, engine=engine, options=options
         )
 
+        @event.listens_for(engine.sync_engine, "before_cursor_execute")
+        def switch_shard_schema_postgres(conn, cursor, statement, parameters, context, executemany):
+            if conn.engine.dialect.name == "postgresql":
+                CURRENT_SHARD_SHEMA_ID_KEY = "current_shard_schema_id"
+                NEW_SHARD_SHEMA_ID_KEY = "shard_schema_id"
+                # FIXME Use SetShardSchemaOption instead
+                shard_schema_id = conn._execution_options.get(
+                    NEW_SHARD_SHEMA_ID_KEY,
+                    context.execution_options.get(NEW_SHARD_SHEMA_ID_KEY, None),
+                )
+                current_shard_schema_id = conn.info.get(CURRENT_SHARD_SHEMA_ID_KEY, None)
+
+                if current_shard_schema_id != shard_schema_id:
+                    instance.logger.debug(
+                        f"Switching schema from {current_shard_schema_id} to {shard_schema_id}"
+                    )
+                    paths = ",".join(
+                        list(filter(lambda x: x is not None, [shard_schema_id, "public"]))
+                    )
+                    cursor.execute(f"SET search_path TO {paths}")
+                    conn.info[CURRENT_SHARD_SHEMA_ID_KEY] = shard_schema_id
+
+    async def _migrate(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
+        # Create database + schema
+        db_skip_creation = options.get("database_skip_creation", False)
+        db_schema_skip_creation = options.get("database_schema_skip_creation", False)
+        db_skip_migration = options.get("database_skip_migration", False)
+
+        if not db_skip_creation:
+            async with self._migrate_db_creation_lock:
+                # Serialize database creation to avoid race condition during concurrent
+                # migration on the same database but different schema
+                if not database_exists(instance.engine_config.connection_uri_plain):
+                    uri = make_url(instance.engine_config.connection_uri_plain)
+                    await self._create_database(
+                        connection_uri=instance.engine_config.connection_default_uri,
+                        db_name=uri.database,
+                    )
+
+        if not db_schema_skip_creation:
+            uri = make_url(instance.engine_config.connection_uri_plain_schema)
+            db_schema = (uri.normalized_query or {}).get("schema", None)
+            if isinstance(db_schema, Tuple):
+                # Case: ('public,)
+                db_schema = db_schema[0]
+
+            if db_schema is not None:
+                async with self._migrate_db_schema_creation_lock:
+                    await self.__database_schema_create(
+                        connection_uri=instance.engine_config.connection_uri, name=db_schema
+                    )
+
+        if not db_skip_migration:
+            # Migrate database
+            inspector = inspect(instance.engine_config.sync_engine)
+            await migrate(
+                connection_context=ConnectionContext(
+                    connection_url=instance.engine_config.connection_uri_plain_schema,
+                    engine=instance.engine_config.engine,
+                    session_create=functools.partial(self.session_scope, config=instance),
+                ),
+                migration_context=options.get(
+                    "migration_context",
+                    MigrationContext(
+                        database_type=DatabaseType.POSTGRESQL,
+                        action=MigrationAction.UPGRADE,
+                        schema=instance.options.get(
+                            "database_schema_name", inspector.default_schema_name
+                        ),
+                    ),
+                ),
+                user_context=self,
+                logger=instance.logger,
+            )
+
     async def _vacuum(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
         """
         :options:
         - profiles: A vacumm profile. Values:
         -- analyze: Updates statistics used by the planner (to speed up queries)
         -- default: Sensible defaults
         """
         # Vacuum requires a connection/session without transaction enabled.
-        async with instance.engine.connect().execution_options(
+        async with instance.engine_config.engine.connect().execution_options(
             isolation_level="AUTOCOMMIT"
         ) as connection:
             commands = {
                 "analyze": ["VACUUM ANALYZE;"],
                 "default": ["VACUUM (ANALYZE, VERBOSE);"],
             }
             for profile in options.get("profiles", ["default"]):
                 for statement in commands[profile]:
                     try:
-                        await connection.execute(statement)
+
+                        @execute_discard_result
+                        async def __command(**kargs):
+                            return text(statement)
+
+                        await __command(session=connection)
                     except BaseException as e:
                         raise Exception(f"Vacuum statement failed: {statement}") from e
```

## constellate/database/sqlalchemy/sqlalchemysqlite3.py

```diff
@@ -1,22 +1,25 @@
+import functools
 from contextlib import contextmanager
 from sqlite3.dbapi2 import Connection
-from typing import Dict, Tuple, Optional
+from typing import Dict, Optional
 
-from sqlalchemy import create_engine, event, text
+from sqlalchemy import event, text, inspect
+from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.ext.asyncio import create_async_engine
+from sqlalchemy.future import create_engine
 from sqlalchemy.pool import NullPool
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
-from sqlalchemy.engine import Engine
 
-from constellate.database.migration.databasetype import DatabaseType
+from constellate.database.common.databasetype import DatabaseType
 from constellate.database.migration.migrate import migrate
-from constellate.database.migration.migrationaction import MigrationAction
+from constellate.database.migration.constant import MigrationAction
+from constellate.database.migration.migrationcontext import MigrationContext, ConnectionContext
 from constellate.database.sqlalchemy.sqlalchemy import SQLAlchemy
 from constellate.database.sqlalchemy.sqlalchemydbconfig import SQLAlchemyDBConfig
+from constellate.database.sqlalchemy.sqlalchemyengineconfig import _EngineConfig
 from constellate.database.sqlite3.sqlite3 import patch_sqlite3_connect
 from constellate.database.sqlite3.sqlite3 import register_functions, Functions
 
 
 @contextmanager
 def raw_sqlite3_connection(engine, issue_begin=True, issue_commit_or_rollback=True, close=True):
     try:
@@ -38,26 +41,29 @@
 class SQLAlchemySqlite3(SQLAlchemy):
     def __init__(self):
         super().__init__()
 
     def _get_database_driver_name(self) -> Optional[str]:
         return "aiosqlite"
 
-    async def _create_engine(self, options: Dict = {}) -> Tuple[str, str, AsyncEngine, Engine]:
+    async def _create_engine(
+        self, instance: SQLAlchemyDBConfig, options: Dict = {}
+    ) -> _EngineConfig:
         """
         :options:
         - db_file:str           . Absolute db file path. Default: None (in memory db)
         - check_same_thread:bool. Default False
         - timeout:int           . Default 20s
         - uri:bool              . Default: True
         """
         db_file = options.get("db_file", None)
         uri_enabled = options.get("uri", db_file is not None)
         timeout = options.get("timeout", 20)
         check_same_thread = options.get("check_same_thread", False)
+        execution_options = options.get("engine_execution_options", None)
 
         # Create engine
         # - https://docs.sqlalchemy.org/en/14/dialects/sqlite.html?highlight=isolation_level#using-temporary-tables-with-sqlite
         # - https://docs.sqlalchemy.org/en/14/dialects/sqlite.html?highlight=isolation_level#threading-pooling-behavior
         scheme_driver = (
             "sqlite"
             if self._get_database_driver_name() == ""
@@ -78,22 +84,36 @@
         connection_uri = (
             f"{scheme_driver}:{db_file}?{check_same_thread_option}{timeout_option}{uri_option}"
         )
         connection_uri_plain = (
             f"sqlite:{db_file}?{check_same_thread_option}{timeout_option}{uri_option}"
         )
 
+        kwargs = {
+            "poolclass": NullPool,
+            "future": True,
+            "echo": False,
+            "echo_pool": False,
+        }
+        if execution_options is not None:
+            kwargs.update({"execution_options": execution_options})
+
         # To see commit statement: add echo=True, echo_pool=True
-        engine = create_async_engine(connection_uri, poolclass=NullPool, future=True)
-        # FIXME (low) Not sure if both engine can connect to the same local file
-        # sync_engine = create_async_engine(connection_uri, poolclass=NullPool, future=True)
-        return connection_uri, connection_uri_plain, engine, None
+        engine = create_async_engine(connection_uri, **kwargs)
+        sync_engine = create_engine(connection_uri_plain, **kwargs)
+        return _EngineConfig(
+            connection_uri=connection_uri,
+            connection_uri_plain=connection_uri_plain,
+            connection_uri_plain_schema=connection_uri_plain,
+            engine=engine,
+            sync_engine=sync_engine,
+        )
 
     async def _setup_engine_connection_connect(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
     ):
         # 2. Improve default db performance, per connection
         @event.listens_for(engine.sync_engine, "connect")
         def improve_perf_on_connection_start(dbapi_connection, connection_record):
             if isinstance(dbapi_connection, Connection):
                 # Prevent python sdk's pysqlite's from emitting BEGIN statement entirely
                 # Also prevent pysqlite from emitting COMMIT before any DDL statement
@@ -105,51 +125,69 @@
                     "pragma synchronous = normal;",
                     "pragma temp_store = memory;",
                 ]:
                     cursor.execute(pragma)
                 cursor.close()
 
     async def _setup_engine_connection_begin(
-        self, instance: SQLAlchemyDBConfig, engine=None, options: Dict = None
+        self, instance: SQLAlchemyDBConfig, engine: AsyncEngine = None, options: Dict = None
     ):
         """
         :options:
         - Key: functions:Dict. Eg: {'my_custom_function': (1, lambda foo: return random_stuff)}
         """
+
         # Register custom SQL function
         @event.listens_for(engine.sync_engine, "begin")
         def do_begin(conn):
             conn.execute(
                 text(
                     "BEGIN -- Note: BEGIN(implicty) (in the sqlalchemy engine logs) means SQLAlchemy considers this moment to be the start of a transaction block BUT did not send any BEGIN statement to the database. Hence the explicit: BEGIN"
                 )
             )
             functions = options.get("functions", {})
             register_functions(connection=conn.connection, functions=functions)
 
     async def _migrate(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
-        migrate(
-            database_type=DatabaseType.SQLITE,
-            connection_url=instance.connection_uri_plain,
-            migration_dirs=options.get("migration_dirs", []),
-            action=MigrationAction.UP,
-            logger=instance.logger,
-        )
+        migration_skipped = options.get("database_skip_migration", False)
+        inspector = inspect(instance.engine_config.sync_engine)
+
+        if not migration_skipped:
+            await migrate(
+                connection_context=ConnectionContext(
+                    connection_url=instance.engine_config.connection_uri_plain_schema,
+                    engine=instance.engine_config.engine,
+                    session_create=functools.partial(self.session_scope, config=instance),
+                ),
+                migration_context=options.get(
+                    "migration_context",
+                    MigrationContext(
+                        database_type=DatabaseType.SQLITE,
+                        action=MigrationAction.UPGRADE,
+                        schema=None,
+                    ),
+                ),
+                user_context=self,
+                logger=instance.logger,
+            )
 
     async def _vacuum(self, instance: SQLAlchemyDBConfig = None, options: Dict = {}):
         """
         :options:
         - profiles: A vacumm profile. Values:
         -- analyze: Updates statistics used by the planner (to speed up queries)
         -- default: Sensible defaults
         """
         # Vacuum requires a connection/session without transaction enabled.
         # src: https://phiresky.github.io/blog/2020/sqlite-performance-tuning/
         with raw_sqlite3_connection(
-            instance.engine, issue_begin=True, issue_commit_or_rollback=True, close=True
+            instance.engine_config.engine,
+            issue_begin=True,
+            issue_commit_or_rollback=True,
+            close=True,
         ) as connection:
             pragma = "pragma wal_checkpoint(TRUNCATE);"
             cursor = connection.execute(pragma)
             data = cursor.fetchone()
             if data is None or len(data) == 0:
                 raise Exception(f"{pragma} failed: {data}")
```

## constellate/database/sqlalchemy/utils/sql_query.py

```diff
@@ -1,41 +1,51 @@
 from typing import Dict, Union
 
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
-from sqlalchemy.orm.query import Query
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.default import DefaultDialect
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
 from sqlalchemy.sql import Select, Executable
 
 
 def stringify(
     query: Union[Select, Executable] = None,
     engine: Engine = None,
     dialect: DefaultDialect = None,
     compile_kwargs: Dict = {},
 ) -> str:
-    """
-    @query: Query object to get plain SQL query from
+    """@query: Query object to get plain SQL query from
     @engine: Database type to know the SQL dialect to convert into
 
     src: https://stackoverflow.com/a/23835766/219728
+
+    :param query: Union[Select:
+    :param Executable]:  (Default value = None)
+    :param engine: Engine:  (Default value = None)
+    :param dialect: DefaultDialect:  (Default value = None)
+    :param compile_kwargs: Dict:  (Default value = {})
+
     """
     return (
         query.compile(engine)
         if engine is not None
         else query.compile(
             dialect=dialect, compile_kwargs={"literal_binds": True, **compile_kwargs}
         )
     )
 
 
 async def resolve_engine_from_query(
     session: AsyncSession = None, query: Union[Select, Executable] = None
 ) -> AsyncEngine:
     """
-    Resovle the engine used by the query. Useful when the db session uses shards
+    Resolve the engine used by the query. Useful when the db session uses shards
     """
-    # PERF: This will execute the query!!!! As of 2021 Mai, I did not find a way to get this info without executing the
+    # PERF: This will execute the query!!!! As of 2021 May, I did not find a way to get this info without executing the
     # query against the db
-    _ignore_result = await session.execute(query)
-    engine = _ignore_result.raw.connection.engine
+    result = await session.execute(query)
+
+    # Fetch 1 or 0 result and **release the underlying cursor**, to prevent
+    # virtual transaction to be held open on the database
+    ignored = result.scalars().all()
+
+    engine = result.raw.connection.engine
     return engine
```

## constellate/database/sqlite3/sqlite3.py

```diff
@@ -1,13 +1,21 @@
 from typing import Dict, Tuple, Callable
+from sqlalchemy.pool.base import _ConnectionFairy
 
 
-def register_functions(connection, functions: Dict[str, Tuple[int, Callable]] = {}):
-    """
-    Register custom functions
+def register_functions(
+    connection: _ConnectionFairy, functions: Dict[str, Tuple[int, Callable]] = {}
+) -> None:
+    """Register custom functions
+
+    :param connection: _ConnectionFairy:
+    :param functions: Dict[str:
+    :param Tuple[int:
+    :param Callable]]:  (Default value = {})
+
     """
 
     def _register(
         connection, function_name: str = "my_func", num_params: int = 0, function: Callable = None
     ):
         connection.create_function(function_name, num_params, function)
 
@@ -37,14 +45,19 @@
 
     :original_connect: See example below
 
     import _sqlite3
     import sqlite3
 
     sqlite3.connect = ...monkeypatch_sqlite3_connect_enable(_sqlite3.connect)
+
+    :param original_connect:
+    :param enable: bool:  (Default value = True)
+    :param functions: Functions:  (Default value = {})
+
     """
 
     def connect_decorator(*args, **kwargs):
         connection = original_connect(*args, **kwargs)
         register_functions(connection=connection, functions=functions)
         return connection
```

## constellate/debugger/debugger.py

```diff
@@ -11,15 +11,15 @@
     if enabled is True:
         try:
             sys.path.append("pydevd-pycharm.egg")
             import pydevd_pycharm
         except BaseException:
             print(
                 "ERROR: PyCharm's remote debugging library not installed: "
-                " - pydevd-pycharm~=202.7660.27; sys.platform=='linux'"
+                " - pydevd-pycharm~=XXX.XXXX.XX; sys.platform=='linux'"
             )
             raise
 
         try:
             pydevd_pycharm.settrace(
                 host, port=port, stdoutToServer=True, stderrToServer=True, suspend=False
             )
@@ -27,13 +27,18 @@
             if not skip_on_missing_debug_server:
                 raise e
 
 
 def debugger_setup_stage(
     stage: str = None, enabled_stages: List[str] = [], skip_on_missing_debug_server: bool = False
 ):
+    """Enable remote debugger if the current stage is one of the enabled stages
+
+    :param stage: str:  (Default value = None)
+    :param enabled_stages: List[str]:  (Default value = [])
+    :param skip_on_missing_debug_server: bool:  (Default value = False)
+
     """
-    Enable remote debugger if the current stage is one of the enabled stages
-    """
+    enabled_stages = enabled_stages or []
     debugger_setup(
         enabled=stage in enabled_stages, skip_on_missing_debug_server=skip_on_missing_debug_server
     )
```

## constellate/logger/log.py

```diff
@@ -1,26 +1,26 @@
 import logging
 import os
-from logging.config import dictConfig
+import sys
 import threading
 import uuid
-import sys
+from logging.config import dictConfig
 from pathlib import PurePath
 from typing import Dict, Union, Tuple, List
 
+import pendulum
 from narration._handler.common.handler.base_handler import NarrationHandler
 from narration._misc.constants import DispatchMode
-from narration.narration import setup_server_handlers, setup_client_handlers
-import pendulum
 from narration.constants import Backend
+from narration.narration import setup_server_handlers, setup_client_handlers
 
 from constellate.datatype.enum.enum import has_flag
-from constellate.logger.logmode import LogMode
-from constellate.logger.loggers import Loggers
 from constellate.logger.handler.stringhandler import StringHandler
+from constellate.logger.loggers import Loggers
+from constellate.logger.logmode import LogMode
 
 
 class _LogDefault:
     LOGS_DIRECTORY = os.getcwd()
     ROOT_LOGGER_NAME = "default"
     MODE = LogMode = (
         LogMode.ENV_PRODUCTION
@@ -44,15 +44,15 @@
             "media": {
                 "logger": "default",
             },
         }
     }
 
 
-class Log(object):
+class Log:
     _LOGGER_NAMES_RETRIEVED = {}
     # Logger instance are held by python sdk private dictionary. Only loggers settings are tracked
     _FQDN_LOGGER_SETTINGS_EXTERNAL = {}
     # Logger instance are held by python sdk private dictionary. Only loggers names are tracked
     _FQDN_LOGGER_NAMES_EXTERNAL = set()
 
     _JOB_LOGGER_NAMES_LOCK = threading.Lock()
@@ -270,30 +270,37 @@
             if name in Log._FQDN_LOGGER_NAMES_EXTERNAL:
                 Log._FQDN_LOGGER_NAMES_EXTERNAL.remove(name)
             Log._LOGGER_NAMES_RETRIEVED.pop(name, None)
 
     @staticmethod
     def get_native_logger(name=None) -> Tuple[bool, logging.Logger]:
         """
-        @return A logger instance and whether it existed before
+
+        :param name:  (Default value = None)
+        :returns: A logger instance and whether it existed before
+
         """
         exist = Log._LOGGER_NAMES_RETRIEVED.get(name, False)
         if not exist:
             Log._LOGGER_NAMES_RETRIEVED[name] = True
         return exist, logging.getLogger(name)
 
     @staticmethod
     def get_hierarchical_logger(
         name: str = None,
         mode: LogMode = LogMode.OPERATE_SERVER,
         mode_settings: Dict = {},
     ):
-        """
-        name_parts: List of a logger's split into parts. Eg: foo.bar.zoo => ['foo','bar','zoo']
-        @return A logger instance
+        """name_parts: List of a logger's split into parts. Eg: foo.bar.zoo => ['foo','bar','zoo']
+
+        :param name: str:  (Default value = None)
+        :param mode: LogMode:  (Default value = LogMode.OPERATE_SERVER)
+        :param mode_settings: Dict:  (Default value = {})
+        :returns: A logger instance
+
         """
         # Construct Fully Qualified Logger Name
         existed, logger = Log.get_native_logger(name=name)
         if not existed:
             # Client mode logger should not have any handlers set by default, as it will create as many handlers as
             # the original "server" logger had
             if has_flag(mode, LogMode.OPERATE_CLIENT):
@@ -358,25 +365,33 @@
             return logger, {}
         elif has_flag(mode, LogMode.OPERATE_STANDALONE):
             return logger, {}
 
     @staticmethod
     def create_job_handler(capacity=sys.maxsize):
         """
-        @return In-Memory Handler instance
+
+        :param capacity:  (Default value = sys.maxsize)
+        :returns: In-Memory Handler instance
+
         """
         handler = StringHandler(capacity=capacity)
         formatter = logging.Formatter("%(message)s")
         handler.setFormatter(formatter)
         return handler
 
     @staticmethod
     def get_available_job_logger(level=logging.DEBUG, capacity=sys.maxsize, console=False):
         """
-        @return Create or get a free Job logger instance
+
+        :param level:  (Default value = logging.DEBUG)
+        :param capacity:  (Default value = sys.maxsize)
+        :param console:  (Default value = False)
+        :returns: Create or get a free Job logger instance
+
         """
         with Log._JOB_LOGGER_NAMES_LOCK:
             defaultHandlers = [Log._CONSOLE_HANDLER] if console else []
 
             handler = Log.create_job_handler(capacity=capacity)
             logger = logging.getLogger(name=str(uuid.uuid4()))
             logger.setLevel(level)
@@ -384,15 +399,18 @@
             for defaultHandler in [handler] + defaultHandlers:
                 logger.addHandler(defaultHandler)
             return logger
 
     @staticmethod
     def free_job_logger(logger=None):
         """
-        @return Create or get a free Job logger instance
+
+        :param logger:  (Default value = None)
+        :returns: Create or get a free Job logger instance
+
         """
         with Log._JOB_LOGGER_NAMES_LOCK:
             if logger is not None:
                 # Note: This is a private controller, at least available on Python 3.7
                 name = logger.name
                 loggers = logging.Logger.manager.loggerDict
                 if name in loggers:
@@ -402,24 +420,29 @@
 
     @staticmethod
     def loggers(
         mode: LogMode = LogMode.OPERATE_SERVER,
         mode_settings: Union[Dict, Loggers] = None,
         logger_names: List[str] = None,
     ) -> Loggers:
-        """
-        mode_settings: Settings vary per LoggerMode.
+        """mode_settings: Settings vary per LoggerMode.
 
         LoggerMode.SERVER's settings are:
         {
             ctx: mp.get_context(...),
             ctx_manager: ctx.Manager()
         }
 
         LoggerMode.CLIENT's settings be: Loggers.setting()
+
+        :param mode: LogMode:  (Default value = LogMode.OPERATE_SERVER)
+        :param mode_settings: Union[Dict:
+        :param Loggers]:  (Default value = None)
+        :param logger_names: List[str]:  (Default value = None)
+
         """
 
         def get_logger_name(parts: List[str]):
             return ".".join(parts)
 
         def get_settings(parts: List[str], mode_settings: Union[Loggers, Dict]):
             if isinstance(mode_settings, Loggers):
```

## constellate/logger/loggers.py

```diff
@@ -1,21 +1,35 @@
-from typing import Dict, List
+from typing import Optional, Union, Dict, List
+from logging import Logger
+from narration._misc.constants import DispatchMode
+from narration.constants import Backend
 
 
 class Loggers:
-    def __init__(self):
+    def __init__(self) -> None:
         self._logger_settings_property_names = set()
         self._logger_property_names = {}
+        self._logger_settings_only = False
 
-    def setup_logger(self, parts: List[str] = None, logger=None, settings: Dict = None):
-        """
-        Once populated with name 'foobar':
+    @property
+    def is_settings_only(self) -> bool:
+        return self._logger_settings_only
+
+    def setup_logger(
+        self, parts: List[str] = None, logger: Optional[Logger] = None, settings: Dict = None
+    ) -> None:
+        """Once populated with name 'foobar':
          - Loggers().foobar and Loggers().foobar_settings will exists
         Once populated with name 'foobar.test':
          - Loggers().foobar.test and Loggers().foobar_test_settings will exists
+
+        :param parts: List[str]:  (Default value = None)
+        :param logger: Optional[Logger]:  (Default value = None)
+        :param settings: Dict:  (Default value = None)
+
         """
         if parts is None or len(parts) <= 1:
             return
 
         count = len(parts) + 1
         parent = self
         for part_index in range(1, count):
@@ -37,46 +51,60 @@
                     key = self._get_logger_setting_property_name(long_name)
                     self._set_property_settings(key, settings)
             elif is_first:
                 parent = self
             else:
                 parent = self._get_property(parent, short_name, None)
 
-    def _set_property_logger(self, obj, short_name, long_name, value):
+    def _set_property_logger(
+        self, obj: Union[Logger], short_name: str, long_name: str, value: Optional[Logger]
+    ) -> None:
         self._set_property(obj, short_name, value)
         self._logger_property_names.update({long_name: value})
 
-    def _set_property_settings(self, name, value):
+    def _set_property_settings(
+        self, name: str, value: Dict[str, Dict[str, Union[int, str, Backend, float, DispatchMode]]]
+    ) -> None:
         self._set_property(self, name, value)
         self._logger_settings_property_names.add(name)
 
-    def _get_logger_setting_property_name(self, name):
+    def _get_logger_setting_property_name(self, name: str) -> str:
         return f"{name}_settings"
 
     def _get_settings(self, parts: List[str]):
         long_name = "_".join(parts)
         key = self._get_logger_setting_property_name(long_name)
         return self._get_property(self, key, None)
 
-    def _get_property(self, obj, key, default_value):
+    def _get_property(
+        self, obj: Union[Logger], key: str, default_value: None
+    ) -> Union[Dict[str, Dict[str, Union[int, str, Backend, float, DispatchMode]]], Logger]:
         return obj.__dict__.get(key, default_value)
 
-    def _set_property(self, obj, key, value):
+    def _set_property(
+        self,
+        obj: Union[Logger],
+        key: str,
+        value: Optional[
+            Union[Dict[str, Dict[str, Union[int, str, Backend, float, DispatchMode]]], Logger]
+        ],
+    ) -> None:
         obj.__dict__[key] = value
 
-    def settings(self):
+    def settings(self) -> "Loggers":
         loggers = Loggers()
+        loggers._logger_settings_only = True
         for name in self._logger_settings_property_names:
             value_settings = self._get_property(self, name, None)
             loggers._set_property_settings(name, value_settings)
         for long_name in list(self._logger_property_names.keys()):
             short_name = long_name.split("_")[-1]
             loggers._set_property_logger(loggers, short_name, long_name, None)
         return loggers
 
-    def native_loggers(self):
+    def native_loggers(self) -> List[Logger]:
         return list(
             filter(
                 None,
                 [logger for logger in list(self._logger_property_names.values())],
             )
         )
```

## constellate/logger/simple.py

```diff
@@ -1,26 +1,33 @@
 import multiprocessing
 from typing import Dict
 
-from narration.narration import teardown_handlers
+from narration.narration import teardown_handlers, logger_dispatch_remaining_messages
 
 from constellate.logger.log import Log
-from constellate.logger.logmode import LogMode
 from constellate.logger.loggers import Loggers
+from constellate.logger.logmode import LogMode
+from multiprocessing.context import SpawnContext
 
 
 def setup_any_process_loggers(
-    root_logger_name="unnamped",
+    root_logger_name: str = "unnamped",
     log_dir_path: str = None,
     mode: LogMode = None,
     config_dict: Dict = None,
     template_dict: Dict = None,
-):
-    """
-    Setup constant applying to all loggers
+) -> None:
+    """Setup constant applying to all loggers
+
+    :param root_logger_name: str:  (Default value = "unnamped")
+    :param log_dir_path: str:  (Default value = None)
+    :param mode: LogMode:  (Default value = None)
+    :param config_dict: Dict:  (Default value = None)
+    :param template_dict: Dict:  (Default value = None)
+
     """
     kwargs = {}
     if root_logger_name is not None:
         kwargs.update(root_logger_name=root_logger_name)
     if log_dir_path is not None:
         kwargs.update(log_dir_path=log_dir_path)
     if mode is not None:
@@ -35,43 +42,46 @@
     elif template_dict is not None:
         kwargs.update(template_config_dict=template_dict)
 
     Log.setup(**kwargs)
 
 
 def setup_standalone_process_loggers() -> Loggers:
-    """
-    Setup loggers for an project (no logging to be shared with child processes , if any)
-    """
+    """Setup loggers for an project (no logging to be shared with child processes , if any)"""
     mode_settings = {}
     return Log.loggers(mode=LogMode.OPERATE_STANDALONE, mode_settings=mode_settings)
 
 
-def setup_main_process_loggers(ctx=multiprocessing.get_context()) -> Loggers:
-    """
-    Setup loggers in "server mode" for an project's main process
+def setup_main_process_loggers(ctx: SpawnContext = multiprocessing.get_context()) -> Loggers:
+    """Setup loggers in "server mode" for an project's main process
+
+    :param ctx: SpawnContext:  (Default value = multiprocessing.get_context())
+
     """
     mode_settings = {"ctx": ctx, "ctx_manager": ctx.Manager()}
     return Log.loggers(
         mode=LogMode.OPERATE_SERVER
         | LogMode.OPERATE_SERVER_OPTION_DEFAULT
         | LogMode.DISPATCH_ASYNC,
         mode_settings=mode_settings,
     )
 
 
 def setup_child_process_loggers(mode_settings: Loggers = Loggers()) -> Loggers:
-    """
-    Setup loggers in "client" mode for an project's child process (ie forked, spawn, etc)
+    """Setup loggers in "client" mode for an project's child process (ie forked, spawn, etc)
+
+    :param mode_settings: Loggers:  (Default value = Loggers())
+
     """
 
     kwargs = {}
     if mode_settings is not None:
         kwargs.update(mode_settings=mode_settings)
     return Log.loggers(mode=LogMode.OPERATE_CLIENT, **kwargs)
 
 
-def teardown_loggers(loggers: Loggers = None, timeout=None):
+def teardown_loggers(loggers: Loggers = None, timeout: None = None) -> None:
     native_loggers = loggers.native_loggers() if loggers is not None else []
+    logger_dispatch_remaining_messages(loggers=native_loggers)
     teardown_handlers(loggers=native_loggers, timeout=timeout)
     "Free/Remove all loggers setup previously"
     Log.teardown_loggers(loggers=native_loggers)
```

## constellate/logger/handler/forwarderhandler.py

```diff
@@ -1,15 +1,13 @@
 import logging
 from typing import Union
 
 
 class LoggerProxyHandler(logging.Handler):
-    """
-    Forward logging messages to a target logger from the logger this handler is attached to
-    """
+    """Forward logging messages to a target logger from the logger this handler is attached to"""
 
     def __init__(self, target_logger: logging.Logger = None, level: Union[int, str] = "DEBUG"):
         super().__init__(level=level)
         self._target_logger = target_logger
 
     def emit(self, record: logging.LogRecord) -> None:
         if self._target_logger is not None and self._target_logger.isEnabledFor(record.levelno):
```

## constellate/network/url/unshortener.py

```diff
@@ -1,12 +1,11 @@
 import requests
 
 
 def unshorten_url(short_url):
-
     r = requests.head(short_url)
     if r.status_code >= 200 and r.status_code < 400:
         url = r.headers.get("location", None)
         if url is not None:
             return url
 
     return None
```

## constellate/project/version.py

```diff
@@ -1,8 +1,5 @@
-from collections import namedtuple
-
-
 def version_int(version: str = "0.0.0") -> int:
     # Integer version
     parts = [int(x, 10) for x in version.split(".")]
     parts.reverse()
-    return sum(x * (1000 ** i) for i, x in enumerate(parts))
+    return sum(x * (1000**i) for i, x in enumerate(parts))
```

## constellate/resource/resource.py

```diff
@@ -1,61 +1,66 @@
 import atexit
-from contextlib import ExitStack, contextmanager
+from contextlib import ExitStack
 from pathlib import PurePath
-from typing import List, Union, Generator, Iterable
+from typing import List, Union
 
 import importlib_resources
 from deprecated.classic import deprecated
-from pkg_resources import resource_listdir
 
 
-def _get_file_manager_cleanup_on_exit():
+def _get_file_manager_cleanup_on_exit() -> ExitStack:
     file_manager = ExitStack()
     # Cleanup context managed files, at program shutdown
     atexit.register(file_manager.close)
     return file_manager
 
 
 @deprecated(
     version="0.5.13",
     reason="Folder possibly extracted in a tmp dir is not cleanup until the program exit.",
 )
 def get_folder(root_pkg_name: str = __package__, directory: str = "data") -> Union[PurePath, str]:
-    """
-    Retrieve folder in module: root_pkg_name.directory
-    @params:
-    - root_pk_name: Typically my_module.__package__
-    @returns: Absolute path
+    """Retrieve folder in module: root_pkg_name.directory
+
+    :param s: root_pk_name: Typically my_module.__package__
+    :param root_pkg_name: str:  (Default value = __package__)
+    :param directory: str:  (Default value = "data")
+    :returns: s: Absolute path
+
     """
     file_manager = _get_file_manager_cleanup_on_exit()
     ref = importlib_resources.files(root_pkg_name) / directory
     path = file_manager.enter_context(importlib_resources.as_file(ref))
     return path
 
 
 @deprecated(
     version="0.5.13",
     reason="Files/Folder possibly extracted in a tmp dir are not cleanup until the program exit. Use importlib.files(...) instead",
 )
 def get_files(
     root_pkg_name: str = __package__, directory: str = "data", ignore_init_file: bool = True
 ) -> List[Union[PurePath, str]]:
-    """
-    Retrieve list of files in module: root_pkg_name.directory
-    @params:
-    - root_pk_name: Typically my_module.__package__
-    @returns: List of absolute paths
+    """Retrieve list of files in module: root_pkg_name.directory
+
+    :param s: root_pk_name: Typically my_module.__package__
+    :param root_pkg_name: str:  (Default value = __package__)
+    :param directory: str:  (Default value = "data")
+    :param ignore_init_file: bool:  (Default value = True)
+    :returns: s: List of absolute paths
+
     """
     paths = [
         filename for filename in importlib_resources.files(f"{root_pkg_name}.{directory}").iterdir()
     ]
 
     paths = [
         p
         for p in paths
-        if not str(p).endswith("__init__.py") and not str(p).endswith("__pycache__")
+        if (ignore_init_file and not str(p).endswith("__init__.py"))
+        and not str(p).endswith("__pycache__")
     ]
     return paths
 
 
 # FUTURE: Migrating to python std lib:
 # https://importlib-resources.readthedocs.io/en/latest/migration.html#pkg-resources-resource-listdir
```

## constellate/storage/filesystem/anyfs/path.py

```diff
@@ -1,102 +1,111 @@
-from pathlib import PurePath
+from pathlib import PurePath, Path
+from typing import Union
 
 
-def get_immediate_parent_folder_if_file(filePath) -> PurePath:
-    path = PurePath(filePath)
-    return path if path.is_dir() else PurePath.parent
+def _get_path(file_path: Union[str, Path]) -> Path:
+    return Path(file_path) if isinstance(file_path, str) else file_path
 
 
-def get_basename_without_extension(filePath) -> str:
-    path = PurePath(filePath)
-    extension = path.suffix
-    extensionLenght = +len(path.name) if len(extension) == 0 else -len(extension)
-    baseName = path.name[:extensionLenght]
-    return baseName
+def get_immediate_parent_folder_if_file(file_path: Union[str, Path]) -> PurePath:
+    file_path2 = _get_path(file_path)
+    return file_path2 if file_path2.is_dir() else file_path2.parent
 
 
-def get_path_without_extension(filePath) -> str:
-    """
-    Get path without the extension
-    @param filePath File Path
-    @return File path without the new extension
+def get_basename_without_extension(file_path: Union[str, Path]) -> str:
+    extension = file_path.suffix
+    extension_lenght = +len(file_path.name) if len(extension) == 0 else -len(extension)
+    base_name = file_path.name[:extension_lenght]
+    return base_name
+
+
+def get_path_without_extension(file_path: Union[str, Path]) -> str:
+    """Get path without the extension
+
+    :param file_path: File Path
+    :returns: File path without the new extension
             Eg: /path/to/file.txt -> /path/to/file
+
     """
-    path = PurePath(filePath)
-    parent = path.parent
-    baseName = get_basename_without_extension(filePath)
-    return str(PurePath(parent, baseName))
+    file_path2 = _get_path(file_path)
+    parent = file_path2.parent
+    base_name = get_basename_without_extension(file_path)
+    return str(PurePath(parent, base_name))
 
 
-def get_path_with_extension(filePath, newExtension) -> PurePath:
-    """
-    Get path with the new extension instead
-    @param filePath File Path
-    @param newExtension Extension to use in the file path
-    @return File path with the new extension
-    """
-    path = get_path_without_extension(filePath)
-    return PurePath(f"{path}.{newExtension}")
+def get_path_with_extension(file_path, new_extension) -> PurePath:
+    """Get path with the new extension instead
 
+    :param file_path: File Path
+    :param new_extension: Extension to use in the file path
+    :returns: File path with the new extension
 
-def get_path_with_parent_and_extension(filePath, newParent, newExtension) -> PurePath:
-    """
-    Get path with the new extension instead
-    @param filePath File Path
-    @param newParent Parent path to use in the file path
-    @param newExtension Extension to use in the file path
-    @return File path with the new parent/extension
     """
-    basename = get_basename_without_extension(filePath)
-    return PurePath(newParent, f"{basename}.{newExtension}")
+    path = get_path_without_extension(file_path)
+    return PurePath(f"{path}.{new_extension}")
 
 
-def get_purepath(filePath) -> PurePath:
-    return PurePath(filePath)
+def get_path_with_parent_and_extension(file_path, new_parent, new_extension) -> PurePath:
+    """Get path with the new extension instead
 
+    :param file_path: File Path
+    :param new_parent: Parent path to use in the file path
+    :param new_extension: Extension to use in the file path
+    :returns: File path with the new parent/extension
 
-def get_file_extension(filePath) -> str:
-    """
-    Get file extension, dotless
     """
-    path = PurePath(filePath)
-    return path.suffix[1:].casefold().lower()
+    basename = get_basename_without_extension(file_path)
+    return PurePath(new_parent, f"{basename}.{new_extension}")
+
+
+def get_purepath(file_path) -> PurePath:
+    return PurePath(file_path)
 
 
-def is_hidden_file(filePath) -> str:
-    basename = get_basename_without_extension(filePath)
+def get_file_extension(file_path) -> str:
+    """Get file extension, dotless"""
+    file_path2 = _get_path(file_path)
+    return file_path2.suffix[1:].casefold().lower()
+
+
+def is_hidden_file(file_path: Union[str, Path]) -> str:
+    basename = get_basename_without_extension(file_path)
     return basename.startswith(".")
 
 
 def escape_occurences(source, escape_string) -> str:
-    """
-    Escape all characters with the escape string.
-    @param source String to escape
-    @param escape_string String to escape the first string with
-    @return Escaped string
+    """Escape all characters with the escape string.
+
+    :param source: String to escape
+    :param escape_string: String to escape the first string with
+    :returns: Escaped string
+
     """
     assert isinstance(source, str), "source must be a str"
 
     escaped_string = list()
     for c in source:
         escaped_string.append(escape_string)
         escaped_string.append(c)
 
     return "".join(escaped_string)
 
 
-def escape_path(path) -> str:
-    """
-    Escape all characters with the escape string.
-    @param path String to escape
-    @param anEscapeString String to escape the first string with
-    @return Escaped string
+def escape_path(file_path) -> str:
+    """Escape all characters with the escape string.
+
+    :param file_path: String to escape
+    :returns: Escaped string
+
     """
-    return escape_occurences(path, "\\")
+    return escape_occurences(file_path, "\\")
 
 
 def same_path(path1, path2) -> bool:
-    """
-    Case sensitive path check
+    """Case sensitive path check
     Assume linux fs path (ie case sensitive paths)
+
+    :param path1:
+    :param path2:
+
     """
     return str(path1) == str(path2)
```

## constellate/storage/filesystem/anyfs/size.py

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
 
 from constellate.storage.filesystem.anyfs.path import get_purepath
 
 
 def file_size(path):
-    """
-    Get file size in bytes
+    """Get file size in bytes
+
+    :param path:
+
     """
     file = get_purepath(path)
     return -1 if file is None else Path(file).stat().st_size
```

## constellate/storage/filesystem/tmpfs/rambacked.py

```diff
@@ -1,23 +1,56 @@
-from memory_tempfile import MemoryTempfile
-import tempfile
 import os
+import tempfile
+import platform
+from contextlib import contextmanager
+from pathlib import Path
 
+from memory_tempfile import MemoryTempfile
+from typing import Optional
+
+
+def mkd_tmpfs(
+    prefix: Optional[str] = None, suffix: Optional[str] = None, dir: None = None
+) -> tempfile.TemporaryDirectory:
+    """Create a temporary directory, preferably RAM backed, for speed
+
+    :param prefix: Optional[str]:  (Default value = None)
+    :param suffix: Optional[str]:  (Default value = None)
+    :param dir: None:  (Default value = None)
+    :returns: tempfile.TemporaryDirectory
 
-def mkd_tmpfs(prefix=None, suffix=None, dir=None):
-    """
-    Create a temporary directory, preferably RAM back, for speed
-    @return tempfile.TemporaryDirectory
     """
     tmpfs_dir = os.environ.get("TMPFS_DIR", None)
     additional_paths = [tmpfs_dir] if tmpfs_dir is not None else []
     temp = MemoryTempfile(additional_paths=additional_paths, fallback=True)
-    if not hasattr(temp, "tempdir"):
+    if platform.system() in ["Darwin"] and not hasattr(temp, "tempdir"):
         # Bug: memory_tempfile does not set the temp.tempdir attribute on non Linux OSes
         # Attribute set manually as a workaround until the library is
         # eventually fixed
-        setattr(temp, "tempdir", tempfile.mkdtemp(prefix=prefix, suffix=suffix, dir=dir))
+        setattr(temp, "tempdir", tempfile.mkdtemp(dir=dir))
     return temp.TemporaryDirectory(prefix=prefix, suffix=suffix, dir=dir)
 
 
-def mkd_tmp(prefix=None, suffix=None, dir=None):
+def mkd_tmp(
+    prefix: Optional[str] = None, suffix: Optional[str] = None, dir: Optional[str] = None
+) -> tempfile.TemporaryDirectory:
     return tempfile.TemporaryDirectory(prefix=prefix, suffix=suffix, dir=dir)
+
+
+@contextmanager
+def mkf_tmpfs(
+    prefix: Optional[str] = None, suffix: Optional[str] = None, dir: Optional[str] = None
+) -> Path:
+    """Create a temporary file, preferably RAM backed, for speed
+
+    :param prefix: Optional[str]:  (Default value = None)
+    :param suffix: Optional[str]:  (Default value = None)
+    :param dir: Optional[str]:  (Default value = None)
+
+    """
+    with mkd_tmpfs(dir=dir) as tmp_dir:
+        file_name = None
+        with tempfile.NamedTemporaryFile(
+            prefix=prefix, suffix=suffix, dir=tmp_dir, delete=False
+        ) as f:
+            file_name = f.name
+        yield Path(file_name)
```

