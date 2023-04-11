# Comparing `tmp/alibabacloud_dingtalk-1.5.62.tar.gz` & `tmp/alibabacloud_dingtalk-1.5.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.62.tar", last modified: Fri Apr  7 09:21:49 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.63.tar", last modified: Tue Apr 11 09:50:13 2023, max compression
```

## Comparing `alibabacloud_dingtalk-1.5.62.tar` & `alibabacloud_dingtalk-1.5.63.tar`

### file list

```diff
@@ -1,345 +1,345 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/
--rw-r--r--   0 root         (0) root         (0)    18909 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22962 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51882 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   179168 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21344 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44730 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18586 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22436 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81490 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140148 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134106 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   294751 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40908 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63666 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177626 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   583083 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3576 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130914 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   326360 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24154 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41993 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31362 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106693 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61834 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121561 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56162 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82298 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51372 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   127231 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260294 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   382552 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18716 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44885 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15642 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32114 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194896 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   555654 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7207 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29122 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47050 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   340246 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503096 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99276 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   149418 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50064 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53792 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40488 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    66172 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   196916 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   261579 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134506 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   276268 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127432 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   192831 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   401586 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   699718 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62504 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110186 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75706 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118345 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4334 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   269266 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   414993 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140236 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   310177 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4520 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9290 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9446 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69681 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140857 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14767 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18751 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4336 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79106 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133812 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   268744 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   381405 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12612 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76078 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83510 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   438740 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   707813 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54446 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   160887 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54782 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111368 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77806 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129784 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14978 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24607 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117228 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   154147 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45940 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    51039 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    39828 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6891 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67864 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137575 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68812 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   125156 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48952 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57536 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   233262 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   399779 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16002 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9973 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   118728 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171405 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71838 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91606 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50744 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82767 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35104 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47649 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   322628 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499096 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28634 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25101 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40406 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105120 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   173162 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   389740 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9158 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31448 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30097 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60784 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   156671 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12502 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21548 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12290 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17800 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16936 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33576 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68340 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110827 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3124 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20769 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4608 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8329 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24540 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28057 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   154430 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385214 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3485 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   416280 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   690137 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11356 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-07 09:21:49.000000 alibabacloud_dingtalk-1.5.62/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/
+-rw-r--r--   0 root         (0) root         (0)    18974 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22962 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51882 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   179168 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21344 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44730 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18586 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22436 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81490 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140148 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134106 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   288074 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40908 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63666 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177626 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   583083 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   130914 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   326360 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24154 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41993 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31362 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106693 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61834 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121561 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56162 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82298 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51372 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   127231 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260294 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   382552 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18716 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44885 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32114 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194896 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   555654 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29122 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47050 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   340246 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503096 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99276 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   149418 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50064 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53792 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40488 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    66172 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196916 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   261579 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134506 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   276268 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127432 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   192831 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   401586 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   699718 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62504 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110186 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75706 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118345 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   273442 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   424209 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140236 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   310177 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9290 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9446 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69681 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140857 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14767 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18751 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4336 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79106 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133812 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   268744 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   381405 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12612 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76078 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83510 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   454060 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731352 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54446 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   160887 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54782 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111368 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77806 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129784 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14978 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24607 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117228 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   154147 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45940 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    51039 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    39828 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6891 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67864 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137575 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68812 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   125156 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48952 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57536 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233262 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   399779 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16002 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   118728 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171405 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71838 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91606 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50744 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82767 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35104 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47649 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   322628 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499096 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28634 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25101 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40406 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105120 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   173162 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   389740 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31448 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12420 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30097 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60784 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   156671 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21548 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12290 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17800 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16936 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33576 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68340 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110827 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20769 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8329 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24540 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28057 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   154430 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385214 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   416280 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   690137 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/setup.py
```

### Comparing `alibabacloud_dingtalk-1.5.62/ChangeLog.md` & `alibabacloud_dingtalk-1.5.63/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-07 Version: 1.5.62
+- Update AddOfficialAccountFollower.
+
 2023-04-04 Version: 1.5.61
 - Update AddOfficialAccountFollower.
 
 2023-03-27 Version: 1.5.59
 - Update AddOfficialAccountFollower.
 
 2023-03-21 Version: 1.5.58
