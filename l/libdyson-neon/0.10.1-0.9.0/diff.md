# Comparing `tmp/libdyson-neon-0.10.1.tar.gz` & `tmp/libdyson-neon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdyson-neon-0.10.1.tar", last modified: Tue Apr 11 02:29:41 2023, max compression
+gzip compressed data, was "libdyson-neon-0.9.0.tar", last modified: Tue Mar 14 02:58:23 2023, max compression
```

## Comparing `libdyson-neon-0.10.1.tar` & `libdyson-neon-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.578775 libdyson-neon-0.10.1/libdyson/
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/libdyson/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/cloud_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_pure_hot_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/dyson_vacuum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/libdyson/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/libdyson_neon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-11 02:29:41.000000 libdyson-neon-0.10.1/libdyson_neon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-11 02:29:41.000000 libdyson-neon-0.10.1/libdyson_neon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:29:41.000000 libdyson-neon-0.10.1/libdyson_neon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 02:29:41.000000 libdyson-neon-0.10.1/libdyson_neon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 02:29:41.000000 libdyson-neon-0.10.1/libdyson_neon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 02:29:41.586775 libdyson-neon-0.10.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:29:41.582775 libdyson-neon-0.10.1/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/test_bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/test_cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/test_dyson_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/mocked_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_fan_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_heating_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_pure_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_purifier_humidify_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-11 02:29:32.000000 libdyson-neon-0.10.1/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 02:58:23.776262 libdyson-neon-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/cloud_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_vacuum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson_neon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 02:58:23.776262 libdyson-neon-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_dyson_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/mocked_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_fan_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_heating_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_purifier_humidify_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_vacuum.py
```

### Comparing `libdyson-neon-0.10.1/LICENSE` & `libdyson-neon-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/PKG-INFO` & `libdyson-neon-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 0.10.1
+Version: 0.9.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-0.10.1/libdyson/__init__.py` & `libdyson-neon-0.9.0/libdyson/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     DEVICE_TYPE_PURE_COOL_DESK,
     DEVICE_TYPE_PURE_COOL_LINK,
     DEVICE_TYPE_PURE_COOL_LINK_DESK,
     DEVICE_TYPE_PURE_HOT_COOL,
     DEVICE_TYPE_PURE_HOT_COOL_NEW,
     DEVICE_TYPE_PURE_HOT_COOL_LINK,
     DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL,
     DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE,
     DEVICE_TYPE_PURIFIER_HOT_COOL,
 )
 from .const import CleaningMode  # noqa: F401
 from .const import CleaningType  # noqa: F401
 from .const import DEVICE_TYPE_NAMES  # noqa: F401
 from .const import HumidifyOscillationMode  # noqa: F401
@@ -64,15 +63,12 @@
         return DysonPureHotCoolLink(serial, credential, device_type)
     if device_type in [
         DEVICE_TYPE_PURE_HOT_COOL,
         DEVICE_TYPE_PURE_HOT_COOL_NEW,
         DEVICE_TYPE_PURIFIER_HOT_COOL,
     ]:
         return DysonPureHotCool(serial, credential, device_type)
-    if device_type in [
-        DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-        DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL
-    ]:
+    if device_type == DEVICE_TYPE_PURE_HUMIDIFY_COOL:
         return DysonPureHumidifyCool(serial, credential, device_type)
     if device_type == DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE:
         return DysonPurifierHumidifyCoolFormaldehyde(serial, credential, device_type)
     return None
```

### Comparing `libdyson-neon-0.10.1/libdyson/cloud/account.py` & `libdyson-neon-0.9.0/libdyson/cloud/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,26 +10,24 @@
     DysonAuthRequired,
     DysonInvalidAccountStatus,
     DysonInvalidAuth,
     DysonLoginFailure,
     DysonNetworkError,
     DysonOTPTooFrequently,
     DysonServerError,
