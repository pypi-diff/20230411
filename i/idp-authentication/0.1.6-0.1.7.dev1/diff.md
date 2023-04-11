# Comparing `tmp/idp_authentication-0.1.6.tar.gz` & `tmp/idp_authentication-0.1.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idp_authentication-0.1.6.tar", last modified: Fri Mar 31 17:52:45 2023, max compression
+gzip compressed data, was "idp_authentication-0.1.7.dev1.tar", last modified: Tue Apr 11 09:42:19 2023, max compression
```

## Comparing `idp_authentication-0.1.6.tar` & `idp_authentication-0.1.7.dev1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       34 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5312 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4486 2023-03-10 11:57:51.000000 idp_authentication-0.1.6/README.md
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      247 2023-03-10 12:04:33.000000 idp_authentication-0.1.6/idp_authentication/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      858 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/config.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     7009 2023-03-31 17:47:05.000000 idp_authentication-0.1.6/idp_authentication/conftest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1695 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/custom_types.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1286 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/enums.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      553 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/exceptions.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/adapters/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3339 2023-03-10 11:44:39.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/orm.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/adapters/repositories/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/repositories/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1616 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/repositories/user_repository.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      317 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/repositories/user_role_repository.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      846 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/adapters/unit_of_work.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/base_classes/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      328 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/base_entity.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1042 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/base_repository.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      721 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/base_unit_of_work.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3267 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/base_use_case.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      511 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/base_classes/singleton.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/di/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/di/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3273 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/di/containers.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/domain/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication/users/domain/entities/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       89 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/entities/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      705 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/entities/app_entity.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1158 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/entities/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      578 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/entities/user_role.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/domain/ports/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       72 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/ports/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      168 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/domain/ports/event_producer.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1300 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/domain/ports/repository.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      100 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/domain/ports/session.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      661 2023-03-10 13:22:58.000000 idp_authentication-0.1.6/idp_authentication/users/domain/ports/unit_of_work.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      603 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1976 2023-03-10 13:24:03.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/authorize_app_entity_records.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2699 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/authorize_or_get_all_allowed_record_identifiers.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1321 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/create_or_update_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      553 2023-03-10 13:24:44.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_allowed_records_identifiers.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      782 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      733 2023-03-30 13:29:46.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_users_with_access_to_app_entity_record.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6332 2023-03-30 13:27:53.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/process_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1166 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/send_app_entity_record_event.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/infrastructure/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       65 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      509 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/base.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1069 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/custom_orm_column_types.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      806 2023-01-05 16:57:41.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      643 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/user_role.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/infrastructure/fastapi/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/infrastructure/fastapi/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/tests/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/tests/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/idp_authentication/users/tests/domain/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1973 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_authorize_and_get_records_or_get_all_allowed.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1703 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_authorize_app_entity_records.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1341 2023-03-10 11:57:51.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_create_or_update_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      978 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_allowed_app_entity_records.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      709 2022-12-23 15:35:48.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2279 2023-03-10 11:57:51.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_users_with_access_to_app_entity_record.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2513 2023-03-31 17:46:49.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_process_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      882 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_send_app_entity_record_event.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      365 2023-01-26 12:59:04.000000 idp_authentication-0.1.6/idp_authentication/users/tests/mock_event_producer.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-03-31 17:52:45.569539 idp_authentication-0.1.6/idp_authentication.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5312 2023-03-31 17:52:45.000000 idp_authentication-0.1.6/idp_authentication.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3710 2023-03-31 17:52:45.000000 idp_authentication-0.1.6/idp_authentication.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-03-31 17:52:45.000000 idp_authentication-0.1.6/idp_authentication.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      296 2023-03-31 17:52:45.000000 idp_authentication-0.1.6/idp_authentication.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       19 2023-03-31 17:52:45.000000 idp_authentication-0.1.6/idp_authentication.egg-info/top_level.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1688 2023-03-31 17:48:23.000000 idp_authentication-0.1.6/pyproject.toml
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2023-03-31 17:52:45.573539 idp_authentication-0.1.6/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-03-10 12:04:33.000000 idp_authentication-0.1.6/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       34 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5317 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4486 2023-03-10 11:57:51.000000 idp_authentication-0.1.7.dev1/README.md
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      247 2023-03-10 12:04:33.000000 idp_authentication-0.1.7.dev1/idp_authentication/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      858 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/config.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     7009 2023-03-31 17:47:05.000000 idp_authentication-0.1.7.dev1/idp_authentication/conftest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1695 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/custom_types.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1286 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/enums.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      553 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/exceptions.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3351 2023-04-11 09:41:03.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/orm.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/repositories/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/repositories/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1616 2023-04-03 15:46:10.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/repositories/user_repository.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      317 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/repositories/user_role_repository.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      846 2023-03-30 13:29:46.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/unit_of_work.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      328 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_entity.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1042 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_repository.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      721 2023-04-03 15:30:28.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_unit_of_work.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3267 2023-03-30 13:29:46.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_use_case.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      511 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/singleton.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/di/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/di/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3273 2023-03-30 13:29:46.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/di/containers.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       89 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      705 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/app_entity.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1158 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      578 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/user_role.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       72 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      168 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/event_producer.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1300 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/repository.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      100 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/session.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      661 2023-03-10 13:22:58.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/unit_of_work.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      603 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1976 2023-03-10 13:24:03.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/authorize_app_entity_records.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2699 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/authorize_or_get_all_allowed_record_identifiers.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1321 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/create_or_update_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      553 2023-03-10 13:24:44.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_allowed_records_identifiers.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      782 2023-03-30 13:29:46.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      733 2023-03-30 13:29:46.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_users_with_access_to_app_entity_record.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6332 2023-03-30 13:27:53.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/process_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1166 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/send_app_entity_record_event.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       65 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      509 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/base.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1069 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/custom_orm_column_types.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      806 2023-01-05 16:57:41.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      643 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/user_role.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/fastapi/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/fastapi/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1973 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_authorize_and_get_records_or_get_all_allowed.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1703 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_authorize_app_entity_records.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1341 2023-03-10 11:57:51.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_create_or_update_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      978 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_allowed_app_entity_records.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      709 2022-12-23 15:35:48.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2279 2023-03-10 11:57:51.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_users_with_access_to_app_entity_record.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2513 2023-03-31 17:46:49.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_process_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      882 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_send_app_entity_record_event.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      365 2023-01-26 12:59:04.000000 idp_authentication-0.1.7.dev1/idp_authentication/users/tests/mock_event_producer.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-11 09:42:19.121269 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5317 2023-04-11 09:42:19.000000 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3710 2023-04-11 09:42:19.000000 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-04-11 09:42:19.000000 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      296 2023-04-11 09:42:19.000000 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       19 2023-04-11 09:42:19.000000 idp_authentication-0.1.7.dev1/idp_authentication.egg-info/top_level.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1693 2023-04-11 09:42:15.000000 idp_authentication-0.1.7.dev1/pyproject.toml
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2023-04-11 09:42:19.125270 idp_authentication-0.1.7.dev1/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-03-10 12:04:33.000000 idp_authentication-0.1.7.dev1/setup.py
```

### Comparing `idp_authentication-0.1.6/LICENSE` & `idp_authentication-0.1.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/PKG-INFO` & `idp_authentication-0.1.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idp_authentication
-Version: 0.1.6
+Version: 0.1.7.dev1
 Summary: IDP Authentication - Hexagonal Architecture Implementation
 Author-email: Lirim Shala <lirim.shala@cardoai.com>, Klajdi Çaushi <klajdi.caushi@cardoai.com>
 Project-URL: Homepage, https://github.com/CardoAI/idp-authentication
 Project-URL: Bug Tracker, https://github.com/CardoAI/idp-authentication/issues
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

