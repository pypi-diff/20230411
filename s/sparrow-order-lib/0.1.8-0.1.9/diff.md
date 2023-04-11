# Comparing `tmp/sparrow-order-lib-0.1.8.tar.gz` & `tmp/sparrow-order-lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hbshun/hg/sparrow-order-lib/dist/tmpfk6sjkli/sparrow-order-lib-0.1.8.tar", last modified: Tue Aug 30 09:18:32 2022, max compression
+gzip compressed data, was "/Users/hbshun/hg/sparrow-order-lib/dist/tmp6d8iuth3/sparrow-order-lib-0.1.9.tar", last modified: Thu Sep  1 08:11:13 2022, max compression
```

## Comparing `sparrow-order-lib-0.1.8.tar` & `sparrow-order-lib-0.1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:32.000000 sparrow-order-lib-0.1.8/
--rw-r--r--   0 hbshun     (501) staff       (20)     1073 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/LICENSE
--rw-r--r--   0 hbshun     (501) staff       (20)     5923 2022-08-30 09:18:32.000000 sparrow-order-lib-0.1.8/PKG-INFO
--rw-r--r--   0 hbshun     (501) staff       (20)     5386 2022-08-30 09:18:14.000000 sparrow-order-lib-0.1.8/README.md
--rw-r--r--   0 hbshun     (501) staff       (20)      103 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/pyproject.toml
--rw-r--r--   0 hbshun     (501) staff       (20)      662 2022-08-30 09:18:32.000000 sparrow-order-lib-0.1.8/setup.cfg
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/
--rw-r--r--   0 hbshun     (501) staff       (20)       76 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/__init__.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2014 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/base_models.py
--rw-r--r--   0 hbshun     (501) staff       (20)      517 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/common_utils.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3745 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1592 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/datastructures.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1353 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/decorators.py
--rw-r--r--   0 hbshun     (501) staff       (20)    12853 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/dt_utils.py
--rw-r--r--   0 hbshun     (501) staff       (20)       90 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/formats.py
--rw-r--r--   0 hbshun     (501) staff       (20)      714 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/model_function.py
--rw-r--r--   0 hbshun     (501) staff       (20)      251 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/numbers.py
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/text.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/db_tool/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/db_tool/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)      842 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/db_tool/query.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/
--rw-r--r--   0 hbshun     (501) staff       (20)     1359 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)      422 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/constants.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/
--rw-r--r--   0 hbshun     (501) staff       (20)       56 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7841 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/base.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1092 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/client.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1228 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3661 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_builder.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3091 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_door.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5145 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3620 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_query_util.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1223 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/exceptions.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2207 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/field.py
--rw-r--r--   0 hbshun     (501) staff       (20)      381 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/in_query_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)      163 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/index.py
--rw-r--r--   0 hbshun     (501) staff       (20)      241 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/mock.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3137 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/operators.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/
--rw-r--r--   0 hbshun     (501) staff       (20)     1619 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1782 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_base.py
--rw-r--r--   0 hbshun     (501) staff       (20)       64 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_client.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2455 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3294 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3947 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2500 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2310 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_field.py
--rw-r--r--   0 hbshun     (501) staff       (20)      515 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)      373 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_mock.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2203 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_operators.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7542 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/mapping_constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3086 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/query_mapping_constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3490 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/test_order_doc_type.py
--rw-r--r--   0 hbshun     (501) staff       (20)       42 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/example.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1406 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_api_path.py
--rw-r--r--   0 hbshun     (501) staff       (20)      815 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_core.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5271 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_core_go.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2778 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
--rw-r--r--   0 hbshun     (501) staff       (20)     4706 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_product.py
--rw-r--r--   0 hbshun     (501) staff       (20)      383 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/svc_config.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/
--rw-r--r--   0 hbshun     (501) staff       (20)       33 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3427 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    65289 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5826 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    13289 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    48596 2022-08-30 09:17:49.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    29654 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/
--rw-r--r--   0 hbshun     (501) staff       (20)      155 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    13431 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    17612 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/
--rw-r--r--   0 hbshun     (501) staff       (20)       68 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    23984 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)   108751 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/
--rw-r--r--   0 hbshun     (501) staff       (20)       30 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     4285 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)      455 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/exceptions.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7599 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_promotions/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_promotions/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1979 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_promotions/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:32.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/
--rw-r--r--   0 hbshun     (501) staff       (20)       32 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2788 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     9065 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/
--rw-r--r--   0 hbshun     (501) staff       (20)     5923 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/PKG-INFO
--rw-r--r--   0 hbshun     (501) staff       (20)     3855 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/SOURCES.txt
--rw-r--r--   0 hbshun     (501) staff       (20)        1 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/dependency_links.txt
--rw-r--r--   0 hbshun     (501) staff       (20)       18 2022-08-30 09:18:31.000000 sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/top_level.txt
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1073 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/LICENSE
+-rw-r--r--   0 hbshun     (501) staff       (20)     5961 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/PKG-INFO
+-rw-r--r--   0 hbshun     (501) staff       (20)     5424 2022-09-01 08:08:40.000000 sparrow-order-lib-0.1.9/README.md
+-rw-r--r--   0 hbshun     (501) staff       (20)      103 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/pyproject.toml
+-rw-r--r--   0 hbshun     (501) staff       (20)      662 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/setup.cfg
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/
+-rw-r--r--   0 hbshun     (501) staff       (20)       76 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/__init__.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2014 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/base_models.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      517 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/common_utils.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3745 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1592 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/datastructures.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1353 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/decorators.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    12853 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/dt_utils.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       90 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/formats.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      714 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/model_function.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      251 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/numbers.py
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/text.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      842 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/query.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1359 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      422 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/constants.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/
+-rw-r--r--   0 hbshun     (501) staff       (20)       56 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7841 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/base.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1092 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/client.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1228 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3661 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_builder.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3091 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_door.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5145 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3620 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_query_util.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1223 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/exceptions.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2207 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/field.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      381 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/in_query_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      163 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/index.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      241 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/mock.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3137 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/operators.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1619 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1782 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_base.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       64 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_client.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2455 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3294 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3947 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2500 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2310 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_field.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      515 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      373 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_mock.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2203 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_operators.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7542 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/mapping_constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3086 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/query_mapping_constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3490 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/test_order_doc_type.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       42 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/example.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1406 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_api_path.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      815 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5271 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core_go.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2778 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     4706 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_product.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      383 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/svc_config.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/
+-rw-r--r--   0 hbshun     (501) staff       (20)       33 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3427 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    65289 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5826 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    13289 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    48594 2022-09-01 08:01:19.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    29654 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/
+-rw-r--r--   0 hbshun     (501) staff       (20)      155 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    13431 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    17612 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/
+-rw-r--r--   0 hbshun     (501) staff       (20)       68 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    23984 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)   108751 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/
+-rw-r--r--   0 hbshun     (501) staff       (20)       30 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     4285 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      455 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/exceptions.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7599 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1979 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/
+-rw-r--r--   0 hbshun     (501) staff       (20)       32 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2788 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     9065 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/
+-rw-r--r--   0 hbshun     (501) staff       (20)     5961 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/PKG-INFO
+-rw-r--r--   0 hbshun     (501) staff       (20)     3855 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 hbshun     (501) staff       (20)        1 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 hbshun     (501) staff       (20)       18 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/top_level.txt
```

### Comparing `sparrow-order-lib-0.1.8/LICENSE` & `sparrow-order-lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/PKG-INFO` & `sparrow-order-lib-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
 # Release History
 
