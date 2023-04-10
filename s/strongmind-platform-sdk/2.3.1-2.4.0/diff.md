# Comparing `tmp/strongmind-platform-sdk-2.3.1.tar.gz` & `tmp/strongmind-platform-sdk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strongmind-platform-sdk-2.3.1.tar", last modified: Thu Apr  6 14:52:30 2023, max compression
+gzip compressed data, was "strongmind-platform-sdk-2.4.0.tar", last modified: Mon Apr 10 22:10:22 2023, max compression
```

## Comparing `strongmind-platform-sdk-2.3.1.tar` & `strongmind-platform-sdk-2.4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.415847 strongmind-platform-sdk-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-06 14:52:30.415847 strongmind-platform-sdk-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.403847 strongmind-platform-sdk-2.3.1/platform_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.407847 strongmind-platform-sdk-2.3.1/platform_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/clients/user_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.407847 strongmind-platform-sdk-2.3.1/platform_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/helpers/exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/helpers/link_header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.407847 strongmind-platform-sdk-2.3.1/platform_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/models/cloud_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/models/link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.407847 strongmind-platform-sdk-2.3.1/platform_sdk/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/platform_sdk/shared/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 14:52:30.415847 strongmind-platform-sdk-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.411847 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-06 14:52:30.000000 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-06 14:52:30.000000 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:52:30.000000 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 14:52:30.000000 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 14:52:30.000000 strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.411847 strongmind-platform-sdk-2.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:52:30.415847 strongmind-platform-sdk-2.3.1/test/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/event_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_academic_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_guidref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_lineitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_org_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/oneroster_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/factories/user_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    32299 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_slack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-06 14:51:05.000000 strongmind-platform-sdk-2.3.1/test/test_user_creation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.726745 strongmind-platform-sdk-2.4.0/platform_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/clients/user_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/helpers/link_header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.730745 strongmind-platform-sdk-2.4.0/platform_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/cloud_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/platform_sdk/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/platform_sdk/shared/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 22:10:22.000000 strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.734746 strongmind-platform-sdk-2.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:10:22.738746 strongmind-platform-sdk-2.4.0/test/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/event_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_academic_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_guidref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_org_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/oneroster_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/factories/user_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_slack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-10 22:09:06.000000 strongmind-platform-sdk-2.4.0/test/test_user_creation_client.py
```

### Comparing `strongmind-platform-sdk-2.3.1/PKG-INFO` & `strongmind-platform-sdk-2.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.3.1
+Version: 2.4.0
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.3.1/README.md` & `strongmind-platform-sdk-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/events_client.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/identity_client.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/identity_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
     def __init__(self, http_error: HTTPError = None):
         if http_error:
             self.response = http_error.response
             self.request = http_error.request
 
 
+class IdentityClientError(Exception):
+    """Identity Client Error"""
+    dependency_name = IDENTITY_SERVER
+
+
 class IdentityServerClient:
     def __init__(self, identity_server_secret):
         self.baseurl = identity_server_secret['baseurl']
         self.client_id = identity_server_secret['client_id']
         self.client_secret = identity_server_secret['client_secret']
         self.token = None
 
@@ -105,15 +110,19 @@
             data["username"] = username
         if email is not None:
             data["email"] = email
         if is_active is not None:
             data["isActive"] = is_active
         response = requests.patch(url, headers=headers, json=data)
         raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
-        if len(response.text) > 0:
+
+        if response.text and 'Error - Identity' in response.text:
+            raise IdentityClientError(response.text)
+
+        if response.text:
             return response.json()
 
     def send_reminder_email(self, identity_id):
         headers = self._headers()
         url = f"{self.baseurl}/api/accounts/SendReminderEmail"
         response = requests.post(url, json=identity_id, headers=headers)
         raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
```

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/ods_client.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/oneroster_authentication.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/oneroster_client.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/slack.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/slack.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/clients/user_creation.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/clients/user_creation.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/helpers/exception_logger.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/helpers/exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/helpers/link_header.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/helpers/link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/platform_sdk/models/user.py` & `strongmind-platform-sdk-2.4.0/platform_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/setup.py` & `strongmind-platform-sdk-2.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strongmind-platform-sdk',
-    version='2.3.1',
+    version='2.4.0',
     packages=find_packages(),
     url='https://github.com/StrongMind/platform-python-sdk',
     license='',
     author='Team Platform',
     author_email='platform@strongmind.com',
     description='Common utilities, models, and clients used with StrongMind Platform APIs',
     long_description=long_description,
```

