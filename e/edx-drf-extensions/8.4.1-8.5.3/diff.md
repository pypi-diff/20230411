# Comparing `tmp/edx-drf-extensions-8.4.1.tar.gz` & `tmp/edx-drf-extensions-8.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-drf-extensions-8.4.1.tar", last modified: Wed Jan 18 15:08:04 2023, max compression
+gzip compressed data, was "edx-drf-extensions-8.5.3.tar", last modified: Tue Apr 11 16:18:48 2023, max compression
```

## Comparing `edx-drf-extensions-8.4.1.tar` & `edx-drf-extensions-8.5.3.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.037530 edx-drf-extensions-8.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-01-18 15:08:04.037530 edx-drf-extensions-8.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/csrf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/csrf/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/csrf/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/csrf/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/csrf/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-01-18 15:08:04.000000 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-01-18 15:08:04.000000 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-18 15:08:04.000000 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-01-18 15:08:04.000000 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-01-18 15:08:04.000000 edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.029530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)     8221 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    11225 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    19901 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.033530 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)    17065 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/edx_rest_framework_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 15:08:04.037530 edx-drf-extensions-8.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-01-18 15:08:04.037530 edx-drf-extensions-8.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2023-01-18 15:08:01.000000 edx-drf-extensions-8.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     5709 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9145 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9145 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12023 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/setup.py
```

### Comparing `edx-drf-extensions-8.4.1/LICENSE.txt` & `edx-drf-extensions-8.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/README.rst` & `edx-drf-extensions-8.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/csrf/api/v1/views.py` & `edx-drf-extensions-8.5.3/csrf/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/csrf/tests/test_api.py` & `edx-drf-extensions-8.5.3/csrf/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/docs/conf.py` & `edx-drf-extensions-8.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_drf_extensions.egg-info/SOURCES.txt` & `edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 csrf/__init__.py
 csrf/apps.py
```

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/cookies.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/decoder.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 a security risk in the general case.)
 """
 import logging
 import sys
 
 import jwt
 from django.conf import settings
+from edx_django_utils.monitoring import set_custom_attribute
 from jwkest.jwk import KEYS
 from jwkest.jws import JWS
 from rest_framework_jwt.settings import api_settings
 from semantic_version import Version
 
 from edx_rest_framework_extensions.settings import get_first_jwt_issuer, get_jwt_issuers
 
@@ -169,14 +170,21 @@
     _set_is_restricted(token)
     _set_filters(token)
     return token
 
 
 def _verify_jwt_signature(token, jwt_issuer, decode_symmetric_token):
     key_set = _get_signing_jwk_key_set(jwt_issuer, add_symmetric_keys=decode_symmetric_token)
+    # .. custom_attribute_name: jwt_auth_verify_keys_count
+    # .. custom_attribute_description: Number of JWT verification keys in use for this
+    #   verification. Should be same as number of asymmetric public keys, plus one if
+    #   a symmetric key secret is set. This is intended to aid in key rotations; once
+    #   the average count stabilizes at a higher number after adding a public key, it
+    #   should be safe to change the secret key.
+    set_custom_attribute('jwt_auth_verify_keys_count', len(key_set))
 
     try:
         _ = JWS().verify_compact(token, key_set)
     except Exception as token_error:
         logger.exception('Token verification failed.')
         exc_info = sys.exc_info()
         raise jwt.InvalidTokenError(exc_info[2]) from token_error
```

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/middleware.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,14 +195,31 @@
     def test_success_asymmetric_jwt_decode(self):
         """
         Validates that a valid asymmetric token is properly decoded
         """
         token = generate_asymmetric_jwt_token(self.payload)
         self.assertEqual(get_asymmetric_only_jwt_decode_handler(token), self.payload)
 