### Comparing `idp_authentication-0.1.6/README.md` & `idp_authentication-0.1.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/config.py` & `idp_authentication-0.1.7.dev1/idp_authentication/config.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/conftest.py` & `idp_authentication-0.1.7.dev1/idp_authentication/conftest.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/custom_types.py` & `idp_authentication-0.1.7.dev1/idp_authentication/custom_types.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/enums.py` & `idp_authentication-0.1.7.dev1/idp_authentication/enums.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/exceptions.py` & `idp_authentication-0.1.7.dev1/idp_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/adapters/orm.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,20 @@
         app_entity_signal = AppEntitySignal(send_event_use_case)
         listen(
             AppEntity,
             "after_insert",
             app_entity_signal.receive_after_insert_or_update,
             propagate=True,
         )
-        listen(
-            AppEntity,
-            "after_update",
-            app_entity_signal.receive_after_insert_or_update,
-            propagate=True,
-        )
+        # listen(
+        #     AppEntity,
+        #     "after_update",
+        #     app_entity_signal.receive_after_insert_or_update,
+        #     propagate=True,
+        # )
         listen(
             AppEntity,
             "after_delete",
             app_entity_signal.receive_after_delete,
             propagate=True,
         )
     except ArgumentError as e:
```

### Comparing `idp_authentication-0.1.6/idp_authentication/users/adapters/repositories/user_repository.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/repositories/user_repository.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/adapters/unit_of_work.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/adapters/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/base_classes/base_repository.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_repository.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/base_classes/base_unit_of_work.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/base_classes/base_use_case.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/base_classes/base_use_case.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/di/containers.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/di/containers.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/entities/app_entity.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/app_entity.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/entities/user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/entities/user_role.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/entities/user_role.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/ports/repository.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/repository.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/ports/unit_of_work.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/ports/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/__init__.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/authorize_app_entity_records.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/authorize_app_entity_records.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/authorize_or_get_all_allowed_record_identifiers.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/authorize_or_get_all_allowed_record_identifiers.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/create_or_update_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/create_or_update_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_allowed_records_identifiers.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_allowed_records_identifiers.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/get_users_with_access_to_app_entity_record.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/get_users_with_access_to_app_entity_record.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/process_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/process_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/domain/use_cases/send_app_entity_record_event.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/domain/use_cases/send_app_entity_record_event.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/custom_orm_column_types.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/custom_orm_column_types.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/infrastructure/database/sqlalchemy/user_role.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/infrastructure/database/sqlalchemy/user_role.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_authorize_and_get_records_or_get_all_allowed.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_authorize_and_get_records_or_get_all_allowed.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_authorize_app_entity_records.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_authorize_app_entity_records.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_create_or_update_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_create_or_update_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_allowed_app_entity_records.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_allowed_app_entity_records.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_get_users_with_access_to_app_entity_record.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_get_users_with_access_to_app_entity_record.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_process_user.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_process_user.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication/users/tests/domain/test_send_app_entity_record_event.py` & `idp_authentication-0.1.7.dev1/idp_authentication/users/tests/domain/test_send_app_entity_record_event.py`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/idp_authentication.egg-info/PKG-INFO` & `idp_authentication-0.1.7.dev1/idp_authentication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idp-authentication
-Version: 0.1.6
+Version: 0.1.7.dev1
 Summary: IDP Authentication - Hexagonal Architecture Implementation
 Author-email: Lirim Shala <lirim.shala@cardoai.com>, Klajdi Çaushi <klajdi.caushi@cardoai.com>
 Project-URL: Homepage, https://github.com/CardoAI/idp-authentication
 Project-URL: Bug Tracker, https://github.com/CardoAI/idp-authentication/issues
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

### Comparing `idp_authentication-0.1.6/idp_authentication.egg-info/SOURCES.txt` & `idp_authentication-0.1.7.dev1/idp_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idp_authentication-0.1.6/pyproject.toml` & `idp_authentication-0.1.7.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 allow-direct-references = true
 
 [tool.hatch.version]
 path = "idp_authentication/__init__.py"
 
 [project]
 name = "idp_authentication"
-version = "0.1.6"
+version = "0.1.7.dev1"
 description = "IDP Authentication - Hexagonal Architecture Implementation"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Lirim Shala", email = "lirim.shala@cardoai.com" },
     { name = "Klajdi Çaushi", email = "klajdi.caushi@cardoai.com" }
 ]
```

