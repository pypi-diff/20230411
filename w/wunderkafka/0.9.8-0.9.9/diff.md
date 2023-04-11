# Comparing `tmp/wunderkafka-0.9.8.tar.gz` & `tmp/wunderkafka-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wunderkafka-0.9.8.tar", last modified: Thu Oct  6 09:03:01 2022, max compression
+gzip compressed data, was "wunderkafka-0.9.9.tar", last modified: Mon Oct 17 12:48:42 2022, max compression
```

## Comparing `wunderkafka-0.9.8.tar` & `wunderkafka-0.9.9.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.258758 wunderkafka-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-06 09:03:01.258758 wunderkafka-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-10-06 09:03:01.258758 wunderkafka-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.246758 wunderkafka-0.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.250758 wunderkafka-0.9.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/integration/test_deserializing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/integration/test_serializing_avromodel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.250758 wunderkafka-0.9.8/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/smoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/smoke/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/smoke/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/smoke/test_factories.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.250758 wunderkafka-0.9.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_derive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_fs_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_krb_timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_parse_kinit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/tests/unit/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.250758 wunderkafka-0.9.8/wunderkafka/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/compat/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/config/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/config/generated/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/generated/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/generated/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/generated/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/rdkafka.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/config/schema_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/consumers/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/consumers/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/consumers/bytes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5523 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/consumers/constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/consumers/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/hotfixes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/hotfixes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/
--rw-r--r--   0 runner    (1001) docker     (121)     6424 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/krb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/krb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/krb/ticket.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/producers/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/producers/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/producers/bytes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/producers/constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/schema_registry/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4813 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/cloudera_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/confluent_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/schema_registry/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka/serdes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.258758 wunderkafka-0.9.8/wunderkafka/serdes/avro/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avro/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/avromodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/serdes/store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.258758 wunderkafka-0.9.8/wunderkafka/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/tests/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/tests/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/tests/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/time.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-06 09:02:54.000000 wunderkafka-0.9.8/wunderkafka/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:03:01.254758 wunderkafka-0.9.8/wunderkafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-06 09:03:01.000000 wunderkafka-0.9.8/wunderkafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2543 2022-10-06 09:03:01.000000 wunderkafka-0.9.8/wunderkafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 09:03:01.000000 wunderkafka-0.9.8/wunderkafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-06 09:03:01.000000 wunderkafka-0.9.8/wunderkafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-06 09:03:01.000000 wunderkafka-0.9.8/wunderkafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-10-17 12:48:42.251072 wunderkafka-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.239071 wunderkafka-0.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/integration/test_deserializing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/integration/test_serializing_avromodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/smoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/smoke/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/smoke/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/smoke/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_derive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_fs_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_krb_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_parse_kinit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/tests/unit/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/wunderkafka/
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/wunderkafka/compat/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/config/generated/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/generated/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/generated/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/generated/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/rdkafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/config/schema_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/consumers/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/consumers/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/consumers/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5523 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/consumers/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/consumers/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/hotfixes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/hotfixes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (121)     6424 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/krb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/krb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/krb/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/producers/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/producers/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/producers/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/producers/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/schema_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/schema_registry/clients/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4813 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/clients/cloudera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/clients/confluent.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/schema_registry/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/serdes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/serdes/avro/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/structures.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avro/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/avromodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/serdes/store.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.247072 wunderkafka-0.9.9/wunderkafka/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/tests/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/tests/producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/tests/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-17 12:48:36.000000 wunderkafka-0.9.9/wunderkafka/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 12:48:42.243072 wunderkafka-0.9.9/wunderkafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-17 12:48:42.000000 wunderkafka-0.9.9/wunderkafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-10-17 12:48:42.000000 wunderkafka-0.9.9/wunderkafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 12:48:42.000000 wunderkafka-0.9.9/wunderkafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-17 12:48:42.000000 wunderkafka-0.9.9/wunderkafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-17 12:48:42.000000 wunderkafka-0.9.9/wunderkafka.egg-info/top_level.txt
```

### Comparing `wunderkafka-0.9.8/LICENSE` & `wunderkafka-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/PKG-INFO` & `wunderkafka-0.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wunderkafka
-Version: 0.9.8
+Version: 0.9.9
 Summary: librdkafka-powered client for Kafka for python with (hopefully) more handful API
 Home-page: https://github.com/severstal-digital/wunderkafka
 Author: Kirill Tribunsky
 Author-email: tribunsky.kir@yandex.ru
 License: Apache-2.0 License
 Project-URL: Bug Tracker, https://github.com/severstal-digital/wunderkafka/issues
 Keywords: kafka,cloudera
