# Comparing `tmp/iam_actions-1.2.20230410.tar.gz` & `tmp/iam_actions-1.2.20230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230410.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230411.tar", max compression
```

## Comparing `iam_actions-1.2.20230410.tar` & `iam_actions-1.2.20230411.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/README.md
--rw-r--r--   0        0        0      228 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/__init__.py
--rw-r--r--   0        0        0  4199871 2023-04-10 02:24:51.320400 iam_actions-1.2.20230410/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-10 02:23:26.963717 iam_actions-1.2.20230410/iam_actions/generate/services.py
--rw-r--r--   0        0        0   539168 2023-04-10 02:24:51.320400 iam_actions-1.2.20230410/iam_actions/policies.json
--rw-r--r--   0        0        0   190022 2023-04-10 02:24:51.320400 iam_actions-1.2.20230410/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   522833 2023-04-10 02:24:51.320400 iam_actions-1.2.20230410/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-10 02:24:52.232451 iam_actions-1.2.20230410/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230410/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230410/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/README.md
+-rw-r--r--   0        0        0      228 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4203173 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   539591 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/policies.json
+-rw-r--r--   0        0        0   190147 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   523243 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-11 02:26:39.519521 iam_actions-1.2.20230411/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230411/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230411/PKG-INFO
```

### Comparing `iam_actions-1.2.20230410/LICENSE` & `iam_actions-1.2.20230411/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/README.md` & `iam_actions-1.2.20230411/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/actions.json` & `iam_actions-1.2.20230411/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991776218364514%*

 * *Differences: {"'aws-portal'": "{'UpdateConsoleActionSetEnforced': OrderedDict([('access_level', "*

 * *                 "'Undocumented'), ('action', 'UpdateConsoleActionSetEnforced'), "*

 * *                 "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *                 "False), ('resources', [])]), 'GetConsoleActionSetEnforced': "*

 * *                 "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                 "'GetConsoleActionSetEnforced'), ('condition_keys', []), ('description', […]*

```diff
@@ -10386,14 +10386,22 @@
             "condition_keys": [],
             "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal.",
             "orphan": false,
             "resources": []
         }
     },
     "aws-portal": {
+        "GetConsoleActionSetEnforced": {
+            "access_level": "Undocumented",
+            "action": "GetConsoleActionSetEnforced",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyAccount": {
             "access_level": "Write",
             "action": "ModifyAccount",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to modify Account Settings",
             "orphan": false,
             "resources": []
@@ -10410,14 +10418,22 @@
             "access_level": "Write",
             "action": "ModifyPaymentMethods",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to modify payment methods",
             "orphan": false,
             "resources": []
         },
+        "UpdateConsoleActionSetEnforced": {
+            "access_level": "Undocumented",
+            "action": "UpdateConsoleActionSetEnforced",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ViewAccount": {
             "access_level": "Read",
             "action": "ViewAccount",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to view account settings",
             "orphan": false,
             "resources": []
@@ -106207,14 +106223,22 @@
             "access_level": "Write",
             "action": "DeletePurchaseOrder",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to delete a purchase order",
             "orphan": false,
             "resources": []
         },
+        "GetConsoleActionSetEnforced": {
+            "access_level": "Undocumented",
+            "action": "GetConsoleActionSetEnforced",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetPurchaseOrder": {
             "access_level": "Read",
             "action": "GetPurchaseOrder",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to get a purchase order",
             "orphan": false,
             "resources": []
@@ -106239,14 +106263,22 @@
             "access_level": "Write",
             "action": "ModifyPurchaseOrders",
             "condition_keys": [],
             "description": "Grants permission to modify purchase orders and details",
             "orphan": false,
             "resources": []
         },
+        "UpdateConsoleActionSetEnforced": {
+            "access_level": "Undocumented",
+            "action": "UpdateConsoleActionSetEnforced",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdatePurchaseOrder": {
             "access_level": "Write",
             "action": "UpdatePurchaseOrder",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to update an existing purchase order",
             "orphan": false,
             "resources": []
@@ -106857,20 +106889,22 @@
             "description": "Grants permission to provision Amazon QuickSight readers",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "CreateRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a refresh schedule for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "refreshschedule"
+            ]
         },
         "CreateTemplate": {
             "access_level": "Write",
             "action": "CreateTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -106996,20 +107030,22 @@
             "description": "Grants permission to delete a dataset",
             "orphan": false,
             "resources": [
                 "dataset"
             ]
         },
         "DeleteDataSetRefreshProperties": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDataSetRefreshProperties",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete dataset refresh properties for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "DeleteDataSource": {
             "access_level": "Write",
             "action": "DeleteDataSource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -107092,20 +107128,22 @@
             "description": "Grants permission to delete a QuickSight namespace",
             "orphan": false,
             "resources": [
                 "namespace"
             ]
         },
         "DeleteRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a refresh schedule for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "refreshschedule"
+            ]
         },
         "DeleteTemplate": {
             "access_level": "Write",
             "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete a template",
             "orphan": false,
@@ -107270,20 +107308,22 @@
             "description": "Grants permission to describe the resource policy of a dataset",
             "orphan": false,
             "resources": [
                 "dataset"
             ]
         },
         "DescribeDataSetRefreshProperties": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeDataSetRefreshProperties",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe refresh properties for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "DescribeDataSource": {
             "access_level": "Read",
             "action": "DescribeDataSource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -107407,20 +107447,22 @@
             "description": "Grants permission to describe a QuickSight namespace",
             "orphan": false,
             "resources": [
                 "namespace"
             ]
         },
         "DescribeRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a refresh schedule for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "refreshschedule"
+            ]
         },
         "DescribeTemplate": {
             "access_level": "Read",
             "action": "DescribeTemplate",
             "condition_keys": [],
             "description": "Grants permission to describe a template",
             "orphan": false,
@@ -107696,18 +107738,18 @@
             "action": "ListNamespaces",
             "condition_keys": [],
             "description": "Grants permission to lists all namespaces in a QuickSight account",
             "orphan": false,
             "resources": []
         },
         "ListRefreshSchedules": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListRefreshSchedules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all refresh schedules on a dataset",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
@@ -107824,20 +107866,22 @@
             "description": "Grants permission to use a data source for a data set",
             "orphan": false,
             "resources": [
                 "datasource"
             ]
         },
         "PutDataSetRefreshProperties": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutDataSetRefreshProperties",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to put dataset refresh properties for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "RegisterUser": {
             "access_level": "Write",
             "action": "RegisterUser",
             "condition_keys": [
                 "quicksight:IamArn",
                 "quicksight:SessionName"
@@ -108194,20 +108238,22 @@
             "action": "UpdatePublicSharingSettings",
             "condition_keys": [],
             "description": "Grants permission to enable or disable public sharing on an account",
             "orphan": false,
             "resources": []
         },
         "UpdateRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a refresh schedule for a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "refreshschedule"
+            ]
         },
         "UpdateResourcePermissions": {
             "access_level": "Write",
             "action": "UpdateResourcePermissions",
             "condition_keys": [],
             "description": "Grants permission to update resource-level permissions in QuickSight",
             "orphan": false,
@@ -112697,14 +112743,22 @@
             "condition_keys": [],
             "description": "Grants permission to create a new Amazon Rekognition Custom Labels dataset",
             "orphan": false,
             "resources": [
                 "project"
             ]
         },
+        "CreateFaceLivenessSession": {
+            "access_level": "Undocumented",
+            "action": "CreateFaceLivenessSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateProject": {
             "access_level": "Write",
             "action": "CreateProject",
             "condition_keys": [],
             "description": "Grants permission to create an Amazon Rekognition Custom Labels project",
             "orphan": false,
             "resources": [
@@ -112943,14 +112997,22 @@
             "access_level": "Read",
             "action": "GetFaceDetection",
             "condition_keys": [],
             "description": "Grants permission to read the faces detection results found in a stored video by an asynchronous face detection job",
             "orphan": false,
             "resources": []
         },
+        "GetFaceLivenessSessionResults": {
+            "access_level": "Undocumented",
+            "action": "GetFaceLivenessSessionResults",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetFaceSearch": {
             "access_level": "Read",
             "action": "GetFaceSearch",
             "condition_keys": [],
             "description": "Grants permission to read the matching collection faces found in a stored video by an asynchronous face search job",
             "orphan": false,
             "resources": []
@@ -113125,14 +113187,22 @@
             "access_level": "Write",
             "action": "StartFaceDetection",
             "condition_keys": [],
             "description": "Grants permission to start asynchronous detection of faces in a stored video",
             "orphan": false,
             "resources": []
         },
+        "StartFaceLivenessSession": {
+            "access_level": "Undocumented",
+            "action": "StartFaceLivenessSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartFaceSearch": {
             "access_level": "Write",
             "action": "StartFaceSearch",
             "condition_keys": [],
             "description": "Grants permission to start an asynchronous search for faces in a collection that match the faces of persons detected in a stored video",
             "orphan": false,
             "resources": [
@@ -120689,14 +120759,22 @@
             ],
             "description": "Grants permission to retrieve a specific version of an object",
             "orphan": false,
             "resources": [
                 "object"
             ]
         },
+        "GetObjectVersionForReplication": {
+            "access_level": "Undocumented",
+            "action": "GetObjectVersionForReplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetObjectVersionTagging": {
             "access_level": "Read",
             "action": "GetObjectVersionTagging",
             "condition_keys": [
                 "s3-outposts:AccessPointNetworkOrigin",
                 "s3-outposts:DataAccessPointAccount",
                 "s3-outposts:DataAccessPointArn",
@@ -120709,14 +120787,22 @@
             ],
             "description": "Grants permission to return the tag set for a specific version of the object",
             "orphan": false,
             "resources": [
                 "object"
             ]
         },
+        "GetReplicationConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetReplicationConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAccessPoints": {
             "access_level": "List",
             "action": "ListAccessPoints",
             "condition_keys": [
                 "s3-outposts:authType",
                 "s3-outposts:signatureAge",
                 "s3-outposts:signatureversion",
@@ -121005,14 +121091,46 @@
                 "s3-outposts:x-amz-content-sha256"
             ],
             "description": "Grants permission to set the supplied tag-set for a specific version of an object",
             "orphan": false,
             "resources": [
                 "object"
             ]
+        },
+        "PutReplicationConfiguration": {
+            "access_level": "Undocumented",
+            "action": "PutReplicationConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ReplicateDelete": {
+            "access_level": "Undocumented",
+            "action": "ReplicateDelete",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ReplicateObject": {
+            "access_level": "Undocumented",
+            "action": "ReplicateObject",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ReplicateTags": {
+            "access_level": "Undocumented",
+            "action": "ReplicateTags",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "sagemaker": {
         "AddAssociation": {
             "access_level": "Write",
             "action": "AddAssociation",
             "condition_keys": [
```

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230411/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230411/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/generate.py` & `iam_actions-1.2.20230411/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230411/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230411/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/generate/services.py` & `iam_actions-1.2.20230411/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230410/iam_actions/policies.json` & `iam_actions-1.2.20230411/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999906184593683%*

 * *Differences: {"'serviceMap'": "{'AWS Billing Console': {'Actions': {insert: [(0, "*

 * *                 "'GetConsoleActionSetEnforced'), (4, 'UpdateConsoleActionSetEnforced')]}}, 'AWS "*

 * *                 "Purchase Orders Console': {'Actions': {insert: [(2, "*

 * *                 "'GetConsoleActionSetEnforced'), (7, 'UpdateConsoleActionSetEnforced')]}}, "*

 * *                 "'Amazon S3 on Outposts': {'Actions': {insert: [(23, "*

 * *                 "'GetObjectVersionForReplication'), (25, 'GetReplicationConfiguration'), (44, "*

 * *         […]*

```diff
@@ -1156,17 +1156,19 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "AWS Billing Console": {
             "Actions": [
+                "GetConsoleActionSetEnforced",
                 "ModifyAccount",
                 "ModifyBilling",
                 "ModifyPaymentMethods",
+                "UpdateConsoleActionSetEnforced",
                 "ViewAccount",
                 "ViewBilling",
                 "ViewPaymentMethods",
                 "ViewUsage"
             ],
             "HasResource": false,
             "StringPrefix": "aws-portal"
@@ -7157,18 +7159,20 @@
         },
         "AWS Purchase Orders Console": {
             "ARNFormat": "arn:${Partition}:purchase-orders::${Account}:${ResourceType}:${ResourceName}",
             "ARNRegex": "^arn:${Partition}:purchase-orders::.+:.+:.+",
             "Actions": [
                 "AddPurchaseOrder",
                 "DeletePurchaseOrder",
+                "GetConsoleActionSetEnforced",
                 "GetPurchaseOrder",
                 "ListPurchaseOrderInvoices",
                 "ListPurchaseOrders",
                 "ModifyPurchaseOrders",
+                "UpdateConsoleActionSetEnforced",
                 "UpdatePurchaseOrder",
                 "UpdatePurchaseOrderStatus",
                 "ViewPurchaseOrders"
             ],
             "HasResource": false,
             "StringPrefix": "purchase-orders"
         },
@@ -16967,14 +16971,15 @@
             "ARNFormat": "arn:aws:rekognition:${Region}:${Account}:${RelativeId}",
             "ARNRegex": "^arn:aws:rekognition:.+",
             "Actions": [
                 "CompareFaces",
                 "CopyProjectVersion",
                 "CreateCollection",
                 "CreateDataset",
+                "CreateFaceLivenessSession",
                 "CreateProject",
                 "CreateProjectVersion",
                 "CreateStreamProcessor",
                 "DeleteCollection",
                 "DeleteDataset",
                 "DeleteFaces",
                 "DeleteProject",
@@ -16993,14 +16998,15 @@
                 "DetectProtectiveEquipment",
                 "DetectText",
                 "DistributeDatasetEntries",
                 "GetCelebrityInfo",
                 "GetCelebrityRecognition",
                 "GetContentModeration",
                 "GetFaceDetection",
+                "GetFaceLivenessSessionResults",
                 "GetFaceSearch",
                 "GetLabelDetection",
                 "GetPersonTracking",
                 "GetSegmentDetection",
                 "GetTextDetection",
                 "IndexFaces",
                 "ListCollections",
@@ -17013,14 +17019,15 @@
                 "PutProjectPolicy",
                 "RecognizeCelebrities",
                 "SearchFaces",
                 "SearchFacesByImage",
                 "StartCelebrityRecognition",
                 "StartContentModeration",
                 "StartFaceDetection",
+                "StartFaceLivenessSession",
                 "StartFaceSearch",
                 "StartLabelDetection",
                 "StartPersonTracking",
                 "StartProjectVersion",
                 "StartSegmentDetection",
                 "StartStreamProcessor",
                 "StartTextDetection",
@@ -17660,15 +17667,17 @@
                 "GetBucketPolicy",
                 "GetBucketTagging",
                 "GetBucketVersioning",
                 "GetLifecycleConfiguration",
                 "GetObject",
                 "GetObjectTagging",
                 "GetObjectVersion",
+                "GetObjectVersionForReplication",
                 "GetObjectVersionTagging",
+                "GetReplicationConfiguration",
                 "ListAccessPoints",
                 "ListBucket",
                 "ListBucketMultipartUploads",
                 "ListBucketVersions",
                 "ListEndpoints",
                 "ListMultipartUploadParts",
                 "ListOutpostsWithS3",
@@ -17678,15 +17687,19 @@
                 "PutBucketPolicy",
                 "PutBucketTagging",
                 "PutBucketVersioning",
                 "PutLifecycleConfiguration",
                 "PutObject",
                 "PutObjectAcl",
                 "PutObjectTagging",
-                "PutObjectVersionTagging"
+                "PutObjectVersionTagging",
+                "PutReplicationConfiguration",
+                "ReplicateDelete",
+                "ReplicateObject",
+                "ReplicateTags"
             ],
             "HasResource": true,
             "StringPrefix": "s3-outposts",
             "conditionKeys": [
                 "s3-outposts:AccessPointNetworkOrigin",
                 "s3-outposts:DataAccessPointAccount",
                 "s3-outposts:DataAccessPointArn",
```

### Comparing `iam_actions-1.2.20230410/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230411/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999166805532412%*

 * *Differences: {"'quicksight'": "{'refreshschedule': OrderedDict([('arn_pattern', "*

 * *                 "'arn:*:quicksight:*:*:dataset/*/refresh-schedule/*'), ('condition_keys', "*

 * *                 'None)])}'}*

```diff
@@ -4784,14 +4784,18 @@
             "arn_pattern": "arn:*:quicksight:*:*:dataset/*/ingestion/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "namespace": {
             "arn_pattern": "arn:*:quicksight:*:*:namespace/*",
             "condition_keys": null
         },
+        "refreshschedule": {
+            "arn_pattern": "arn:*:quicksight:*:*:dataset/*/refresh-schedule/*",
+            "condition_keys": null
+        },
         "template": {
             "arn_pattern": "arn:*:quicksight:*:*:template/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "theme": {
             "arn_pattern": "arn:*:quicksight:*:*:theme/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230410/iam_actions/services.json` & `iam_actions-1.2.20230411/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999321889814101%*

 * *Differences: {"'aws-portal'": "{'Actions': {insert: [(0, 'GetConsoleActionSetEnforced'), (4, "*

 * *                 "'UpdateConsoleActionSetEnforced')]}}",*

 * * "'purchase-orders'": "{'Actions': {insert: [(2, 'GetConsoleActionSetEnforced'), (7, "*

 * *                      "'UpdateConsoleActionSetEnforced')]}}",*

 * * "'rekognition'": "{'Actions': {insert: [(4, 'CreateFaceLivenessSession'), (31, "*

 * *                  "'GetFaceLivenessSessionResults'), (52, 'StartFaceLivenessSession')]}}",*

 * * "'s3-outposts'": "{'Actions': {insert: [(23, 'GetO […]*

```diff
@@ -1664,17 +1664,19 @@
             "AWS Marketplace Management Portal"
         ]
     },
     "aws-portal": {
         "ARNFormats": [],
         "ARNRegexes": [],
         "Actions": [
+            "GetConsoleActionSetEnforced",
             "ModifyAccount",
             "ModifyBilling",
             "ModifyPaymentMethods",
+            "UpdateConsoleActionSetEnforced",
             "ViewAccount",
             "ViewBilling",
             "ViewPaymentMethods",
             "ViewUsage"
         ],
         "ConditionKeys": [],
         "HasResource": false,
@@ -14931,18 +14933,20 @@
         ],
         "ARNRegexes": [
             "^arn:${Partition}:purchase-orders::.+:.+:.+"
         ],
         "Actions": [
             "AddPurchaseOrder",
             "DeletePurchaseOrder",
+            "GetConsoleActionSetEnforced",
             "GetPurchaseOrder",
             "ListPurchaseOrderInvoices",
             "ListPurchaseOrders",
             "ModifyPurchaseOrders",
+            "UpdateConsoleActionSetEnforced",
             "UpdatePurchaseOrder",
             "UpdatePurchaseOrderStatus",
             "ViewPurchaseOrders"
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
@@ -15809,14 +15813,15 @@
             "^arn:aws:rekognition:.+"
         ],
         "Actions": [
             "CompareFaces",
             "CopyProjectVersion",
             "CreateCollection",
             "CreateDataset",
+            "CreateFaceLivenessSession",
             "CreateProject",
             "CreateProjectVersion",
             "CreateStreamProcessor",
             "DeleteCollection",
             "DeleteDataset",
             "DeleteFaces",
             "DeleteProject",
@@ -15835,14 +15840,15 @@
             "DetectProtectiveEquipment",
             "DetectText",
             "DistributeDatasetEntries",
             "GetCelebrityInfo",
             "GetCelebrityRecognition",
             "GetContentModeration",
             "GetFaceDetection",
+            "GetFaceLivenessSessionResults",
             "GetFaceSearch",
             "GetLabelDetection",
             "GetPersonTracking",
             "GetSegmentDetection",
             "GetTextDetection",
             "IndexFaces",
             "ListCollections",
@@ -15855,14 +15861,15 @@
             "PutProjectPolicy",
             "RecognizeCelebrities",
             "SearchFaces",
             "SearchFacesByImage",
             "StartCelebrityRecognition",
             "StartContentModeration",
             "StartFaceDetection",
+            "StartFaceLivenessSession",
             "StartFaceSearch",
             "StartLabelDetection",
             "StartPersonTracking",
             "StartProjectVersion",
             "StartSegmentDetection",
             "StartStreamProcessor",
             "StartTextDetection",
@@ -16816,15 +16823,17 @@
             "GetBucketPolicy",
             "GetBucketTagging",
             "GetBucketVersioning",
             "GetLifecycleConfiguration",
             "GetObject",
             "GetObjectTagging",
             "GetObjectVersion",
+            "GetObjectVersionForReplication",
             "GetObjectVersionTagging",
+            "GetReplicationConfiguration",
             "ListAccessPoints",
             "ListBucket",
             "ListBucketMultipartUploads",
             "ListBucketVersions",
             "ListEndpoints",
             "ListMultipartUploadParts",
             "ListOutpostsWithS3",
@@ -16834,15 +16843,19 @@
             "PutBucketPolicy",
             "PutBucketTagging",
             "PutBucketVersioning",
             "PutLifecycleConfiguration",
             "PutObject",
             "PutObjectAcl",
             "PutObjectTagging",
-            "PutObjectVersionTagging"
+            "PutObjectVersionTagging",
+            "PutReplicationConfiguration",
+            "ReplicateDelete",
+            "ReplicateObject",
+            "ReplicateTags"
         ],
         "ConditionKeys": [
             "s3-outposts:AccessPointNetworkOrigin",
             "s3-outposts:DataAccessPointAccount",
             "s3-outposts:DataAccessPointArn",
             "s3-outposts:ExistingObjectTag/<key>",
             "s3-outposts:RequestObjectTag/<key>",
```

### Comparing `iam_actions-1.2.20230410/pyproject.toml` & `iam_actions-1.2.20230411/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230410"
+version = "1.2.20230411"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230410/setup.py` & `iam_actions-1.2.20230411/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230410',
+    'version': '1.2.20230411',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230410/PKG-INFO` & `iam_actions-1.2.20230411/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230410
+Version: 1.2.20230411
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