+    @mock.patch('edx_rest_framework_extensions.auth.jwt.decoder.set_custom_attribute')
+    def test_keyset_size_monitoring(self, mock_set_custom_attribute):
+        """
+        Validates that a custom attribute is recorded for the keyset size.
+        """
+        token = generate_asymmetric_jwt_token(self.payload)
+
+        # The secret key is included by default making a list of length 2, but for
+        # asymmetric-only there is only 1 key in the keyset.
+        self.assertEqual(jwt_decode_handler(token), self.payload)
+        self.assertEqual(get_asymmetric_only_jwt_decode_handler(token), self.payload)
+
+        assert mock_set_custom_attribute.call_args_list == [
+            mock.call('jwt_auth_verify_keys_count', 2),
+            mock.call('jwt_auth_verify_keys_count', 1),
+        ]
+
 
 def _jwt_decode_handler_with_defaults(token):  # pylint: disable=unused-argument
     """
     Accepts anything as a token and returns a fake JWT payload with defaults.
     """
     return {
         'scopes': ['fake:scope'],
```

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,24 +91,24 @@
             pass
 
         @api_view(["GET"])
         @some_auth_decorator(include_jwt_auth, include_required_perm)
         def some_function_view(request):  # pylint: disable=unused-argument
             pass
 
-        views = dict(
-            class_view=SomeClassView,
-            view_set=SomeClassViewSet.as_view({'get': 'list'}),
-            function_view=some_function_view,
-        )
-        view_classes = dict(
-            class_view=SomeClassView,
-            view_set=views['view_set'].cls,  # pylint: disable=no-member
-            function_view=views['function_view'].view_class,
-        )
+        views = {
+            "class_view": SomeClassView,
+            "view_set": SomeClassViewSet.as_view({'get': 'list'}),
+            "function_view": some_function_view
+        }
+        view_classes = {
+            "class_view": SomeClassView,
+            "view_set": views['view_set'].cls,  # pylint: disable=no-member
+            "function_view": views['function_view'].view_class,
+        }
         view = views[view_type]
         view_class = view_classes[view_type]
 
         # verify pre-conditions
         self._assert_included(
             SomeJwtAuthenticationSubclass,
             view_class.authentication_classes,
```

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/jwt/tests/utils.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/auth/session/tests/test_authentication.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/config.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/config.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/middleware.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/paginators.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/permissions.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/settings.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_middleware.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_paginators.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_permissions.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,17 @@
     def _create_request(self, user, username_in_param=None, username_in_resource=None):
         url = '/'
         if username_in_param:
             url += f'?username={username_in_param}'
         request = RequestFactory().get(url)
         request.user = user
         if username_in_resource:
-            request.parser_context = dict(kwargs=dict(username=username_in_resource))
+            request.parser_context = {
+                "kwargs": {"username": username_in_resource}
+            }
         return request
 
     @ddt.data(True, False)
     def test_user_in_url_param(self, has_user_in_url):
         user = factories.UserFactory(username='this_user')
         request = self._create_request(
             user,
@@ -286,40 +288,40 @@
         self._create_session(request, user)
 
         response = self.SomeClassView().dispatch(request)
         self.assertEqual(response.status_code, 200)
 
     @ddt.data(
         # unrestricted
-        dict(
-            is_restricted=False,
-            is_user_in_url=True,
-            expected_response=200,
-            expected_log=JwtIsUnrestrictedDebugLog
-        ),
-        dict(
-            is_restricted=False,
-            is_user_in_url=False,
-            expected_response=403,
-            expected_log=IsUserInUrlLog
-        ),
+        {
+            "is_restricted": False,
+            "is_user_in_url": True,
+            "expected_response": 200,
+            "expected_log": JwtIsUnrestrictedDebugLog
+        },
+        {
+            "is_restricted": False,
+            "is_user_in_url": False,
+            "expected_response": 403,
+            "expected_log": IsUserInUrlLog
+        },
 
         # restricted (note: further test cases for scopes and filters are in tests below)
-        dict(
-            is_restricted=True,
-            is_user_in_url=True,
-            expected_response=403,
-            expected_log=JwtScopesErrorLog
-        ),
-        dict(
-            is_restricted=True,
-            is_user_in_url=False,
-            expected_response=403,
-            expected_log=JwtScopesErrorLog
-        ),
+        {
+            "is_restricted": True,
+            "is_user_in_url": True,
+            "expected_response": 403,
+            "expected_log": JwtScopesErrorLog
+        },
+        {
+            "is_restricted": True,
+            "is_user_in_url": False,
+            "expected_response": 403,
+            "expected_log": JwtScopesErrorLog
+        },
     )
     @ddt.unpack
     def test_jwt_without_scopes_and_filters(
             self,
             is_restricted,
             is_user_in_url,
             expected_response,
@@ -336,80 +338,92 @@
 
             response = self.SomeClassView().dispatch(request)
             self.assertEqual(response.status_code, expected_response)
             self._assert_log(mock_log, expected_log)
 
     @ddt.data(
         # valid scopes
-        dict(scopes=['required_scope'], expected_response=200, expected_log=JwtIsRestrictedDebugLog),
-        dict(scopes=['required_scope', 'another_scope'], expected_response=200, expected_log=JwtIsRestrictedDebugLog),
+        {
+            "scopes": ['required_scope'], "expected_response": 200,
+            "expected_log": JwtIsRestrictedDebugLog
+        },
+        {
+            "scopes": ['required_scope', 'another_scope'],
+            "expected_response": 200, "expected_log": JwtIsRestrictedDebugLog
+        },
 
         # invalid scopes
-        dict(scopes=[], expected_response=403, expected_log=JwtScopesErrorLog),
-        dict(scopes=['another_scope'], expected_response=403, expected_log=JwtScopesErrorLog),
+        {
+            "scopes": [], "expected_response": 403,
+            "expected_log": JwtScopesErrorLog
+        },
+        {
+            "scopes": ['another_scope'], "expected_response": 403,
+            "expected_log": JwtScopesErrorLog
+        },
     )
     @ddt.unpack
     def test_jwt_scopes(self, scopes, expected_response, expected_log):
         self._assert_jwt_restricted_case(
             scopes=scopes,
             filters=['content_org:some_org'],
             is_user_in_url=False,
             expected_response=expected_response,
             expected_log=expected_log,
         )
 
     @ddt.data(
         # valid org filters
-        dict(
-            filters=['content_org:some_org', 'content_org:another_org'],
-            expected_response=200,
-            expected_log=JwtIsRestrictedDebugLog
-        ),
+        {
+            "filters": ['content_org:some_org', 'content_org:another_org'],
+            "expected_response": 200,
+            "expected_log": JwtIsRestrictedDebugLog
+        },
 
         # invalid org filters
-        dict(
-            filters=['content_org:another_org'],
-            expected_response=403,
-            expected_log=JwtOrgFilterErrorLog
-        ),
-        dict(
-            filters=[],
-            expected_response=403,
-            expected_log=JwtOrgFilterErrorLog
-        ),
+        {
+            "filters": ['content_org:another_org'],
+            "expected_response": 403,
+            "expected_log": JwtOrgFilterErrorLog
+        },
+        {
+            "filters": [],
+            "expected_response": 403,
+            "expected_log": JwtOrgFilterErrorLog
+        },
     )
     @ddt.unpack
     def test_jwt_org_filters(self, filters, expected_response, expected_log):
         self._assert_jwt_restricted_case(
             scopes=['required_scope'],
             filters=filters,
             is_user_in_url=False,
             expected_response=expected_response,
             expected_log=expected_log,
         )
 
     @ddt.data(
         # valid user filters
-        dict(
-            user_filters=['user:me'], is_user_in_url=True,
-            expected_response=200,
-            expected_log=JwtIsRestrictedDebugLog,
-        ),
+        {
+            "user_filters": ['user:me'], "is_user_in_url": True,
+            "expected_response": 200,
+            "expected_log": JwtIsRestrictedDebugLog,
+        },
 
         # invalid user filters
-        dict(
-            user_filters=['user:me'], is_user_in_url=False,
-            expected_response=403,
-            expected_log=JwtUserFilterErrorLog,
-        ),
-        dict(
-            user_filters=['user:another'], is_user_in_url=True,
-            expected_response=403,
-            expected_log=JwtUserFilterErrorLog,
-        ),
+        {
+            "user_filters": ['user:me'], "is_user_in_url": False,
+            "expected_response": 403,
+            "expected_log": JwtUserFilterErrorLog,
+        },
+        {
+            "user_filters": ['user:another'], "is_user_in_url": True,
+            "expected_response": 403,
+            "expected_log": JwtUserFilterErrorLog,
+        },
     )
     @ddt.unpack
     def test_jwt_user_filters(self, user_filters, is_user_in_url, expected_response, expected_log):
         self._assert_jwt_restricted_case(
             scopes=['required_scope'],
             filters=['content_org:some_org'] + user_filters,
             is_user_in_url=is_user_in_url,
```

### Comparing `edx-drf-extensions-8.4.1/edx_rest_framework_extensions/tests/test_settings.py` & `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/requirements/constraints.txt` & `edx-drf-extensions-8.5.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.4.1/setup.py` & `edx-drf-extensions-8.5.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,19 +84,23 @@
     if version_match:
         return version_match.group(1)
     raise RuntimeError('Unable to find version string.')
 
 
 VERSION = get_version("edx_rest_framework_extensions", "__init__.py")
 
+README = open(os.path.join(os.path.dirname(__file__), 'README.rst'), encoding="utf8").read()
+CHANGELOG = open(os.path.join(os.path.dirname(__file__), 'CHANGELOG.rst'), encoding="utf8").read()
+
 
 setup(
     name='edx-drf-extensions',
     version=VERSION,
     description='edX extensions of Django REST Framework',
+    long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/openedx/edx-drf-extensions',
     license='Apache 2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
```