-    DysonAPIProvisionFailure,
 )
 
 from .device_info import DysonDeviceInfo
 
 DYSON_API_HOST = "https://appapi.cp.dyson.com"
 DYSON_API_HOST_CN = "https://appapi.cp.dyson.cn"
 DYSON_API_HEADERS = {
     "User-Agent": "android client"
 }
 
-API_PATH_PROVISION_APP = "/v1/provisioningservice/application/Android/version"
 API_PATH_USER_STATUS = "/v3/userregistration/email/userstatus"
 API_PATH_EMAIL_REQUEST = "/v3/userregistration/email/auth"
 API_PATH_EMAIL_VERIFY = "/v3/userregistration/email/verify"
 API_PATH_MOBILE_REQUEST = "/v3/userregistration/mobile/auth"
 API_PATH_MOBILE_VERIFY = "/v3/userregistration/mobile/verify"
 API_PATH_DEVICES = "/v2/provisioningservice/manifest"
 
@@ -114,46 +112,17 @@
             raise DysonNetworkError
         if response.status_code in [401, 403]:
             raise DysonInvalidAuth
         if 500 <= response.status_code < 600:
             raise DysonServerError
         return response
 
-    def provision_api(self) -> None:
-        """Provision the client connection to the API
-
-        Calls an app provisioning API. This is expected by the Dyson App API and makes the API server ready to accept
-        other API calls from the current IP Address.
-
-        Basically, this unlocks the API - the return value is not needed, and we don't need to save any cookies or
-        session tokens. It seems like the API Server sets some internal flag allowing API Calls from a specific address
-        based solely on this endpoint being called.
-
-        This isn't likely to be a security measure. It returns a version number in a json-encoded string: `"5.0.21061"`
-        and that is likely consumed by an app. Presumably, an official Dyson mobile app could check the version against
-        some internal expected value and, for example, prompt a user that it is outdated and direct them to the app
-        store to download a new version in order to continue working.
-        """
-
-        response = self.request(
-            "GET",
-            API_PATH_PROVISION_APP,
-            params=None,
-            data=None,
-            auth=False,
-        )
-
-        if response.status_code != 200:
-            raise DysonAPIProvisionFailure
-
-    def login_email_otp(self, email: str, region: str) -> Callable[[str, str], dict]:
+    def login_email_otp(self, email: str, region: str) -> Callable[[str], dict]:
         """Login using email and OTP code."""
-        self.provision_api()
-
-        # Check account status. This tells us whether an account is active or not.
+        # Check account status first. This is expected by the cloud API.
         response = self.request(
             "POST",
             API_PATH_USER_STATUS,
             params={"country": region},
             data={"email": email},
             auth=False,
         )
@@ -193,15 +162,14 @@
             body = response.json()
             self._auth_info = body
             return self._auth_info
 
         return _verify
 
     def devices(self) -> List[DysonDeviceInfo]:
-        self.provision_api()
         """Get device info from cloud account."""
         devices = []
         response = self.request("GET", API_PATH_DEVICES)
         for raw in response.json():
             if raw.get("LocalCredentials") is None:
                 # Lightcycle lights don't have LocalCredentials.
                 # They're not supported so just skip.
@@ -213,16 +181,14 @@
 
 class DysonAccountCN(DysonAccount):
     """Dyson account in Mainland China."""
 
     _HOST = DYSON_API_HOST_CN
 
     def login_mobile_otp(self, mobile: str) -> Callable[[str], dict]:
-        self.provision_api()
-
         """Login using phone number and OTP code."""
         response = self.request(
             "POST",
             API_PATH_MOBILE_REQUEST,
             data={"mobile": mobile},
             auth=False,
         )