```

### Comparing `wunderkafka-0.9.8/README.md` & `wunderkafka-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/setup.cfg` & `wunderkafka-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wunderkafka
-version = 0.9.8
+version = 0.9.9
 description = librdkafka-powered client for Kafka for python with (hopefully) more handful API
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = kafka, cloudera
 license = Apache-2.0 License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `wunderkafka-0.9.8/tests/integration/test_deserializing.py` & `wunderkafka-0.9.9/tests/integration/test_deserializing.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/integration/test_serializing_avromodel.py` & `wunderkafka-0.9.9/tests/integration/test_serializing_avromodel.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/smoke/test_callbacks.py` & `wunderkafka-0.9.9/tests/smoke/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/smoke/test_configs.py` & `wunderkafka-0.9.9/tests/smoke/test_configs.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/smoke/test_factories.py` & `wunderkafka-0.9.9/tests/smoke/test_factories.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/unit/test_derive.py` & `wunderkafka-0.9.9/tests/unit/test_derive.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import time
 from typing import Optional
 from datetime import datetime
 from dataclasses import dataclass
 
 import pytest
-from pydantic import BaseModel, BaseSettings, Field
+from pydantic import Field, BaseModel, BaseSettings
 
 from wunderkafka.compat.types import AvroModel
 from wunderkafka.serdes.avromodel import derive
 
 
 @dataclass
 class SomeData(AvroModel):
```

### Comparing `wunderkafka-0.9.8/tests/unit/test_fs_repo.py` & `wunderkafka-0.9.9/tests/unit/test_fs_repo.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/unit/test_headers.py` & `wunderkafka-0.9.9/tests/unit/test_headers.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/unit/test_krb_timeout.py` & `wunderkafka-0.9.9/tests/unit/test_krb_timeout.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/unit/test_parse_kinit.py` & `wunderkafka-0.9.9/tests/unit/test_parse_kinit.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/tests/unit/test_subscription.py` & `wunderkafka-0.9.9/tests/unit/test_subscription.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/__init__.py` & `wunderkafka-0.9.9/wunderkafka/__init__.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/callbacks.py` & `wunderkafka-0.9.9/wunderkafka/callbacks.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/compat/types.py` & `wunderkafka-0.9.9/wunderkafka/compat/types.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/config/generated/enums.py` & `wunderkafka-0.9.9/wunderkafka/config/generated/enums.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/config/generated/fields.py` & `wunderkafka-0.9.9/wunderkafka/config/generated/fields.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/config/generated/models.py` & `wunderkafka-0.9.9/wunderkafka/config/generated/models.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/config/rdkafka.py` & `wunderkafka-0.9.9/wunderkafka/config/rdkafka.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/config/schema_registry.py` & `wunderkafka-0.9.9/wunderkafka/config/schema_registry.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/consumers/abc.py` & `wunderkafka-0.9.9/wunderkafka/consumers/abc.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/consumers/bytes.py` & `wunderkafka-0.9.9/wunderkafka/consumers/bytes.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/consumers/constructor.py` & `wunderkafka-0.9.9/wunderkafka/consumers/constructor.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/consumers/subscription.py` & `wunderkafka-0.9.9/wunderkafka/consumers/subscription.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/errors.py` & `wunderkafka-0.9.9/wunderkafka/errors.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/factories.py` & `wunderkafka-0.9.9/wunderkafka/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """This module contains some ready-to-go combinations of the Consumer/Producer."""
 