```

### Comparing `alibabacloud_dingtalk-1.5.62/LICENSE` & `alibabacloud_dingtalk-1.5.63/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/PKG-INFO` & `alibabacloud_dingtalk-1.5.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 1.5.62
+Version: 1.5.63
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.62/README-CN.md` & `alibabacloud_dingtalk-1.5.63/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/README.md` & `alibabacloud_dingtalk-1.5.63/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5643,91 +5643,14 @@
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class GroupAddRequestResourcePermissionMap(TeaModel):
-    def __init__(
-        self,
-        camera_check: str = None,
-        check_position_type: str = None,
-        check_time: str = None,
-        group_member: str = None,
-        group_type: str = None,
-        out_side_check: str = None,
-        over_time_rule: str = None,
-        schedule: str = None,
-    ):
-        # 设置拍照打卡规则。
-        self.camera_check = camera_check
-        # 设置打卡方式。
-        self.check_position_type = check_position_type
-        # 设置考勤时间。
-        self.check_time = check_time
-        # 设置参与考勤人员。
-        self.group_member = group_member
-        # 设置考勤类型。
-        self.group_type = group_type
-        # 设置外勤打卡。
-        self.out_side_check = out_side_check
-        # 设置加班规则。
-        self.over_time_rule = over_time_rule
-        # 员工排班。
-        self.schedule = schedule
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.camera_check is not None:
-            result['cameraCheck'] = self.camera_check
-        if self.check_position_type is not None:
-            result['checkPositionType'] = self.check_position_type
-        if self.check_time is not None:
-            result['checkTime'] = self.check_time
-        if self.group_member is not None:
-            result['groupMember'] = self.group_member
-        if self.group_type is not None:
-            result['groupType'] = self.group_type
-        if self.out_side_check is not None:
-            result['outSideCheck'] = self.out_side_check
-        if self.over_time_rule is not None:
-            result['overTimeRule'] = self.over_time_rule
-        if self.schedule is not None:
-            result['schedule'] = self.schedule
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('cameraCheck') is not None:
-            self.camera_check = m.get('cameraCheck')
-        if m.get('checkPositionType') is not None:
-            self.check_position_type = m.get('checkPositionType')
-        if m.get('checkTime') is not None:
-            self.check_time = m.get('checkTime')
-        if m.get('groupMember') is not None:
-            self.group_member = m.get('groupMember')
-        if m.get('groupType') is not None:
-            self.group_type = m.get('groupType')
-        if m.get('outSideCheck') is not None:
-            self.out_side_check = m.get('outSideCheck')
-        if m.get('overTimeRule') is not None:
-            self.over_time_rule = m.get('overTimeRule')
-        if m.get('schedule') is not None:
-            self.schedule = m.get('schedule')
-        return self
-
-
 class GroupAddRequestShiftVOList(TeaModel):
     def __init__(
         self,
         shift_id: int = None,
     ):
         # 班次ID，可通过获取班次摘要信息接口获取。
         self.shift_id = shift_id
@@ -5820,15 +5743,15 @@
         modify_member: bool = None,
         offset: int = None,
         open_face_check: bool = None,
         outside_check_approve_mode_id: int = None,
         overtime_setting_id: int = None,
         owner: str = None,
         positions: List[GroupAddRequestPositions] = None,
-        resource_permission_map: List[GroupAddRequestResourcePermissionMap] = None,
+        resource_permission_map: Dict[str, Any] = None,
         shift_volist: List[GroupAddRequestShiftVOList] = None,
         skip_holidays: bool = None,
         special_days: str = None,
         trim_distance: int = None,
         type: str = None,
         wifis: List[GroupAddRequestWifis] = None,
         workday_class_list: List[int] = None,
@@ -5933,19 +5856,14 @@
         self.outside_check_approve_mode_id = outside_check_approve_mode_id
         # 加班规则settingId。
         self.overtime_setting_id = overtime_setting_id
         # 考勤组负责人。
         self.owner = owner
         # 考勤地点相关设置信息。
         self.positions = positions
-        # 子管理员权限范围。
-        # 
-        # w：可管理
-        # 
-        # r：可读
         self.resource_permission_map = resource_permission_map
         # 班次相关配置信息。
         self.shift_volist = shift_volist
         # 是否跳过节假日。
         # 
         # true：跳过（默认值）
         # 
@@ -5984,18 +5902,14 @@
             for k in self.members:
                 if k:
                     k.validate()
         if self.positions:
             for k in self.positions:
                 if k:
                     k.validate()
-        if self.resource_permission_map:
-            for k in self.resource_permission_map:
-                if k:
-                    k.validate()
         if self.shift_volist:
             for k in self.shift_volist:
                 if k:
                     k.validate()
         if self.wifis:
             for k in self.wifis:
                 if k:
@@ -6077,18 +5991,16 @@
             result['overtimeSettingId'] = self.overtime_setting_id
         if self.owner is not None:
             result['owner'] = self.owner
         result['positions'] = []
         if self.positions is not None:
             for k in self.positions:
                 result['positions'].append(k.to_map() if k else None)
-        result['resourcePermissionMap'] = []
         if self.resource_permission_map is not None:
-            for k in self.resource_permission_map:
-                result['resourcePermissionMap'].append(k.to_map() if k else None)
+            result['resourcePermissionMap'] = self.resource_permission_map
         result['shiftVOList'] = []
         if self.shift_volist is not None:
             for k in self.shift_volist:
                 result['shiftVOList'].append(k.to_map() if k else None)
         if self.skip_holidays is not None:
             result['skipHolidays'] = self.skip_holidays
         if self.special_days is not None:
@@ -6183,19 +6095,16 @@
         if m.get('owner') is not None:
             self.owner = m.get('owner')
         self.positions = []
         if m.get('positions') is not None:
             for k in m.get('positions'):
                 temp_model = GroupAddRequestPositions()
                 self.positions.append(temp_model.from_map(k))
-        self.resource_permission_map = []
         if m.get('resourcePermissionMap') is not None:
-            for k in m.get('resourcePermissionMap'):
-                temp_model = GroupAddRequestResourcePermissionMap()
-                self.resource_permission_map.append(temp_model.from_map(k))
+            self.resource_permission_map = m.get('resourcePermissionMap')
         self.shift_volist = []
         if m.get('shiftVOList') is not None:
             for k in m.get('shiftVOList'):
                 temp_model = GroupAddRequestShiftVOList()
                 self.shift_volist.append(temp_model.from_map(k))
         if m.get('skipHolidays') is not None:
             self.skip_holidays = m.get('skipHolidays')
@@ -6481,91 +6390,14 @@
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class GroupUpdateRequestResourcePermissionMap(TeaModel):
-    def __init__(
-        self,
-        camera_check: str = None,
-        check_position_type: str = None,
-        check_time: str = None,
-        group_member: str = None,
-        group_type: str = None,
-        out_side_check: str = None,
-        over_time_rule: str = None,
-        schedule: str = None,
-    ):
-        # 设置拍照打卡规则。
-        self.camera_check = camera_check
-        # 设置打卡方式。
-        self.check_position_type = check_position_type
-        # 设置考勤时间。
-        self.check_time = check_time
-        # 设置参与考勤人员。
-        self.group_member = group_member
-        # 设置考勤类型。
-        self.group_type = group_type
-        # 设置外勤打卡。
-        self.out_side_check = out_side_check
-        # 设置加班规则。
-        self.over_time_rule = over_time_rule
-        # 员工排班。
-        self.schedule = schedule
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.camera_check is not None:
-            result['cameraCheck'] = self.camera_check
-        if self.check_position_type is not None:
-            result['checkPositionType'] = self.check_position_type
-        if self.check_time is not None:
-            result['checkTime'] = self.check_time
-        if self.group_member is not None:
-            result['groupMember'] = self.group_member
-        if self.group_type is not None:
-            result['groupType'] = self.group_type
-        if self.out_side_check is not None:
-            result['outSideCheck'] = self.out_side_check
-        if self.over_time_rule is not None:
-            result['overTimeRule'] = self.over_time_rule
-        if self.schedule is not None:
-            result['schedule'] = self.schedule
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('cameraCheck') is not None:
-            self.camera_check = m.get('cameraCheck')
-        if m.get('checkPositionType') is not None:
-            self.check_position_type = m.get('checkPositionType')
-        if m.get('checkTime') is not None:
-            self.check_time = m.get('checkTime')
-        if m.get('groupMember') is not None:
-            self.group_member = m.get('groupMember')
-        if m.get('groupType') is not None:
-            self.group_type = m.get('groupType')
-        if m.get('outSideCheck') is not None:
-            self.out_side_check = m.get('outSideCheck')
-        if m.get('overTimeRule') is not None:
-            self.over_time_rule = m.get('overTimeRule')
-        if m.get('schedule') is not None:
-            self.schedule = m.get('schedule')
-        return self
-
-
 class GroupUpdateRequestShiftVOList(TeaModel):
     def __init__(
         self,
         shift_id: int = None,
     ):
         # 班次ID，可通过获取班次摘要信息接口获取。
         self.shift_id = shift_id