```

### Comparing `libdyson-neon-0.10.1/libdyson/cloud/cloud_360_eye.py` & `libdyson-neon-0.9.0/libdyson/cloud/cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/cloud/device_info.py` & `libdyson-neon-0.9.0/libdyson/cloud/device_info.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/cloud/regions.py` & `libdyson-neon-0.9.0/libdyson/cloud/regions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/cloud/utils.py` & `libdyson-neon-0.9.0/libdyson/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/const.py` & `libdyson-neon-0.9.0/libdyson/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 DEVICE_TYPE_PURE_COOL_LINK = "475"
 DEVICE_TYPE_PURE_COOL_LINK_DESK = "469"
 DEVICE_TYPE_PURE_COOL = "438"
 DEVICE_TYPE_PURIFIER_COOL = "438K"
 DEVICE_TYPE_PURE_COOL_FORMALDEHYDE = "438E"
 DEVICE_TYPE_PURE_COOL_DESK = "520"
 DEVICE_TYPE_PURE_HUMIDIFY_COOL = "358"
-DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL = "358"
 DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE = "358E"
 DEVICE_TYPE_PURE_HOT_COOL_LINK = "455"
 DEVICE_TYPE_PURE_HOT_COOL = "527"
 DEVICE_TYPE_PURE_HOT_COOL_NEW = "527E"
 DEVICE_TYPE_PURIFIER_HOT_COOL = "527K"
 
 DEVICE_TYPE_NAMES = {
@@ -26,15 +25,14 @@
     DEVICE_TYPE_PURE_COOL_DESK: "Pure Cool Desk",
     DEVICE_TYPE_PURE_COOL_LINK: "Pure Cool Link",
     DEVICE_TYPE_PURE_COOL_LINK_DESK: "Pure Cool Link Desk",
     DEVICE_TYPE_PURE_HOT_COOL: "Pure Hot+Cool",
     DEVICE_TYPE_PURE_HOT_COOL_NEW: "Pure Hot+Cool (New)",
     DEVICE_TYPE_PURE_HOT_COOL_LINK: "Pure Hot+Cool Link",
     DEVICE_TYPE_PURE_HUMIDIFY_COOL: "Pure Humidify+Cool",
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL: "Purifier Humidify+Cool",
     DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE: "Purifier Humidify+Cool Formaldehyde",
     DEVICE_TYPE_PURIFIER_HOT_COOL: "Purifier Hot+Cool",
 }
 
 ENVIRONMENTAL_OFF = -1
 ENVIRONMENTAL_INIT = -2
 ENVIRONMENTAL_FAIL = -3
```

### Comparing `libdyson-neon-0.10.1/libdyson/discovery.py` & `libdyson-neon-0.9.0/libdyson/discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_360_eye.py` & `libdyson-neon-0.9.0/libdyson/dyson_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_360_heurist.py` & `libdyson-neon-0.9.0/libdyson/dyson_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_device.py` & `libdyson-neon-0.9.0/libdyson/dyson_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_pure_cool.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_pure_cool_link.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_pure_hot_cool_link.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_pure_humidify_cool.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/dyson_vacuum_device.py` & `libdyson-neon-0.9.0/libdyson/dyson_vacuum_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson/exceptions.py` & `libdyson-neon-0.9.0/libdyson/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,14 @@
     """Represents invalid account status."""
 
 
 class DysonLoginFailure(DysonException):
     """Represents failure during logging in."""
 
 
-class DysonAPIProvisionFailure(DysonException):
-    """Represents failure during logging in."""
-
-
 class DysonOTPTooFrequently(DysonException):
     """Represents requesting OTP code too frequently."""
 
 
 class DysonAuthRequired(DysonException):
     """Represents not logged into could."""
