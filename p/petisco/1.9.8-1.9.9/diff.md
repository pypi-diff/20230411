# Comparing `tmp/petisco-1.9.8.tar.gz` & `tmp/petisco-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-1.9.8.tar", last modified: Tue Sep 13 11:19:40 2022, max compression
+gzip compressed data, was "petisco-1.9.9.tar", last modified: Thu Sep 29 11:37:51 2022, max compression
```

## Comparing `petisco-1.9.8.tar` & `petisco-1.9.9.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-13 11:19:29.000000 petisco-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-13 11:19:29.000000 petisco-1.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-13 11:19:40.481794 petisco-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-09-13 11:19:29.000000 petisco-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-13 11:19:32.000000 petisco-1.9.8/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/controller/controller_executor_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/controller/http_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/dependency_injection/dependency.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/dependency_injection/injector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/handlers/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.461793 petisco-1.9.8/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.465793 petisco-1.9.8/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.465793 petisco-1.9.8/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.465793 petisco-1.9.8/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.465793 petisco-1.9.8/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/persistence/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/persistence/interface_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/persistence/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/domain/persistence/persistence_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_operational_database_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/elastic_session_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/elastic/is_elastic_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.469794 petisco-1.9.8/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/application/fastapi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6962 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.473794 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (121)    16386 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.477794 petisco-1.9.8/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/base_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlalchemy/sqlalchemy_operational_database_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/extra/threading/pool_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/petisco/legacy/logger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/logger/interface_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/legacy/logger/not_implemented_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6043 2022-09-13 11:19:29.000000 petisco-1.9.8/petisco/public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.457793 petisco-1.9.8/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-13 11:19:40.000000 petisco-1.9.8/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-13 11:19:29.000000 petisco-1.9.8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-13 11:19:40.481794 petisco-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-09-13 11:19:29.000000 petisco-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-09-13 11:19:29.000000 petisco-1.9.8/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:40.481794 petisco-1.9.8/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 11:19:29.000000 petisco-1.9.8/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-29 11:37:42.000000 petisco-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-29 11:37:42.000000 petisco-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-29 11:37:51.127008 petisco-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-09-29 11:37:42.000000 petisco-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-29 11:37:43.000000 petisco-1.9.9/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/controller_executor_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/http_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/injector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/interface_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/persistence_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_operational_database_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_session_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/is_elastic_available.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/application/fastapi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6962 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16386 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/base_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sqlalchemy_operational_database_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/threading/pool_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/legacy/logger/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/interface_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/not_implemented_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6043 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-29 11:37:42.000000 petisco-1.9.9/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-29 11:37:51.127008 petisco-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-09-29 11:37:42.000000 petisco-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/modules/__init__.py
```

### Comparing `petisco-1.9.8/LICENSE` & `petisco-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/PKG-INFO` & `petisco-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 1.9.8
+Version: 1.9.9
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petisco-1.9.8/README.md` & `petisco-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/application.py` & `petisco-1.9.9/petisco/base/application/application.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/controller/controller.py` & `petisco-1.9.9/petisco/base/application/controller/controller.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/dependency_injection/container.py` & `petisco-1.9.9/petisco/base/application/dependency_injection/container.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/dependency_injection/dependency.py` & `petisco-1.9.9/petisco/base/application/dependency_injection/dependency.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/handlers/message_handler.py` & `petisco-1.9.9/petisco/base/application/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/middleware/notifier_middleware.py` & `petisco-1.9.9/petisco/base/application/middleware/notifier_middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/notifier/notifier.py` & `petisco-1.9.9/petisco/base/application/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-1.9.9/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/patterns/crud_repository.py` & `petisco-1.9.9/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-1.9.9/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/application/use_case/use_case.py` & `petisco-1.9.9/petisco/base/application/use_case/use_case.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/errors/default_http_error_map.py` & `petisco-1.9.9/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-1.9.9/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/errors/defaults/not_found.py` & `petisco-1.9.9/petisco/base/domain/errors/defaults/not_found.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/errors/domain_error.py` & `petisco-1.9.9/petisco/base/domain/errors/domain_error.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/errors/unknown_error.py` & `petisco-1.9.9/petisco/base/domain/errors/unknown_error.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-1.9.9/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/command.py` & `petisco-1.9.9/petisco/base/domain/message/command.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/command_bus.py` & `petisco-1.9.9/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/command_subscriber.py` & `petisco-1.9.9/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/consumer_derived_action.py` & `petisco-1.9.9/petisco/base/domain/message/consumer_derived_action.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/domain_event.py` & `petisco-1.9.9/petisco/base/domain/message/domain_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, Optional, Type, Union
 
 from petisco.base.domain.message.message import Message
 
 
 class DomainEvent(Message):
     def __init__(self, **kwargs):