@@ -6613,15 +6445,15 @@
         manager_list: List[str] = None,
         offset: int = None,
         open_face_check: bool = None,
         outside_check_approve_mode_id: int = None,
         overtime_setting_id: int = None,
         owner: str = None,
         positions: List[GroupUpdateRequestPositions] = None,
-        resource_permission_map: List[GroupUpdateRequestResourcePermissionMap] = None,
+        resource_permission_map: Dict[str, Any] = None,
         shift_volist: List[GroupUpdateRequestShiftVOList] = None,
         skip_holidays: bool = None,
         trim_distance: int = None,
         workday_class_list: List[int] = None,
         op_user_id: str = None,
     ):
         # 补卡规则settingId。
@@ -6668,15 +6500,14 @@
         self.outside_check_approve_mode_id = outside_check_approve_mode_id
         # 加班规则settingId。
         self.overtime_setting_id = overtime_setting_id
         # 考勤组负责人。
         self.owner = owner
         # 考勤地点相关设置信息。
         self.positions = positions
-        # 子管理员权限范围。w：可管理r：可读
         self.resource_permission_map = resource_permission_map
         # 班次相关配置信息。
         self.shift_volist = shift_volist
         # 是否跳过节假日。true：跳过（默认值）false：不跳过
         self.skip_holidays = skip_holidays
         # 地点微调范围（单位米）。
         self.trim_distance = trim_distance
@@ -6688,18 +6519,14 @@
     def validate(self):
         if self.free_check_setting:
             self.free_check_setting.validate()
         if self.positions:
             for k in self.positions:
                 if k:
                     k.validate()
-        if self.resource_permission_map:
-            for k in self.resource_permission_map:
-                if k:
-                    k.validate()
         if self.shift_volist:
             for k in self.shift_volist:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -6753,18 +6580,16 @@
             result['overtimeSettingId'] = self.overtime_setting_id
         if self.owner is not None:
             result['owner'] = self.owner
         result['positions'] = []
         if self.positions is not None:
             for k in self.positions:
                 result['positions'].append(k.to_map() if k else None)
-        result['resourcePermissionMap'] = []
         if self.resource_permission_map is not None:
-            for k in self.resource_permission_map:
-                result['resourcePermissionMap'].append(k.to_map() if k else None)
+            result['resourcePermissionMap'] = self.resource_permission_map
         result['shiftVOList'] = []
         if self.shift_volist is not None:
             for k in self.shift_volist:
                 result['shiftVOList'].append(k.to_map() if k else None)
         if self.skip_holidays is not None:
             result['skipHolidays'] = self.skip_holidays
         if self.trim_distance is not None:
@@ -6825,19 +6650,16 @@
         if m.get('owner') is not None:
             self.owner = m.get('owner')
         self.positions = []
         if m.get('positions') is not None:
             for k in m.get('positions'):
                 temp_model = GroupUpdateRequestPositions()
                 self.positions.append(temp_model.from_map(k))
-        self.resource_permission_map = []
         if m.get('resourcePermissionMap') is not None:
-            for k in m.get('resourcePermissionMap'):
-                temp_model = GroupUpdateRequestResourcePermissionMap()
-                self.resource_permission_map.append(temp_model.from_map(k))
+            self.resource_permission_map = m.get('resourcePermissionMap')
         self.shift_volist = []
         if m.get('shiftVOList') is not None:
             for k in m.get('shiftVOList'):
                 temp_model = GroupUpdateRequestShiftVOList()
                 self.shift_volist.append(temp_model.from_map(k))
         if m.get('skipHolidays') is not None:
             self.skip_holidays = m.get('skipHolidays')
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2395,14 +2395,86 @@
             body=OpenApiUtilClient.parse_to_map(body)
         )
         return TeaCore.from_map(
             dingtalkexclusive__1__0_models.GetOaOperatorLogListResponse(),
             await self.do_roarequest_async('GetOaOperatorLogList', 'exclusive_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/exclusive/oaOperatorLogs/query', 'json', req, runtime)
         )
 