### Comparing `strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/PKG-INFO` & `strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.3.1
+Version: 2.4.0
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.3.1/strongmind_platform_sdk.egg-info/SOURCES.txt` & `strongmind-platform-sdk-2.4.0/strongmind_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/event_factories.py` & `strongmind-platform-sdk-2.4.0/test/factories/event_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_academic_session.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_academic_session.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_class.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_class.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_course.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_course.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_enrollment.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_enrollment.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_guidref.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_guidref.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_lineitem.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_lineitem.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_org_factory.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_org_factory.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_result.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_result.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/oneroster_user.py` & `strongmind-platform-sdk-2.4.0/test/factories/oneroster_user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/factories/user_factories.py` & `strongmind-platform-sdk-2.4.0/test/factories/user_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_events_client.py` & `strongmind-platform-sdk-2.4.0/test/test_events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_exception_logger.py` & `strongmind-platform-sdk-2.4.0/test/test_exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_identity_client.py` & `strongmind-platform-sdk-2.4.0/test/test_identity_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from expects import *
 from faker import Faker
 from freezegun import freeze_time
 from mockito import when, mock, unstub, verify, verifyStubbedInvocationsAreUsed
 from requests import HTTPError
 from requests.auth import HTTPBasicAuth
 
-from platform_sdk.clients.identity_client import IdentityServerClient, IdentityNotFoundError
+from platform_sdk.clients.identity_client import IdentityServerClient, IdentityNotFoundError, IdentityClientError
 from test.helpers.test_helpers import create_http_error
 
 fake = Faker()
 
 
 class TestIdentityTokenRetrieval(unittest.TestCase):
     def setUp(self) -> None:
@@ -40,14 +40,28 @@
         when(requests).post(
             f"https://{self.identity_server_domain}/connect/token",
             auth=HTTPBasicAuth(
                 username=self.identity_server_secret["client_id"],
                 password=self.identity_server_secret["client_secret"]),
             data={'grant_type': 'client_credentials'}).thenReturn(response)
 
+    def test_update_account_raises_identity_client_error_on_page_error(self):
+        identity_id = fake.uuid4()
+        url = f"https://{self.identity_server_domain}/api/accounts/{identity_id}"
+        headers = {'header': 'token'}
+        data = {'username': fake.word()}
+        response_text = '<html><head><title>Error - Identity</title>'
+        mock_response = mock({'text': response_text})
+        when(self.id_server_client)._headers().thenReturn(headers)
+        when(requests).patch(url, headers=headers, json=data).thenReturn(mock_response)
+        with self.assertRaises(IdentityClientError) as assert_error:
+            self.id_server_client.update_account(identity_id, username=data['username'])
+        expect(str(assert_error.exception)).to(equal(response_text))
+
+
     @freeze_time("2020-07-31")
     def test_identity_client_issues_new_token_when_none_exists(self):
         """When there is no token, we should get a new one so that we can have access"""
         expected_token = fake.word()
         response = mock({'status_code': 200, 'json': lambda: {"access_token": expected_token, "expires_in": 3600}})
         self.mock_token_retrieval(response)
         token = self.id_server_client.get_token()
```

### Comparing `strongmind-platform-sdk-2.3.1/test/test_link_header.py` & `strongmind-platform-sdk-2.4.0/test/test_link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_ods_client.py` & `strongmind-platform-sdk-2.4.0/test/test_ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_oneroster_authentication.py` & `strongmind-platform-sdk-2.4.0/test/test_oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_oneroster_client.py` & `strongmind-platform-sdk-2.4.0/test/test_oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_slack_client.py` & `strongmind-platform-sdk-2.4.0/test/test_slack_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.3.1/test/test_user_creation_client.py` & `strongmind-platform-sdk-2.4.0/test/test_user_creation_client.py`

 * *Files identical despite different names*