-        self._set_data()
+        super(DomainEvent, self).__init__()
         self._set_attributes(**kwargs)
         self.type = "domain_event"
 
     @staticmethod
     def from_dict(message_data: Dict, target_type: Optional[Type] = None):
         target_type = DomainEvent if target_type is None else target_type
         data = message_data.get("data")
```

### Comparing `petisco-1.9.8/petisco/base/domain/message/domain_event_bus.py` & `petisco-1.9.9/petisco/base/domain/message/domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-1.9.9/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/message.py` & `petisco-1.9.9/petisco/base/domain/message/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,23 +31,22 @@
         namespace["attributes"] = {}
         namespace["meta"] = {}
 
         return super().__new__(mcs, name, bases, namespace)
 
 
 class Message(metaclass=MetaMessage):
-    message_id: Uuid
-    name: str
-    version: int
-    occurred_on: datetime
-    attributes: Dict
-    meta: Dict
-    type: str = "message"
-
     def __init__(self, **kwargs):
+        self.message_id: Uuid
+        self.name: str
+        self.version: int
+        self.occurred_on: datetime
+        self.attributes: Dict = {}
+        self.meta: Dict = {}
+        self.type: str = "message"
         self._set_data(**kwargs)
 
     def _set_data(self, **kwargs):
         if kwargs:
             self.message_id = (
                 Uuid.from_value(kwargs.get("id")) if kwargs.get("id") else Uuid.v4()
             )
```

### Comparing `petisco-1.9.8/petisco/base/domain/message/message_bus.py` & `petisco-1.9.9/petisco/base/domain/message/message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/message_configurer.py` & `petisco-1.9.9/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/message_consumer.py` & `petisco-1.9.9/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/message_subscriber.py` & `petisco-1.9.9/petisco/base/domain/message/message_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-1.9.9/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/not_implemented_message_bus.py` & `petisco-1.9.9/petisco/base/domain/message/not_implemented_message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-1.9.9/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/model/aggregate_root.py` & `petisco-1.9.9/petisco/base/domain/model/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/model/value_object.py` & `petisco-1.9.9/petisco/base/domain/model/value_object.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/persistence/fake_database.py` & `petisco-1.9.9/petisco/base/domain/persistence/fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/persistence/interface_database.py` & `petisco-1.9.9/petisco/base/domain/persistence/interface_database.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/persistence/persistence.py` & `petisco-1.9.9/petisco/base/domain/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/domain/persistence/persistence_models.py` & `petisco-1.9.9/petisco/base/domain/persistence/persistence_models.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/misc/builder.py` & `petisco-1.9.9/petisco/base/misc/builder.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/misc/result_mapper.py` & `petisco-1.9.9/petisco/base/misc/result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/misc/singleton.py` & `petisco-1.9.9/petisco/base/misc/singleton.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/base/misc/wrapper.py` & `petisco-1.9.9/petisco/base/misc/wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/cli/petisco.py` & `petisco-1.9.9/petisco/cli/petisco.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/cli/petisco_rabbitmq.py` & `petisco-1.9.9/petisco/cli/petisco_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/__init__.py` & `petisco-1.9.9/petisco/extra/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/elastic_apm_monitoring_app_service.py` & `petisco-1.9.9/petisco/extra/elastic/elastic_apm_monitoring_app_service.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/elastic_connection.py` & `petisco-1.9.9/petisco/extra/elastic/elastic_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/elastic_database.py` & `petisco-1.9.9/petisco/extra/elastic/elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-1.9.9/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/elastic/elastic_session_scope_provider.py` & `petisco-1.9.9/petisco/extra/elastic/elastic_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/fastapi/__init__.py` & `petisco-1.9.9/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/__init__.py` & `petisco-1.9.9/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/dependencies.py` & `petisco-1.9.9/petisco/extra/rabbitmq/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-1.9.9/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-1.9.9/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/__init__.py` & `petisco-1.9.9/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-1.9.9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-1.9.9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/slack/dependencies.py` & `petisco-1.9.9/petisco/extra/slack/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/__init__.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/base_sql_repository.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/base_sql_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py` & `petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-1.9.9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/extra/threading/pool_executor.py` & `petisco-1.9.9/petisco/extra/threading/pool_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/legacy/__init__.py` & `petisco-1.9.9/petisco/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/legacy/logger/log_message.py` & `petisco-1.9.9/petisco/legacy/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/legacy/logger/logging_based_logger.py` & `petisco-1.9.9/petisco/legacy/logger/logging_based_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco/public_api.py` & `petisco-1.9.9/petisco/public_api.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/petisco.egg-info/PKG-INFO` & `petisco-1.9.9/petisco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 1.9.8
+Version: 1.9.9
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petisco-1.9.8/petisco.egg-info/SOURCES.txt` & `petisco-1.9.9/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/setup.py` & `petisco-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.8/tests/fixtures.py` & `petisco-1.9.9/tests/fixtures.py`

 * *Files identical despite different names*