+    def get_outside_audit_group_message_by_page(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageRequest,
+    ) -> dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageHeaders()
+        return self.get_outside_audit_group_message_by_page_with_options(request, headers, runtime)
+
+    async def get_outside_audit_group_message_by_page_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageRequest,
+    ) -> dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageHeaders()
+        return await self.get_outside_audit_group_message_by_page_with_options_async(request, headers, runtime)
+
+    def get_outside_audit_group_message_by_page_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageRequest,
+        headers: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse(),
+            self.do_roarequest('GetOutsideAuditGroupMessageByPage', 'exclusive_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/exclusive/audits/outsideGroups/messages/query', 'json', req, runtime)
+        )
+
+    async def get_outside_audit_group_message_by_page_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageRequest,
+        headers: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse(),
+            await self.do_roarequest_async('GetOutsideAuditGroupMessageByPage', 'exclusive_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/exclusive/audits/outsideGroups/messages/query', 'json', req, runtime)
+        )
+
     def get_partner_type_by_parent_id(
         self,
         parent_id: str,
     ) -> dingtalkexclusive__1__0_models.GetPartnerTypeByParentIdResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.GetPartnerTypeByParentIdHeaders()
         return self.get_partner_type_by_parent_id_with_options(parent_id, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6130,14 +6130,299 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetOaOperatorLogListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetOutsideAuditGroupMessageByPageHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: int = None,
+        open_conversation_id: str = None,
+    ):
+        # 页大小，一次请求几条消息，合法区间[20,50]
+        self.max_results = max_results
+        # 毫秒时间戳，从该时间向过去拉消息
+        self.next_token = next_token
+        # 会话
+        self.open_conversation_id = open_conversation_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageListSender(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+        id_type: str = None,
+        type: str = None,
+    ):
+        # 根据id的类型决定是哪一种id
+        self.id = id
+        # 发送者的id类型，可以是userId或者unionId
+        self.id_type = id_type
+        # 用户-user 机器人-bot 系统账号-sys
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.id_type is not None:
+            result['idType'] = self.id_type
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('idType') is not None:
+            self.id_type = m.get('idType')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageList(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        content_type: str = None,
+        create_at: str = None,
+        open_conversation_id: str = None,
+        sender: GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageListSender = None,
+    ):
+        # 内容
+        self.content = content
+        # 内容类型 文本/语音/视频
+        self.content_type = content_type
+        # 发送时间 格式:yyyy-MM-dd HH:mm:ss
+        self.create_at = create_at
+        # 会话id
+        self.open_conversation_id = open_conversation_id
+        # 发送人
+        self.sender = sender
+
+    def validate(self):
+        if self.sender:
+            self.sender.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['content'] = self.content
+        if self.content_type is not None:
+            result['contentType'] = self.content_type
+        if self.create_at is not None:
+            result['createAt'] = self.create_at
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.sender is not None:
+            result['sender'] = self.sender.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('contentType') is not None:
+            self.content_type = m.get('contentType')
+        if m.get('createAt') is not None:
+            self.create_at = m.get('createAt')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('sender') is not None:
+            temp_model = GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageListSender()
+            self.sender = temp_model.from_map(m['sender'])
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageResponseBodyResponseBody(TeaModel):
+    def __init__(
+        self,
+        message_list: List[GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageList] = None,
+        next_token: str = None,
+    ):
+        # 消息列表
+        self.message_list = message_list
+        # 下一次请求的token,无返回值则下一条消息不存在
+        self.next_token = next_token
+
+    def validate(self):
+        if self.message_list:
+            for k in self.message_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['messageList'] = []
+        if self.message_list is not None:
+            for k in self.message_list:
+                result['messageList'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.message_list = []
+        if m.get('messageList') is not None:
+            for k in m.get('messageList'):
+                temp_model = GetOutsideAuditGroupMessageByPageResponseBodyResponseBodyMessageList()
+                self.message_list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageResponseBody(TeaModel):
+    def __init__(
+        self,
+        response_body: GetOutsideAuditGroupMessageByPageResponseBodyResponseBody = None,
+    ):
+        # 返回结构体
+        self.response_body = response_body
+
+    def validate(self):
+        if self.response_body:
+            self.response_body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.response_body is not None:
+            result['responseBody'] = self.response_body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('responseBody') is not None:
+            temp_model = GetOutsideAuditGroupMessageByPageResponseBodyResponseBody()
+            self.response_body = temp_model.from_map(m['responseBody'])
+        return self
+
+
+class GetOutsideAuditGroupMessageByPageResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetOutsideAuditGroupMessageByPageResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetOutsideAuditGroupMessageByPageResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetPartnerTypeByParentIdHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8151,14 +8151,310 @@
             query=OpenApiUtilClient.query(query)
         )
         return TeaCore.from_map(
             dingtalkindustry__1__0_models.SaveUserExtendValuesResponse(),
             await self.do_roarequest_async('SaveUserExtendValues', 'industry_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/industry/medicals/users/{user_id}/extends', 'json', req, runtime)
         )
 
