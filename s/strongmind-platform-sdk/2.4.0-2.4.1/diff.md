# Comparing `tmp/strongmind-platform-sdk-2.4.0.tar.gz` & `tmp/strongmind-platform-sdk-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strongmind-platform-sdk-2.4.0.tar", last modified: Mon Apr 10 22:10:22 2023, max compression
+gzip compressed data, was "strongmind-platform-sdk-2.4.1.tar", last modified: Mon Apr 10 22:44:15 2023, max compression
```

## Comparing `strongmind-platform-sdk-2.4.0.tar` & `strongmind-platform-sdk-2.4.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.726745 strongmind-platform-sdk-2.4.0/platform_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/user_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/link_header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/cloud_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/platform_sdk/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/test/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/event_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_academic_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_guidref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_lineitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_org_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/user_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_slack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_user_creation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/user_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/link_header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/cloud_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.482132 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.482132 strongmind-platform-sdk-2.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/test/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/event_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_academic_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_guidref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_org_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/user_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_slack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_user_creation_client.py
```

### Comparing `strongmind-platform-sdk-2.4.0/PKG-INFO` & `strongmind-platform-sdk-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.4.0
+Version: 2.4.1
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.4.0/README.md` & `strongmind-platform-sdk-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/events_client.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/identity_client.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/identity_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/ods_client.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_authentication.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_client.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/slack.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/slack.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/clients/user_creation.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/clients/user_creation.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/helpers/exception_logger.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/helpers/exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/helpers/link_header.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/helpers/link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/platform_sdk/models/user.py` & `strongmind-platform-sdk-2.4.1/platform_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/setup.py` & `strongmind-platform-sdk-2.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strongmind-platform-sdk',
-    version='2.4.0',
+    version='2.4.1',
     packages=find_packages(),
     url='https://github.com/StrongMind/platform-python-sdk',
     license='',
     author='Team Platform',
     author_email='platform@strongmind.com',
     description='Common utilities, models, and clients used with StrongMind Platform APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.7',
     install_requires=[
         'pytz',
-        'oneroster-client>=2.0.2',
+        'strongmind-oneroster-client>=2.0.2',
         'pydantic>=1.8.2',
         'cryptography>=37.0.4'
     ],
 )
```

### Comparing `strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/PKG-INFO` & `strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.4.0
+Version: 2.4.1
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/SOURCES.txt` & `strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/event_factories.py` & `strongmind-platform-sdk-2.4.1/test/factories/event_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_academic_session.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_academic_session.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_class.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_class.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_course.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_course.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_enrollment.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_enrollment.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_guidref.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_guidref.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_lineitem.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_lineitem.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_org_factory.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_org_factory.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_result.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_result.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/oneroster_user.py` & `strongmind-platform-sdk-2.4.1/test/factories/oneroster_user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/factories/user_factories.py` & `strongmind-platform-sdk-2.4.1/test/factories/user_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_events_client.py` & `strongmind-platform-sdk-2.4.1/test/test_events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_exception_logger.py` & `strongmind-platform-sdk-2.4.1/test/test_exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_identity_client.py` & `strongmind-platform-sdk-2.4.1/test/test_identity_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_link_header.py` & `strongmind-platform-sdk-2.4.1/test/test_link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_ods_client.py` & `strongmind-platform-sdk-2.4.1/test/test_ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_oneroster_authentication.py` & `strongmind-platform-sdk-2.4.1/test/test_oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_oneroster_client.py` & `strongmind-platform-sdk-2.4.1/test/test_oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_slack_client.py` & `strongmind-platform-sdk-2.4.1/test/test_slack_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.0/test/test_user_creation_client.py` & `strongmind-platform-sdk-2.4.1/test/test_user_creation_client.py`

 * *Files identical despite different names*