```

### Comparing `libdyson-neon-0.10.1/libdyson/utils.py` & `libdyson-neon-0.9.0/libdyson/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/libdyson_neon.egg-info/PKG-INFO` & `libdyson-neon-0.9.0/libdyson_neon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 0.10.1
+Version: 0.9.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-0.10.1/libdyson_neon.egg-info/SOURCES.txt` & `libdyson-neon-0.9.0/libdyson_neon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/pyproject.toml` & `libdyson-neon-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/setup.cfg` & `libdyson-neon-0.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libdyson-neon
-version = 0.10.1
+version = 0.9.0
 author = The libdyson Working Group
 author_email = dotvezz@gmail.com
 license = MIT License
 license_file = LICENSE
 platforms = any
 description = A Python library for Dyson devices.
 long_description = file: README.md
```

### Comparing `libdyson-neon-0.10.1/tests/cloud/mocked_requests.py` & `libdyson-neon-0.9.0/tests/cloud/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/cloud/test_bearer_auth.py` & `libdyson-neon-0.9.0/tests/cloud/test_bearer_auth.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/cloud/test_cloud_360_eye.py` & `libdyson-neon-0.9.0/tests/cloud/test_cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/cloud/test_dyson_account.py` & `libdyson-neon-0.9.0/tests/cloud/test_dyson_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 from libdyson.cloud.account import (
     API_PATH_DEVICES,
     API_PATH_EMAIL_REQUEST,
     API_PATH_EMAIL_VERIFY,
     API_PATH_MOBILE_REQUEST,
     API_PATH_MOBILE_VERIFY,
     API_PATH_USER_STATUS,
-    API_PATH_PROVISION_APP,
     DYSON_API_HOST_CN,
     DysonAccountCN,
     HTTPBearerAuth,
 )
 from libdyson.exceptions import (
     DysonAuthRequired,
     DysonInvalidAccountStatus,
     DysonInvalidAuth,
     DysonLoginFailure,
     DysonNetworkError,
     DysonOTPTooFrequently,
     DysonServerError,
-    DysonAPIProvisionFailure,
 )
 
 from . import AUTH_ACCOUNT, AUTH_INFO, AUTH_PASSWORD
 from .mocked_requests import MockedRequests
 from .utils import encrypt_credential
 
 EMAIL = "user@example.com"
@@ -97,26 +95,14 @@
         "NewVersionAvailable": False,
         "ProductType": "552",
         "ConnectionType": "wss",
     },
 ]
 
 
-def _app_provision_handler(
-        params: dict, json: dict, auth: Optional[AuthBase], **kwargs
-) -> Tuple[int, Optional[str]]:
-    return 200, '"5.0.21061"'
-
-
-def _app_provision_handler_error(
-        params: dict, json: dict, auth: Optional[AuthBase], **kwargs
-) -> Tuple[int, Optional[str]]:
-    return 404, ''
-
-
 @pytest.fixture(autouse=True)
 def mocked_requests(mocked_requests: MockedRequests) -> MockedRequests:
     """Return mocked requests library."""
 
     def _user_status_handler(
         params: dict, json: dict, auth: Optional[AuthBase], **kwargs
     ) -> Tuple[int, Optional[dict]]:
@@ -172,15 +158,14 @@
             or auth.username != AUTH_ACCOUNT
             or auth.password != AUTH_PASSWORD
         ) and (not isinstance(auth, HTTPBearerAuth) or auth.token != BEARER_TOKEN):
             return (401, None)
         return (200, DEVICES)
 
     mocked_requests.register_handler("POST", API_PATH_USER_STATUS, _user_status_handler)
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler)
     mocked_requests.register_handler(
         "POST", API_PATH_EMAIL_REQUEST, _email_request_handler
     )
     mocked_requests.register_handler(
         "POST", API_PATH_EMAIL_VERIFY, _email_verify_handler
     )
     mocked_requests.register_handler(
@@ -189,26 +174,14 @@
     mocked_requests.register_handler(
         "POST", API_PATH_MOBILE_VERIFY, _mobile_verify_handler
     )
     mocked_requests.register_handler("GET", API_PATH_DEVICES, _devices_handler)
     return mocked_requests
 
 
-def test_account_provision_api(mocked_requests: MockedRequests):
-    account = DysonAccount()
-
-    assert account.provision_api() is None
-
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler_error)
-
-    with pytest.raises(DysonAPIProvisionFailure):
-        account.provision_api()
-
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler)
-
 def test_account():
     """Test account functionalities."""
     account = DysonAccount()
 
     # Incorrect email
     with pytest.raises(DysonInvalidAccountStatus):
         account.login_email_otp("unregistered@example.com", REGION)