+    def supply_add_dept(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddDeptHeaders()
+        return self.supply_add_dept_with_options(request, headers, runtime)
+
+    async def supply_add_dept_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddDeptHeaders()
+        return await self.supply_add_dept_with_options_async(request, headers, runtime)
+
+    def supply_add_dept_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_name):
+            query['deptName'] = request.dept_name
+        if not UtilClient.is_unset(request.partner_number):
+            query['partnerNumber'] = request.partner_number
+        if not UtilClient.is_unset(request.super_dept_id):
+            query['superDeptId'] = request.super_dept_id
+        if not UtilClient.is_unset(request.supply_dept_type):
+            query['supplyDeptType'] = request.supply_dept_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddDeptResponse(),
+            self.do_roarequest('SupplyAddDept', 'industry_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/industry/supplyChains/departments', 'json', req, runtime)
+        )
+
+    async def supply_add_dept_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_name):
+            query['deptName'] = request.dept_name
+        if not UtilClient.is_unset(request.partner_number):
+            query['partnerNumber'] = request.partner_number
+        if not UtilClient.is_unset(request.super_dept_id):
+            query['superDeptId'] = request.super_dept_id
+        if not UtilClient.is_unset(request.supply_dept_type):
+            query['supplyDeptType'] = request.supply_dept_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddDeptResponse(),
+            await self.do_roarequest_async('SupplyAddDept', 'industry_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/industry/supplyChains/departments', 'json', req, runtime)
+        )
+
+    def supply_add_member(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddMemberHeaders()
+        return self.supply_add_member_with_options(request, headers, runtime)
+
+    async def supply_add_member_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddMemberHeaders()
+        return await self.supply_add_member_with_options_async(request, headers, runtime)
+
+    def supply_add_member_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_partner_manager):
+            query['isPartnerManager'] = request.is_partner_manager
+        if not UtilClient.is_unset(request.member_mobile):
+            query['memberMobile'] = request.member_mobile
+        if not UtilClient.is_unset(request.member_name):
+            query['memberName'] = request.member_name
+        if not UtilClient.is_unset(request.member_work_number):
+            query['memberWorkNumber'] = request.member_work_number
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddMemberResponse(),
+            self.do_roarequest('SupplyAddMember', 'industry_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/industry/supplyChains/members', 'json', req, runtime)
+        )
+
+    async def supply_add_member_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_partner_manager):
+            query['isPartnerManager'] = request.is_partner_manager
+        if not UtilClient.is_unset(request.member_mobile):
+            query['memberMobile'] = request.member_mobile
+        if not UtilClient.is_unset(request.member_name):
+            query['memberName'] = request.member_name
+        if not UtilClient.is_unset(request.member_work_number):
+            query['memberWorkNumber'] = request.member_work_number
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddMemberResponse(),
+            await self.do_roarequest_async('SupplyAddMember', 'industry_1.0', 'HTTP', 'POST', 'AK', f'/v1.0/industry/supplyChains/members', 'json', req, runtime)
+        )
+
+    def supply_get_member(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyGetMemberHeaders()
+        return self.supply_get_member_with_options(request, headers, runtime)
+
+    async def supply_get_member_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyGetMemberHeaders()
+        return await self.supply_get_member_with_options_async(request, headers, runtime)
+
+    def supply_get_member_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyGetMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyGetMemberResponse(),
+            self.do_roarequest('SupplyGetMember', 'industry_1.0', 'HTTP', 'GET', 'AK', f'/v1.0/industry/supplyChains/members', 'json', req, runtime)
+        )
+
+    async def supply_get_member_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyGetMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyGetMemberResponse(),
+            await self.do_roarequest_async('SupplyGetMember', 'industry_1.0', 'HTTP', 'GET', 'AK', f'/v1.0/industry/supplyChains/members', 'json', req, runtime)
+        )
+
+    def supply_list_dept_members(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListDeptMembersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListDeptMembersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListDeptMembersHeaders()
+        return self.supply_list_dept_members_with_options(request, headers, runtime)
+
+    async def supply_list_dept_members_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListDeptMembersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListDeptMembersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListDeptMembersHeaders()
+        return await self.supply_list_dept_members_with_options_async(request, headers, runtime)
+
+    def supply_list_dept_members_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListDeptMembersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListDeptMembersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListDeptMembersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListDeptMembersResponse(),
+            self.do_roarequest('SupplyListDeptMembers', 'industry_1.0', 'HTTP', 'GET', 'AK', f'/v1.0/industry/supplyChains/departments/members', 'json', req, runtime)
+        )
+
+    async def supply_list_dept_members_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListDeptMembersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListDeptMembersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListDeptMembersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListDeptMembersResponse(),
+            await self.do_roarequest_async('SupplyListDeptMembers', 'industry_1.0', 'HTTP', 'GET', 'AK', f'/v1.0/industry/supplyChains/departments/members', 'json', req, runtime)
+        )
+
     def update_user_extend_info(
         self,
         user_id: str,
         request: dingtalkindustry__1__0_models.UpdateUserExtendInfoRequest,
     ) -> dingtalkindustry__1__0_models.UpdateUserExtendInfoResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.UpdateUserExtendInfoHeaders()
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10036,19 +10036,21 @@
             self.node_id = m.get('nodeId')
         return self
 
 
 class DigitalStoreSubNodesResponseBodyContent(TeaModel):
     def __init__(
         self,
+        ding_dept_id: int = None,
         id: int = None,
         name: str = None,
         parent_id: int = None,
         type: int = None,
     ):