-from typing import Dict, Optional, Union, Type
+from typing import Dict, Type, Union, Optional
 
 from wunderkafka import ConsumerConfig, ProducerConfig
 from wunderkafka.types import TopicName, MessageDescription
 from wunderkafka.serdes.avro import (
     FastAvroSerializer,
     AvroModelSerializer,
     FastAvroDeserializer,
     ConfluentClouderaHeadersHandler,
 )
 from wunderkafka.serdes.store import AvroModelRepo, SchemaTextRepo
 from wunderkafka.consumers.bytes import BytesConsumer
 from wunderkafka.producers.bytes import BytesProducer
-from wunderkafka.schema_registry import SimpleCache, ClouderaSRClient, KerberizableHTTPClient, ConfluentSRClient
+from wunderkafka.schema_registry import SimpleCache, ClouderaSRClient, KerberizableHTTPClient
 from wunderkafka.hotfixes.watchdog import check_watchdog
 from wunderkafka.consumers.constructor import HighLevelDeserializingConsumer
 from wunderkafka.producers.constructor import HighLevelSerializingProducer
+from wunderkafka.schema_registry.clients.confluent import ConfluentSRClient
 
 
 class AvroConsumer(HighLevelDeserializingConsumer):
     """Kafka Consumer client to get AVRO-serialized messages from Confluent/Cloudera installation."""
 
     def __init__(
         self,
```

### Comparing `wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/__init__.py` & `wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import time
 import subprocess
-from typing import Any, Dict, Tuple, Optional, Set
+from typing import Any, Set, Dict, Tuple, Optional
 from threading import Thread
 from dataclasses import dataclass
 
 from confluent_kafka import libversion
 
 from wunderkafka.time import ts2dt
 from wunderkafka.logger import logger
```

### Comparing `wunderkafka-0.9.8/wunderkafka/hotfixes/watchdog/krb/ticket.py` & `wunderkafka-0.9.9/wunderkafka/hotfixes/watchdog/krb/ticket.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/producers/abc.py` & `wunderkafka-0.9.9/wunderkafka/producers/abc.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/producers/bytes.py` & `wunderkafka-0.9.9/wunderkafka/producers/bytes.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/producers/constructor.py` & `wunderkafka-0.9.9/wunderkafka/producers/constructor.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/protocols.py` & `wunderkafka-0.9.9/wunderkafka/protocols.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/schema_registry/abc.py` & `wunderkafka-0.9.9/wunderkafka/schema_registry/abc.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/schema_registry/cloudera_client.py` & `wunderkafka-0.9.9/wunderkafka/schema_registry/clients/cloudera.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/schema_registry/confluent_client.py` & `wunderkafka-0.9.9/wunderkafka/schema_registry/clients/confluent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,128 @@
-import json
-from typing import Dict, Union, Optional
-
-from requests import HTTPError
-
-from wunderkafka.errors import SchemaRegistryLookupException
-from wunderkafka.logger import logger
-from wunderkafka.schema_registry.abc import AbstractHTTPClient, AbstractSchemaRegistry
-from wunderkafka.schema_registry.cache import SimpleCache
-from wunderkafka.schema_registry.models import RegisteredSchema
-from wunderkafka.structures import SRMeta, SchemaMeta, ParsedHeader
-
-RegistrySchema = Dict[str, Union[str, int, Dict[str, Union[str, int]]]]
-
-
-def _body(
-    schema_text: str,
-    references: Optional[dict],
-) -> RegistrySchema:
-    body = {
-        'schema': schema_text,
-        'schemaType': 'AVRO',
-    }
-    if references is not None:
-        body['references'] = references
-    return body
-
-
-class ConfluentSRClient(AbstractSchemaRegistry):
-
-    def __init__(self, http_client: AbstractHTTPClient, cache: Optional[SimpleCache] = None) -> None:
-        self._client = http_client
-        self._cache = SimpleCache() if cache is None else cache
-
-    def get_schema_text(self, meta: SchemaMeta) -> str:
-        hdr = meta.header
-        schema_text = self._cache.get(hdr)
-        if schema_text is None:
-            logger.debug("Couldn't find header ({0}) in cache, re-requesting...".format(hdr))
-            schema_text = self._choose_schema(hdr, meta.subject)
-            self._cache.set(hdr, schema_text)
-        return schema_text
-
-    def register_schema(self, topic: str, schema_text: str, *, is_key: bool = True) -> SRMeta:
-        uid = (topic, schema_text, is_key)
-        meta = self._cache.get(uid)
-        if meta is None:
-            subject = '{0}{1}'.format(topic, '_key' if is_key else '_value')
-
-            subjects = self._client.make_request('subjects/', query={'subjectPrefix': subject})
-            if subject not in subjects:
-                schema = self._register_schema(subject, schema_text)
-            else:
-                # ToDo (aa.perelygin): add check compatibility
-                #  (https://docs.confluent.io/platform/current/schema-registry/develop/api.html#sr-api-compatibility)
-                schema = self._register_new_version(subject, schema_text)
-
-            if isinstance(schema, int):
-                schema = self._get_schema(subject, 'latest')
-
-            meta = SRMeta(
-                schema_version=schema.version,
-                schema_id=schema.schema_id
-            )
-            self._cache.set(uid, meta)
-        return meta
-
-    def _register_schema(
-        self,
-        subject: str,
-        schema_text: str,
-        references: Optional[dict] = None,
-        *,
-        normalize_schemas: bool = False
-    ) -> int:
-        response = self._client.make_request(
-            'subjects/{0}/versions'.format(subject),
-            method='POST',
-            body=_body(schema_text, references),
-            query={'normalize': normalize_schemas}
-        )
-        return response['id']
-
-    def _choose_schema(self, hdr: ParsedHeader, subject: str):
-        try:
-            resp = self._client.make_request('schemas/ids/{}'.format(hdr.schema_id), query={'subject': subject})
-            return resp['schema']
-        except HTTPError:
-            raise SchemaRegistryLookupException("Couldn't find schema for {0}".format(hdr))
-
-    def _get_schema(self, subject: str, version_schema: Union[int, str]) -> RegisteredSchema:
-        response = self._client.make_request('subjects/{0}/versions/{1}'.format(subject, version_schema))
-        schema = json.loads(response['schema'])
-        ref = schema.get('references')
-        if ref is not None:
-            del schema['ref']
-        schema = RegisteredSchema(
-            schema_id=response['id'],
-            schema=schema,
-            subject=subject,
-            version=response['version'],
-            references=ref
-        )
-        return schema
-
-    def _register_new_version(self, subject: str, schema_text: str) -> int:
-        client_schema = json.loads(schema_text)
-        versions = self._client.make_request('subjects/{0}/versions'.format(subject))
-        latest_schema = None
-        for ver in versions:
-            reg_schema = self._get_schema(subject, ver)
-            if client_schema == reg_schema.schema:
-                return reg_schema
-            latest_schema = reg_schema
-        logger.debug('Schema {} not found'.format(subject))
-
-        ref = None
-        if latest_schema and not latest_schema.references:
-            ref = {
-                'name': latest_schema.subject,
-                'subject': latest_schema.subject,
-                'version': latest_schema.version
-            }
-        return self._register_schema(subject, schema_text, ref)
+import json
+from typing import Dict, Union, Optional
+
+from requests import HTTPError
+
+from wunderkafka.errors import SchemaRegistryLookupException
+from wunderkafka.logger import logger
+from wunderkafka.structures import SRMeta, SchemaMeta, ParsedHeader
+from wunderkafka.schema_registry.abc import AbstractHTTPClient, AbstractSchemaRegistry
+from wunderkafka.schema_registry.cache import SimpleCache
+from wunderkafka.schema_registry.models import RegisteredSchema
+
+RegistrySchema = Dict[str, Union[str, int, Dict[str, Union[str, int]]]]
+
+
+def _body(
+    schema_text: str,
+    references: Optional[dict],
+) -> RegistrySchema:
+    body = {
+        'schema': schema_text,
+        'schemaType': 'AVRO',
+    }
+    if references is not None:
+        body['references'] = references
+    return body
+
+
+class ConfluentSRClient(AbstractSchemaRegistry):
+
+    def __init__(self, http_client: AbstractHTTPClient, cache: Optional[SimpleCache] = None) -> None:
+        self._client = http_client
+        self._cache = SimpleCache() if cache is None else cache
+
+    def get_schema_text(self, meta: SchemaMeta) -> str:
+        hdr = meta.header
+        schema_text = self._cache.get(hdr)
+        if schema_text is None:
+            logger.debug("Couldn't find header ({0}) in cache, re-requesting...".format(hdr))
+            schema_text = self._choose_schema(hdr, meta.subject)
+            self._cache.set(hdr, schema_text)
+        return schema_text
+
+    def register_schema(self, topic: str, schema_text: str, *, is_key: bool = True) -> SRMeta:
+        uid = (topic, schema_text, is_key)
+        meta = self._cache.get(uid)
+        if meta is None:
+            subject = '{0}{1}'.format(topic, '_key' if is_key else '_value')
+
+            subjects = self._client.make_request('subjects/', query={'subjectPrefix': subject})
+            if subject not in subjects:
+                schema = self._register_schema(subject, schema_text)
+            else:
+                # ToDo (aa.perelygin): add check compatibility
+                #  (https://docs.confluent.io/platform/current/schema-registry/develop/api.html#sr-api-compatibility)
+                schema = self._register_new_version(subject, schema_text)
+
+            if isinstance(schema, int):
+                schema = self._get_schema(subject, 'latest')
+
+            meta = SRMeta(
+                schema_version=schema.version,
+                schema_id=schema.schema_id
+            )
+            self._cache.set(uid, meta)
+        return meta
+
+    def _register_schema(
+        self,
+        subject: str,
+        schema_text: str,
+        references: Optional[dict] = None,
+        *,
+        normalize_schemas: bool = False
+    ) -> int:
+        response = self._client.make_request(
+            'subjects/{0}/versions'.format(subject),
+            method='POST',
+            body=_body(schema_text, references),
+            query={'normalize': normalize_schemas}
+        )
+        return response['id']
+
+    def _choose_schema(self, hdr: ParsedHeader, subject: str):
+        try:
+            resp = self._client.make_request('schemas/ids/{}'.format(hdr.schema_id), query={'subject': subject})
+            return resp['schema']
+        except HTTPError:
+            raise SchemaRegistryLookupException("Couldn't find schema for {0}".format(hdr))
+
+    def _get_schema(self, subject: str, version_schema: Union[int, str]) -> RegisteredSchema:
+        response = self._client.make_request('subjects/{0}/versions/{1}'.format(subject, version_schema))
+        schema = json.loads(response['schema'])
+
+        if isinstance(schema, str):
+            ref = None
+        else:
+            ref = schema.get('references')
+            if ref is not None:
+                del schema['ref']
+        schema = RegisteredSchema(
+            schema_id=response['id'],
+            schema=schema,
+            subject=subject,
+            version=response['version'],
+            references=ref
+        )
+        return schema
+
+    def _register_new_version(self, subject: str, schema_text: str) -> int:
+        client_schema = json.loads(schema_text)
+        versions = self._client.make_request('subjects/{0}/versions'.format(subject))
+        latest_schema = None
+        for ver in versions:
+            reg_schema = self._get_schema(subject, ver)
+            if client_schema == reg_schema.schema:
+                return reg_schema
+            latest_schema = reg_schema
+        logger.debug('Schema {} not found'.format(subject))
+
+        ref = None
+        if latest_schema and not latest_schema.references:
+            ref = {
+                'name': latest_schema.subject,
+                'subject': latest_schema.subject,
+                'version': latest_schema.version
+            }
+        return self._register_schema(subject, schema_text, ref)
```

### Comparing `wunderkafka-0.9.8/wunderkafka/schema_registry/transport.py` & `wunderkafka-0.9.9/wunderkafka/schema_registry/transport.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/abc.py` & `wunderkafka-0.9.9/wunderkafka/serdes/abc.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/avro/deserializers.py` & `wunderkafka-0.9.9/wunderkafka/serdes/avro/deserializers.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/avro/headers.py` & `wunderkafka-0.9.9/wunderkafka/serdes/avro/headers.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/avro/serializers.py` & `wunderkafka-0.9.9/wunderkafka/serdes/avro/serializers.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/avromodel.py` & `wunderkafka-0.9.9/wunderkafka/serdes/avromodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Type, Dict, Any
+from typing import Any, Dict, Type
 from dataclasses import is_dataclass
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 
 from wunderkafka.compat.types import AvroModel
```

### Comparing `wunderkafka-0.9.8/wunderkafka/serdes/store.py` & `wunderkafka-0.9.9/wunderkafka/serdes/store.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/structures.py` & `wunderkafka-0.9.9/wunderkafka/structures.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/tests/consumer.py` & `wunderkafka-0.9.9/wunderkafka/tests/consumer.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/tests/producer.py` & `wunderkafka-0.9.9/wunderkafka/tests/producer.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/tests/schema_registry.py` & `wunderkafka-0.9.9/wunderkafka/tests/schema_registry.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/time.py` & `wunderkafka-0.9.9/wunderkafka/time.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka/types.py` & `wunderkafka-0.9.9/wunderkafka/types.py`

 * *Files identical despite different names*

### Comparing `wunderkafka-0.9.8/wunderkafka.egg-info/PKG-INFO` & `wunderkafka-0.9.9/wunderkafka.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wunderkafka
-Version: 0.9.8
+Version: 0.9.9
 Summary: librdkafka-powered client for Kafka for python with (hopefully) more handful API
 Home-page: https://github.com/severstal-digital/wunderkafka
 Author: Kirill Tribunsky
 Author-email: tribunsky.kir@yandex.ru
 License: Apache-2.0 License
 Project-URL: Bug Tracker, https://github.com/severstal-digital/wunderkafka/issues
 Keywords: kafka,cloudera
```

### Comparing `wunderkafka-0.9.8/wunderkafka.egg-info/SOURCES.txt` & `wunderkafka-0.9.9/wunderkafka.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,18 +57,19 @@
 wunderkafka/producers/__init__.py
 wunderkafka/producers/abc.py
 wunderkafka/producers/bytes.py
 wunderkafka/producers/constructor.py
 wunderkafka/schema_registry/__init__.py
 wunderkafka/schema_registry/abc.py
 wunderkafka/schema_registry/cache.py
-wunderkafka/schema_registry/cloudera_client.py
-wunderkafka/schema_registry/confluent_client.py
 wunderkafka/schema_registry/models.py
 wunderkafka/schema_registry/transport.py
+wunderkafka/schema_registry/clients/__init__.py
+wunderkafka/schema_registry/clients/cloudera.py
+wunderkafka/schema_registry/clients/confluent.py
 wunderkafka/serdes/__init__.py
 wunderkafka/serdes/abc.py
 wunderkafka/serdes/avromodel.py
 wunderkafka/serdes/store.py
 wunderkafka/serdes/avro/__init__.py
 wunderkafka/serdes/avro/deserializers.py
 wunderkafka/serdes/avro/headers.py
```

