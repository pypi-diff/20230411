# Comparing `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1.tar.gz` & `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1.tar", last modified: Tue Mar 14 09:49:27 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar", last modified: Tue Apr 11 10:20:05 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1.tar` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.411512 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/
--rw-r--r--   0 mati      (1000) mati      (1000)      375 2023-03-14 09:49:27.410513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/PKG-INFO
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.407513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.407513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.408512 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/
--rw-r--r--   0 mati      (1000) mati      (1000)       41 2022-07-26 09:18:31.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      709 2023-03-14 09:49:13.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.408512 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/data/
--rw-r--r--   0 mati      (1000) mati      (1000)        0 2022-07-29 12:12:47.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/data/data.xml
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.408512 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/i18n/
--rw-r--r--   0 mati      (1000) mati      (1000)    26377 2023-01-02 13:00:50.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.409513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/
--rw-r--r--   0 mati      (1000) mati      (1000)      211 2023-03-14 09:33:32.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      361 2023-02-08 12:58:56.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/account_allocation.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1214 2022-07-19 10:07:46.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py
--rw-r--r--   0 mati      (1000) mati      (1000)      368 2023-03-14 09:33:32.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/participant_liquidations.py
--rw-r--r--   0 mati      (1000) mati      (1000)      549 2022-09-26 07:54:13.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py
--rw-r--r--   0 mati      (1000) mati      (1000)      258 2023-01-02 13:09:16.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/res_partner.py
--rw-r--r--   0 mati      (1000) mati      (1000)      236 2022-12-16 11:24:29.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/res_partner_interest.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.409513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/security/
--rw-r--r--   0 mati      (1000) mati      (1000)      349 2023-03-09 10:33:40.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/security/ir.model.access.csv
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.409513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/
--rw-r--r--   0 mati      (1000) mati      (1000)      541 2022-07-18 17:51:47.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml
--rw-r--r--   0 mati      (1000) mati      (1000)      603 2022-07-13 10:00:01.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml
--rw-r--r--   0 mati      (1000) mati      (1000)      655 2022-09-26 07:54:13.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml
--rw-r--r--   0 mati      (1000) mati      (1000)      564 2023-01-02 13:00:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml
--rw-r--r--   0 mati      (1000) mati      (1000)     2325 2022-12-16 11:24:29.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.410513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/
--rw-r--r--   0 mati      (1000) mati      (1000)       52 2022-07-18 17:51:47.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)      532 2022-07-19 11:26:32.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py
--rw-r--r--   0 mati      (1000) mati      (1000)      673 2022-07-18 17:51:47.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2023-03-14 09:49:27.410513 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/
--rw-r--r--   0 mati      (1000) mati      (1000)      375 2023-03-14 09:49:27.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/PKG-INFO
--rw-r--r--   0 mati      (1000) mati      (1000)     1727 2023-03-14 09:49:27.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2023-03-14 09:49:27.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/dependency_links.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2023-02-23 01:22:53.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/not-zip-safe
--rw-r--r--   0 mati      (1000) mati      (1000)       21 2023-03-14 09:49:27.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/requires.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        5 2023-03-14 09:49:27.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/top_level.txt
--rw-r--r--   0 mati      (1000) mati      (1000)       38 2023-03-14 09:49:27.411512 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/setup.cfg
--rw-r--r--   0 mati      (1000) mati      (1000)      235 2023-03-14 09:33:32.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.031493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.032493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    26377 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.038493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/account_allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/participant_liquidations.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/res_partner_interest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.038493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/security/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.040494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.041494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.043494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/setup.py
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Photovoltaic Management Extended",
-    'version': '13.0.1.0.4',
+    'version': '13.0.1.1.0',
     'depends': ['photovoltaic_mgmt', 'photovoltaic_participant_liquidations'],
     'author': "Librecoop",
     'category': 'Sales',
     'description': """
     This module extendes the functionality of the Photovoltaic Management module
     """,
     "installable": True,
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.0.4.dev1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