+        self.ding_dept_id = ding_dept_id
         # 节点Id
         self.id = id
         # 门店名称
         self.name = name
         # 上级节点id
         self.parent_id = parent_id
         # 节点类型
@@ -10059,26 +10061,30 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.ding_dept_id is not None:
+            result['dingDeptId'] = self.ding_dept_id
         if self.id is not None:
             result['id'] = self.id
         if self.name is not None:
             result['name'] = self.name
         if self.parent_id is not None:
             result['parentId'] = self.parent_id
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('dingDeptId') is not None:
+            self.ding_dept_id = m.get('dingDeptId')
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('parentId') is not None:
             self.parent_id = m.get('parentId')
         if m.get('type') is not None:
@@ -22608,14 +22614,787 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = SaveUserExtendValuesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SupplyAddDeptHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyAddDeptRequest(TeaModel):
+    def __init__(
+        self,
+        dept_name: str = None,
+        partner_number: str = None,
+        super_dept_id: int = None,
+        supply_dept_type: str = None,
+    ):
+        # 部门名字
+        self.dept_name = dept_name
+        # 供应商编号
+        self.partner_number = partner_number
+        # 上级部门id
+        self.super_dept_id = super_dept_id
+        # 供应链部门类型
+        self.supply_dept_type = supply_dept_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_name is not None:
+            result['deptName'] = self.dept_name
+        if self.partner_number is not None:
+            result['partnerNumber'] = self.partner_number
+        if self.super_dept_id is not None:
+            result['superDeptId'] = self.super_dept_id
+        if self.supply_dept_type is not None:
+            result['supplyDeptType'] = self.supply_dept_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptName') is not None:
+            self.dept_name = m.get('deptName')
+        if m.get('partnerNumber') is not None:
+            self.partner_number = m.get('partnerNumber')
+        if m.get('superDeptId') is not None:
+            self.super_dept_id = m.get('superDeptId')
+        if m.get('supplyDeptType') is not None:
+            self.supply_dept_type = m.get('supplyDeptType')
+        return self
+
+
+class SupplyAddDeptResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+    ):
+        # 部门id
+        self.dept_id = dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        return self
+
+
+class SupplyAddDeptResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SupplyAddDeptResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SupplyAddDeptResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SupplyAddDeptResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: SupplyAddDeptResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = SupplyAddDeptResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyAddMemberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyAddMemberRequest(TeaModel):
+    def __init__(
+        self,
+        is_partner_manager: bool = None,
+        member_mobile: str = None,
+        member_name: str = None,
+        member_work_number: str = None,
+        supply_dept_id: int = None,
+    ):
+        # 是否为伙伴负责人
+        self.is_partner_manager = is_partner_manager
+        # 成员手机号
+        self.member_mobile = member_mobile
+        # 成员名字
+        self.member_name = member_name
+        # 成员编码/工号
+        self.member_work_number = member_work_number
+        # 所属伙伴/子部门
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_partner_manager is not None:
+            result['isPartnerManager'] = self.is_partner_manager
+        if self.member_mobile is not None:
+            result['memberMobile'] = self.member_mobile
+        if self.member_name is not None:
+            result['memberName'] = self.member_name
+        if self.member_work_number is not None:
+            result['memberWorkNumber'] = self.member_work_number
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('isPartnerManager') is not None:
+            self.is_partner_manager = m.get('isPartnerManager')
+        if m.get('memberMobile') is not None:
+            self.member_mobile = m.get('memberMobile')
+        if m.get('memberName') is not None:
+            self.member_name = m.get('memberName')
+        if m.get('memberWorkNumber') is not None:
+            self.member_work_number = m.get('memberWorkNumber')
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyAddMemberResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        ding_member_status: str = None,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        # 成员在钉钉组织的状态
+        self.ding_member_status = ding_member_status
+        # isv内用户唯一id
+        self.union_id = union_id
+        # 已经进组织的用户唯一id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ding_member_status is not None:
+            result['dingMemberStatus'] = self.ding_member_status
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dingMemberStatus') is not None:
+            self.ding_member_status = m.get('dingMemberStatus')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyAddMemberResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SupplyAddMemberResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SupplyAddMemberResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SupplyAddMemberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: SupplyAddMemberResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = SupplyAddMemberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyGetMemberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyGetMemberRequest(TeaModel):
+    def __init__(
+        self,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        # isv下钉钉唯一账号ID
+        self.union_id = union_id
+        # 组织内钉钉员工ID
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyGetMemberResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        ding_member_status: str = None,
+        is_active: bool = None,
+        member_name: str = None,
+        member_work_number: str = None,
+    ):
+        # 成员状态，已进组织或者待接收邀请
+        self.ding_member_status = ding_member_status
+        # 成员是否激活
+        self.is_active = is_active
+        # 成员名字
+        self.member_name = member_name
+        # 成员在上下游中的工号
+        self.member_work_number = member_work_number
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ding_member_status is not None:
+            result['dingMemberStatus'] = self.ding_member_status
+        if self.is_active is not None:
+            result['isActive'] = self.is_active
+        if self.member_name is not None:
+            result['memberName'] = self.member_name
+        if self.member_work_number is not None:
+            result['memberWorkNumber'] = self.member_work_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dingMemberStatus') is not None:
+            self.ding_member_status = m.get('dingMemberStatus')
+        if m.get('isActive') is not None:
+            self.is_active = m.get('isActive')
+        if m.get('memberName') is not None:
+            self.member_name = m.get('memberName')
+        if m.get('memberWorkNumber') is not None:
+            self.member_work_number = m.get('memberWorkNumber')
+        return self
+
+
+class SupplyGetMemberResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SupplyGetMemberResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SupplyGetMemberResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SupplyGetMemberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: SupplyGetMemberResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = SupplyGetMemberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyListDeptMembersHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListDeptMembersRequest(TeaModel):
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+        supply_dept_id: int = None,
+    ):
+        # 页码
+        self.page_number = page_number
+        # 单页的条目数
+        self.page_size = page_size
+        # 供应链部门id
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyListDeptMembersResponseBodyList(TeaModel):
+    def __init__(
+        self,
+        ding_member_status: str = None,
+        is_active: bool = None,
+        member_name: str = None,
+        member_work_number: str = None,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        # 人员状态，已进组织 或 待接收邀请
+        self.ding_member_status = ding_member_status
+        # 是否激活
+        self.is_active = is_active
+        # 名字
+        self.member_name = member_name
+        # 人员在上下游中的工号
+        self.member_work_number = member_work_number
+        # 应用层面的唯一id
+        self.union_id = union_id
+        # 人员组织内id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ding_member_status is not None:
+            result['dingMemberStatus'] = self.ding_member_status
+        if self.is_active is not None:
+            result['isActive'] = self.is_active
+        if self.member_name is not None:
+            result['memberName'] = self.member_name
+        if self.member_work_number is not None:
+            result['memberWorkNumber'] = self.member_work_number
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dingMemberStatus') is not None:
+            self.ding_member_status = m.get('dingMemberStatus')
+        if m.get('isActive') is not None:
+            self.is_active = m.get('isActive')
+        if m.get('memberName') is not None:
+            self.member_name = m.get('memberName')
+        if m.get('memberWorkNumber') is not None:
+            self.member_work_number = m.get('memberWorkNumber')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyListDeptMembersResponseBody(TeaModel):
+    def __init__(
+        self,
+        has_more: bool = None,
+        list: List[SupplyListDeptMembersResponseBodyList] = None,
+    ):
+        # 是否还有下一页
+        self.has_more = has_more
+        self.list = list
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = SupplyListDeptMembersResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListDeptMembersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: SupplyListDeptMembersResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = SupplyListDeptMembersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateUserExtendInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 1.5.62
+Version: 1.5.63
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.62/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.62/setup.py` & `alibabacloud_dingtalk-1.5.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 07/04/2023
+Created on 11/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

