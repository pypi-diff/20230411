# Comparing `tmp/cloud-governance-1.1.86.tar.gz` & `tmp/cloud-governance-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-governance-1.1.86.tar", last modified: Tue Apr 11 14:35:16 2023, max compression
+gzip compressed data, was "cloud-governance-1.1.9.tar", last modified: Thu Oct 13 17:22:12 2022, max compression
```

## Comparing `cloud-governance-1.1.86.tar` & `cloud-governance-1.1.9.tar`

### file list

```diff
@@ -1,219 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.626390 cloud-governance-1.1.86/cloud_governance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.626390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/common/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.630390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cost_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/price/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/aws/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.634390 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/cost_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/gcp/google_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/classic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/google_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/google_drive/google_drive_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.638390 cloud-governance-1.1.86/cloud_governance/common/jira/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/jira/jira_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/common/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/ldap/ldap_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/common/mails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/mails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/mails/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/mails/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/mails/postfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/common/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/common/tool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/main/environment_variables_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/main/es_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/main/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.642390 cloud-governance-1.1.86/cloud_governance/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.646390 cloud-governance-1.1.86/cloud_governance/policy/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/cost_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ebs_in_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ebs_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ec2_idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ec2_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ec2_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/empty_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/ip_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/monthly_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/s3_inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/skipped_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/aws/zombie_snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.646390 cloud-governance-1.1.86/cloud_governance/policy/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/azure/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.646390 cloud-governance-1.1.86/cloud_governance/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/tag_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/ibm/tag_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.650390 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    41468 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.654389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.654389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.654389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gitleaks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:16.626390 cloud-governance-1.1.86/cloud_governance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 14:35:16.000000 cloud-governance-1.1.86/cloud_governance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 14:35:16.658389 cloud-governance-1.1.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-11 14:35:01.000000 cloud-governance-1.1.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.724618 cloud-governance-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14313 2022-10-13 17:22:12.724618 cloud-governance-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13664 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.676617 cloud-governance-1.1.9/cloud_governance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.680617 cloud-governance-1.1.9/cloud_governance/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.680617 cloud-governance-1.1.9/cloud_governance/aws/cost_expenditure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/cost_expenditure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/cost_expenditure/cost_report_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.684617 cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.684617 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25550 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/remove_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5065 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/tag_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41698 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/tag_cluster_resouces.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.688617 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7267 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/non_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8337 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11430 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6139 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/update_na_tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.692617 cloud-governance-1.1.9/cloud_governance/aws/tag_user/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_user/iam_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_user/remove_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_user/run_tag_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10235 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/tag_user/tag_iam_user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.696617 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26104 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_ec2_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_iam_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_s3_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9089 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/validate_zombies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12772 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.696617 cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12134 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.696617 cloud-governance-1.1.9/cloud_governance/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.696617 cloud-governance-1.1.9/cloud_governance/common/clouds/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.696617 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.700618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12182 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.700618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.700618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.700618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.704618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17235 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.704618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/iam/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.704618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/price/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/price/price.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.708618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10510 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.708618 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/aws/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.708618 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.708618 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/account/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.708618 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/classic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.712618 cloud-governance-1.1.9/cloud_governance/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20927 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.712618 cloud-governance-1.1.9/cloud_governance/common/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/google_drive/google_drive_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.712618 cloud-governance-1.1.9/cloud_governance/common/ldap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/ldap/ldap_search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.716618 cloud-governance-1.1.9/cloud_governance/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.716618 cloud-governance-1.1.9/cloud_governance/common/mails/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/mails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/mails/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6389 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/mails/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4441 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/mails/postfix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/common/tool/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/common/tool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/gitleaks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/gitleaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/gitleaks/gitleaks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/ibm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/ibm/ibm_operations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/ibm_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/ibm_operations/ibm_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/ibm_operations/tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/ibm/tagging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/ibm/tagging/tagging_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/main/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/main/es_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15900 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/main/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.720618 cloud-governance-1.1.9/cloud_governance/policy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.724618 cloud-governance-1.1.9/cloud_governance/policy/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/cost_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4778 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/ebs_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8929 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/ec2_idle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/ec2_stop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/empty_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/empty_roles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50664 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_elastic_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.724618 cloud-governance-1.1.9/cloud_governance/policy/ibm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/cloud_governance/policy/ibm/tag_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:22:12.680617 cloud-governance-1.1.9/cloud_governance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14313 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-13 17:22:12.000000 cloud-governance-1.1.9/cloud_governance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-13 17:22:12.724618 cloud-governance-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-10-13 17:21:53.000000 cloud-governance-1.1.9/setup.py
```

### Comparing `cloud-governance-1.1.86/LICENSE` & `cloud-governance-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/PKG-INFO` & `cloud-governance-1.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.86
+Version: 1.1.9
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cloud-governance.svg)](https://pypi.org/project/cloud-governance/)
 [![Container Repository on Quay](https://quay.io/repository/projectquay/quay/status "Container Repository on Quay")](https://quay.io/repository/ebattat/cloud-governance?tab=tags)
 [![Actions Status](https://github.com/redhat-performance/cloud-governance/workflows/Build/badge.svg)](https://github.com/redhat-performance/cloud-governance/actions)
@@ -36,28 +36,23 @@
 
 This tool support the following policies:
 [policy](cloud_governance/policy)
 
 [AWS Polices](cloud_governance/policy/aws)
 
 * Real time Openshift Cluster cost, User cost
-* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 4 days, cpu < 2% & network < 5mb.
-* [ec2_run](cloud_governance/policy/aws/ec2_run.py): running ec2.
-* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.py): volumes that did not connect to instance, volume in available status.
-* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.py): in use volumes.
-* [tag_resources](cloud_governance/policy/policy_operations/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
+* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 2 days, cpu < 2% & network < 5mb [ec2_idle](cloud_governance/policy/aws/ec2_idle.py)
+* [ec2_run](cloud_governance/policy/aws/ec2_run.yml): running ec2 [ec2_run](cloud_governance/policy/aws/ec2_run.yml)
+* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml): volumes that did not connect to instance, volume in available status [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml)
+* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml): in use volumes [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml)
+* [tag_resources](cloud_governance/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
 * [zombie_cluster_resource](cloud_governance/policy/aws/zombie_cluster_resource.py): Delete cluster's zombie resources
-* [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
-* [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
+* [tag_non_cluster](cloud_governance/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
+* [tag_iam_user](cloud_governance/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
-* [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
-* [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
-* [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
-* [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
@@ -137,29 +132,29 @@
 GOOGLE_APPLICATION_CREDENTIALS=$pwd/service_account.json
 
 # Configuration
 
 ### AWS Configuration
 
 #### Create a user and a bucket
-* Create user with IAM [iam](iam/clouds)
-* Create a logs bucket [create_bucket.sh](iam/cloud/aws/create_bucket.sh)
+* Create user with IAM [iam](iam)
+* Create a logs bucket [create_bucket.sh](iam/create_bucket.sh)
 
 ### IBM Configuration
 * Create classic infrastructure API key
 
 ## Run AWS Policy Using Podman 
 ```sh
 # policy=ec2_idle
 sudo podman run --rm --name cloud-governance -e policy="ec2_idle" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ec2_run
 sudo podman run --rm --name cloud-governance -e policy="ec2_run" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
-# select policy ['ec2_stop', 's3_inactive', 'empty_roles', 'ip_unattached', 'nat_gateway_unused', 'zombie_snapshots']
+# select policy ['ec2_stop', 'empty_buckets', 'empty_roles', 'zombie_elastic_ips', 'zombie_nat_gateways', 'zombie_snapshots']
 sudo podman run --rm --name cloud-governance -e policy="policy" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes"  -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_unattached
 sudo podman run --rm --name cloud-governance -e policy="ebs_unattached" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_in_use
 sudo podman run --rm --name cloud-governance -e policy="ebs_in_use" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
@@ -234,7 +229,9 @@
 
 ## Post Installation
 
 #### Delete cloud-governance image
 ```sh
 sudo podman rmi quay.io/ebattat/cloud-governance
 ```
+
+
```

### Comparing `cloud-governance-1.1.86/README.md` & `cloud-governance-1.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,23 @@
 
 This tool support the following policies:
 [policy](cloud_governance/policy)
 
 [AWS Polices](cloud_governance/policy/aws)
 
 * Real time Openshift Cluster cost, User cost
-* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 4 days, cpu < 2% & network < 5mb.
-* [ec2_run](cloud_governance/policy/aws/ec2_run.py): running ec2.
-* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.py): volumes that did not connect to instance, volume in available status.
-* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.py): in use volumes.
-* [tag_resources](cloud_governance/policy/policy_operations/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
+* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 2 days, cpu < 2% & network < 5mb [ec2_idle](cloud_governance/policy/aws/ec2_idle.py)
+* [ec2_run](cloud_governance/policy/aws/ec2_run.yml): running ec2 [ec2_run](cloud_governance/policy/aws/ec2_run.yml)
+* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml): volumes that did not connect to instance, volume in available status [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml)
+* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml): in use volumes [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml)
+* [tag_resources](cloud_governance/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
 * [zombie_cluster_resource](cloud_governance/policy/aws/zombie_cluster_resource.py): Delete cluster's zombie resources
-* [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
-* [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
+* [tag_non_cluster](cloud_governance/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
+* [tag_iam_user](cloud_governance/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
-* [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
-* [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
-* [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
-* [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
@@ -119,29 +114,29 @@
 GOOGLE_APPLICATION_CREDENTIALS=$pwd/service_account.json
 
 # Configuration
 
 ### AWS Configuration
 
 #### Create a user and a bucket
-* Create user with IAM [iam](iam/clouds)
-* Create a logs bucket [create_bucket.sh](iam/cloud/aws/create_bucket.sh)
+* Create user with IAM [iam](iam)
+* Create a logs bucket [create_bucket.sh](iam/create_bucket.sh)
 
 ### IBM Configuration
 * Create classic infrastructure API key
 
 ## Run AWS Policy Using Podman 
 ```sh
 # policy=ec2_idle
 sudo podman run --rm --name cloud-governance -e policy="ec2_idle" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ec2_run
 sudo podman run --rm --name cloud-governance -e policy="ec2_run" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
-# select policy ['ec2_stop', 's3_inactive', 'empty_roles', 'ip_unattached', 'nat_gateway_unused', 'zombie_snapshots']
+# select policy ['ec2_stop', 'empty_buckets', 'empty_roles', 'zombie_elastic_ips', 'zombie_nat_gateways', 'zombie_snapshots']
 sudo podman run --rm --name cloud-governance -e policy="policy" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes"  -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_unattached
 sudo podman run --rm --name cloud-governance -e policy="ebs_unattached" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_in_use
 sudo podman run --rm --name cloud-governance -e policy="ebs_in_use" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
```

### Comparing `cloud-governance-1.1.86/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/ec2_stop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,98 @@
 import datetime
+import operator
 
-import boto3
-
-from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
+from cloud_governance.common.clouds.aws.cloudtrail.cloudtrail_operations import CloudTrailOperations
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-
-from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
-from cloud_governance.common.jira.jira_operations import JiraOperations
-from cloud_governance.main.environment_variables import environment_variables
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from operator import ge
 
 
-class TagLongRun:
+class EC2Stop(NonClusterZombiePolicy):
     """
-    This class tag the long run days and tag extend the long run days
+    This class delete the stopped ec2 instance
+    Send mail to the user if the ec2 instance is stopped > 20, 25th days
+    Delete the instance when it stopped 30 days
     """
 
-    DEFAULT_SEARCH_TAG = 'JiraId'
-    KEY = 'Key'
-    VALUE = 'Value'
-
-    def __init__(self, region_name: str = ''):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.__region_name = region_name if region_name else self.__environment_variables_dict.get('AWS_DEFAULT_REGION')
-        self.__ec2_client = boto3.client('ec2', region_name=self.__region_name)
-        self.__ec2_operations = EC2Operations(region=self.__region_name)
-        self.jira_operations = JiraOperations()
-        self.__es_upload = ElasticUpload()
-        self.__jira_queue = self.__environment_variables_dict.get('JIRA_QUEUE')
-
-    @logger_time_stamp
-    def tag_extend_instances(self, sub_tasks: list, jira_id: str):
-        """This method extend the longrun days if the user opened the jira ticket"""
-        filters = {'Filters': [{'Name': 'tag:JiraId', 'Values': [jira_id]}]}
-        extend_long_run_days = 0
-        for task_id in sub_tasks:
-            description = self.jira_operations.get_issue_description(jira_id=task_id, sub_task=True)
-            extend_long_run_days += int(description.get('Days'))
-        instances = self.__ec2_operations.get_instances(**filters)
-        long_run_days = 0
-        instance_ids = []
-        for instance in instances:
-            for resource in instance['Instances']:
-                tags = resource.get('Tags')
-                if tags:
-                    long_run_days = int(self.__ec2_operations.get_tag_value_from_tags(tag_name='LongRunDays', tags=tags))
-                instance_ids.append(resource.get('InstanceId'))
-        if long_run_days > 0:
-            long_run_days += extend_long_run_days
-            tag = [{'Key': 'LongRunDays', 'Value': str(long_run_days)}]
-            self.__ec2_client.create_tags(Resources=instance_ids, Tags=tag)
-            data = {
-                'long_run_days': long_run_days,
-                'timestamp': datetime.datetime.utcnow()
-            }
-            if self.__es_upload.elastic_search_operations:
-                self.__es_upload.elastic_search_operations.update_elasticsearch_index(metadata=data, id=jira_id, index=self.__es_upload.es_index)
-            for task_id in sub_tasks:
-                self.jira_operations.move_issue_state(jira_id=task_id, state='closed')
-
-    @logger_time_stamp
-    def tag_jira_id_attach_instance(self, jira_id: str, instance_id: str, volume_ids: list):
-        """
-        This method tag the long run instance with tags
-        """
-        jira_description = self.jira_operations.get_issue_description(jira_id=jira_id, state=self.jira_operations.JIRA_TRANSITION_IDS.get('INPROGRESS'))
-        if jira_description:
-            if self.__jira_queue not in jira_id:
-                jira_id = f'{self.__jira_queue}-{jira_id}'
-            long_run_days = jira_description.get('Days')
-            manager_approved = jira_description.get('ApprovedManager')
-            if not manager_approved:
-                manager_approved = jira_description.get('ManagerApprovalAddress')
-            user_email = jira_description.get('EmailAddress')
-            user = user_email.split('@')[0]
-            project = jira_description.get('Project')
-            tags = [{self.KEY: 'LongRunDays', self.VALUE: long_run_days},
-                    {self.KEY: 'ApprovedManager', self.VALUE: manager_approved},
-                    {self.KEY: 'Project', self.VALUE: project.upper()},
-                    {self.KEY: 'Email', self.VALUE: user_email},
-                    {self.KEY: self.DEFAULT_SEARCH_TAG, self.VALUE: jira_id},
-                    {self.KEY: 'User', self.VALUE: user}]
-            self.__ec2_client.create_tags(Resources=[instance_id], Tags=tags)
-            self.jira_operations.move_issue_state(jira_id=jira_id, state='inprogress')
-            logger.info(f'Extra tags are added to the instances: {instance_id}, had an jira_id: {jira_id}')
-            if volume_ids:
-                self.__ec2_client.create_tags(Resources=volume_ids, Tags=tags)
-                logger.info(f'Tagged the instance: {instance_id} attached volumes {volume_ids}')
-            return True
-        return False
-
-    def __get_instance_volumes(self, block_device_mappings: list):
-        """This method returns the instance volumes"""
-        volumes_list = []
-        for mapping in block_device_mappings:
-            if mapping.get('Ebs').get('VolumeId'):
-                volumes_list.append(mapping.get('Ebs').get('VolumeId'))
-        return volumes_list
+    FIRST_MAIL_NOTIFICATION_INSTANCE_DAYS = 20
+    SECOND_MAIL_NOTIFICATION_INSTANCE_DAYS = 25
+    DELETE_INSTANCE_DAYS = 30
+
+    def __init__(self):
+        super().__init__()
+        self._cloudtrail = CloudTrailOperations(region_name=self._region)
 
-    @logger_time_stamp
-    def __find_tag_instances(self):
+    def run(self):
         """
-        This method list the instances and tagged the instances which have the tag IssueId
+        This method list all stopped instances for more than 30 days and terminate if dry_run no
+        @return:
         """
-        instances = self.__ec2_operations.get_instances()
-        jira_id_instances = {}
+        return self.__fetch_stop_instance(sign=ge, instance_days=self.FIRST_MAIL_NOTIFICATION_INSTANCE_DAYS, delete_instance_days=self.DELETE_INSTANCE_DAYS)
+
+    def __fetch_stop_instance(self, instance_days: int, delete_instance_days: int, sign: operator = ge):
+        """
+        This method list all stopped instances for more than 30 days and terminate if dry_run no
+        @return:
+        """
+        instances = self._ec2_client.describe_instances(Filters=[{'Name': 'instance-state-name', 'Values': ['stopped']}])['Reservations']
+        stopped_instances = []
+        stopped_instance_tags = {}
+        ec2_types = {}
+        stopped_time = ''
+        days = 0
         for instance in instances:
             for resource in instance['Instances']:
                 instance_id = resource.get('InstanceId')
-                jira_id = ''
-                if resource.get('Tags'):
-                    jira_id = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name=self.DEFAULT_SEARCH_TAG)
-                if jira_id:
-                    long_run_days = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name='LongRunDays')
-                    if not long_run_days:
-                        volume_ids = self.__get_instance_volumes(resource.get('BlockDeviceMappings'))
-                        if self.tag_jira_id_attach_instance(jira_id=jira_id, instance_id=instance_id, volume_ids=volume_ids):
-                            jira_id_instances.setdefault(jira_id, []).append(instance_id)
-        return jira_id_instances
-
-    def run(self):
-        """
-        This method run the tagging of long run
-        """
-        return self.__find_tag_instances()
+                stopped_time = self._cloudtrail.get_stop_time(resource_id=instance_id, event_name='StopInstances')
+                if not stopped_time:
+                    stopped_time = datetime.datetime.now()
+                days = self._calculate_days(create_date=stopped_time)
+                if days in (instance_days, self.SECOND_MAIL_NOTIFICATION_INSTANCE_DAYS):
+                    user = self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User')
+                    if user:
+                        self.__trigger_mail(tags=resource.get('Tags'), stopped_time=stopped_time, resource_id=instance_id, days=days, ec2_type=resource.get("InstanceType"), instance_id=instance_id)
+                    else:
+                        logger.info('User is missing')
+                if sign(days, instance_days):
+                    if days >= delete_instance_days:
+                        stopped_instance_tags[instance_id] = resource.get('Tags')
+                        ec2_types[instance_id] = resource.get('InstanceType')
+                    stopped_instances.append([resource.get('InstanceId'), self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Name'),
+                                              self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User'), str(resource.get('LaunchTime')),
+                                              self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Policy')
+                                              ])
+        if self._dry_run == "no":
+            for instance_id, tags in stopped_instance_tags.items():
+                if self._get_policy_value(tags=tags) not in ('NOTDELETE', 'SKIP'):
+                    tags.append({'Key': 'Policy', 'Value': 'backup'})
+                    tag_specifications = [{'ResourceType': 'image', 'Tags': tags}]
+                    if sign == ge:
+                        tag_specifications.append({'ResourceType': 'snapshot', 'Tags': tags})
+                    try:
+                        ami_id = self._ec2_client.create_image(InstanceId=instance_id, Name=self._get_tag_name_from_tags(tags=tags), TagSpecifications=tag_specifications)['ImageId']
+                        self.__trigger_mail(tags=tags, stopped_time=stopped_time, days=days, resource_id=instance_id, image_id=ami_id, ec2_type=ec2_types[instance_id], instance_id=instance_id)
+                        self._ec2_client.terminate_instances(InstanceIds=[instance_id])
+                        logger.info(f'Deleted the instance: {instance_id}')
+                    except Exception as err:
+                        logger.info(err)
+        return stopped_instances
+
+    def __trigger_mail(self, tags: list, stopped_time: str, resource_id: str, days: int, image_id: str = '', ec2_type: str = '', instance_id: str = ''):
+        """
+        This method send triggering mail
+        @param tags:
+        @param stopped_time:
+        @param resource_id:
+        @param days:
+        @return:
+        """
+        try:
+            special_user_mails = self._literal_eval(self._special_user_mails)
+            user, instance_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(tags=tags, tag_name='Name')
+            to = user if user not in special_user_mails else special_user_mails[user]
+            ldap_data = self._ldap.get_user_details(user_name=to)
+            cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com']
+            subject, body = self._mail_description.ec2_stop(name=ldap_data.get('displayName'), days=days, image_id=image_id, delete_instance_days=self.DELETE_INSTANCE_DAYS, instance_name=instance_name, resource_id=resource_id, stopped_time=stopped_time, ec2_type=ec2_type)
+            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=instance_id)
+        except Exception as err:
+            logger.info(err)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,49 +97,31 @@
                                     if username:
                                         return [username, assumed_event]
                                     return [role_username, event]
             return ['', '']
         except Exception as err:
             return ['', '']
 
-    def __ger_username_from_arn(self, resource_arn: str):
-        """
-        This method return the username from the userIdentity arn
-        """
-        events = self.__get_cloudtrail_responses(resource_arn=resource_arn, start_time=None, end_time=None)
-        for event in events:
-            for resource in event.get('Resources'):
-                if resource.get('ResourceType') == 'AWS::STS::AssumedRole':
-                    if resource.get('ResourceName') == resource_arn:
-                        username, assumed_event = self.__check_event_is_assumed_role(event.get('CloudTrailEvent'))
-                        if username:
-                            return [username, assumed_event]
-                        return [event.get('Username'), event]
-        return ['', '']
-
     def __check_event_is_assumed_role(self, cloudtrail_event: str):
         """
         This method checks if it assumed_role, if it is return the username and its event from role.
         @param cloudtrail_event:
         @return:
         """
         try:
             cloudtrail_event = json.loads(cloudtrail_event)
             if cloudtrail_event.get('userIdentity').get('type') == "AssumedRole":
                 role_name = cloudtrail_event.get('userIdentity').get('sessionContext').get('sessionIssuer').get('arn')
                 assumerole_username, event = self.__get_username_by_role(role_name, "CreateRole", "AWS::IAM::Role")
-                if not assumerole_username:
-                    arn = cloudtrail_event.get('userIdentity').get('arn')
-                    assumerole_username, event = self.__ger_username_from_arn(resource_arn=arn)
                 return [assumerole_username, event]
             return [False, '']
         except Exception as err:
             return [False, '']
 
-    def get_full_responses(self, **kwargs):
+    def __get_full_responses(self, **kwargs):
         """
         This method return all responses
         @param kwargs:
         @return:
         """
         responses = []
         response = self.__cloudtrail.lookup_events(**kwargs)
@@ -157,15 +139,15 @@
         @param start_time:
         @param end_time:
         @param resource_id:
         @param resource_type:
         @return:
         """
         try:
-            responses = self.get_full_responses(StartTime=start_time, EndTime=end_time, LookupAttributes=[{
+            responses = self.__get_full_responses(StartTime=start_time, EndTime=end_time, LookupAttributes=[{
                 'AttributeKey': event_type, 'AttributeValue': resource_type}])
             for event in responses:
                 if event.get('EventName') == resource_type:
                     if event.get('Resources'):
                         for resource in event.get('Resources'):
                             if resource.get('ResourceName') == resource_id:
                                 username, assumed_event = self.__check_event_is_assumed_role(event.get('CloudTrailEvent'))
@@ -259,16 +241,14 @@
         """
         try:
             events = self.__cloudtrail.lookup_events(StartTime=start_time, EndTime=end_time, LookupAttributes=[{
                 'AttributeKey': 'ResourceName', 'AttributeValue': resource_id
             }])['Events']
             if events:
                 events = sorted(events, key=lambda event: event['EventTime'], reverse=True)
-                while events[0].get('EventName') in ('CreateTags', 'DeleteTags'):
-                    events.pop(0)
                 if events[0].get('EventName') == event_name:
                     return events[0].get('EventTime')
                 if kwargs:
                     if len(events) == 1:
                         if events[0].get('EventName') == kwargs['optional_event_name'][0]:
                             return events[0].get('EventTime')
                     elif len(events) == 2:
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 
 import boto3
 import typeguard
 
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class EC2Operations:
     """
     This class is useful for writing EC2 Operations
     """
 
     def __init__(self, region: str = 'us-east-2'):
         """
         Initializing the AWS resources
         """
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.elb1_client = boto3.client('elb', region_name=region)
         self.elbv2_client = boto3.client('elbv2', region_name=region)
         self.ec2_client = boto3.client('ec2', region_name=region)
         self.get_full_list = Utils().get_details_resource_list
         self.utils = Utils(region=region)
 
     @logger_time_stamp
@@ -316,29 +314,29 @@
                         break
             if found:
                 cluster.append(resource)
             else:
                 non_cluster.append(resource)
         return [cluster, non_cluster]
 
-    def get_instances(self, **kwargs):
+    def get_instances(self):
         """
         This method returns all instances from the region
         @return:
         """
         return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_instances,
-                                                    input_tag='Reservations', check_tag='NextToken', **kwargs)
+                                                    input_tag='Reservations', check_tag='NextToken')
 
-    def get_volumes(self, **kwargs):
+    def get_volumes(self):
         """
         This method returns all volumes in the region
         @return:
         """
         return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_volumes, input_tag='Volumes',
-                                                    check_tag='NextToken', **kwargs)
+                                                    check_tag='NextToken')
 
     def get_images(self):
         """
         This method returns all images in the region
         @return:
         """
         return self.ec2_client.describe_images(Owners=['self'])['Images']
@@ -491,28 +489,16 @@
             instances = self.get_ec2_list(region_ec2_client.describe_instances()['Reservations'])
             for instance in instances:
                 user_data = {'InstanceId': instance.get('InstanceId'),
                              'Name': self.get_tag(name='Name', tags=instance.get('Tags')),
                              'InstanceType': instance.get('InstanceType'),
                              'LaunchTime': instance.get('LaunchTime').strftime('%Y/%m/%d %H:%M:%S'),
                              'Region': region.get('RegionName'),
-                             'Account': self.__environment_variables_dict.get('account', '').upper(),
+                             'Account': os.environ.get('account', '').upper(),
                              'State': instance.get('State')['Name']
                              }
                 user = self.get_tag(name='User', tags=instance.get('Tags'))
                 if user in users_list:
                     users_list[user].append(user_data)
                 else:
                     users_list[user] = [user_data]
         return users_list
-
-    def get_tag_value_from_tags(self, tags: list, tag_name: str) -> str:
-        """
-        This method return the tag value inputted by tag_name
-        """
-        if tags:
-            for tag in tags:
-                key = tag.get('Key').lower().replace("_", '').replace("-", '')
-                if key == tag_name.lower():
-                    return tag.get('Value')
-        return ''
-
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import datetime
 import gzip
 import json
 import os
-import tempfile
 import boto3
 import typeguard
 from botocore.exceptions import ClientError
 from os import listdir
 from os.path import isfile, join
 
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 
 
 class S3Operations:
     """ This class is responsible for S3 operations """
 
-    def __init__(self, region_name, report_file_name: str = "zombie_report.json",
-                 resource_file_name: str = "resources.json.gz", bucket: str = '', logs_bucket_key: str = ''):
+    def __init__(self, region_name,  report_file_name: str = "zombie_report.json", resource_file_name: str = "resources.json.gz"):
         #  @Todo ask AWS support regarding about this issue
         if region_name == 'eu-south-1':
             self.__s3_client = boto3.client('s3', region_name='us-east-1')
         else:
             self.__s3_client = boto3.client('s3', region_name=region_name)
         self.__region = region_name
         self.__report_file_name = report_file_name
         self.__resource_file_name = resource_file_name
         self.__report_file_full_path = os.path.join(os.path.dirname(__file__), self.__report_file_name)
         self.__resources_file_full_path = os.path.join(os.path.dirname(__file__), self.__resource_file_name)
-        if bucket and logs_bucket_key:
-            self.__bucket, self.__logs_bucket_key = bucket, logs_bucket_key
 
     @logger_time_stamp
     @typeguard.typechecked
     def upload_file(self, file_name_path: str, bucket: str, key: str, upload_file: str):
         """
         This method upload file to s3
         STANDARD_IA , ONEZONE_IA , INTELLIGENT_TIERING , GLACIER , or DEEP_ARCHIVE
@@ -287,35 +283,7 @@
         :return:
         """
         response = self.__s3_client.list_buckets()
         for bucket in response['Buckets']:
             if bucket['Name'] == bucket_name:
                 return True
         return False
-
-    def __get_s3_latest_policy_file(self, policy: str):
-        """
-        This method return latest policy logs
-        @param policy:
-        @return:
-        """
-        return self.get_last_objects(bucket=self.__bucket,
-                                     logs_bucket_key=f'{self.__logs_bucket_key}/{self.__region}',
-                                     policy=policy)
-
-    def get_last_s3_policy_content(self, policy: str, file_name: str):
-        """
-        This method return last policy content
-        @return:
-        """
-        with tempfile.TemporaryDirectory() as temp_local_directory:
-            local_file = temp_local_directory + '/' + file_name + '.gz'
-            if self.__get_s3_latest_policy_file(policy=policy):
-                latest_policy_path = self.__get_s3_latest_policy_file(policy=policy)
-                self.download_file(bucket=self.__bucket,
-                                   key=str(latest_policy_path),
-                                   download_file=file_name + '.gz',
-                                   file_name_path=local_file)
-                # gzip
-                os.system(f"gzip -d {local_file}")
-                with open(os.path.join(temp_local_directory, file_name)) as f:
-                    return f.read()
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/clouds/aws/utils/utils.py` & `cloud-governance-1.1.9/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     """
 
     def __init__(self, region: str = 'us-east-2'):
         self.region = region
         pass
 
     @typeguard.typechecked
-    def get_details_resource_list(self, func_name: Callable, input_tag: str, check_tag: str, **kwargs):
+    def get_details_resource_list(self, func_name: Callable, input_tag: str, check_tag: str):
         """
         This method fetch all Items of the resource i.e: EC2, IAM
         :param func_name:
         :param input_tag:
         :param check_tag:
         :return:
         """
         resource_list = []
-        resources = func_name(**kwargs)
+        resources = func_name()
         resource_list.extend(resources[input_tag])
         while check_tag in resources.keys():
             if check_tag == 'NextToken':
-                resources = func_name(NextToken=resources[check_tag], **kwargs)
+                resources = func_name(NextToken=resources[check_tag])
             elif check_tag == 'Marker':
-                resources = func_name(Marker=resources[check_tag], **kwargs)
+                resources = func_name(Marker=resources[check_tag])
             resource_list.extend(resources[input_tag])
         return resource_list
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/google_drive/google_drive_operations.py` & `cloud-governance-1.1.9/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,199 +2,130 @@
 import os.path
 
 import google.auth
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class GoogleDriveOperations:
     """
     This class perform the Google Drive Operations
     methods
     1. download_spreadsheet
     """
 
-    RETRIES = 3
-
     def __init__(self):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.__service = None
-        if self.__environment_variables_dict.get('GOOGLE_APPLICATION_CREDENTIALS'):
+        if os.environ.get('GOOGLE_APPLICATION_CREDENTIALS'):
             self.__creds, _ = google.auth.default()
-            self.__service = build('sheets', 'v4', credentials=self.__creds, num_retries=self.RETRIES)
+            self.__service = build('sheets', 'v4', credentials=self.__creds)
 
-    @logger_time_stamp
-    def create_work_sheet(self, gsheet_id: str, sheet_name: str):
-        """
-        This method checks for worksheet and create the worksheet
-        @return:
-        """
-        try:
-            if not self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=gsheet_id):
-                create_worksheet_meta_data = {
-                    'requests': [{
-                        'addSheet': {
-                            'properties': {
-                                'title': sheet_name
-                            }
-                        }
-                    }]}
-                if self.__service:
-                    self.__service.spreadsheets().batchUpdate(spreadsheetId=gsheet_id, body=create_worksheet_meta_data).execute()
-                    logger.info(f'{sheet_name} worksheet created')
-            else:
-                logger.info(f'{sheet_name} Worksheet Already present')
-        except Exception as err:
-            raise err
-
-    @logger_time_stamp
     def download_spreadsheet(self, spreadsheet_id: str, sheet_name: str, file_path: str):
         """
         This method download spreadsheet from the Google Drive
         Used the Google Drive API
         Create GCP Project, enable Google Drive API, enable Google Spreadsheet API
         Create Service Account, and generate keys in json format
         export GOOGLE_APPLICATION_CREDENTIALS=file_location
         @return:
         """
-        if self.__service:
-            try:
-                result = self.__service.spreadsheets().values().get(spreadsheetId=spreadsheet_id, range=sheet_name).execute()
-                file_name = f'{sheet_name}.csv'
-                output_file = os.path.join(file_path, file_name)
-                if result.get('values'):
-                    with open(output_file, 'w') as f:
-                        writer = csv.writer(f)
-                        writer.writerows(result.get('values'))
-                    logger.info(f'Successfully downloaded {sheet_name}.csv')
-            except HttpError as error:
-                logger.info(f'An error occurred: {error}')
+        try:
+            result = self.__service.spreadsheets().values().get(spreadsheetId=spreadsheet_id, range=sheet_name).execute()
+            file_name = f'{sheet_name}.csv'
+            output_file = os.path.join(file_path, file_name)
+            with open(output_file, 'w') as f:
+                writer = csv.writer(f)
+                writer.writerows(result.get('values'))
+        except HttpError as error:
+            logger.info(f'An error occurred: {error}')
+        logger.info(f'Successfully downloaded {sheet_name}.csv')
 
-    @logger_time_stamp
     def append_values(self, spreadsheet_id, sheet_name: str, values: list, value_input_option: str = 'USER_ENTERED'):
         """
         This method append the values in the spreadsheet
         @param spreadsheet_id:
         @param sheet_name:
         @param values:
         @param value_input_option:
         @return:
         """
-        if self.__service:
-            try:
-                body = {'values': values}
-                result = self.__service.spreadsheets().values().append(
-                    spreadsheetId=spreadsheet_id, range=sheet_name,
-                    valueInputOption=value_input_option, body=body).execute()
-                logger.info(f'Data is append to the end of the worksheet {sheet_name}')
-                return result
-            except HttpError as error:
-                logger.info(f'An error occurred: {error}')
+        try:
+            body = {'values': values}
+            result = self.__service.spreadsheets().values().append(
+                spreadsheetId=spreadsheet_id, range=sheet_name,
+                valueInputOption=value_input_option, body=body).execute()
+            return result
+        except HttpError as error:
+            logger.info(f'An error occurred: {error}')
 
-    @logger_time_stamp
     def find_sheet_id_by_name(self, sheet_name: str, spreadsheet_id: str):
         """
         This method find the sheet id in the spreadsheet
         @param sheet_name:
         @param spreadsheet_id:
         @return:
         """
-        if self.__service:
-            sheets_with_properties = self.__service.spreadsheets().get(spreadsheetId=spreadsheet_id,
-                                                                       fields='sheets.properties').execute().get('sheets')
-            for sheet in sheets_with_properties:
-                if 'title' in sheet['properties'].keys():
-                    if sheet['properties']['title'] == sheet_name:
-                        return sheet['properties']['sheetId']
-        return ''
+        sheets_with_properties = self.__service.spreadsheets() .get(spreadsheetId=spreadsheet_id, fields='sheets.properties').execute().get('sheets')
+        for sheet in sheets_with_properties:
+            if 'title' in sheet['properties'].keys():
+                if sheet['properties']['title'] == sheet_name:
+                    return sheet['properties']['sheetId']
 
-    @logger_time_stamp
     def delete_rows(self, spreadsheet_id: str, sheet_name: str, row_number: int):
         """
         This method delete row from the spreadsheet bases on row number
         @param spreadsheet_id:
         @param sheet_name:
         @param row_number:
         @return:
         """
-        if self.__service:
-            try:
-                spreadsheet_data = [
-                    {
-                        "deleteDimension": {
-                            "range": {
-                                "sheetId": self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=spreadsheet_id),
-                                "dimension": "ROWS",
-                                "startIndex": row_number,
-                                "endIndex": row_number + 1
-                            }
+        try:
+            spreadsheet_data = [
+                {
+                    "deleteDimension": {
+                        "range": {
+                            "sheetId": self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=spreadsheet_id),
+                            "dimension": "ROWS",
+                            "startIndex": row_number,
+                            "endIndex": row_number+1
                         }
                     }
-                ]
-                update_data = {"requests": spreadsheet_data}
-                updating = self.__service.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body=update_data)
-                updating.execute()
-            except HttpError as error:
-                logger.into(f'An error occurred: {error}')
+                }
+            ]
+            update_data = {"requests": spreadsheet_data}
+            updating = self.__service.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body=update_data)
+            updating.execute()
+        except HttpError as error:
+            logger.into(f'An error occurred: {error}')
 
-    @logger_time_stamp
     def paste_csv_to_gsheet(self, csv_path, spreadsheet_id: str, sheet_name: str):
         """
         This method paste the csv data into the specific sheet
         Note: replaces the content in the rowIndex, columnIndex you specified
         @param csv_path:
         @param spreadsheet_id:
         @param sheet_name:
         @return:
         """
-        if self.__service:
-            csv_contents = None
-            with open(csv_path, 'r') as csv_file:
-                csv_contents = csv_file.read()
-            if csv_contents:
-                sheet_id = self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=spreadsheet_id)
-                body = {
-                    'requests': [{
-                        'pasteData': {
-                            "coordinate": {
-                                "sheetId": sheet_id,
-                                "rowIndex": "0",
-                                "columnIndex": "0",
-                            },
-                            "data": csv_contents,
-                            "type": 'PASTE_NORMAL',
-                            "delimiter": ',',
-                        }
-                    }]
-                }
-                request = self.__service.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body=body)
-                response = request.execute()
-                logger.info(f'Pasted data into the {sheet_name}')
-                return response
-
-    @logger_time_stamp
-    def update_row_in_gsheet(self, data: list, gsheet_id: str, row: int, sheet_name: str):
-        """
-        This method update the values in a row
-        @return:
-        """
-        if self.__service:
-            sheet_id = self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=gsheet_id)
-            requests_body = {'requests': [{
-                'updateCells': {
-                    'rows': [{"values": data}],
-                    'fields': '*',
-                    'start': {
-                        "sheetId": sheet_id,
-                        "rowIndex": row,
-                        "columnIndex": '0'
+        csv_contents = None
+        with open(csv_path, 'r') as csv_file:
+            csv_contents = csv_file.read()
+        if csv_contents:
+            sheet_id = self.find_sheet_id_by_name(sheet_name=sheet_name, spreadsheet_id=spreadsheet_id)
+            body = {
+                'requests': [{
+                    'pasteData': {
+                        "coordinate": {
+                            "sheetId": sheet_id,
+                            "rowIndex": "0",
+                            "columnIndex": "0",
+                        },
+                        "data": csv_contents,
+                        "type": 'PASTE_NORMAL',
+                        "delimiter": ',',
                     }
-                }
-            }]}
-            request = self.__service.spreadsheets().batchUpdate(spreadsheetId=gsheet_id, body=requests_body)
+                }]
+            }
+            request = self.__service.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body=body)
             response = request.execute()
-            logger.info(f'Updated the row in the worksheet {sheet_name}')
             return response
```

### Comparing `cloud-governance-1.1.86/cloud_governance/common/ldap/ldap_search.py` & `cloud-governance-1.1.9/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/common/logger/logger_time_stamp.py` & `cloud-governance-1.1.9/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/common/mails/gmail.py` & `cloud-governance-1.1.9/cloud_governance/common/mails/gmail.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+import os
 import smtplib
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class Gmail:
     """
     This class send mail by accepting the receivers list and body
     export sender_mail and sender_password
     before creating a password enable two-factor authentication
     create sender_password by GoogleAccount ->  Security --> Apps password
     """
 
     SMTP_PORT = 465
 
     def __init__(self):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.sender_mail = self.__environment_variables_dict.get('SENDER_MAIL', '')
-        self.sender_password = self.__environment_variables_dict.get('SENDER_PASSWORD', '')
+        self.sender_mail = os.environ.get('SENDER_MAIL', '')
+        self.sender_password = os.environ.get('SENDER_PASSWORD', '')
 
     def send_mail(self, receivers_list: list, subject: str, body: str, cc: list):
         """
         This method sends email
         sender_password: generate from gmail apps
         @param cc:
         @param receivers_list:
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/ebs_unattached.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+import datetime
+
+from cloud_governance.common.logger.init_logger import logger
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
 class EbsUnattached(NonClusterZombiePolicy):
     """
     This class deletes the ebs unattached if more than 7 days, trigger mail if more than 3 days
     add Tag policy=skip/Not_Delete to skip deletion
     """
@@ -21,40 +24,32 @@
         """
         This method list all ebs volumes and delete if it is unattached more than 7 days, trigger mail after 4 days
         @return:
         """
         volumes = self._ec2_client.describe_volumes(Filters=[{'Name': 'status', 'Values': ['available']}])['Volumes']
         unattached_volumes_data = []
         for volume in volumes:
-            if not self._check_cluster_tag(tags=volume.get('Tags')) or self._get_policy_value(tags=volume.get('Tags')) not in ('NOTDELETE', 'SKIP'):
+            if not self._check_live_cluster_tag(tags=volume.get('Tags')):
                 volume_id = volume.get('VolumeId')
                 launch_days = self._calculate_days(create_date=volume.get('CreateTime'))
                 if launch_days >= self.DAYS_TO_DELETE_RESOURCE:
                     last_detached_time = self._cloudtrail.get_last_time_accessed(resource_id=volume_id,
                                                                                  event_name='DetachVolume',
                                                                                  start_time=self._start_date,
                                                                                  end_time=self._end_date,
                                                                                  optional_event_name=['CreateVolume',
                                                                                                       'CreateTags'])
                     if last_detached_time:
                         last_detached_days = self._calculate_days(create_date=last_detached_time)
-                        ebs_cost = self.resource_pricing.get_ebs_cost(volume_type=volume.get('VolumeType'), volume_size=volume.get('Size'), hours=(self.DAILY_HOURS * last_detached_days))
-                        delta_cost = 0
-                        if last_detached_days == self.DAYS_TO_NOTIFY_ADMINS:
-                            delta_cost = self.resource_pricing.get_ebs_cost(volume_type=volume.get('VolumeType'), volume_size=volume.get('Size'), hours=(self.DAILY_HOURS * (self.DAYS_TO_DELETE_RESOURCE - self.DAYS_TO_NOTIFY_ADMINS)))
-                        else:
-                            if last_detached_days == self.DAYS_TO_DELETE_RESOURCE:
-                                delta_cost = self.resource_pricing.get_ebs_cost(volume_type=volume.get('VolumeType'), volume_size=volume.get('Size'), hours=(self.DAILY_HOURS * (self.DAYS_TO_DELETE_RESOURCE - self.DAYS_TO_NOTIFY_ADMINS)))
                         unattached_volumes = self._check_resource_and_delete(resource_name='EBS Volume',
                                                                              resource_id='VolumeId',
                                                                              resource_type='CreateVolume',
                                                                              resource=volume,
                                                                              empty_days=last_detached_days,
-                                                                             days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
-                                                                             extra_purse=ebs_cost, delta_cost=delta_cost)
+                                                                             days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE)
                         if unattached_volumes:
                             unattached_volumes_data.append([volume.get('VolumeId'),
                                                             self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Name'),
                                                             self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='User'),
                                                             str(last_detached_days),
                                                             self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Policy')])
         return unattached_volumes_data
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/ec2_idle.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/ec2_idle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta
 
 from cloud_governance.common.clouds.aws.cloudwatch.cloudwatch_operations import CloudWatchOperations
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
 class EC2Idle(NonClusterZombiePolicy):
     """
     This class stop the idle ec2 instances more than 4 days if the matches the required metrics
     CpuUtilization < 2 percent
     NetworkIN < 5k bytes
@@ -21,14 +21,34 @@
     NETWORK_OUT_BYTES = 5000
     INSTANCE_LAUNCH_DAYS = 7
 
     def __init__(self):
         super().__init__()
         self._cloudwatch = CloudWatchOperations(region=self._region)
 
+    def __organise_instance_data(self, instances_data: list):
+        """
+        This method convert all datetime into string
+        @param instances_data:
+        @return:
+        """
+        organize_data = []
+        for instance in instances_data:
+            instance['LaunchTime'] = instance['LaunchTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
+            for index, device_mappings in enumerate(instance['BlockDeviceMappings']):
+                instance['BlockDeviceMappings'][index]['Ebs']['AttachTime'] = device_mappings['Ebs']['AttachTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
+            for index, network_interface in enumerate(instance['NetworkInterfaces']):
+                instance['NetworkInterfaces'][index]['Attachment']['AttachTime'] = network_interface['Attachment']['AttachTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
+            if instance.get('UsageOperationUpdateTime'):
+                instance['UsageOperationUpdateTime'] = instance['UsageOperationUpdateTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
+            for index, metric in enumerate(instance['metrics']):
+                instance['metrics'][index]['Timestamps'] = [date.strftime("%Y-%m-%dT%H:%M:%S+00:00") for date in metric['Timestamps']]
+            organize_data.append(instance)
+        return organize_data
+
     def run(self):
         """
         This method list all idle instances and stop if it is idle since 4 days
         @return:
         """
         return self.__stop_idle_instances(instance_launch_days=self.INSTANCE_LAUNCH_DAYS)
 
@@ -37,60 +57,47 @@
         This method list all idle instances and stop  if it s idle since 4 days
         @param instance_launch_days:
         @return:
         """
         instances = self._ec2_client.describe_instances(Filters=[{'Name': 'instance-state-name', 'Values': ['running']}])['Reservations']
         running_idle_instances = {}
         running_instance_tags = {}
-        ec2_idle_cost = {}
-        block_device_mappings = {}
         ec2_types = {}
         for instance in instances:
             for resource in instance['Instances']:
-                if self._get_policy_value(tags=resource.get('Tags', [])) not in ('NOTDELETE', 'SKIP') and not self._check_cluster_tag(tags=resource.get('Tags', [])):
-                    launch_days = self.__get_time_difference(launch_time=resource.get('LaunchTime'))
-                    if launch_days >= instance_launch_days:
-                        instance_id = resource.get('InstanceId')
-                        metrics_4_days = self.__get_metrics_from_cloud_watch(instance_id=instance_id, instance_period=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS)
-                        cpu_metric_4_days, network_in_4_days, network_out_2_days = self.__get_proposed_metrics(metrics=metrics_4_days, metric_period=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS)
-                        if cpu_metric_4_days < self.CPU_UTILIZATION_PERCENTAGE and network_in_4_days < self.NETWORK_IN_BYTES and network_out_2_days < self.NETWORK_OUT_BYTES:
-                            if not self._ec2_operations.is_cluster_resource(resource_id=instance_id):
-                                resource['metrics'] = metrics_4_days
-                                running_idle_instances[instance_id] = resource
-                            user = self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User')
-                            if user:
-                                idle_cost = self.resource_pricing.ec2_instance_type_cost(instance_type=resource.get('InstanceType'), hours=(self.DAILY_HOURS*self.DAYS_TO_TRIGGER_RESOURCE_MAIL))
-                                idle_ebs_cost = self.get_ebs_cost(resource=resource.get('BlockDeviceMappings'), resource_type='ec2', resource_hours=(self.DAILY_HOURS * self.DAYS_TO_TRIGGER_RESOURCE_MAIL))
-                                self.__trigger_mail(tags=resource.get('Tags'), resource_id=instance_id, days=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS, ec2_type=resource.get('InstanceType'),
-                                                    instance_id=instance_id, message_type='notification', extra_purse=(idle_cost+idle_ebs_cost), delta_cost=(idle_cost+idle_ebs_cost))
-                            else:
-                                logger.info('User is missing')
+                launch_days = self.__get_time_difference(launch_time=resource.get('LaunchTime'))
+                if launch_days > instance_launch_days:
+                    instance_id = resource.get('InstanceId')
+                    metrics_2_days = self.__get_metrics_from_cloud_watch(instance_id=instance_id, instance_period=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS)
+                    cpu_metric_2_days, network_in_2_days, network_out_2_days = self.__get_proposed_metrics(metrics=metrics_2_days, metric_period=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS)
+                    if cpu_metric_2_days < self.CPU_UTILIZATION_PERCENTAGE and network_in_2_days < self.NETWORK_IN_BYTES and network_out_2_days < self.NETWORK_OUT_BYTES:
                         if not self._ec2_operations.is_cluster_resource(resource_id=instance_id):
-                            metrics_7_days = self.__get_metrics_from_cloud_watch(instance_id=instance_id, instance_period=self.STOP_INSTANCE_IDLE_DAYS)
-                            cpu_metric_7_days, network_in_7_days, network_out_7_days = self.__get_proposed_metrics(metrics=metrics_4_days, metric_period=self.STOP_INSTANCE_IDLE_DAYS)
-                            if cpu_metric_7_days < self.CPU_UTILIZATION_PERCENTAGE and network_in_4_days < self.NETWORK_IN_BYTES and network_out_7_days < self.NETWORK_OUT_BYTES:
-                                resource['metrics'] = metrics_7_days
-                                idle_cost = self.resource_pricing.ec2_instance_type_cost(
-                                    instance_type=resource.get('InstanceType'),
-                                    hours=(self.DAILY_HOURS * self.DAYS_TO_TRIGGER_RESOURCE_MAIL))
-                                idle_ebs_cost = self.get_ebs_cost(resource=resource.get('BlockDeviceMappings'), resource_type='ec2', resource_hours=(self.DAILY_HOURS * self.DAYS_TO_TRIGGER_RESOURCE_MAIL))
-                                ec2_idle_cost[instance_id] = idle_ebs_cost + idle_cost
-                                block_device_mappings[instance_id] = resource.get('BlockDeviceMappings')
-                                running_idle_instances[instance_id] = resource
-                                running_instance_tags[instance_id] = resource.get('Tags')
-                                ec2_types[instance_id] = resource.get('InstanceType')
+                            resource['metrics'] = metrics_2_days
+                            running_idle_instances[instance_id] = resource
+                        user = self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User')
+                        if user:
+                            self.__trigger_mail(tags=resource.get('Tags'), resource_id=instance_id, days=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS, ec2_type=resource.get('InstanceType'),
+                                                instance_id=instance_id)
+                        else:
+                            logger.info('User is missing')
+                    if not self._ec2_operations.is_cluster_resource(resource_id=instance_id):
+                        metrics_4_days = self.__get_metrics_from_cloud_watch(instance_id=instance_id, instance_period=self.STOP_INSTANCE_IDLE_DAYS)
+                        cpu_metric_4_days, network_in_4_days, network_out_4_days = self.__get_proposed_metrics(metrics=metrics_4_days, metric_period=self.STOP_INSTANCE_IDLE_DAYS)
+                        if cpu_metric_4_days < self.CPU_UTILIZATION_PERCENTAGE and network_in_4_days < self.NETWORK_IN_BYTES and network_out_4_days < self.NETWORK_OUT_BYTES:
+                            resource['metrics'] = metrics_4_days
+                            running_idle_instances[instance_id] = resource
+                            running_instance_tags[instance_id] = resource.get('Tags')
+                            ec2_types[instance_id] = resource.get('InstanceId')
         if self._dry_run == "no":
             for instance_id, tags in running_instance_tags.items():
                 if self._get_policy_value(tags=tags) not in ('NOTDELETE', 'SKIP'):
                     self._ec2_client.stop_instances(InstanceIds=[instance_id])
                     logger.info(f'Stopped the instance: {instance_id}')
-                    idle_cost = self.resource_pricing.ec2_instance_type_cost(instance_type=ec2_types[instance_id], hours=(self.DAILY_HOURS * self.DAYS_TO_DELETE_RESOURCE))
-                    idle_ebs_cost = self.get_ebs_cost(resource=block_device_mappings[instance_id], resource_type='ec2', resource_hours=(self.DAILY_HOURS * self.DAYS_TO_DELETE_RESOURCE))
-                    self.__trigger_mail(tags=tags, resource_id=instance_id, days=self.STOP_INSTANCE_IDLE_DAYS, ec2_type=ec2_types[instance_id], instance_id=instance_id, message_type='delete', extra_purse=(idle_ebs_cost+idle_cost), delta_cost=ec2_idle_cost[instance_id])
-        return self._organise_instance_data(list(running_idle_instances.values()))
+                    self.__trigger_mail(tags=tags, resource_id=instance_id, days=self.STOP_INSTANCE_IDLE_DAYS, ec2_type=ec2_types[instance_id], instance_id=instance_id)
+        return self.__organise_instance_data(list(running_idle_instances.values()))
 
     def __get_metrics_average(self, metric_list: list, metric_period: int):
         """
         This method calculate the average of the metrics
         @param metric_list:
         @param metric_period:
         @return:
@@ -128,24 +135,24 @@
         This method return the difference of datetime
         @param launch_time:
         @return:
         """
         end_time = datetime.now()
         return (end_time - launch_time.replace(tzinfo=None)).days
 
-    def __trigger_mail(self, tags: list, resource_id: str, days: int, ec2_type: str = '', instance_id: str = '', **kwargs):
+    def __trigger_mail(self, tags: list, resource_id: str, days: int, ec2_type: str = '', instance_id: str = ''):
         """
         This method send triggering mail
         @param tags:
         @param resource_id:
         @return:
         """
         try:
             special_user_mails = self._literal_eval(self._special_user_mails)
             user, instance_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(tags=tags, tag_name='Name')
             to = user if user not in special_user_mails else special_user_mails[user]
             ldap_data = self._ldap.get_user_details(user_name=to)
             cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com']
-            subject, body = self._mail_description.ec2_idle(name=ldap_data.get('displayName'), days=days, notification_days=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS, stop_days=self.STOP_INSTANCE_IDLE_DAYS, instance_name=instance_name, resource_id=resource_id, ec2_type=ec2_type, extra_purse=kwargs.get('extra_purse'))
-            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=instance_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
+            subject, body = self._mail_description.ec2_idle(name=ldap_data.get('displayName'), days=days, notification_days=self.INSTANCE_IDLE_MAIL_NOTIFICATION_DAYS, stop_days=self.STOP_INSTANCE_IDLE_DAYS, instance_name=instance_name, resource_id=resource_id, ec2_type=ec2_type)
+            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=instance_id)
         except Exception as err:
             logger.info(err)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/empty_roles.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/empty_roles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
 class EmptyRoles(NonClusterZombiePolicy):
-    """
-    This class sends an alert mail for empty role to the user after 4 days and delete after 7 days.
-    """
 
     def __init__(self):
         super().__init__()
 
     def run(self):
         """
         This method return all empty roles, delete if dry_run no
@@ -25,15 +22,15 @@
         zombie_roles = []
         roles = self._iam_operations.get_roles()
         for role in roles:
             role_name = role.get('RoleName')
             try:
                 get_role = self._iam_client.get_role(RoleName=role.get('RoleName'))['Role']
                 tags = get_role.get('Tags')
-                if not self._check_cluster_tag(tags=tags):
+                if not self._check_live_cluster_tag(tags=tags):
                     role_empty = False
                     role_attached_policies = self._iam_client.list_attached_role_policies(RoleName=role_name)
                     role_inline_policies = self._iam_client.list_role_policies(RoleName=role_name)
                     if not role_inline_policies.get('PolicyNames') and not role_attached_policies.get('AttachedPolicies'):
                         role_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='Name'):
                             tags.append({'Key': 'Name', 'Value': role_name})
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/nat_gateway_unused.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_nat_gateways.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
-class NatGatewayUnused(NonClusterZombiePolicy):
-    """
-    This class sends an alert mail for zombie Nat gateways ( based on vpc routes )
-    to the user after 4 days and delete after 7 days.
-    """
+class ZombieNatGateways(NonClusterZombiePolicy):
 
     def __init__(self):
         super().__init__()
 
     def __check_nat_gateway_in_routes(self, nat_gateway_id: str):
         route_tables = self._ec2_client.describe_route_tables()['RouteTables']
         nat_gateway_found = False
@@ -22,30 +18,30 @@
 
     def run(self):
         """
         This method return zombie NatGateways, delete if dry_run no
         @return:
         """
         nat_gateways = self._ec2_operations.get_nat_gateways()
-        nat_gateway_unused_data = []
+        zombie_nat_gateways_data = []
         for nat_gateway in nat_gateways:
-            if self._get_policy_value(tags=nat_gateway.get('Tags', [])) not in ('NOTDELETE', 'SKIP'):
-                nat_gateway_id = nat_gateway.get('NatGatewayId')
-                tags = nat_gateway.get('Tags')
-                gateway_unused = False
-                if not self._check_cluster_tag(tags=tags):
-                    if nat_gateway.get('State') == 'available':
-                        if not self.__check_nat_gateway_in_routes(nat_gateway_id=nat_gateway_id):
-                            gateway_unused = True
-                            unused_days = self._get_resource_last_used_days(tags=tags)
-                            zombie_nat_gateway = self._check_resource_and_delete(resource_name='NatGateway',
-                                                                                 resource_id='NatGatewayId',
-                                                                                 resource_type='CreateNatGateway',
-                                                                                 resource=nat_gateway,
-                                                                                 empty_days=unused_days,
-                                                                                 days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
-                            if zombie_nat_gateway:
-                                nat_gateway_unused_data.append([nat_gateway_id, self._get_tag_name_from_tags(tags=tags, tag_name='User'), zombie_nat_gateway.get('VpcId'), self._get_policy_value(tags=tags), unused_days])
-                        else:
-                            unused_days = 0
-                        self._update_resource_tags(resource_id=nat_gateway_id, tags=tags, left_out_days=unused_days, resource_left_out=gateway_unused)
-        return nat_gateway_unused_data
+            nat_gateway_id = nat_gateway.get('NatGatewayId')
+            tags = nat_gateway.get('Tags')
+            gateway_unused = False
+            if not self._check_live_cluster_tag(tags=tags):
+                if nat_gateway.get('State') == 'available':
+                    if not self.__check_nat_gateway_in_routes(nat_gateway_id=nat_gateway_id):
+                        gateway_unused = True
+                        unused_days = self._get_resource_last_used_days(tags=tags)
+                        zombie_nat_gateway = self._check_resource_and_delete(resource_name='NatGateway',
+                                                                             resource_id='NatGatewayId',
+                                                                             resource_type='CreateNatGateway',
+                                                                             resource=nat_gateway,
+                                                                             empty_days=unused_days,
+                                                                             days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
+                        if zombie_nat_gateway:
+                            zombie_nat_gateways_data.append([nat_gateway_id, self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                             zombie_nat_gateway.get('VpcId'), self._get_policy_value(tags=tags), unused_days])
+                    else:
+                        unused_days = 0
+                    self._update_resource_tags(resource_id=nat_gateway_id, tags=tags, left_out_days=unused_days, resource_left_out=gateway_unused)
+        return zombie_nat_gateways_data
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/s3_inactive.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/empty_buckets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+import operator
+from operator import ge
 
+import boto3
 from botocore.exceptions import ClientError
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
-class S3Inactive(NonClusterZombiePolicy):
-    """
-    This class sends an alert mail for empty bucket to the user after 4 days and delete after 7 days.
-    """
+class EmptyBuckets(NonClusterZombiePolicy):
 
     def __init__(self):
         super().__init__()
 
     def run(self):
         """
         This method return all Empty buckets and delete if dry_run no
         @return:
         """
-        return self.__delete_s3_inactive()
+        return self.__delete_empty_bucket()
 
-    def __delete_s3_inactive(self):
+    def __delete_empty_bucket(self):
         """
         This method delete the empty bucket more than 7 days
         @return:
         """
         empty_buckets = []
         buckets = self._s3_client.list_buckets()['Buckets']
         for bucket in buckets:
@@ -35,15 +35,15 @@
                 try:
                     bucket_tags = self._s3_client.get_bucket_tagging(Bucket=bucket_name)
                     tags = bucket_tags.get('TagSet')
                 except ClientError:
                     tags = []
                 bucket_data = self._s3_client.list_objects_v2(Bucket=bucket_name)
                 if not bucket_data.get('Contents'):
-                    if not self._check_cluster_tag(tags=tags):
+                    if not self._check_live_cluster_tag(tags=tags):
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='Name'):
                             tags.append({'Key': 'Name', 'Value': bucket_name})
                         empty_days = self._get_resource_last_used_days(tags=tags)
                         bucket_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='User'):
                             region = self._s3_client.get_bucket_location(Bucket=bucket_name)['LocationConstraint']
                             self._cloudtrail.set_cloudtrail(region_name=region)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/zombie_cluster_resource.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import boto3
 
-from cloud_governance.policy.policy_operations.aws.zombie_cluster.zombie_cluster_common_methods import ZombieClusterCommonMethods
+from cloud_governance.aws.zombie_cluster.zombie_cluster_common_methods import ZombieClusterCommonMethods
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 
 # @todo add next token
 # response = client.get_servers()
 # results = response["serverList"]
 # while "NextToken" in response:
 #     response = client.get_servers(NextToken=response["NextToken"])
 #     results.extend(response["serverList"])
-from cloud_governance.policy.policy_operations.aws.zombie_cluster.delete_ec2_resources import DeleteEC2Resources
-from cloud_governance.policy.policy_operations.aws.zombie_cluster.delete_iam_resources import DeleteIAMResources
-from cloud_governance.policy.policy_operations.aws.zombie_cluster.delete_s3_resources import DeleteS3Resources
+from cloud_governance.aws.zombie_cluster.delete_ec2_resources import DeleteEC2Resources
+from cloud_governance.aws.zombie_cluster.delete_iam_resources import DeleteIAMResources
+from cloud_governance.aws.zombie_cluster.delete_s3_resources import DeleteS3Resources
 
 
 class ZombieClusterResources(ZombieClusterCommonMethods):
     """
-    This class filter and deletes zombie cluster resources, which are not deleted while cleanup the clusters,
-    alert user after 4 days of cluster deleted. and delete the resources after 7 days of cluster deleted.
+    This class filter zombie cluster resourcesfrom cloud_governance.aws.zombie_cluster.ZombieClusterCommonResources import ZombieClusterCommonResources
+
     """
 
     def __init__(self, cluster_prefix: str = None, delete: bool = False, region: str = 'us-east-2',
-                 cluster_tag: str = '', resource_name: str = '', force_delete: bool = False):
-        super().__init__(region=region, force_delete=force_delete)
+                 cluster_tag: str = '', resource_name: str = ''):
+        super().__init__(region=region)
         self.cluster_prefix = cluster_prefix
         self.delete = delete
         self.cluster_tag = cluster_tag
         self.resource_name = resource_name
         self.delete_ec2_resource = DeleteEC2Resources(self.ec2_client, self.elb_client, self.elbv2_client,
                                                       region=region)
         self.delete_iam_resource = DeleteIAMResources(iam_client=self.iam_client)
@@ -195,17 +195,16 @@
         resources = self._get_tags_of_zombie_resources(resources=volumes_data, resource_id_name='VolumeId', zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_ami(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's ami according to cluster tag name and cluster name data
         """
@@ -220,18 +219,17 @@
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(
                     resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie,
                     cluster_tag=cluster_tag)
                 try:
                     if delete_cluster_resource and self.delete:
                         self.ec2_client.deregister_image(ImageId=zombie)
                         logger.info(f'deregister_image: {zombie}')
-                    else:
-                        if self._force_delete and self.delete:
-                            self.ec2_client.deregister_image(ImageId=zombie)
-                            logger.info(f'deregister_image: {zombie}')
+                    elif self.delete:
+                        self.ec2_client.deregister_image(ImageId=zombie)
+                        logger.info(f'deregister_image: {zombie}')
                 except Exception as err:
                     logger.exception(f'Cannot deregister_image: {zombie}, {err}')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_snapshot(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's snapshot according to cluster tag name and cluster name data
@@ -242,17 +240,16 @@
         resources = self._get_tags_of_zombie_resources(resources=snapshots_data, resource_id_name='SnapshotId', zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='ebs_snapshots', resource_id=zombie)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='ebs_snapshots', resource_id=zombie)
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='ebs_snapshots', resource_id=zombie)
         return zombies, cluster_left_out_days
 
     def __get_tag_from_resource_tags(self, tags: list, cluster_tag: str):
         """
         This method retunrs the cluster tag
         @param tags:
         @param cluster_tag:
@@ -333,18 +330,17 @@
                 security_groups = self.ec2_operations.get_security_groups()
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=security_groups, input_tag='GroupId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=security_groups, output_tag='GroupId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_elastic_ip(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's elastic ip according to existing instances and cluster name data
         """
@@ -364,25 +360,23 @@
         resources_all = self._get_tags_of_zombie_resources(resources=elastic_ips_data, resource_id_name='AllocationId', zombies=zombies_all, aws_service='ec2')
         cluster_left_out_days = {}
         if zombies_ass:
             for zombie, cluster_tag in zombies_ass.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources_ass, cluster_left_out_days=cluster_left_out_days, zombie=zombie,cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, deletion_type='disassociate')
-                else:
-                    if self._force_delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, deletion_type='disassociate')
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, deletion_type='disassociate')
         if zombies_all:
             for zombie, cluster_tag in zombies_all.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources_all, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
         zombies = {**zombies_all}
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_interface(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's network interface according to existing instances and cluster name data
         """
@@ -401,18 +395,17 @@
                     zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=network_interfaces_data, output_tag='NetworkInterfaceId', cluster_tag=cluster_tag, tags='TagSet')
                 else:
                     zombie_ids = [zombie]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days( resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's load balancer according to cluster vpc and cluster name data
         """
 
@@ -436,17 +429,16 @@
         resources = self._get_tags_of_zombie_resources(resources=load_balancers_data, resource_id_name='LoadBalancerName', zombies=zombies, aws_service='elbv1')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer_v2(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's load balancer according to cluster vpc and cluster name data
         """
         exist_load_balancer = {}
@@ -469,17 +461,16 @@
         resources = self._get_tags_of_zombie_resources(resources=load_balancers_data, resource_id_name='LoadBalancerArn', zombies=zombies, aws_service='elbv2')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def __get_all_exist_vpcs(self):
         """
         This method return all exist vpc ids (for supporting Network ACL - missing OpenShift tags)
         :return:
         """
@@ -505,17 +496,16 @@
         resources = self._get_tags_of_zombie_resources(resources=vpcs_data, resource_id_name='VpcId', zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
+                elif self.delete:
+                    self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_subnet(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's subnet according to cluster tag name and cluster name data
         """
@@ -532,18 +522,18 @@
                 subnets_data = self.ec2_operations.get_subnets()
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=subnets_data, input_tag='SubnetId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=subnets_data, output_tag='SubnetId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id,  cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id,
+                                                                        cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_route_table(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's route table according to cluster tag name and cluster name data
         """
         route_tables_data = self.ec2_operations.get_route_tables()
@@ -559,18 +549,18 @@
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=route_tables_data, input_tag='RouteTableId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=route_tables_data,
                                                           output_tag='RouteTableId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id,
+                                                                        vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_internet_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's route table internet gateway according to cluster tag name and cluster name data
         """
         internet_gateways_data = self.ec2_operations.get_internet_gateways()
@@ -588,18 +578,17 @@
                     zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=internet_gateways_data, output_tag='InternetGatewayId', cluster_tag=cluster_tag, input_tag='Attachments')
                 else:
                     zombie_ids = [zombie]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_dhcp_option(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's dhcp option according to cluster tag name and cluster name data
         """
@@ -614,20 +603,19 @@
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=vpcs, input_tag='DhcpOptionsId')
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     if vpc_id:
                         self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
                     else:
                         self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
-                else:
-                    if self._force_delete and self.delete:
-                        if vpc_id:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
-                        else:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
+                elif self.delete:
+                    if vpc_id:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
+                    else:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_vpc_endpoint(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's vpc endpoint according to cluster tag name and cluster name data
         """
         vpc_endpoints_data = self.ec2_operations.get_vpce()
@@ -645,18 +633,17 @@
                     zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=vpc_endpoints_data, output_tag='VpcEndpointId', cluster_tag=cluster_tag)
                 else:
                     zombie_ids = [zombies]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_nat_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's nat gateway according to cluster tag name and cluster name data
         """
         nat_gateways_data = self.ec2_operations.get_nat_gateways()
@@ -671,18 +658,18 @@
                 nat_gateways_data = self.ec2_operations.get_nat_gateways()
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie, nat_gateways_data, input_tag='NatGatewayId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=nat_gateways_data, output_tag='NatGatewayId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id,
+                                                                        cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_acl(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's network acl according to existing vpc id and cluster name data
         """
         exist_network_acl = {}
@@ -708,18 +695,17 @@
                 if not vpc_id:
                     vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=network_acls_data, input_tag='NetworkAclId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=network_acls_data, output_tag='NetworkAclId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
-                else:
-                    if self._force_delete and self.delete:
-                        for zombie_id in zombie_ids:
-                            self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
+                elif self.delete:
+                    for zombie_id in zombie_ids:
+                        self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_role(self):
         """
         This method return list of cluster's role in all regions according to cluster name and cluster name data
         * Role is a global resource, need to scan for live cluster in all regions
         """
@@ -746,17 +732,16 @@
             zombies = self.__get_all_zombie_resources(exist_role_name_tag)
             resources = self._get_tags_of_zombie_resources(resources=roles_data, resource_id_name='RoleName', zombies=zombies, aws_service='role')
             if zombies:
                 for zombie, cluster_tag in zombies.items():
                     cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                     if delete_cluster_resource and self.delete:
                         self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
-                    else:
-                        if self._force_delete and self.delete:
-                            self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
+                    elif self.delete:
+                        self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_user(self):
         """
         This method return list of cluster's user according to cluster name and cluster name data
         * User is a global resource, need to scan for live cluster in all regions
         """
@@ -780,17 +765,16 @@
         resources = self._get_tags_of_zombie_resources(resources=users_data, resource_id_name='UserName', zombies=zombies, aws_service='user')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
+                elif self.delete:
+                    self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_s3_bucket(self, cluster_stamp: str = 'image-registry'):
         """
         This method return list of cluster's s3 bucket according to cluster name and cluster name data
         * S3 is a global resource, need to scan for live cluster in all regions
@@ -819,15 +803,14 @@
         resources = self._get_tags_of_zombie_resources(resources=response['Buckets'], resource_id_name='Name', zombies=zombies, aws_service='bucket', aws_tag='TagSet')
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_s3_resource.delete_zombie_s3_resource(resource_type='s3_bucket', resource_id=zombie)
-                else:
-                    if self._force_delete and self.delete:
-                        self.delete_s3_resource.delete_zombie_s3_resource(resource_type='s3_bucket', resource_id=zombie)
+                elif self.delete:
+                    self.delete_s3_resource.delete_zombie_s3_resource(resource_type='s3_bucket', resource_id=zombie)
 
         return zombies, cluster_left_out_days
 
 # zombie_cluster_resources = ZombieClusterResources(cluster_prefix='kubernetes.io/cluster/', delete=False, region='us-east-2')
 # print(zombie_cluster_resources.zombie_cluster_subnet())
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/aws/zombie_snapshots.py` & `cloud-governance-1.1.9/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
 class ZombieSnapshots(NonClusterZombiePolicy):
-    """
-    This class sends an alert mail for zombie snapshots ( AMI abandoned ) to the user after 4 days and delete after 7 days.
-    """
 
     def __init__(self):
         super().__init__()
 
     def _get_image_ids_from_description(self, snapshot_description: str):
         """
         This method gets image Ids from snapshot description
@@ -28,37 +25,36 @@
         This method return all the zombie snapshots, delete if dry_run no
         @return:
         """
         snapshots = self._ec2_operations.get_snapshots()
         zombie_snapshots = []
         image_ids = self._get_ami_ids()
         for snapshot in snapshots:
-            if not self._check_cluster_tag(tags=snapshot.get('Tags')):
-                if snapshot.get('Description'):
-                    snapshot_images = self._get_image_ids_from_description(snapshot.get('Description'))
-                    tags = snapshot.get('Tags')
-                    found = False
-                    for snapshot_image in snapshot_images:
-                        if snapshot_image in image_ids:
-                            found = True
-                    snapshot_id = snapshot.get('SnapshotId')
-                    if not found:
-                        unused_days = self._get_resource_last_used_days(tags=tags)
-                        zombie_snapshot = self._check_resource_and_delete(resource_name='Snapshot',
-                                                                          resource_id='SnapshotId',
-                                                                          resource_type='CreateSnapshot',
-                                                                          resource=snapshot,
-                                                                          empty_days=unused_days,
-                                                                          days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
-                                                                          tags=tags)
-                        if zombie_snapshot:
-                            zombie_snapshots.append([snapshot.get('SnapshotId'),
-                                                     self._get_tag_name_from_tags(tags=tags),
-                                                     self._get_tag_name_from_tags(tags=tags, tag_name='User'),
-                                                     f'{str(snapshot.get("VolumeSize"))}Gb',
-                                                     self._get_policy_value(tags=snapshot.get('Tags')), str(unused_days)
-                                                     ])
-                    else:
-                        unused_days = 0
-                    self._update_resource_tags(resource_id=snapshot_id, tags=tags, left_out_days=unused_days,
-                                               resource_left_out=not found)
+            if snapshot.get('Description'):
+                snapshot_images = self._get_image_ids_from_description(snapshot.get('Description'))
+                tags = snapshot.get('Tags')
+                found = False
+                for snapshot_image in snapshot_images:
+                    if snapshot_image in image_ids:
+                        found = True
+                snapshot_id = snapshot.get('SnapshotId')
+                if not found:
+                    unused_days = self._get_resource_last_used_days(tags=tags)
+                    zombie_snapshot = self._check_resource_and_delete(resource_name='Snapshot',
+                                                                      resource_id='SnapshotId',
+                                                                      resource_type='CreateSnapshot',
+                                                                      resource=snapshot,
+                                                                      empty_days=unused_days,
+                                                                      days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
+                                                                      tags=tags)
+                    if zombie_snapshot:
+                        zombie_snapshots.append([snapshot.get('SnapshotId'),
+                                                 self._get_tag_name_from_tags(tags=tags),
+                                                 self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                 f'{str(snapshot.get("VolumeSize"))}Gb',
+                                                 self._get_policy_value(tags=snapshot.get('Tags')), str(unused_days)
+                                                 ])
+                else:
+                    unused_days = 0
+                self._update_resource_tags(resource_id=snapshot_id, tags=tags, left_out_days=unused_days,
+                                           resource_left_out=not found)
         return zombie_snapshots
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/ibm/tag_baremetal.py` & `cloud-governance-1.1.9/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-from cloud_governance.policy.policy_operations.ibm.tagging.tagging_operations import TaggingOperations
+from cloud_governance.ibm.tagging.tagging_operations import TaggingOperations
 
 
 class TagBareMetal(TaggingOperations):
     """
-    This class tags IBM Bare metal machines
+    This method tag IBM bare-metal machines
     """
-
     def __init__(self):
         super().__init__()
 
     def get_hardware_username(self, hardware_id: str):
         """
         This method returns the hardware_username form the order details
         @param hardware_id:
         @return:
         """
-        hardware_data = self._classic_operations.get_hardware_data(hardware_id=str(hardware_id))
-        if hardware_data:
-            return hardware_data.get('billingItem').get('orderItem').get('order').get('userRecord').get('username'), f'{hardware_data.get("hostname")}.{hardware_data.get("domain")}'
-        return '', ''
+        hardware_data = self._classic_operations.get_hardware_data(hardware_id=hardware_id)
+        return hardware_data.get('billingItem').get('orderItem').get('order').get('userRecord').get('username'), f'{hardware_data.get("hostname")}.{hardware_data.get("domain")}'
 
     def tag_remove_hardware(self, user_tags: list, hardware_tags: list, hardware_id: str, hardware_name: str):
         """
         This method removes the hardware tags
         @param user_tags:
         @param hardware_tags:
         @param hardware_id:
@@ -76,33 +72,28 @@
     def tag_hardware(self, hardware_id: str):
         """
         This method perform tag operations - update, remove read
         @param hardware_id:
         @return:
         """
         username, hardware_name = self.get_hardware_username(hardware_id=hardware_id)
-        if username and hardware_name:
-            hardware_tags = self._classic_operations.get_hardware_tags(hardware_id=str(hardware_id))
-            user_tags = self._ibm_client.get_user_tags_from_gsheet(username=username)
-            if self._tag_operation == 'remove':
-                tags = self.tag_remove_hardware(user_tags, hardware_tags, hardware_id, hardware_name)
-            else:
-                tags = self.tag_update_hardware(user_tags, hardware_tags, hardware_id, hardware_name)
-            return tags
-        return []
+        hardware_tags = self._classic_operations.get_hardware_tags(hardware_id=hardware_id)
+        user_tags = self._ibm_client.get_user_tags_from_gsheet(username=username)
+        if self._tag_operation == 'remove':
+            tags = self.tag_remove_hardware(user_tags, hardware_tags, hardware_id, hardware_name)
+        else:
+            tags = self.tag_update_hardware(user_tags, hardware_tags, hardware_id, hardware_name)
+        return tags
 
-    @logger_time_stamp
     def run(self, hardware_id: str = ''):
         """
         This method tag hardware ( bare-metals ) from the user tags from the gsheet
         @return:
         """
         response = []
         if hardware_id:
             response = self.tag_hardware(hardware_id=hardware_id)
         else:
             hardware_ids = self._classic_operations.get_hardware_ids()
             for hardware_id in hardware_ids:
-                response_data = self.tag_hardware(hardware_id=hardware_id.get('id'))
-                if response_data:
-                    response.append({hardware_id.get('hostname'): response_data})
+                response.append({hardware_id.get('hostname'): self.tag_hardware(hardware_id=hardware_id.get('id'))})
         return response
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/ibm/tag_vm.py` & `cloud-governance-1.1.9/cloud_governance/policy/ibm/tag_vm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-from cloud_governance.policy.policy_operations.ibm.tagging.tagging_operations import TaggingOperations
+from cloud_governance.ibm.tagging.tagging_operations import TaggingOperations
 
 
 class TagVM(TaggingOperations):
     """
-    This class tags IBM virtual machines
+    This method tag IBM bare-metal machines
     """
-
     def __init__(self):
         super().__init__()
 
     def get_virtual_machine_username(self, vm_id: str):
         """
         This method return the virtual machine username from the billing order lists
         @param vm_id:
         @return:
         """
-        vm_data = self._classic_operations.get_virtual_machine_data(vm_id=str(vm_id))
+        vm_data = self._classic_operations.get_virtual_machine_data(vm_id=vm_id)
         return vm_data.get('billingItem').get('orderItem').get('order').get('userRecord').get('username'), f'{vm_data.get("hostname")}.{vm_data.get("domain")}'
 
     def tag_update_virtual_machine(self, user_tags: list, vm_tags: list, vm_id: str, vm_name: str):
         """
         this method updates th etags of the virtual machine
         @param user_tags:
         @param vm_tags:
@@ -74,31 +72,28 @@
     def tag_virtual_machine(self, vm_id: str):
         """
         This method perform the tag operations - read, update, remove
         @param vm_id:
         @return:
         """
         username, vm_name = self.get_virtual_machine_username(vm_id=vm_id)
-        vm_tags = self._classic_operations.get_virtual_machine_tags(vm_id=str(vm_id))
+        vm_tags = self._classic_operations.get_virtual_machine_tags(vm_id=vm_id)
         user_tags = self._ibm_client.get_user_tags_from_gsheet(username=username)
         if self._tag_operation == 'remove':
             tags = self.tag_remove_virtual_machine(user_tags=user_tags, vm_tags=vm_tags, vm_id=vm_id, vm_name=vm_name)
         else:
             tags = self.tag_update_virtual_machine(user_tags=user_tags, vm_tags=vm_tags, vm_id=vm_id, vm_name=vm_name)
         return tags
 
-    @logger_time_stamp
     def run(self, vm_id: str = ''):
         """
         This method tag vm ( virtual machines ) from the user tags from the gsheet
         @return:
         """
         response = []
         if vm_id:
             response = self.tag_virtual_machine(vm_id=vm_id)
         else:
             vm_ids = self._classic_operations.get_virtual_machine_ids()
             for vm_id in vm_ids:
-                response_data = self.tag_virtual_machine(vm_id=vm_id.get('id'))
-                if response_data:
-                    response.append({vm_id.get('hostname'): response_data})
+                response.append({vm_id.get('hostname'): self.tag_virtual_machine(vm_id=vm_id.get('id'))})
         return response
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `cloud-governance-1.1.9/cloud_governance/ibm/ibm_operations/tag_resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import importlib
 import inspect
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.main.environment_variables import environment_variables
+from cloud_governance.ibm.ibm_operations.ibm_operations import IBMOperations
 
 
-class CostReportPolicies:
+class TagResources(IBMOperations):
+    """
+    This class run the IBM Policies from policy/ibm
+    """
 
     def __init__(self):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self._account = self.__environment_variables_dict.get('account', '')
-        self._policy = self.__environment_variables_dict.get('policy', '')
+        super().__init__()
 
     def run(self):
         """
-        This method run the AWS cost policies
+        This method run the ibm tag policies
         @return:
         """
-        logger.info(f'account={self._account}, policy={self._policy}')
-        cost_report_policy_module = importlib.import_module(f'cloud_governance.policy.aws.{self._policy}')
-        for cls in inspect.getmembers(cost_report_policy_module, inspect.isclass):
-            if self._policy.replace('_', '') == cls[0].lower():
-                response = cls[1]().run()
-                if response:
-                    logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
+        logger.info(f'account={self._account}, policy={self._policy}, dry_run={self._dry_run}, tag_operation={self._tag_operation}')
+        if self._policy.startswith('tag') or self._policy.startswith('remove'):
+            tag_ibm_policy_module = importlib.import_module(f'cloud_governance.policy.ibm.{self._policy}')
+            for cls in inspect.getmembers(tag_ibm_policy_module, inspect.isclass):
+                if self._policy.replace('_', '') == cls[0].lower():
+                    response = cls[1]().run()
+                    if len(response) > 0:
+                        logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from cloud_governance.policy.policy_operations.aws.dynamodb_upload_data.upload_data_to_dynamodb import UploadDataToDynamoDb
+from cloud_governance.aws.dynamodb_upload_data.upload_data_to_dynamodb import UploadDataToDynamoDb
 
 
 class CloudTrailToDynamoDb(UploadDataToDynamoDb):
     """
     This class upload cloudtrail data to dynamodb
     """
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `cloud-governance-1.1.9/cloud_governance/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,31 @@
+import os
 from datetime import datetime, timedelta
 
 import boto3
 
 from cloud_governance.common.clouds.aws.cloudtrail.cloudtrail_operations import CloudTrailOperations
 from cloud_governance.common.clouds.aws.dynamodb.dynamodb_operations import DynamoDbOperations
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class UploadDataToDynamoDb:
     """
     This class is upload cloudtrail data to DynamoDb
     """
 
     def __init__(self):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self._region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
+        self._region = os.environ.get('AWS_DEFAULT_REGION', 'ap-northeast-1')
         self._db_client = boto3.client('dynamodb', region_name=self._region)
         self._db_operations = DynamoDbOperations(region_name=self._region)
-        self._table_name = self.__environment_variables_dict.get('TABLE_NAME', '')
+        self._table_name = os.environ.get('TABLE_NAME', 'test_data')
         self._end_time = datetime.now() - timedelta(days=0)
         self._start_time = self._end_time - timedelta(days=1)
         self._cloudtrail_operations = CloudTrailOperations(region_name=self._region)
 
-    def set_region(self, value: str):
-        self._region = value
-
-    def set_table_name(self, value: str):
-        self._table_name = value
-
     def __convert_datatime_to_timestamp_in_data(self, data: list):
         """
         This method convert datetime to timestamp
         @param data:
         @return:
         """
         for item in data:
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/remove_cluster_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from multiprocessing import Process, Queue
 
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_cluster.tag_cluster_operations import TagClusterOperations
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.remove_non_cluster_tags import RemoveNonClusterTags
+from cloud_governance.aws.tag_cluster.tag_cluster_operations import TagClusterOperations
+from cloud_governance.aws.tag_non_cluster.remove_non_cluster_tags import RemoveNonClusterTags
 
 
 class RemoveClusterTags(TagClusterOperations):
     """
     This class removes the tags of cluster resources
     """
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_cluster.remove_cluster_tags import RemoveClusterTags
-from cloud_governance.policy.policy_operations.aws.tag_cluster.tag_cluster_resouces import TagClusterResources
+from cloud_governance.aws.tag_cluster.remove_cluster_tags import RemoveClusterTags
+from cloud_governance.aws.tag_cluster.tag_cluster_resouces import TagClusterResources
 
 
 def tag_cluster_resource(cluster_name: str = '', mandatory_tags: dict = None, region: str = 'us-east-2', tag_operation: str = 'yes', cluster_only: bool = False):
     """
     This method scan for cluster name in all the cluster resources
     :return: list of cluster resources according to cluster name
     """
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_cluster.tag_cluster_operations import TagClusterOperations
+from cloud_governance.aws.tag_cluster.tag_cluster_operations import TagClusterOperations
 
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.tag_non_cluster_resources import TagNonClusterResources
+from cloud_governance.aws.tag_non_cluster.tag_non_cluster_resources import TagNonClusterResources
 
 
 class TagClusterResources(TagClusterOperations):
     """
     This class filter cluster resources by cluster name, and update tags when passing input_tags
     """
 
@@ -244,29 +244,32 @@
         """
         cluster_instances = {}
         result_instance_list = []
         cluster_tags = {}
         for instance in resources:
             for item in instance:
                 instance_id = item['InstanceId']
-                tags = item.get('Tags')
-                if tags:
+                if item.get('Tags'):
                     # search that not exist permanent tags in the resource
-                    if not self.__validate_existing_tag(tags):
-                        for tag in tags:
+                    if not self.__validate_existing_tag(item.get('Tags')):
+                        for tag in item['Tags']:
                             if self.cluster_prefix in tag.get('Key'):
                                 add_tags = self.__append_input_tags()
                                 cluster_name = tag.get('Key').split('/')[-1]
                                 if cluster_name in cluster_instances:
-                                    add_tags = self.__filter_resource_tags_by_add_tags(tags=tags, search_tags=cluster_tags[cluster_name])
+                                    add_tags = self.__filter_resource_tags_by_add_tags(tags=item.get('Tags'),
+                                                                                       search_tags=cluster_tags[
+                                                                                           cluster_name])
                                     if add_tags:
                                         cluster_instances[cluster_name].append(instance_id)
                                     break
                                 else:
-                                    username = self.get_username(start_time=item.get('LaunchTime'), resource_id=instance_id, resource_type='AWS::EC2::Instance', tags=tags)
+                                    username = self._get_username_from_instance_id_and_time(
+                                        start_time=item.get('LaunchTime'), resource_id=instance_id,
+                                        resource_type='AWS::EC2::Instance')
                                     if username:
                                         if username == 'AutoScaling':
                                             add_tags.extend(self._fill_na_tags(user=username))
                                             logger.info(f'Autoscaling instance :: {instance_id}')
                                         else:
                                             user_tags = self.iam_operations.get_user_tags(username=username)
                                             if not self.__check_user_in_username_tags(user_tags):
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,210 +1,160 @@
 from datetime import datetime
 
-import boto3
+from cloud_governance.common.logger.init_logger import logger
+from cloud_governance.aws.tag_non_cluster.non_cluster_operations import NonClusterOperations
 
-from cloud_governance.common.clouds.aws.cloudtrail.cloudtrail_operations import CloudTrailOperations
-from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
-from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
-from cloud_governance.common.clouds.aws.utils.utils import Utils
 
-
-class NonClusterOperations:
+class RemoveNonClusterTags(NonClusterOperations):
 
     def __init__(self, region: str = 'us-east-2', dry_run: str = 'yes', input_tags: dict = ''):
-        self.region = region
-        self.dry_run = dry_run
-        self.input_tags = input_tags
-        self.cloudtrail = boto3.client('cloudtrail', region_name=region)
-        self.cluster_prefix = 'kubernetes.io/cluster/'
-        self.ec2_client = boto3.client('ec2', region_name=region)
-        self.cloudtrail = CloudTrailOperations(region_name=self.region)
-        self.iam_client = IAMOperations()
-        self.ec2_operations = EC2Operations(region=region)
-        self.utils = Utils(region=region)
-        self.iam_users = self.iam_client.get_iam_users_list()
-
-    def _get_instances_data(self, instance_id: str = ''):
-        """
-        This method go over all instances
-        :return:
-        """
-        ec2s_data = self.ec2_operations.get_instances()
-        if instance_id:
-            for items in ec2s_data:
-                if items.get('Instances'):
-                    for item in items['Instances']:
-                        if item.get('InstanceId') == instance_id:
-                            return items['Instances']
-        else:
-            instances_list = []
-            for items in ec2s_data:
-                if items.get('Instances'):
-                    instances_list.append(items['Instances'])
-            return instances_list
-
-    def _append_input_tags(self):
-        """
-        This method build tags list according to input tags dictionary
-        @return:
-        """
-        tags_list = []
-        for key, value in self.input_tags.items():
-            tags_list.append({'Key': key, 'Value': value})
-        return tags_list
+        super().__init__(region=region, dry_run=dry_run, input_tags=input_tags)
 
-    def _get_tags_of_resources(self, tags: list, search_tags: list):
+    def __get_instance_tags(self, launch_time: datetime, instance_id: str, tags: list):
         """
-        This method extracts tags from the resource tags
+        This method returns the tags to update  the instance tags
+        @param launch_time:
+        @param instance_id:
         @param tags:
-        @param search_tags:
-        @return:
-        """
-        add_tags = []
-        if tags:
-            for search_tag in search_tags:
-                found = False
-                for tag in tags:
-                    if tag.get('Key') == search_tag.get('Key'):
-                        found = True
-                if not found:
-                    add_tags.append(search_tag)
-        else:
-            add_tags.extend(search_tags)
-        return add_tags
-
-    def _fill_na_tags(self, user: str = None):
-        """
-        This method fill NA tags
-        @param user:
-        @return:
-        """
-        tags = []
-        keys = ['User', 'Owner', 'Manager', 'Project', 'Environment', 'Email']
-        value = 'NA'
-        for key in keys:
-            if user and key == 'User':
-                tags.append({'Key': key, 'Value': user})
-            elif user and key == 'Email':
-                tags.append({'Key': key, 'Value': f'{user}@redhat.com'})
-            else:
-                tags.append({'Key': key, 'Value': value})
-        return tags
-
-    def _get_username_from_cloudtrail(self, start_time: datetime, resource_id: str, resource_type: str):
-        """
-        This method return username fom cloudtrail
-        @param start_time:
-        @param resource_id:
-        @param resource_type:
-        @return:
-        """
-        return self.cloudtrail.get_username_by_instance_id_and_time(start_time=start_time, resource_id=resource_id, resource_type=resource_type)
-
-    def _get_resource_data(self, resource_method: callable):
-        """
-        This method returns the resource_data
         @return:
         """
-        resource_data = resource_method()
-        if 'ec2_operations' not in str(resource_method):
-            _, resource_list = self.ec2_operations.scan_cluster_or_non_cluster_instance(resource_data)
-        else:
-            _, resource_list = self.ec2_operations.scan_cluster_non_cluster_resources(resource_data)
-        return resource_list
-
-    def _convert_datetime_format(self, date_time: datetime):
-        """
-        This method convert datetime to YYYY/MM/DD H:M:S
-        @param date_time:
-        @return:
-        """
-        return date_time.strftime('%Y/%m/%d %H:%M:%S')
-
-    def _build_tag(self, key: str, value: any):
-        """
-        This method return Key value pair
-        @param key:
-        @param value:
-        @return:
-        """
-        if isinstance(value, datetime):
-            value = self._convert_datetime_format(date_time=value)
-        return {'Key': key, 'Value': value}
-
-    def _get_tags_from_instance_item(self, instance_item: dict):
-        tags = []
-        username = ''
-        if instance_item.get('Tags'):
-            tags.extend(
-                [tag for tag in instance_item.get('Tags') if not tag.get('Key') == 'Name'])
-            for tag in instance_item.get('Tags'):
-                if tag.get('Key') == 'User':
-                    username = tag.get('Value')
-                elif tag.get('Key') == 'LaunchTime':
-                    tags.append({'Key': 'LaunchTime', 'Value': tag.get('Key')})
+        username = self._get_username_from_cloudtrail(start_time=launch_time, resource_id=instance_id, resource_type='AWS::EC2::Instance')
+        search_tags = []
+        user_tags = self.iam_client.get_user_tags(username=username)
         if not username:
-            tags.extend(self._append_input_tags())
-            username = self._get_username_from_cloudtrail(start_time=instance_item.get('LaunchTime'),
-                                                          resource_id=instance_item.get('InstanceId'),
-                                                          resource_type='AWS::EC2::Instance')
-            launch_time = instance_item.get('LaunchTime')
-            tags.append(self._build_tag(key='LaunchTime', value=launch_time))
-        return tags, username
-
-    def _get_tags_fom_attachments(self, attachments: list):
-        """
-        This method return tags from attachments
-        @param attachments:
-        @return:
-        """
-        tags = []
-        username = ''
-        if attachments:
-            for attachment in attachments:
-                for item in self._get_instances_data(attachment.get('InstanceId')):
-                    item_tags, username = self._get_tags_from_instance_item(instance_item=item)
+            search_tags.extend(self._fill_na_tags())
         else:
-            tags.extend(self._append_input_tags())
-        return tags, username
-
-    def _get_tags_from_snapshot_description_images(self, description: str):
-        tags = []
-        username = ''
-        if description and 'Created' in description:
-            image_id = description.split(" ")[-1]
-            images = self.ec2_client.describe_images(Owners=['self'])['Images']
-            for image in images:
-                if image.get('ImageId') == image_id:
-                    if image.get('tags'):
-                        tags.extend(
-                            [tag for tag in image.get('Tags') if not tag.get('Key') == "Name"])
-                    else:
-                        tags.extend(self._append_input_tags())
-                    start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
-                    username = self._get_username_from_cloudtrail(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami')
-        return tags, username
-
-    def get_user_name_from_name_tag(self, tags: list = None, resource_name: str = None):
-        """
-        This method retuns the username from the name tag verified  with iam users
-        :param resource_name:
-        :param tags:
-        :return:
-        """
-        name_tag = self.ec2_operations.get_tag_value_from_tags(tags=tags, tag_name='Name') if tags else resource_name
-        for user in self.iam_users:
-            if user in name_tag:
-                return user
-        return None
-
-    def get_username(self, start_time: datetime, resource_id: str, resource_type: str, tags: list, resource_name: str = ''):
-        """
-        This method returns the username
-        :return:
-        """
-        iam_username = self.get_user_name_from_name_tag(tags=tags, resource_name=resource_name)
-        if not iam_username:
-            iam_username = self.get_user_name_from_name_tag(resource_name=resource_name)
-            if not iam_username:
-                return self._get_username_from_cloudtrail(start_time=start_time, resource_id=resource_id, resource_type=resource_type)
-        return iam_username
+            search_tags.append(self._build_tag(key='Email', value=f'{username}@redhat.com'))
+        search_tags.append(self._build_tag(key='LaunchTime', value=launch_time))
+        search_tags.extend(self._append_input_tags())
+        search_tags.extend(user_tags)
+        return search_tags
+
+    def non_cluster_update_ec2(self, instances_list: list = None):
+        """
+        This method removes the tags of ec2 instances
+        @return:
+        """
+        if not instances_list:
+            instances_list = self._get_resource_data(resource_method=self._get_instances_data)
+        instances_ids = []
+        for instance in instances_list:
+            for item in instance:
+                instance_id = item.get('InstanceId')
+                launch_time = item.get('LaunchTime')
+                add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=item.get('Tags'))
+                if add_tags:
+                    if self.dry_run == 'no':
+                        self.ec2_client.delete_tags(Resources=[instance_id], Tags=add_tags)
+                        logger.info(f'Delete tags of instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
+                    instances_ids.append(instance_id)
+        logger.info(f'non_cluster_ec2 count: {len(sorted(instances_ids))} {sorted(instances_ids)}')
+        return sorted(instances_ids)
+
+    def update_volumes(self, volumes_data: list = None):
+        """
+        This method removes the tags of non-cluster volumes
+        @param volumes_data:
+        @return:
+        """
+        if not volumes_data:
+            volumes_data = self._get_resource_data(resource_method=self.ec2_operations.get_volumes)
+        volume_ids = []
+        for volume in volumes_data:
+            volume_id = volume.get('VolumeId')
+            tag_name = ''
+            username = self._get_username_from_cloudtrail(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume')
+            search_tags = []
+            if not username:
+                get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
+                search_tags.extend(get_tags)
+            else:
+                search_tags.extend(self._append_input_tags())
+            if username and not tag_name:
+                user_tags = self.iam_client.get_user_tags(username=username)
+                search_tags.extend(user_tags)
+                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+            else:
+                search_tags.extend(self._fill_na_tags())
+                search_tags.extend(self._append_input_tags())
+                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+            if search_tags:
+                if self.dry_run == 'no':
+                    self.ec2_client.delete_tags(Resources=[volume_id], Tags=search_tags)
+                    logger.info(f'Remove tags of volume_id: {volume_id} total: {len(search_tags)}  tags: {search_tags}')
+                volume_ids.append(volume_id)
+        logger.info(f'non_cluster_volumes count: {len(sorted(volume_ids))} {sorted(volume_ids)}')
+        return sorted(volume_ids)
+
+    def update_snapshots(self, snapshots: list = None):
+        """
+        This method removes the tags of  non-cluster snapshots
+        @param snapshots:
+        @return:
+        """
+        if not snapshots:
+            snapshots = self._get_resource_data(resource_method=self.ec2_operations.get_snapshots)
+        snapshot_ids = []
+        for snapshot in snapshots:
+            snapshot_id = snapshot.get('SnapshotId')
+            username = self._get_username_from_cloudtrail(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot')
+            search_tags = []
+            if not username:
+                if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
+                    image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
+                    if not username:
+                        instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
+                        instances = self._get_instances_data(instance_id)
+                        if instances:
+                            for item in instances:
+                                if item.get('InstanceId') == instance_id:
+                                    item_tags, username = self._get_tags_from_instance_item(instance_item=item)
+            else:
+                search_tags.extend(self._append_input_tags())
+            if username:
+                user_tags = self.iam_client.get_user_tags(username=username)
+                search_tags.extend(user_tags)
+                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+            else:
+                search_tags.extend(self._fill_na_tags())
+                search_tags.extend(self._append_input_tags())
+            search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
+            if search_tags:
+                if self.dry_run == 'no':
+                    self.ec2_client.delete_tags(Resources=[snapshot_id], Tags=search_tags)
+                    logger.info(
+                        f'Remove tags of snapshots: {snapshot_id} total: {len(search_tags)} tags: {search_tags}')
+                snapshot_ids.append(snapshot_id)
+        logger.info(f'non_cluster_snapshot count: {len(sorted(snapshot_ids))} {sorted(snapshot_ids)}')
+        return sorted(snapshot_ids)
+
+    def update_ami(self, images: list = None):
+        """
+        This method removes the tags of non-cluster Amazon Machine Images
+        @param images:
+        @return:
+        """
+        if not images:
+            images = self.ec2_operations.get_images()
+            _, images = self.ec2_operations.scan_cluster_non_cluster_resources(images)
+        image_ids = []
+        for image in images:
+            image_id = image.get('ImageId')
+            start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
+            username = self._get_username_from_cloudtrail(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami')
+            search_tags = []
+            search_tags.extend(self._append_input_tags())
+            if username:
+                user_tags = self.iam_client.get_user_tags(username=username)
+                search_tags.extend(user_tags)
+                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+            else:
+                search_tags.extend(self._fill_na_tags())
+            search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
+            if search_tags:
+                if self.dry_run == 'no':
+                    self.ec2_client.delete_tags(Resources=[image_id], Tags=search_tags)
+                    logger.info(f'Remove tags of image: {image_id} total: {len(search_tags)} tags: {search_tags}')
+                image_ids.append(image_id)
+        logger.info(f'non_cluster_amis count: {len(sorted(image_ids))} {sorted(image_ids)}')
+        return sorted(image_ids)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,136 @@
 from datetime import datetime
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.non_cluster_operations import NonClusterOperations
+from cloud_governance.aws.tag_non_cluster.non_cluster_operations import NonClusterOperations
 
 
-class RemoveNonClusterTags(NonClusterOperations):
+class TagNonClusterResources(NonClusterOperations):
+    """
+    This class update tags of Non-Cluster Resources
+    """
+    
+    SHORT_RESOURCE_ID = 5
+    SHORT_RESOURCE_NAME = 3
+    SHOT_SNAPSHOT_ID = 4
 
     def __init__(self, region: str = 'us-east-2', dry_run: str = 'yes', input_tags: dict = ''):
         super().__init__(region=region, dry_run=dry_run, input_tags=input_tags)
 
+    def __check_name_in_tags(self, tags: list):
+        """
+        This method check name in tags
+        @param tags:
+        @return:
+        """
+        if tags:
+            for tag in tags:
+                if tag.get('Key') == 'Name':
+                    return True
+        return False
+
     def __get_instance_tags(self, launch_time: datetime, instance_id: str, tags: list):
         """
         This method returns the tags to update  the instance tags
         @param launch_time:
         @param instance_id:
         @param tags:
         @return:
         """
         username = self._get_username_from_cloudtrail(start_time=launch_time, resource_id=instance_id, resource_type='AWS::EC2::Instance')
         search_tags = []
-        user_tags = self.iam_client.get_user_tags(username=username)
+        user_tags = []
         if not username:
             search_tags.extend(self._fill_na_tags())
         else:
             search_tags.append(self._build_tag(key='Email', value=f'{username}@redhat.com'))
+            user_tags = self.iam_client.get_user_tags(username=username)
+            if not user_tags:
+                search_tags.extend(self._fill_na_tags(user=username))
+        if not self.__check_name_in_tags(tags):
+            tag_name = f'{username}-{instance_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{instance_id[0:1]}-{self.region}-{instance_id[-self.SHORT_RESOURCE_ID:]}'
+            search_tags.append(self._build_tag(key='cg-Name', value=tag_name))
         search_tags.append(self._build_tag(key='LaunchTime', value=launch_time))
         search_tags.extend(self._append_input_tags())
         search_tags.extend(user_tags)
-        return search_tags
+        add_tags = self._get_tags_of_resources(tags=tags, search_tags=search_tags)
+        return add_tags
 
     def non_cluster_update_ec2(self, instances_list: list = None):
         """
-        This method removes the tags of ec2 instances
+        This method tagged the ec2 instances without having tags
         @return:
         """
         if not instances_list:
             instances_list = self._get_resource_data(resource_method=self._get_instances_data)
         instances_ids = []
         for instance in instances_list:
             for item in instance:
                 instance_id = item.get('InstanceId')
                 launch_time = item.get('LaunchTime')
                 add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=item.get('Tags'))
                 if add_tags:
                     if self.dry_run == 'no':
-                        self.ec2_client.delete_tags(Resources=[instance_id], Tags=add_tags)
-                        logger.info(f'Delete tags of instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
+                        try:
+                            self.ec2_client.create_tags(Resources=[instance_id], Tags=add_tags)
+                            logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
+                        except Exception as err:
+                            logger.info(err)
                     instances_ids.append(instance_id)
         logger.info(f'non_cluster_ec2 count: {len(sorted(instances_ids))} {sorted(instances_ids)}')
         return sorted(instances_ids)
 
     def update_volumes(self, volumes_data: list = None):
         """
-        This method removes the tags of non-cluster volumes
+        This method updates the tags of non-cluster volumes
         @param volumes_data:
         @return:
         """
         if not volumes_data:
             volumes_data = self._get_resource_data(resource_method=self.ec2_operations.get_volumes)
         volume_ids = []
         for volume in volumes_data:
             volume_id = volume.get('VolumeId')
-            tag_name = ''
             username = self._get_username_from_cloudtrail(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume')
             search_tags = []
             if not username:
                 get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
                 search_tags.extend(get_tags)
             else:
                 search_tags.extend(self._append_input_tags())
-            if username and not tag_name:
+            if username:
                 user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.extend(user_tags)
-                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                if not user_tags:
+                    search_tags.extend(self._fill_na_tags(user=username))
+                else:
+                    search_tags.extend(user_tags)
+                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
                 search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
             else:
                 search_tags.extend(self._fill_na_tags())
                 search_tags.extend(self._append_input_tags())
                 search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
-            if search_tags:
+            if not self.__check_name_in_tags(volume.get('Tags')):
+                tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
+                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+            volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
+            if volume_tags:
                 if self.dry_run == 'no':
-                    self.ec2_client.delete_tags(Resources=[volume_id], Tags=search_tags)
-                    logger.info(f'Remove tags of volume_id: {volume_id} total: {len(search_tags)}  tags: {search_tags}')
+                    try:
+                        self.ec2_client.create_tags(Resources=[volume_id], Tags=volume_tags)
+                        logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
+                    except Exception as err:
+                        logger.info(err)
                 volume_ids.append(volume_id)
         logger.info(f'non_cluster_volumes count: {len(sorted(volume_ids))} {sorted(volume_ids)}')
         return sorted(volume_ids)
 
     def update_snapshots(self, snapshots: list = None):
         """
-        This method removes the tags of  non-cluster snapshots
+        This method updates the tags of  non-cluster snapshots
         @param snapshots:
         @return:
         """
         if not snapshots:
             snapshots = self._get_resource_data(resource_method=self.ec2_operations.get_snapshots)
         snapshot_ids = []
         for snapshot in snapshots:
@@ -109,32 +147,41 @@
                             for item in instances:
                                 if item.get('InstanceId') == instance_id:
                                     item_tags, username = self._get_tags_from_instance_item(instance_item=item)
             else:
                 search_tags.extend(self._append_input_tags())
             if username:
                 user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.extend(user_tags)
                 search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                if not user_tags:
+                    search_tags.extend(self._fill_na_tags(user=username))
+                else:
+                    search_tags.extend(user_tags)
             else:
                 search_tags.extend(self._fill_na_tags())
                 search_tags.extend(self._append_input_tags())
+            if not self.__check_name_in_tags(snapshot.get('Tags')):
+                tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
+                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
             search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
-            if search_tags:
+            snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
+            if snapshot_tags:
                 if self.dry_run == 'no':
-                    self.ec2_client.delete_tags(Resources=[snapshot_id], Tags=search_tags)
-                    logger.info(
-                        f'Remove tags of snapshots: {snapshot_id} total: {len(search_tags)} tags: {search_tags}')
+                    try:
+                        self.ec2_client.create_tags(Resources=[snapshot_id], Tags=snapshot_tags)
+                        logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
+                    except Exception as err:
+                        logger.info(err)
                 snapshot_ids.append(snapshot_id)
         logger.info(f'non_cluster_snapshot count: {len(sorted(snapshot_ids))} {sorted(snapshot_ids)}')
         return sorted(snapshot_ids)
 
     def update_ami(self, images: list = None):
         """
-        This method removes the tags of non-cluster Amazon Machine Images
+        This method update the tags of non-cluster Amazon Machine Images
         @param images:
         @return:
         """
         if not images:
             images = self.ec2_operations.get_images()
             _, images = self.ec2_operations.scan_cluster_non_cluster_resources(images)
         image_ids = []
@@ -142,19 +189,29 @@
             image_id = image.get('ImageId')
             start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
             username = self._get_username_from_cloudtrail(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami')
             search_tags = []
             search_tags.extend(self._append_input_tags())
             if username:
                 user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.extend(user_tags)
                 search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                if not user_tags:
+                    search_tags.extend(self._fill_na_tags(user=username))
+                else:
+                    search_tags.extend(user_tags)
             else:
                 search_tags.extend(self._fill_na_tags())
+            if not self.__check_name_in_tags(image.get('Tags')):
+                tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
+                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
             search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
-            if search_tags:
+            image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
+            if image_tags:
                 if self.dry_run == 'no':
-                    self.ec2_client.delete_tags(Resources=[image_id], Tags=search_tags)
-                    logger.info(f'Remove tags of image: {image_id} total: {len(search_tags)} tags: {search_tags}')
+                    try:
+                        self.ec2_client.create_tags(Resources=[image_id], Tags=image_tags)
+                        logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
+                    except Exception as err:
+                        logger.info(err)
                 image_ids.append(image_id)
         logger.info(f'non_cluster_amis count: {len(sorted(image_ids))} {sorted(image_ids)}')
         return sorted(image_ids)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.remove_non_cluster_tags import RemoveNonClusterTags
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.tag_non_cluster_resources import TagNonClusterResources
-from cloud_governance.policy.policy_operations.aws.tag_non_cluster.update_na_tag_resources import UpdateNATags
+from cloud_governance.aws.tag_non_cluster.remove_non_cluster_tags import RemoveNonClusterTags
+from cloud_governance.aws.tag_non_cluster.tag_non_cluster_resources import TagNonClusterResources
+from cloud_governance.aws.tag_non_cluster.update_na_tag_resources import UpdateNATags
 
 
 def tag_non_cluster_resource(mandatory_tags: dict, region: str, tag_operation: str = 'read'):
     if tag_operation == 'update':
         action = 'Tag'
         dry_run = 'no'
     else:
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_user/run_tag_iam_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+import os
 
 from cloud_governance.common.google_drive.google_drive_operations import GoogleDriveOperations
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.tag_user.iam_user_tags import ValidateIAMUserTags
-from cloud_governance.policy.policy_operations.aws.tag_user.remove_user_tags import RemoveUserTags
-from cloud_governance.policy.policy_operations.aws.tag_user.tag_iam_user import TagUser
-from cloud_governance.main.environment_variables import environment_variables
+from cloud_governance.aws.tag_user.iam_user_tags import ValidateIAMUserTags
+from cloud_governance.aws.tag_user.remove_user_tags import RemoveUserTags
+from cloud_governance.aws.tag_user.tag_iam_user import TagUser
 
 
 def tag_iam_user(user_tag_operation: str, remove_keys: list, username: str = '', file_name: str = 'tag_user.csv'):
     """
     This method fetch the users from account and writes to the csv file if user_type = csv
     else   updated the tags of user from the csv file if user_type = update
     @param user_tag_operation:
     @param username:
     @param remove_keys:
     @param file_name:
     @return:
     """
-    environment_variables_dict = environment_variables.environment_variables_dict
-    account_name = environment_variables_dict.get("account", '').upper()
-    spreadsheet_id = environment_variables_dict.get('SPREADSHEET_ID', '')
+    account_name = os.environ.get("account", '').upper()
+    spreadsheet_id = os.environ.get('SPREADSHEET_ID', '')
     if user_tag_operation == 'update' and not file_name and spreadsheet_id:
         google_drive = GoogleDriveOperations()
         google_drive.download_spreadsheet(spreadsheet_id=spreadsheet_id, sheet_name=account_name, file_path='/tmp')
         file_name = f'{account_name}.csv'
     if not file_name:
         file_name = 'tag_user.csv'
     file_path = f'/tmp/{file_name}'
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `cloud-governance-1.1.9/cloud_governance/aws/tag_user/tag_iam_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import csv
+import os
 import re
 from ast import literal_eval
 
 import boto3
 import pandas as pd
 
 from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 from cloud_governance.common.google_drive.google_drive_operations import GoogleDriveOperations
 from cloud_governance.common.ldap.ldap_search import LdapSearch
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.common.mails.mail_message import MailMessage
 from cloud_governance.common.mails.postfix import Postfix
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class TagUser:
     """
     Tag user in the AWS account
     """
 
     def __init__(self, file_name: str):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.iam_client = boto3.client('iam')
         self.get_detail_resource_list = Utils().get_details_resource_list
         self.IAMOperations = IAMOperations()
         self.file_name = file_name
-        self.__SPREADSHEET_ID = self.__environment_variables_dict.get('SPREADSHEET_ID', '')
-        self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
+        self.__SPREADSHEET_ID = os.environ.get('SPREADSHEET_ID', '')
+        self.__ldap_host_name = os.environ.get('LDAP_HOST_NAME', '')
         self.__ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
-        self._special_user_mails = self.__literal_eval(self.__environment_variables_dict.get('special_user_mails', '{}'))
+        self._special_user_mails = self.__literal_eval(os.environ.get('special_user_mails', '{}'))
         if self.__SPREADSHEET_ID:
             self.__google_drive_operations = GoogleDriveOperations()
-            self.__sheet_name = self.__environment_variables_dict.get('account', '')
+            self.__sheet_name = os.environ.get('account', '')
             self.__mail = Postfix()
 
+
     def __literal_eval(self, data: any):
         if data:
             return literal_eval(data)
         return data
 
     def __cluster_user(self, tags: list):
         """
@@ -241,14 +241,14 @@
         """
         This method send mail
         @param user:
         @return:
         """
         to = user if user not in self._special_user_mails else self._special_user_mails[user]
         ldap_data = self.__ldap.get_user_details(user_name=to)
-        cc = [self.__environment_variables_dict.get("account_admin", '')]
+        cc = [os.environ.get("account_admin", '')]
         name = to
         if ldap_data:
             cc.append(f'{ldap_data.get("managerId")}@redhat.com')
             name = ldap_data.get('displayName')
         subject, body = MailMessage().iam_user_add_tags(name=name, user=user, spreadsheet_id=self.__SPREADSHEET_ID)
         self.__mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,17 +161,16 @@
                                     logger.info(f'delete_load_balancer: {resource_id}')
                                 except Exception as err:
                                     logger.exception(f'Cannot delete_load_balancer: {resource_id}, {err}')
 
     @typeguard.typechecked
     def __delete_volume(self, resource_id: str):
         try:
-            logger.info(f'Cluster volumes are handled by ebs_unattached')
-            # self.client.delete_volume(VolumeId=resource_id)
-            # logger.info(f'delete_volume: {resource_id}')
+            self.client.delete_volume(VolumeId=resource_id)
+            logger.info(f'delete_volume: {resource_id}')
         except Exception as err:
             logger.exception(f'Cannot delete_volume: {resource_id}, {err}')
 
     @typeguard.typechecked
     def __delete_snapshots(self, resource_id: str):
         try:
             self.client.delete_snapshot(SnapshotId=resource_id)
@@ -257,39 +256,30 @@
         :param resource_id:
         :return:
         """
         try:
             security_groups = self.ec2_operations.get_security_groups()
             vpc_security_groups = self.__get_cluster_references(resource_id=vpc_id, resource_list=security_groups, input_resource_id='VpcId', output_result='')
             for vpc_security_group in vpc_security_groups:
-                if resource_id != vpc_security_group.get('GroupId'):
-                    if vpc_security_group.get('GroupName') == 'default':
-                        logger.info(f'Removing the {resource_id} ingress rule from Default Security Group: {vpc_security_group.get("GroupId")}')
-                        if vpc_security_group.get('IpPermissions'):
-                            for ip_permission in vpc_security_group.get('IpPermissions'):
-                                if ip_permission.get('UserIdGroupPairs'):
-                                    for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
-                                        if user_id_group_pair.get('GroupId') == resource_id:
-                                            ingress_rule = {'FromPort': ip_permission.get('FromPort'), 'IpProtocol': ip_permission.get('IpProtocol'), 'IpRanges': ip_permission.get('IpRanges'), 'Ipv6Ranges': ip_permission.get('Ipv6Ranges'), 'PrefixListIds': ip_permission.get('PrefixListIds'), 'ToPort': ip_permission.get('ToPort'), 'UserIdGroupPairs': [user_id_group_pair]}
-                                            self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ingress_rule])
-                                            logger.info(f'Removed the Ingress rules of Security Group {vpc_security_group.get("GroupId")} :: {ingress_rule}')
-                    else:
-                        if vpc_security_group.get('Tags'):
-                            if self.__is_cluster_resource(tags=vpc_security_group.get('Tags'), cluster_tag=self.cluster_tag):
-                                logger.info(vpc_security_group.get('GroupId'))
-                                if vpc_security_group.get('IpPermissions'):
-                                    for ip_permission in vpc_security_group.get('IpPermissions'):
-                                        if ip_permission.get('UserIdGroupPairs'):
-                                            for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
-                                                if user_id_group_pair.get('GroupId') == resource_id:
-                                                    ingress_rule = {'FromPort': ip_permission.get('FromPort'), 'IpProtocol': ip_permission.get('IpProtocol'), 'IpRanges': ip_permission.get('IpRanges'),
-                                                                    'Ipv6Ranges': ip_permission.get('Ipv6Ranges'), 'PrefixListIds': ip_permission.get('PrefixListIds'),
-                                                                    'ToPort': ip_permission.get('ToPort'), 'UserIdGroupPairs': [user_id_group_pair]}
-                                                    self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ingress_rule])
-                                                    logger.info(f'Removed the Ingress rules of Security Group {resource_id} from {ingress_rule}')
+                if vpc_security_group.get('GroupName') == 'default':
+                    if vpc_security_group.get('IpPermissions'):
+                        for ip_permission in vpc_security_group.get('IpPermissions'):
+                            self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ip_permission])
+                            logger.info(f'Removed the Ingress rules of Security Group {resource_id} :: {ip_permission}')
+                else:
+                    if vpc_security_group.get('Tags'):
+                        if self.__is_cluster_resource(tags=vpc_security_group.get('Tags'), cluster_tag=self.cluster_tag):
+                            logger.info(vpc_security_group.get('GroupId'))
+                            if vpc_security_group.get('IpPermissions'):
+                                for ip_permission in vpc_security_group.get('IpPermissions'):
+                                    if ip_permission.get('UserIdGroupPairs'):
+                                        for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
+                                            if user_id_group_pair.get('GroupId') == resource_id:
+                                                self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ip_permission])
+                                                logger.info(f'Removed the Ingress rules of Security Group {resource_id} from {vpc_security_group.get("GroupId")}')
             network_interfaces = self.ec2_operations.get_network_interface()
             network_interface_ids = self.__get_cluster_references(resource_id=vpc_id, resource_list=network_interfaces,
                                                                   input_resource_id='VpcId',
                                                                   output_result='')
             default_security_group_id = [security_group.get('GroupId') for security_group in vpc_security_groups
                                          if security_group.get('GroupName') == 'default']
             if default_security_group_id:
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import os
 
 import typeguard
 
-from cloud_governance.policy.policy_operations.aws.zombie_cluster.zombie_cluster_common_methods import ZombieClusterCommonMethods
+from cloud_governance.aws.zombie_cluster.zombie_cluster_common_methods import ZombieClusterCommonMethods
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.policy.aws.zombie_cluster_resource import ZombieClusterResources
 
 
 @typeguard.typechecked
 def __get_resource_list(region, delete: bool = False, resource: str = '', cluster_tag: str = '',
                         resource_name: str = '', service_type: str = ' '):
+    global zombie_cluster_resources
     zombie_cluster_resources = ZombieClusterResources(cluster_prefix='kubernetes.io/cluster/', delete=delete,
                                                       region=region, cluster_tag=cluster_tag,
                                                       resource_name=resource_name)
     zombie_cluster_resources_dict = {'zombie_cluster_volume': zombie_cluster_resources.zombie_cluster_volume,
                                      'zombie_cluster_ami': zombie_cluster_resources.zombie_cluster_ami,
                                      'zombie_cluster_snapshot': zombie_cluster_resources.zombie_cluster_snapshot,
                                      'zombie_cluster_security_group': zombie_cluster_resources.zombie_cluster_security_group,
@@ -74,15 +75,14 @@
     if delete:
         return delete_func_resource_list
     else:
         return scan_func_resource_list
 
 
 @typeguard.typechecked
-@logger_time_stamp
 def zombie_cluster_resource(delete: bool = False, region: str = 'us-east-2', resource: str = '', cluster_tag: str = '',
                             resource_name: str = '', service_type: str = ''):
     """
     This method return zombie cluster resources,
     How its works? if not exist an instance cluster, the resource is zombie
     if delete true it will delete the zombie resource
     :return: list of zombie resources
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,44 +3,39 @@
 from ast import literal_eval
 from copy import deepcopy
 
 import boto3
 
 from cloud_governance.common.ldap.ldap_search import LdapSearch
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.common.mails.mail_message import MailMessage
 from cloud_governance.common.mails.postfix import Postfix
-from cloud_governance.main.environment_variables import environment_variables
 
 
 class ZombieClusterCommonMethods:
     DAYS_TO_TRIGGER_RESOURCE_MAIL = 4
     DAYS_TO_DELETE_RESOURCE = 7
 
-    def __init__(self, region: str, force_delete: bool = False):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
+    def __init__(self, region: str):
         self.region = region
-        self.dry_run = self.__environment_variables_dict.get('dry_run', 'yes')
-        self.policy = self.__environment_variables_dict.get('policy', '')
+        self.dry_run = os.environ.get('dry_run', 'yes')
+        self.policy = os.environ.get('policy', '')
         self.ec2_client = boto3.client('ec2', region_name=region)
         self.ec2_resource = boto3.resource('ec2', region_name=region)
         self.elb_client = boto3.client('elb', region_name=region)
         self.elbv2_client = boto3.client('elbv2', region_name=region)
         self.iam_client = boto3.client('iam', region_name=region)
         self.s3_client = boto3.client('s3')
         self.s3_resource = boto3.resource('s3')
-        self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
-        self._special_user_mails = self.__environment_variables_dict.get('special_user_mails', '{}')
-        self._account_admin = self.__environment_variables_dict.get('account_admin', '')
-        self.__email_alert = self.__environment_variables_dict.get('EMAIL_ALERT') if self.__environment_variables_dict.get('EMAIL_ALERT') else False
+        self.__ldap_host_name = os.environ.get('LDAP_HOST_NAME', '')
+        self._special_user_mails = os.environ.get('special_user_mails', '{}')
+        self._account_admin = os.environ.get('account_admin', '')
         self._ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
         self._mail = Postfix()
         self._mail_description = MailMessage()
-        self._force_delete = self.__environment_variables_dict.get('FORCE_DELETE') if self.__environment_variables_dict.get('FORCE_DELETE') else force_delete
 
     def _literal_eval(self, data: any):
         tags = {}
         if data:
             tags = literal_eval(data)
         return tags
 
@@ -82,50 +77,35 @@
         @return:
         """
         resources_tags = {}
         for resource in resources:
             aws_tags = []
             resource_id = resource.get(resource_id_name)
             if aws_service == 'elbv1':
-                try:
-                    aws_tags = self.elb_client.describe_tags(LoadBalancerNames=[resource_id]).get('TagDescriptions')
-                    if len(aws_tags) > 0:
-                        aws_tags = aws_tags[0].get(aws_tag)
-                except:
-                    return []
+                aws_tags = self.elb_client.describe_tags(LoadBalancerNames=[resource_id]).get('TagDescriptions')
+                if len(aws_tags) > 0:
+                    aws_tags = aws_tags[0].get(aws_tag)
             elif aws_service == 'elbv2':
-                try:
-                    aws_tags = self.elbv2_client.describe_tags(ResourceArns=[resource_id]).get('TagDescriptions')
-                    if len(aws_tags) > 0:
-                        aws_tags = aws_tags[0].get(aws_tag)
-                except:
-                    return []
+                aws_tags = self.elbv2_client.describe_tags(ResourceArns=[resource_id]).get('TagDescriptions')
+                if len(aws_tags) > 0:
+                    aws_tags = aws_tags[0].get(aws_tag)
             elif aws_service == 'role' and resource_id in zombies:
-                try:
-                    role_data = self.iam_client.get_role(RoleName=resource_id)['Role']
-                    if role_data.get(aws_tag):
-                        aws_tags = role_data.get(aws_tag)
-                except:
-                    return []
+                role_data = self.iam_client.get_role(RoleName=resource_id)['Role']
+                if role_data.get(aws_tag):
+                    aws_tags = role_data.get(aws_tag)
             elif aws_service == 'user' and resource_id in zombies:
-                try:
-                    user_data = self.iam_client.get_user(UserName=resource_id)['User']
-                    if user_data.get(aws_tag):
-                        aws_tags = user_data.get(aws_tag)
-                except Exception as err:
-                    return []
+                user_data = self.iam_client.get_user(UserName=resource_id)['User']
+                if user_data.get(aws_tag):
+                    aws_tags = user_data.get(aws_tag)
             elif aws_service == 'bucket' and resource_id in zombies:
-                try:
-                    bucket_data = self.s3_client.get_bucket_tagging(Bucket=resource_id)
-                    if bucket_data.get(aws_tag):
-                        aws_tags = bucket_data.get(aws_tag)
-                except Exception as err:
-                    return []
+                bucket_data = self.s3_client.get_bucket_tagging(Bucket=resource_id)
+                if bucket_data.get(aws_tag):
+                    aws_tags = bucket_data.get(aws_tag)
             else:
-                if resource.get(aws_tag) and resource_id in zombies:
+                if resource.get(aws_tag):
                     aws_tags = resource.get(aws_tag)
             if aws_tags:
                 old_tags = deepcopy(aws_tags)
                 tags = aws_tags[:]
                 cluster_delete_days = self.get_tag_name_from_tags(tags=tags, tag_name='ClusterDeleteDays')
                 if cluster_delete_days:
                     if resource_id in zombies:
@@ -133,29 +113,26 @@
                                                          tag_value=str(int(cluster_delete_days) + 1))
                     else:
                         tags = self.update_resource_tags(tags=tags, tag_name='ClusterDeleteDays', tag_value=str(0))
                 else:
                     if resource_id in zombies:
                         tags = self.update_resource_tags(tags=tags, tag_name='ClusterDeleteDays', tag_value=str(1))
                 if old_tags != tags:
-                    try:
-                        if aws_service == 'ec2':
-                            self.ec2_client.create_tags(Resources=[resource_id], Tags=tags)
-                        elif aws_service == 'elbv1':
-                            self.elb_client.add_tags(LoadBalancerNames=[resource_id], Tags=tags)
-                        elif aws_service == 'elbv2':
-                            self.elbv2_client.add_tags(ResourceArns=[resource_id], Tags=tags)
-                        elif aws_service == 'role':
-                            self.iam_client.tag_role(RoleName=resource_id, Tags=tags)
-                        elif aws_service == 'user':
-                            self.iam_client.tag_user(UserName=resource_id, Tags=tags)
-                        elif aws_service == 'bucket':
-                            self.s3_client.put_bucket_tagging(Bucket=resource_id, Tagging={'TagSet': tags})
-                    except:
-                        return []
+                    if aws_service == 'ec2':
+                        self.ec2_client.create_tags(Resources=[resource_id], Tags=tags)
+                    elif aws_service == 'elbv1':
+                        self.elb_client.add_tags(LoadBalancerNames=[resource_id], Tags=tags)
+                    elif aws_service == 'elbv2':
+                        self.elbv2_client.add_tags(ResourceArns=[resource_id], Tags=tags)
+                    elif aws_service == 'role':
+                        self.iam_client.tag_role(RoleName=resource_id, Tags=tags)
+                    elif aws_service == 'user':
+                        self.iam_client.tag_user(UserName=resource_id, Tags=tags)
+                    elif aws_service == 'bucket':
+                        self.s3_client.put_bucket_tagging(Bucket=resource_id, Tagging={'TagSet': tags})
                 if resource_id in zombies:
                     resources_tags[resource_id] = tags
         return resources_tags
 
     def update_resource_tags(self, tags: list, tag_name: str, tag_value: str):
         """
         This method updates tags of the resource
@@ -185,19 +162,17 @@
         cluster_delete_days = self.get_tag_name_from_tags(tags=tags, tag_name='ClusterDeleteDays')
         if not cluster_delete_days:
             cluster_delete_days = 1
         else:
             cluster_delete_days = int(cluster_delete_days) + 1
         return cluster_delete_days
 
-    @logger_time_stamp
-    def trigger_mail(self, tags: list, resource_id: str, days: int, resources: list, message_type: str):
+    def trigger_mail(self, tags: list, resource_id: str, days: int, resources: list):
         """
         This method send triggering mail
-        @param message_type:
         @param resources:
         @param days:
         @param tags:
         @param resource_id:
         @return:
         """
         try:
@@ -214,15 +189,15 @@
                 name = ldap_data.get('displayName')
             file_name = os.path.join('/tmp', f'{resource_name.replace("/", "-")}.json')
             with open(file_name, 'w') as file:
                 json.dump(resources, file, indent=4)
             subject, body = self._mail_description.zombie_cluster_mail_message(name=name, days=days,
                                                                                notification_days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
                                                                                resource_name=resource_name, delete_days=self.DAYS_TO_DELETE_RESOURCE)
-            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id, filename=file_name, message_type=message_type)
+            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id, filename=file_name)
         except Exception as err:
             logger.info(err)
 
     def collect_notify_cluster_data(self, resource_data: dict, cluster_left_out_days: dict, notify_data: dict,
                                     delete_data: dict, cluster_data: dict, func_name: str):
         """
         This method store the notify_data, delete_data of clusters
@@ -251,35 +226,32 @@
             if cluster_tag in cluster_left_out_days:
                 if cluster_tag in notify_tag_data:
                     notify_data.setdefault(cluster_tag, []).append({func_name: notify_tag_data[cluster_tag]})
                 if cluster_tag in delete_tag_data:
                     delete_data.setdefault(cluster_tag, []).append({func_name: delete_tag_data[cluster_tag]})
         return notify_data, delete_data, cluster_data
 
-    @logger_time_stamp
     def send_mails_to_cluster_user(self, notify_data: dict, delete_data: dict, cluster_data: dict):
         """
         This method send mail to the user to notify cluster status
         @param cluster_data:
         @param notify_data:
         @param delete_data:
         @return:
         """
-        if self.__email_alert:
-            for cluster_tag, resource_ids in notify_data.items():
-                self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
-                self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
-                                  days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
-                                  resources=resource_ids, message_type='notification')
-            for cluster_tag, resource_ids in delete_data.items():
-                self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
-                self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
-                                  days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids, message_type='delete')
+        for cluster_tag, resource_ids in notify_data.items():
+            self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
+            self.trigger_mail(tags=cluster_data[cluster_tag], resource_id='Cluster',
+                              days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
+                              resources=resource_ids)
+        for cluster_tag, resource_ids in delete_data.items():
+            self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
+            self.trigger_mail(tags=cluster_data[cluster_tag], resource_id='Cluster',
+                              days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids)
 
-    @logger_time_stamp
     def _check_zombie_cluster_deleted_days(self, resources: dict, cluster_left_out_days: dict, zombie: str, cluster_tag: str):
         """
         This method check the cluster delete days and return the clusters
         @param resources:
         @param cluster_left_out_days:
         @return:
         """
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,70 @@
+import os
 import datetime
 from ast import literal_eval
 
 import boto3
 
 from cloud_governance.common.clouds.aws.cloudtrail.cloudtrail_operations import CloudTrailOperations
 from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
-from cloud_governance.common.clouds.aws.price.resources_pricing import ResourcesPricing
 from cloud_governance.common.clouds.aws.s3.s3_operations import S3Operations
-from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
 from cloud_governance.common.ldap.ldap_search import LdapSearch
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.common.mails.mail_message import MailMessage
 from cloud_governance.common.mails.postfix import Postfix
-from cloud_governance.main.environment_variables import environment_variables
 from cloud_governance.policy.aws.zombie_cluster_resource import ZombieClusterResources
 
 
 class NonClusterZombiePolicy:
 
     DAYS_TO_DELETE_RESOURCE = 7
-    DAYS_TO_NOTIFY_ADMINS = 6
     DAYS_TO_TRIGGER_RESOURCE_MAIL = 4
-    DAILY_HOURS = 24
 
     def __init__(self):
-        self.__environment_variables_dict = environment_variables.environment_variables_dict
         self._end_date = datetime.datetime.now()
         self._start_date = self._end_date - datetime.timedelta(days=self.DAYS_TO_DELETE_RESOURCE)
-        self._account = self.__environment_variables_dict.get('account', '')
-        self._dry_run = self.__environment_variables_dict.get('dry_run', 'yes')
-        self._region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', 'us-east-2')
-        self._policy = self.__environment_variables_dict.get('policy', '')
-        self._policy_output = self.__environment_variables_dict.get('policy_output', '')
+        self._account = os.environ.get('account', '')
+        self._dry_run = os.environ.get('dry_run', 'yes')
+        self._region = os.environ.get('AWS_DEFAULT_REGION', 'us-east-2')
+        self._policy = os.environ.get('policy', '')
+        self._policy_output = os.environ.get('policy_output', '')
         self._ec2_client = boto3.client('ec2', region_name=self._region)
         self._ec2_operations = EC2Operations(region=self._region)
         self._s3_client = boto3.client('s3')
         self._iam_operations = IAMOperations()
         self._iam_client = boto3.client('iam')
         self._cluster_prefix = 'kubernetes.io/cluster'
         self._zombie_cluster = ZombieClusterResources(cluster_prefix=self._cluster_prefix)
         self._s3operations = S3Operations(region_name=self._region)
         self._cloudtrail = CloudTrailOperations(region_name=self._region)
-        self._special_user_mails = self.__environment_variables_dict.get('special_user_mails', '{}')
-        self._account_admin = self.__environment_variables_dict.get('account_admin', '')
+        self._special_user_mails = os.environ.get('special_user_mails', '{}')
+        self._account_admin = os.environ.get('account_admin', '')
         self._mail = Postfix()
         self._mail_description = MailMessage()
-        self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
+        self.__ldap_host_name = os.environ.get('LDAP_HOST_NAME', '')
         self._ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
-        self.__email_alert = self.__environment_variables_dict.get('EMAIL_ALERT') if self.__environment_variables_dict.get('EMAIL_ALERT') else False
-        self.__manager_email_alert = self.__environment_variables_dict.get('MANAGER_EMAIL_ALERT')
-        self._admins = ['athiruma@redhat.com', 'ebattat@redhat.com']
-        self._es_upload = ElasticUpload()
-        self.resource_pricing = ResourcesPricing()
-
-    def set_dryrun(self, value: str):
-        self._dry_run = value
-
-    def set_policy(self, value: str):
-        self._policy = value
-
-    def set_region(self, value: str):
-        self._region = value
+        self._active_clusters = self._zombie_cluster.all_cluster_instance()
 
     def _literal_eval(self, data: any):
         tags = {}
         if data:
             tags = literal_eval(data)
         return tags
 
-    def _check_cluster_tag(self, tags: list):
+    def _check_live_cluster_tag(self, tags: list):
         """
         This method returns True if it is live cluster tag is active False not
         @param tags:
         @return:
         """
         if tags:
             for tag in tags:
                 if tag.get('Key').startswith(self._cluster_prefix):
-                    return True
+                    return tag.get('Key') in self._active_clusters.values()
         return False
 
     def _get_tag_name_from_tags(self, tags: list, tag_name: str = 'Name'):
         """
         This method returns the tag_name from resource tags
         @param tags:
         @param tag_name:
@@ -123,15 +105,15 @@
         """
         upload_data = []
         for resource_data in upload_resource_data:
             if isinstance(resource_data, list):
                 resource_str = ''
                 for resource in resource_data[:-1]:
                     resource_str += f'{resource} | '
-                resource_str += str(resource_data[-1])
+                resource_str += resource_data[-1]
                 upload_data.append(resource_str)
             else:
                 upload_data.append(resource_data)
         return upload_data
 
     def _get_resource_username(self, resource_id: str, resource_type: str, create_date: datetime = '', event_type: str = ''):
         """
@@ -155,47 +137,41 @@
         @return:
         """
         policy_value = self._get_tag_name_from_tags(tags=tags, tag_name='Policy').strip()
         if policy_value:
             return policy_value.replace('_', '').replace('-', '').upper()
         return 'NA'
 
-    def _trigger_mail(self, tags: list, resource_id: str, days: int, resource_type: str, **kwargs):
+    def _trigger_mail(self, tags: list, resource_id: str, days: int, resource_type: str):
         """
         This method send triggering mail
         @param tags:
         @param resource_id:
         @return:
         """
-        if self.__email_alert:
-            try:
-                special_user_mails = self._literal_eval(self._special_user_mails)
-                user, resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(
-                    tags=tags, tag_name='Name')
-                if not resource_name:
-                    resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='cg-Name')
-                to = user if user not in special_user_mails else special_user_mails[user]
-                ldap_data = self._ldap.get_user_details(user_name=to)
-                cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com'] if self.__manager_email_alert else []
-                name = to
-                if ldap_data:
-                    name = ldap_data.get('displayName')
-                subject, body = self._mail_description.resource_message(name=name, days=days,
-                                                                        notification_days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
-                                                                        delete_days=self.DAYS_TO_DELETE_RESOURCE,
-                                                                        resource_name=resource_name, resource_id=resource_id,
-                                                                        resource_type=resource_type, msgadmins=self.DAYS_TO_NOTIFY_ADMINS, extra_purse=kwargs.get('extra_purse'))
-                if not kwargs.get('admins'):
-                    self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
-                else:
-                    if self.__manager_email_alert:
-                        kwargs['admins'].append(f'{ldap_data.get("managerId")}@redhat.com')
-                    self._mail.send_email_postfix(to=kwargs.get('admins'), content=body, subject=subject, cc=[], resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
-            except Exception as err:
-                logger.info(err)
+        try:
+            special_user_mails = self._literal_eval(self._special_user_mails)
+            user, resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(
+                tags=tags, tag_name='Name')
+            if not resource_name:
+                resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='cg-Name')
+            to = user if user not in special_user_mails else special_user_mails[user]
+            ldap_data = self._ldap.get_user_details(user_name=to)
+            cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com']
+            name = to
+            if ldap_data:
+                name = ldap_data.get('displayName')
+            subject, body = self._mail_description.resource_message(name=name, days=days,
+                                                                    notification_days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
+                                                                    delete_days=self.DAYS_TO_DELETE_RESOURCE,
+                                                                    resource_name=resource_name, resource_id=resource_id,
+                                                                    resource_type=resource_type)
+            self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id)
+        except Exception as err:
+            logger.info(err)
 
     def _update_tag_value(self, tags: list, tag_name: str, tag_value: str):
         """
         This method updates the tag value
         @param tags:
         @param tag_name:
         @param tag_value:
@@ -223,31 +199,31 @@
             last_used_day = 1
         else:
             last_used_day = int(last_used_day) + 1
         return last_used_day
 
     def __delete_resource_on_name(self, resource_id: str):
         try:
-            if self._policy == 's3_inactive':
+            if self._policy == 'empty_buckets':
                 self._s3_client.delete_bucket(Bucket=resource_id)
             elif self._policy == 'empty_roles':
                 self._iam_client.delete_role(RoleName=resource_id)
             elif self._policy == 'ebs_unattached':
                 self._ec2_client.delete_volume(VolumeId=resource_id)
-            elif self._policy == 'ip_unattached':
+            elif self._policy == 'zombie_elastic_ips':
                 self._ec2_client.release_address(AllocationId=resource_id)
-            elif self._policy == 'nat_gateway_unused':
+            elif self._policy == 'zombie_nat_gateways':
                 self._ec2_client.delete_nat_gateway(NatGatewayId=resource_id)
             elif self._policy == 'zombie_snapshots':
                 self._ec2_client.delete_snapshot(SnapshotId=resource_id)
             logger.info(f'{self._policy} deleted: {resource_id}')
         except Exception as err:
             logger.info(f'Exception raised: {err}: {resource_id}')
 
-    def _check_resource_and_delete(self, resource_name: str, resource_id: str, resource_type: str, resource: dict, empty_days: int, days_to_delete_resource: int, tags: list = [], **kwargs):
+    def _check_resource_and_delete(self, resource_name: str, resource_id: str, resource_type: str, resource: dict, empty_days: int, days_to_delete_resource: int, tags: list = []):
         """
         This method check and delete resources
         @param resource_name:
         @param resource_id:
         @param resource_type:
         @param resource:
         @param empty_days:
@@ -262,79 +238,33 @@
         if not user:
             user = self._get_resource_username(resource_id=resource_id, resource_type=resource_type, event_type='EventName')
             if user:
                 tags.append({'Key': 'User', 'Value': user})
         zombie_resource = {}
         if empty_days >= self.DAYS_TO_TRIGGER_RESOURCE_MAIL:
             if empty_days == self.DAYS_TO_TRIGGER_RESOURCE_MAIL:
-                kwargs['delta_cost'] = kwargs.get('extra_purse')
-                self._trigger_mail(resource_type=resource_name, resource_id=resource_id, tags=tags, days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL, message_type='notification', extra_purse=kwargs.get('extra_purse'), delta_cost=kwargs.get('delta_cost', 0))
-            elif empty_days == self.DAYS_TO_NOTIFY_ADMINS:
-                self._trigger_mail(resource_type=resource_name, resource_id=resource_id, tags=tags, days=empty_days, admins=self._admins, message_type='notify_admin', extra_purse=kwargs.get('extra_purse'), delta_cost=kwargs.get('delta_cost', 0))
+                self._trigger_mail(resource_type=resource_name, resource_id=resource_id, tags=tags, days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL)
             elif empty_days >= days_to_delete_resource:
                 if self._dry_run == 'no':
                     if self._get_policy_value(tags=tags) not in ('NOTDELETE', 'SKIP'):
-                        self._trigger_mail(resource_type=resource_name, resource_id=resource_id, tags=tags, days=empty_days, message_type='delete', extra_purse=kwargs.get('extra_purse'), delta_cost=kwargs.get('delta_cost', 0))
+                        self._trigger_mail(resource_type=resource_name, resource_id=resource_id, tags=tags, days=empty_days)
                         self.__delete_resource_on_name(resource_id=resource_id)
             zombie_resource = resource
         return zombie_resource
 
     def _update_resource_tags(self, resource_id: str, left_out_days: int, tags: list, resource_left_out: bool):
         """
         This method update the tags in aws
         @return:
         """
         if left_out_days < 7 or self._dry_run == 'yes' or self._get_policy_value(tags=tags) in ('NOTDELETE', 'SKIP'):
             if self._get_tag_name_from_tags(tags=tags, tag_name='LastUsedDay') or resource_left_out:
                 tags = self._update_tag_value(tags=tags, tag_name='LastUsedDay', tag_value=str(left_out_days))
                 try:
-                    if self._policy == 's3_inactive':
+                    if self._policy == 'empty_buckets':
                         self._s3_client.put_bucket_tagging(Bucket=resource_id, Tagging={'TagSet': tags})
                     elif self._policy == 'empty_roles':
                         self._iam_client.tag_role(RoleName=resource_id, Tags=tags)
-                    elif self._policy in ('ip_unattached', 'nat_gateway_unused', 'zombie_snapshots'):
+                    elif self._policy in ('zombie_elastic_ips', 'zombie_nat_gateways', 'zombie_snapshots'):
                         self._ec2_client.create_tags(Resources=[resource_id], Tags=tags)
                 except Exception as err:
                     logger.info(f'Exception raised: {err}: {resource_id}')
-
-    def _organise_instance_data(self, resources: list):
-        """
-        This method convert all datetime into string
-        @param resources:
-        @return:
-        """
-        organize_data = []
-        if 'ec2' in self._policy:
-            for instance in resources:
-                instance['LaunchTime'] = instance['LaunchTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                for index, device_mappings in enumerate(instance['BlockDeviceMappings']):
-                    instance['BlockDeviceMappings'][index]['Ebs']['AttachTime'] = device_mappings['Ebs']['AttachTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                for index, network_interface in enumerate(instance['NetworkInterfaces']):
-                    instance['NetworkInterfaces'][index]['Attachment']['AttachTime'] = network_interface['Attachment']['AttachTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                if instance.get('UsageOperationUpdateTime'):
-                    instance['UsageOperationUpdateTime'] = instance['UsageOperationUpdateTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                if instance.get('metrics'):
-                    for index, metric in enumerate(instance['metrics']):
-                        instance['metrics'][index]['Timestamps'] = [date.strftime("%Y-%m-%dT%H:%M:%S+00:00") for date in metric['Timestamps']]
-                organize_data.append(instance)
-        else:
-            for volume in resources:
-                if volume.get('Attachments'):
-                    for attachment in volume.get('Attachments'):
-                        attachment['AttachTime'] = attachment['AttachTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                volume['CreateTime'] = volume['CreateTime'].strftime("%Y-%m-%dT%H:%M:%S+00:00")
-                organize_data.append(volume)
-        return organize_data
-
-    def get_ebs_cost(self, resource: any, resource_type: str, resource_hours: int):
-        ebs_cost = 0
-        if resource_type == 'ec2':
-            volume_ids = []
-            for block_device in resource:
-                volume_ids.append(block_device.get('Ebs').get('VolumeId'))
-            volumes = self._ec2_client.describe_volumes(VolumeIds=volume_ids)['Volumes']
-            for volume in volumes:
-                ebs_cost += self.resource_pricing.get_ebs_cost(volume_size=volume.get('Size'), volume_type=volume.get('VolumeType'), hours=resource_hours)
-        else:
-            if resource_type == 'ebs':
-                ebs_cost += self.resource_pricing.get_ebs_cost(volume_size=resource.get('Size'), volume_type=resource.get('VolumeType'), hours=resource_hours)
-        return round(ebs_cost, 3)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `cloud-governance-1.1.9/cloud_governance/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import inspect
 
 from cloud_governance.common.logger.init_logger import logger
-from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
+from cloud_governance.aws.zombie_non_cluster.run_zombie_non_cluster_policies import NonClusterZombiePolicy
 
 
 class ZombieNonClusterPolicies(NonClusterZombiePolicy):
 
     def __init__(self):
         super().__init__()
 
@@ -17,18 +17,15 @@
         """
         logger.info(f'account={self._account}, region={self._region}, policy={self._policy}, dry_run={self._dry_run}')
         zombie_non_cluster_policy_module = importlib.import_module(f'cloud_governance.policy.aws.{self._policy}')
 
         for cls in inspect.getmembers(zombie_non_cluster_policy_module, inspect.isclass):
             if self._policy.replace('_', '') == cls[0].lower():
                 response = cls[1]().run()
-                if isinstance(response, str):
-                    logger.info(f'key: {cls[0]}, Response: {response}')
-                else:
-                    logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
-                    policy_result = response
-                    if self._policy_output:
-                        if self._policy not in ('ec2_idle', 'ebs_in_use', 'ec2_run'):
-                            beautify_data = self._beautify_upload_data(upload_resource_data=response)
-                            policy_result = {'count': len(beautify_data), self._policy: beautify_data}
-                        logger.info(policy_result)
-                        self._s3operations.save_results_to_s3(policy=self._policy.replace('_', '-'), policy_output=self._policy_output, policy_result=policy_result)
+                logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
+                policy_result = response
+                if self._policy_output:
+                    if self._policy != 'ec2_idle':
+                        beautify_data = self._beautify_upload_data(upload_resource_data=response)
+                        policy_result = {'count': len(beautify_data), self._policy: beautify_data}
+                    logger.info(policy_result)
+                    self._s3operations.save_results_to_s3(policy=self._policy.replace('_', '-'), policy_output=self._policy_output, policy_result=policy_result)
```

### Comparing `cloud-governance-1.1.86/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `cloud-governance-1.1.9/cloud_governance/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.86/cloud_governance.egg-info/PKG-INFO` & `cloud-governance-1.1.9/cloud_governance.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.86
+Version: 1.1.9
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cloud-governance.svg)](https://pypi.org/project/cloud-governance/)
 [![Container Repository on Quay](https://quay.io/repository/projectquay/quay/status "Container Repository on Quay")](https://quay.io/repository/ebattat/cloud-governance?tab=tags)
 [![Actions Status](https://github.com/redhat-performance/cloud-governance/workflows/Build/badge.svg)](https://github.com/redhat-performance/cloud-governance/actions)
@@ -36,28 +36,23 @@
 
 This tool support the following policies:
 [policy](cloud_governance/policy)
 
 [AWS Polices](cloud_governance/policy/aws)
 
 * Real time Openshift Cluster cost, User cost
-* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 4 days, cpu < 2% & network < 5mb.
-* [ec2_run](cloud_governance/policy/aws/ec2_run.py): running ec2.
-* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.py): volumes that did not connect to instance, volume in available status.
-* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.py): in use volumes.
-* [tag_resources](cloud_governance/policy/policy_operations/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
+* [ec2_idle](cloud_governance/policy/aws/ec2_idle.py): idle ec2 in last 2 days, cpu < 2% & network < 5mb [ec2_idle](cloud_governance/policy/aws/ec2_idle.py)
+* [ec2_run](cloud_governance/policy/aws/ec2_run.yml): running ec2 [ec2_run](cloud_governance/policy/aws/ec2_run.yml)
+* [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml): volumes that did not connect to instance, volume in available status [ebs_unattached](cloud_governance/policy/aws/ebs_unattached.yml)
+* [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml): in use volumes [ebs_in_use](cloud_governance/policy/aws/ebs_in_use.yml)
+* [tag_resources](cloud_governance/aws/tag_cluster): Update cluster and non cluster resource tags fetching from the user tags or from the mandatory tags
 * [zombie_cluster_resource](cloud_governance/policy/aws/zombie_cluster_resource.py): Delete cluster's zombie resources
-* [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
-* [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
+* [tag_non_cluster](cloud_governance/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
+* [tag_iam_user](cloud_governance/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
-* [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
-* [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
-* [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
-* [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
@@ -137,29 +132,29 @@
 GOOGLE_APPLICATION_CREDENTIALS=$pwd/service_account.json
 
 # Configuration
 
 ### AWS Configuration
 
 #### Create a user and a bucket
-* Create user with IAM [iam](iam/clouds)
-* Create a logs bucket [create_bucket.sh](iam/cloud/aws/create_bucket.sh)
+* Create user with IAM [iam](iam)
+* Create a logs bucket [create_bucket.sh](iam/create_bucket.sh)
 
 ### IBM Configuration
 * Create classic infrastructure API key
 
 ## Run AWS Policy Using Podman 
 ```sh
 # policy=ec2_idle
 sudo podman run --rm --name cloud-governance -e policy="ec2_idle" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ec2_run
 sudo podman run --rm --name cloud-governance -e policy="ec2_run" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
-# select policy ['ec2_stop', 's3_inactive', 'empty_roles', 'ip_unattached', 'nat_gateway_unused', 'zombie_snapshots']
+# select policy ['ec2_stop', 'empty_buckets', 'empty_roles', 'zombie_elastic_ips', 'zombie_nat_gateways', 'zombie_snapshots']
 sudo podman run --rm --name cloud-governance -e policy="policy" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes"  -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_unattached
 sudo podman run --rm --name cloud-governance -e policy="ebs_unattached" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
 
 # policy=ebs_in_use
 sudo podman run --rm --name cloud-governance -e policy="ebs_in_use" -e AWS_ACCESS_KEY_ID="$AWS_ACCESS_KEY_ID" -e AWS_SECRET_ACCESS_KEY="$AWS_SECRET_ACCESS_KEY" -e AWS_DEFAULT_REGION="us-east-2" -e dry_run="yes" -e policy_output="s3://bucket/logs" -e log_level="INFO" "quay.io/ebattat/cloud-governance"
@@ -234,7 +229,9 @@
 
 ## Post Installation
 
 #### Delete cloud-governance image
 ```sh
 sudo podman rmi quay.io/ebattat/cloud-governance
 ```
+
+
```

