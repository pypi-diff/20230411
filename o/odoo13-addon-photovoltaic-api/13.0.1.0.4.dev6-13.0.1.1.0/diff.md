# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6.tar", last modified: Tue Mar 14 09:45:55 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.0.tar", last modified: Tue Apr 11 10:20:00 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.759100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/
--rw-r--r--   0 mati      (1000) mati      (1000)      398 2023-03-14 09:45:55.759100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/PKG-INFO
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.755100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.755100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.756100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/
--rw-r--r--   0 mati      (1000) mati      (1000)       70 2023-01-09 09:49:38.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      950 2023-02-23 01:25:14.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.756100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/controllers/
--rw-r--r--   0 mati      (1000) mati      (1000)       24 2022-07-29 12:18:12.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      240 2022-09-26 07:54:13.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.756100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/data/
--rw-r--r--   0 mati      (1000) mati      (1000)     3883 2023-01-03 13:11:56.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.757100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/models/
--rw-r--r--   0 mati      (1000) mati      (1000)       33 2022-09-26 07:54:13.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/models/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      510 2022-09-26 07:54:13.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.757100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/
--rw-r--r--   0 mati      (1000) mati      (1000)     1303 2022-11-18 13:03:18.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      295 2022-11-16 16:00:36.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-r--r--   0 mati      (1000) mati      (1000)      148 2022-11-16 16:00:27.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-r--r--   0 mati      (1000) mati      (1000)      540 2023-02-08 12:43:19.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-r--r--   0 mati      (1000) mati      (1000)      273 2023-01-03 13:34:34.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-r--r--   0 mati      (1000) mati      (1000)      187 2022-09-01 10:35:06.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-r--r--   0 mati      (1000) mati      (1000)      977 2022-12-02 09:53:38.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-r--r--   0 mati      (1000) mati      (1000)      134 2022-11-16 16:00:45.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2001 2023-03-07 13:27:22.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.757100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/security/
--rw-r--r--   0 mati      (1000) mati      (1000)     2699 2023-03-14 09:33:19.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.758100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/
--rw-r--r--   0 mati      (1000) mati      (1000)      164 2022-08-26 12:57:00.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)     4558 2023-03-14 09:33:19.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/account.py
--rw-r--r--   0 mati      (1000) mati      (1000)     5158 2022-11-07 14:22:44.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/allocations.py
--rw-r--r--   0 mati      (1000) mati      (1000)     3533 2023-03-14 09:33:32.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-r--r--   0 mati      (1000) mati      (1000)     5878 2023-02-08 12:43:19.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/contracts.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2057 2023-01-02 12:58:40.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/info.py
--rw-r--r--   0 mati      (1000) mati      (1000)     3290 2022-12-02 09:53:38.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-r--r--   0 mati      (1000) mati      (1000)     3502 2023-03-14 09:33:32.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.758100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/tests/
--rw-r--r--   0 mati      (1000) mati      (1000)       27 2023-01-09 15:10:31.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1029 2023-03-14 09:33:19.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/tests/common.py
--rw-r--r--   0 mati      (1000) mati      (1000)     5641 2023-01-11 14:02:40.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:45:55.759100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 mati      (1000) mati      (1000)      398 2023-03-14 09:45:55.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 mati      (1000) mati      (1000)     1808 2023-03-14 09:45:55.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2023-03-14 09:45:55.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2023-02-23 01:21:17.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 mati      (1000) mati      (1000)      208 2023-03-14 09:45:55.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        5 2023-03-14 09:45:55.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 mati      (1000) mati      (1000)       38 2023-03-14 09:45:55.759100 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/setup.cfg
--rw-r--r--   0 mati      (1000) mati      (1000)      328 2022-11-07 14:22:44.000000 odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.763423 odoo13-addon-photovoltaic_api-13.0.1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-11 10:20:00.762422 odoo13-addon-photovoltaic_api-13.0.1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.746421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.746421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.750421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.751422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.751422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.752422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.755422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.756422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.759422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4715 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3698 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.760422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.762422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:20:00.763423 odoo13-addon-photovoltaic_api-13.0.1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.0.3',
+    'version': '13.0.1.1.0',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
@@ -13,15 +13,15 @@
         'photovoltaic_participant_activities',
         'res_partner_custom',
         'portal',
         'base_vat'
     ],
     "external_dependencies": {
         "python": [
-            "pydantic[email]",
+            "pydantic[email]<2.0",
             "pyjwt"
         ]
     },
     'author': 'Librecoop',
     'author_email': 'librecoop@protonmail.com',
     'category': 'Sales',
     'description': '''
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     lastname:       Optional[str]
     street:         Optional[str]
     street2:        Optional[str] = Field(alias='additional_street')
     zip:            Optional[str]
     city:           Optional[str]
     state_id:       Optional[int]
     country_id:     Optional[int]
-    email:          Optional[EmailStr]
+    email:          Optional[str]
     phone:          Optional[str]
     mobile:         Optional[str]
     alias:          Optional[str]
     vat:            Optional[str]
     gender_partner: Optional[str] = Field(alias='gender')
     birthday:       Optional[str]
     representative: Optional[UserShort]
@@ -44,15 +44,15 @@
     lastname:          str
     street:            str
     additional_street: Optional[str]
     zip:               str
     city:              str
     state:             Optional[State]
     country:           Optional[Country]
-    email:             EmailStr
+    email:             str
     phone:             Optional[str]
     mobile:            Optional[str]
     alias:             Optional[str]
     vat:               str
     gender:            Optional[str]
     birthday:          Optional[str]
     bank_accounts:     List[BankAccountOut]
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,13 @@
 access_participant_liquidations,participant.liquidations.portal,photovoltaic_participant_liquidations.model_participant_liquidations,base.group_portal,1,0,0,0
 access_product_template_mode,product.template.mode.portal,photovoltaic_mgmt.model_product_template_mode,base.group_portal,1,0,0,0
 access_account_allocation,account.allocation.portal,photovoltaic_mgmt.model_account_allocation,base.group_portal,1,0,0,0
 access_account_period_type,account.period.type.portal,photovoltaic_mgmt.model_account_period_type,base.group_portal,1,0,0,0
 access_res_partner_bank,res.partner.bank.portal,account.model_res_partner_bank,base.group_portal,1,1,1,1
 access_photovoltaic_power_station,photovoltaic.power.station.portal,photovoltaic_mgmt.model_photovoltaic_power_station,base.group_portal,1,0,0,0
 access_photovoltaic_power_energy,photovoltaic.power.energy.portal,photovoltaic_mgmt.model_photovoltaic_power_energy,base.group_portal,1,0,0,0
-access_account_allocation,account.allocation.portal,photovoltaic_mgmt.model_account_allocation,base.group_portal,1,0,0,0
 access_mail_tracking_value,mail.tracking.value,mail.model_mail_tracking_value,base.group_portal,1,0,0,0
 access_snailmail_letter,snailmail.letter,snailmail.model_snailmail_letter,base.group_portal,1,0,0,0
 access_mail_activity,mail.activity,mail.model_mail_activity,base.group_portal,1,1,0,0
 access_plant_expense,plant.expense,photovoltaic_mgmt.model_plant_expense,base.group_portal,1,0,0,0
 access_plant_income,plant.income,photovoltaic_mgmt.model_plant_income,base.group_portal,1,0,0,0
 access_res_partner_interest,res.partner.interest.portal,photovoltaic_mgmt_extended.model_res_partner_interest,base.group_portal,1,1,0,0
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from odoo.addons.component.core import Component
-from odoo.addons.base_rest import restapi
-from odoo.exceptions import MissingError, UserError, AccessDenied
 import secrets
 from datetime import datetime, timedelta
+
 import jwt
+from odoo.addons.base_rest import restapi
+from odoo.addons.component.core import Component
+from odoo.exceptions import AccessDenied, MissingError, UserError
 
 
 class AccountService(Component):
     _inherit = 'base.rest.service'
     _name = 'account.service'
     _usage = 'account'
     _collection = 'photovoltaic_api.services'
@@ -59,21 +60,24 @@
 
         if len(partner) != 1:
             raise MissingError('Missing error')
 
         user = self.env['res.users'].search([('partner_id', '=', partner.id)])
 
         if len(user) == 0:
+            firstname = partner.firstname
+            lastname = partner.lastname
             self.env['res.users'].signup({
                 'login': partner.vat,
                 'email': partner.email,
                 'groups_id': [(6, 0, [self.env.ref('base.group_portal').id])],
                 'password': password
             }, token)
             user = self.env['res.users'].search([('login', '=', partner.vat)])
+            partner.write({'firstname': firstname, 'lastname': lastname})
         else:
             self.env['res.users'].signup({
                 'password': password
             }, token)
 
         return {
             'login': partner.vat,
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     )
     def search(self, contract_id=None, offset=0, limit=None):
         domain = [('partner_id', '=', self.env.user.partner_id.id)]
         if contract_id :
             domain.append(('contract_id', '=', int(contract_id)))
         
         # Get allocations
-        allocations = self.env['account.allocation'].search(domain, limit, offset, order='start_period_date')
-        total_allocations = self.env['account.allocation'].search_count(domain)
+        allocations = self.env['account.allocation'].search([*domain, ('start_period_date', '>=', '2021-01-01'), ('is_portal', '=', 'true')], limit, offset, order='start_period_date')
+        total_allocations = self.env['account.allocation'].search_count([*domain, ('start_period_date', '>=', '2021-01-01')])
 
         # Get liquidation (legacy allocations)
         liquidations = self.env['participant.liquidations'].search(domain, limit, offset, order='period')
         total_liquidations = self.env['participant.liquidations'].search_count(domain)
 
         rows = []
         for allocation in allocations:
@@ -38,20 +38,14 @@
         for liquidation in liquidations:
             rows.append(self._liquidation_to_json(liquidation))
 
         rows.sort(key=lambda datum: (datum['year'], datum['period']), reverse=True)
         return parse_obj_as(ListResponse[Allocation], {'total': total_allocations+total_liquidations, 'rows': [Allocation.parse_obj(r) for r in rows]})
 
 
-    # Private methods
-    def _calculate_allocation_period(self, start_date, end_date):
-        if (end_date.month - start_date.month == 2): #If only two months have passed from start to finish then it is trimestral otherwise is yearly
-            return int(end_date.month/3), end_date.year
-        return 0, end_date.year
-
     def _calculate_liquidation_period(self, full_period, payment_period):
         if (payment_period == 'Trimestral'):
             return int(full_period[0]), int(full_period.split(' ')[-1])
         return 0, int(full_period[len(full_period) - 4:])
 
     def _calculate_dates_of_period(self, period, year):
         if (period == 1):
@@ -76,21 +70,20 @@
                 energy_generated += production.energy_generated_contract
                 tn_co2_avoided += production.tn_co2_avoided_contract
                 eq_family_consumption += production.eq_family_consum_contract
 
         return energy_generated, tn_co2_avoided, eq_family_consumption
 
     def _allocation_to_json(self, allocation):
-        period, year = self._calculate_allocation_period(allocation.start_period_date, allocation.end_period_date)
         energy_generated, tn_co2_avoided, eq_family_consumption = self._calculate_production(allocation.contract_id.contract_production_ids, allocation.start_period_date, allocation.end_period_date)
         return {
             'id': allocation.id,
             'amount': allocation.total,
-            'period': period,
-            'year': year,
+            'period': int(allocation.end_period_date.month/3) if allocation.contract_id.payment_period_id.name == 'Trimestral' else 0,
+            'year': allocation.end_period_date.year,
             'state': allocation.state,
             'energy_generated': energy_generated,
             'tn_co2_avoided': tn_co2_avoided,
             'eq_family_consumption': eq_family_consumption,
             'type': 'allocation'
         }
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         [(['/'], 'GET')],
         input_param=restapi.CerberusValidator('_validator_search'),
         output_param=restapi.PydanticModel(ListResponse[Contract])
     )
     def search(self, offset=0, limit=None):
         try:
             contracts = self.env['contract.participation'].search(
-                [('partner_id', '=', self.env.user.partner_id.id)], limit, offset)
+                [('partner_id', '=', self.env.user.partner_id.id), ('photovoltaic_power_station_id.name', '!=', 'LAS NAVES BRILLEN'), ('product_mode_id.name', '!=', 'Comunero')], limit, offset)
             return self._list_to_pydantic(contracts)
 
         except AccessError:
             # Return 404 even if it is from a different user
             # to not leak information
             raise MissingError('Access error')
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/powerstation.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/powerstation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     def update(self, user_in):
         duplicated_vat_partners = self.env['res.partner'].sudo().search([('vat', '=', user_in.vat)])
         if user_in.vat and len(duplicated_vat_partners) > 0 and duplicated_vat_partners[0]['id'] != self.env.user.partner_id.id:
             raise UserError('vat already exists')
 
         user_dict = user_in.dict(exclude_unset=True, exclude={'representative', 'interests'})
 
+        if (user_in.zip or user_in.state or user_in.country_id):
+            user_dict['zip_id'] = None
+
         partner = self.env.user.partner_id
         is_login_vat = (partner.vat == self.env.user.login)
         partner.write(user_dict)
 
         if (partner.company_type == 'company' and partner.child_ids and user_in.representative):
             representative = partner.child_ids[0]
             representative.write(user_in.representative.dict(exclude_unset=True))
@@ -58,16 +61,16 @@
         representative = None
         if (user.company_type == 'company' and user.child_ids):
             representative = UserShort.from_orm(user.child_ids[0])
         
         return UserOut.parse_obj({
             'id': user.id,
             'person_type': user.company_type,
-            'firstname': user.firstname,
-            'lastname': user.lastname,
+            'firstname': user.firstname if user.company_type != 'company' else user.name,
+            'lastname': user.lastname if user.company_type != 'company' else '',
             'street': user.street,
             'additional_street': false_to_none(user, 'street2'),
             'zip': user.zip,
             'city': user.city,
             'state': State.from_orm(user.state_id) if user.state_id else None,
             'country': Country.from_orm(user.country_id) if user.country_id else None,
             'email': user.email,
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from odoo.tests.common import tagged
+from odoo.tools import mute_logger
 from .common import CommonCase
 from faker import Faker
 from faker.providers import ssn
 
 fake = Faker('es_ES')
 fake.add_provider(ssn)
 NAME = fake.name()
@@ -10,32 +11,35 @@
 EMAIL = fake.email()
 PASSWORD = fake.password(special_chars=False)
 PASSWORD2 = fake.password(special_chars=False)
 
 @tagged('post_install', '-at_install')
 class TestSignupRequest(CommonCase):
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_signup_request_no_partner(self):
         request = self.http('POST', '/api/account/signup_request', { 'vat': VAT }, { 'api_key': self.api_key })
         self.assertEqual(request.status_code, 404)
 
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_signup_request_not_participant(self):
         self.env['res.partner'].create({
             'name': NAME,
             'vat': VAT
         })
 
         self.assertEqual(len(self.env['res.partner'].search([('vat', '=', VAT)])), 1)
         self.assertEqual(self.env['res.partner'].search([('vat', '=', VAT)])[0].name, NAME)
 
         request = self.http('POST', '/api/account/signup_request', { 'vat': VAT }, { 'api_key': self.api_key })
         self.assertEqual(request.status_code, 400)
 
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_signup_request_correct(self):
         self.env['res.partner'].create({
             'name': NAME,
             'vat': VAT,
             'participant': True
         })
 
@@ -52,20 +56,22 @@
 
         self.signup_token = request.json()['token']
 
 
 @tagged('post_install', '-at_install')
 class TestSignup(TestSignupRequest):
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_signup_no_token(self):
         super().test_signup_request_correct()
         request = self.http('POST', '/api/account/signup', { 'token': 'asdfasdf', 'password': PASSWORD }, { 'api_key': self.api_key })
         self.assertEquals(request.status_code, 404)
 
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_signup_no_password(self):
         super().test_signup_request_correct()
         request = self.http('POST', '/api/account/signup', { 'token': self.signup_token }, { 'api_key': self.api_key })
         self.assertEquals(request.status_code, 500)
 
 
     def test_signup_correct(self):
@@ -74,14 +80,15 @@
 
         self.assertTrue(request.ok)
         self.assertEqual(request.json()['login'], VAT)
         self.assertEqual(len(self.env['res.users'].search([('login', '=', VAT)])), 1)
         self.assertIn(self.env.ref('base.group_portal'), self.env['res.users'].search([('login', '=', VAT)]).groups_id)
 
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_change_password(self):
         self.test_signup_correct()
 
         request = self.http('POST', '/api/account/signup_request', { 'vat': VAT }, { 'api_key': self.api_key })
         self.assertTrue(request.ok)
         signup_token = request.json()['token']
 
@@ -97,20 +104,22 @@
         request = self.http('POST', '/api/account/login', { 'vat': VAT, 'password': PASSWORD2 }, { 'api_key': self.api_key })
         self.assertTrue(request.ok)
 
 
 @tagged('post_install', '-at_install')
 class TestLogin(TestSignup):
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_login_wrong_password(self):
         super().test_signup_correct()
         request = self.http('POST', '/api/account/login', { 'vat': VAT, 'password': 'wrong' }, { 'api_key': self.api_key })
         self.assertEqual(request.status_code, 403)
 
 
+    @mute_logger('odoo.addons.base_rest.http')
     def test_login_not_participant(self):
         super().test_signup_correct()
         request = self.http('POST', '/api/account/login', { 'vat': 'wrong', 'password': 'wrong' }, { 'api_key': self.api_key })
         self.assertEqual(request.status_code, 403)
 
 
     def test_login_email(self):
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.0.4.dev6/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 setup.py
+odoo/addons/photovoltaic_api/CHANGELOG.md
 odoo/addons/photovoltaic_api/__init__.py
 odoo/addons/photovoltaic_api/__manifest__.py
 odoo/addons/photovoltaic_api/controllers/__init__.py
 odoo/addons/photovoltaic_api/controllers/controller.py
 odoo/addons/photovoltaic_api/data/data.xml
 odoo/addons/photovoltaic_api/models/__init__.py
 odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
```