+## version==0.1.9
+允许取消发货
+
 ## version==0.1.8
 虚拟商品发起售后 不拆单
 
 ## version==0.1.7
 发货单address group 在库-已合
 
 ## version==0.1.6
```

### Comparing `sparrow-order-lib-0.1.8/README.md` & `sparrow-order-lib-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Project Description
 
 # Release History
 
+## version==0.1.9
+允许取消发货
+
 ## version==0.1.8
 虚拟商品发起售后 不拆单
 
 ## version==0.1.7
 发货单address group 在库-已合
 
 ## version==0.1.6
```

### Comparing `sparrow-order-lib-0.1.8/setup.cfg` & `sparrow-order-lib-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-order-lib
-version = 0.1.8
+version = 0.1.9
 author = Jessica Liao
 author_email = 18610193367@sina.cn
 description = This is a lib for sparrow order projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/sparrow614/sparrow-order-lib
 project_urls =
```

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/base_models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/base_models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/common_utils.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/datastructures.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/decorators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/dt_utils.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/dt_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/core/model_function.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/model_function.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/db_tool/query.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/query.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/__init__.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/base.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/client.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/client.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_builder.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_door.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/es_query_util.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/exceptions.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/field.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/operators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/__init__.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_base.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_door.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_field.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/es_util/tests/test_operators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/mapping_constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/query_mapping_constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/query_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/es/test_order_doc_type.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/test_order_doc_type.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_api_path.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_api_path.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_core.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_core_go.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core_go.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_lanyue.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_lanyue.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/remote_call/sparrow_product.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_product.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_aftersale/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_disstorage/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
                     DistributeStatus.SERVICE_DESK,
                     DistributeStatus.SERVICE_STORE,
                     DistributeStatus.SERVICE_STOP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.PACKAGED,
         },
         CANCEL_PACKAGE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                # DistributeStatus.PACKAGED
+                DistributeStatus.PACKAGED
                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,
         },
         SERVICESTOP_CANCEL_PACKAGE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                 DistributeStatus.PACKAGED,
                 DistributeStatus.CUSSERVICE_PICKED_UP,
```

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_distribute/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_exchange/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_orders/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_parcel/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_promotions/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib/sparrow_shipping/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/PKG-INFO` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
 # Release History
 
+## version==0.1.9
+允许取消发货
+
 ## version==0.1.8
 虚拟商品发起售后 不拆单
 
 ## version==0.1.7
 发货单address group 在库-已合
 
 ## version==0.1.6
```

### Comparing `sparrow-order-lib-0.1.8/src/sparrow_order_lib.egg-info/SOURCES.txt` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

