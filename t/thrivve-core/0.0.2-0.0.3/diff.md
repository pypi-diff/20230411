# Comparing `tmp/thrivve_core-0.0.2.tar.gz` & `tmp/thrivve_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-qit8mazn/thrivve_core-0.0.2.tar", last modified: Tue Apr 11 11:56:53 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-wwvex738/thrivve_core-0.0.3.tar", last modified: Tue Apr 11 12:46:33 2023, max compression
```

## Comparing `thrivve_core-0.0.2.tar` & `thrivve_core-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12208 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-11 12:46:21.000000 thrivve_core-0.0.3/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 12:46:33.000000 thrivve_core-0.0.3/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.0.2/PKG-INFO` & `thrivve_core-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.0.2
+Version: 0.0.3
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.2/setup.py` & `thrivve_core-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.0.2",
+    version="0.0.3",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.0.2/thrivve_core/__init__.py` & `thrivve_core-0.0.3/thrivve_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .base import WeDeliverCore
+from .base import ThrivveCore
 from .app_decorators.app_entry import route
 from .helpers.log_config import init_logger
 from .helpers.config import Config
 from .helpers.kafka_producer import Producer
 from .helpers.topics import Topics
 from .helpers.micro_fetcher import MicroFetcher
 from .helpers.atomic_transactions import Transactions
 from .helpers.atomic_transactions_v2 import Transactions as TransactionV2
 from .helpers.auth import Auth
 from .helpers.enums import Service
 from .helpers.database.base_model import init_base_model
 from .helpers.database.log_model import init_log_model
 
 __all__ = [
-    "WeDeliverCore",
+    "ThrivveCore",
     "route",
     "Config",
     "Producer",
     "init_logger",
     "Topics",
     "MicroFetcher",
     "Transactions",
```

### Comparing `thrivve_core-0.0.2/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.0.3/thrivve_core/app_decorators/app_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from functools import wraps
 
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 from thrivve_core.app_decorators import (
     handle_response,
     handle_auth,
     handle_exceptions,
     serializer,
 )
 from thrivve_core.helpers.get_prefix import get_prefix
 
 
 def route(path, methods=["GET"], schema=None, many=False, allowed_roles=None, require_auth=True,
           append_auth_args=None,
           pre_login=False,
           allowed_permissions=None):
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
 
     def factory(func):
         @app.route(path, methods=methods)
         @app.route(get_prefix(path), methods=methods)
         @handle_response
         @handle_exceptions
         @handle_auth(require_auth=require_auth, append_auth_args=append_auth_args, allowed_roles=allowed_roles,
```

### Comparing `thrivve_core-0.0.2/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.0.3/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.0.3/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import traceback
 from functools import wraps
 from sqlalchemy.exc import SQLAlchemyError
 
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 from thrivve_core.helpers.auth import Auth
 from thrivve_core.helpers.format_exception import format_exception
 from thrivve_core.helpers.notification_center import (
     send_critical_error,
 )
 from thrivve_core.helpers.validate_parameters import (
     validate_parameters,
 )
 
 
 def handle_exceptions(func):
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
 
     @wraps(func)
     def inner_function(*args, **kws):
         try:
             result = func(*args, **kws)
             return result
```

### Comparing `thrivve_core-0.0.2/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.0.3/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.0.3/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/base.py` & `thrivve_core-0.0.3/thrivve_core/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-class WeDeliverCore:
+class ThrivveCore:
     __app = None
 
     @staticmethod
     def get_app():
         """ Static access method. """
-        if WeDeliverCore.__app == None:
-            WeDeliverCore()
-        return WeDeliverCore.__app
+        if ThrivveCore.__app == None:
+            ThrivveCore()
+        return ThrivveCore.__app
 
     def __init__(self, app=None):
         """ Virtually private constructor. """
-        if WeDeliverCore.__app != None:
+        if ThrivveCore.__app != None:
             raise Exception("This class is a singleton!")
         else:
-            WeDeliverCore.__app = app
+            ThrivveCore.__app = app
             setup_default_routes(app)
 
 
 def setup_default_routes(app):
     from thrivve_core.app_decorators.app_entry import route
     from thrivve_core.helpers.fetch_relational_data import fetch_relational_data
     @route(
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.0.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.0.3/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.0.3/thrivve_core/helpers/atomic_transactions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 
 
 class Transactions(object):
     savepoint = None
     db = None
 
     def __init__(self):
-        app = WeDeliverCore.get_app()
+        app = ThrivveCore.get_app()
 
         self.db = app.extensions['sqlalchemy'].db
         self.savepoint = self.db.session.begin_nested()
 
     @staticmethod
     def atomic():
         return Transactions()
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.0.3/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 
 
 class Transactions(object):
     """
 
     """
     session = None
 
     def __init__(self):
-        app = WeDeliverCore.get_app()
+        app = ThrivveCore.get_app()
 
         self.session = app.extensions['sqlalchemy'].db.session
 
     @staticmethod
     def atomic():
         """
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/auth.py` & `thrivve_core-0.0.3/thrivve_core/helpers/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 from flask import request
 
 from app.helpers.auth.enums import Language
 from .exceptions import AppValidationError, AppMissingAuthError
 from flask import session
 
-from .. import WeDeliverCore
+from .. import ThrivveCore
 
 
 class Auth:
     def __init__(self):
         pass
 
     @staticmethod
@@ -19,15 +19,15 @@
         user["is_admin"] = user.get("role") == "Administrator"
 
         if request.headers.get("Accept-Language") in ("ar", "en"):
             user["language"] = request.headers.get("Accept-Language")
         else:
             user["language"] = user.get("language", "ar")
 
-        app = WeDeliverCore.get_app()
+        app = ThrivveCore.get_app()
         app.logger.debug(user)
         session["user"] = user
 
     @staticmethod
     def get_user():
         default_user_str = 'Guest'
         try:
@@ -35,30 +35,30 @@
         except Exception:
             user = dict(user_id=default_user_str, email=default_user_str)
 
         return user
 
     @staticmethod
     def get_user_str():
-        # app = WeDeliverCore.get_app()
+        # app = ThrivveCore.get_app()
         # with app.test_request_context():
         user = Auth.get_user()
 
         if user.get('role') == 'captain':
             return "{} : {} : {}".format(
                 user.get("captain_id"),
                 user.get("full_name"),
                 user.get("mobile"),
             )
         else:
             return user.get('email')
 
 
 def verify_user_token(token, allowed_permissions=None, pre_login=False):
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
 
     url = f"{app.config.get('AUTH_SERVICE')}/api/v1/authenticate?token={token}"
     try:
         language = (
             request.headers["Accept-Language"].lower()
             if (
                     "Accept-Language" in request.headers
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/config.py` & `thrivve_core-0.0.3/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.0.3/thrivve_core/helpers/database/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 from thrivve_core.helpers.auth import Auth
 
 
 def init_base_model():
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     db = app.extensions['sqlalchemy'].db
 
     class BaseModel(db.Model):
         __abstract__ = True
         id = db.Column(db.Integer, primary_key=True)
         creation = db.Column(db.DateTime, default=db.func.now())
         created_by = db.Column(db.String(64), default=Auth.get_user_str)
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.0.3/thrivve_core/helpers/database/log_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from sqlalchemy import event, inspect
 from sqlalchemy.orm import object_mapper, ColumnProperty
 
-from thrivve_core import WeDeliverCore, Auth
+from thrivve_core import ThrivveCore, Auth
 from thrivve_core.helpers.kafka_producers.log_model_changes import log_model_changes
 
 
 def init_log_model():
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     db = app.extensions['sqlalchemy'].db
 
     class LogModel(db.Model):
         __abstract__ = True
         __log_column_changes__ = []
         __log_parent_instance__ = None
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/enums.py` & `thrivve_core-0.0.3/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.0.3/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.0.3/thrivve_core/helpers/fetch_relational_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         functions=None,
         query_type=None,
         search_list=None,
         append_extra=None,
         use_country_code=None,
 
 ):
-    # app = WeDeliverCore.get_app()
+    # app = ThrivveCore.get_app()
     # db = app.extensions['sqlalchemy'].db
 
     if query_type == QueryTypes.SEARCH.value:
         result, validation = search_function(table_name=table_name, search_list=search_list, append_extra=append_extra,
                                              use_country_code=use_country_code)
         return dict(
             result=result,
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/filters.py` & `thrivve_core-0.0.3/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.0.3/thrivve_core/helpers/format_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 from datetime import datetime
 from sys import platform
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 from flask import request
 
 
 def format_exception(exception, user=None, status_code=None, soft_message=None):
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     user = user or dict()
     try:
         caller_frame = request.path
     except Exception:
         try:
             caller_frame = inspect.currentframe()
             caller_frame = inspect.getouterframes(caller_frame, 2)[1][3]
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.0.3/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.0.3/thrivve_core/helpers/kafka_producer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import random
 import string
 
 
 from confluent_kafka import Producer as kafka_Producer
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 
 
 class Producer:
     app = None
 
     def __init__(self):
-        self.app = WeDeliverCore.get_app()
+        self.app = ThrivveCore.get_app()
         self._producer = (
             None
             if not self.app or self.app.config.get("FLASK_ENV") == "local"
             else kafka_Producer(
                 {
                     "sasl.mechanisms": "PLAIN",
                     "request.timeout.ms": 20000,
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.0.3/thrivve_core/helpers/micro_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import flask_sqlalchemy
 
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 from thrivve_core.helpers.exceptions import AppMicroFetcherError, AppFetchServiceDataError
 import requests
 import json
 
 from thrivve_core.helpers.get_obj_value import get_obj_value
 
 from thrivve_core.helpers.service_config import ServiceConfig
@@ -26,15 +26,15 @@
     lookup_key = None
     module_name = None
     function_params = None
     query_type = None
     search_list = None
 
     def __init__(self, service):
-        self.app = WeDeliverCore.get_app()
+        self.app = ThrivveCore.get_app()
 
         if isinstance(service, ServiceConfig):
             service = service.initialize()
             service_name = service.name
             service_url = service.url
         else:
             service_name = service
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/notification_center.py` & `thrivve_core-0.0.3/thrivve_core/helpers/notification_center.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 from datetime import datetime
 
 from .kafka_producer import Producer
-from .. import WeDeliverCore
+from .. import ThrivveCore
 from thrivve_core.helpers.topics import Topics
 
 def send_critical_error(message, channel=None):
     channel = channel or "critical-errors"
     send_notification_message(
         channel=channel,
         title="critical",
@@ -15,15 +15,15 @@
         emoji=":pleading_face:"
     )
 
 
 def send_notification_message(
         message, channel="logs", title="Log", color="#32a4a7", emoji=":dizzy_face:"
 ):
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     channel = "eng-{0}-{1}".format(
         app.config.get("FLASK_ENV")
         if app.config.get("FLASK_ENV") == "production"
         else "development",
         channel,
     )
     datetime_now = datetime.now().strftime("%Y-%m-%d %H:%M")
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/search_function.py` & `thrivve_core-0.0.3/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/service_config.py` & `thrivve_core-0.0.3/thrivve_core/helpers/service_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 
 service_endpoint = dict(
     local='http://localhost:5000',
     development='http://{}-service.services',
     staging='http://{}-service.services',
     sandbox='http://{}-service-sandbox.sandbox',
     production='http://{}-service.services',
@@ -14,15 +14,15 @@
     url = None
 
     def __init__(self, name):
 
         self.name = name
 
     def initialize(self):
-        app = WeDeliverCore.get_app()
+        app = ThrivveCore.get_app()
 
         url = service_endpoint.get(app.config.get('FLASK_ENV'))
 
         if url:
             self.url = url.format(self.name.replace('_SERVICE', '').lower())
 
         return self
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/sql.py` & `thrivve_core-0.0.3/thrivve_core/helpers/sql.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from sqlalchemy import text
-from thrivve_core import WeDeliverCore
+from thrivve_core import ThrivveCore
 
 
 def sql(query):
     """
 
     :param query:
     :return:
     """
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     db = app.extensions['sqlalchemy'].db
 
     result = db.engine.execute(text(query))
     result_list = list()
     # app.logger.debug(result)
     for rowproxy in result:
         temp = dict()
@@ -26,11 +26,11 @@
 
 
 def no_result_sql(query):
     """
 
     :param query:
     """
-    app = WeDeliverCore.get_app()
+    app = ThrivveCore.get_app()
     db = app.extensions['sqlalchemy'].db
     app.logger.debug(query)
     db.engine.execute(text(query))
```

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.0.3/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.0.3/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.2/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.0.3/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.2/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.0.3/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