```

### Comparing `libdyson-neon-0.10.1/tests/cloud/utils.py` & `libdyson-neon-0.9.0/tests/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/conftest.py` & `libdyson-neon-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/mocked_mqtt.py` & `libdyson-neon-0.9.0/tests/mocked_mqtt.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_360_eye.py` & `libdyson-neon-0.9.0/tests/test_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_360_heurist.py` & `libdyson-neon-0.9.0/tests/test_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_device.py` & `libdyson-neon-0.9.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_discovery.py` & `libdyson-neon-0.9.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_fan_device.py` & `libdyson-neon-0.9.0/tests/test_fan_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_heating_device.py` & `libdyson-neon-0.9.0/tests/test_heating_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_init.py` & `libdyson-neon-0.9.0/tests/test_init.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     DEVICE_TYPE_PURE_COOL_DESK,
     DEVICE_TYPE_PURE_COOL_LINK,
     DEVICE_TYPE_PURE_COOL_LINK_DESK,
     DEVICE_TYPE_PURE_HOT_COOL,
     DEVICE_TYPE_PURE_HOT_COOL_NEW,
     DEVICE_TYPE_PURE_HOT_COOL_LINK,
     DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL,
     DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE,
     DEVICE_TYPE_PURIFIER_HOT_COOL,
     Dyson360Eye,
     Dyson360Heurist,
     DysonDevice,
     DysonPureCool,
     DysonPureCoolFormaldehyde,
@@ -44,15 +43,14 @@
         (DEVICE_TYPE_PURE_COOL, DysonPureCool),
         (DEVICE_TYPE_PURE_COOL_FORMALDEHYDE, DysonPureCoolFormaldehyde),
         (DEVICE_TYPE_PURE_COOL_DESK, DysonPureCool),
         (DEVICE_TYPE_PURE_HOT_COOL_LINK, DysonPureHotCoolLink),
         (DEVICE_TYPE_PURE_HOT_COOL, DysonPureHotCool),
         (DEVICE_TYPE_PURE_HOT_COOL_NEW, DysonPureHotCool),
         (DEVICE_TYPE_PURE_HUMIDIFY_COOL, DysonPureHumidifyCool),
-        (DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL, DysonPureHumidifyCool),
         (DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE, DysonPurifierHumidifyCoolFormaldehyde),
         (DEVICE_TYPE_PURIFIER_HOT_COOL, DysonPureHotCool),
     ],
 )
 def test_get_device(device_type: str, class_type: Type[DysonDevice]):
     """Test get_device."""
     device = get_device(SERIAL, CREDENTIAL, device_type)
```

### Comparing `libdyson-neon-0.10.1/tests/test_pure_cool.py` & `libdyson-neon-0.9.0/tests/test_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_pure_cool_formaldehyde.py` & `libdyson-neon-0.9.0/tests/test_pure_cool_formaldehyde.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_pure_cool_link.py` & `libdyson-neon-0.9.0/tests/test_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_pure_hot_cool_link.py` & `libdyson-neon-0.9.0/tests/test_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_pure_humidify_cool.py` & `libdyson-neon-0.9.0/tests/test_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_purifier_humidify_cool_formaldehyde.py` & `libdyson-neon-0.9.0/tests/test_purifier_humidify_cool_formaldehyde.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_utils.py` & `libdyson-neon-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.10.1/tests/test_vacuum.py` & `libdyson-neon-0.9.0/tests/test_vacuum.py`

 * *Files identical despite different names*

