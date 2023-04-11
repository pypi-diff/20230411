# Comparing `tmp/osc_sdk_python-0.24.0.tar.gz` & `tmp/osc_sdk_python-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_sdk_python-0.24.0.tar", last modified: Tue Feb 28 09:03:46 2023, max compression
+gzip compressed data, was "osc_sdk_python-0.25.0.tar", last modified: Tue Apr 11 14:51:09 2023, max compression
```

## Comparing `osc_sdk_python-0.24.0.tar` & `osc_sdk_python-0.25.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:03:46.845902 osc_sdk_python-0.24.0/osc_sdk_python/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/call.py
--rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/osc_sdk_python/osc-api/
--rw-r--r--   0 runner    (1001) docker     (122)   508025 2023-02-28 09:03:29.000000 osc_sdk_python-0.24.0/osc_sdk_python/osc-api/outscale.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8477 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/outscale_gateway.py
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/osc_sdk_python/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    24496 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/osc_sdk_python/resources/gateway_errors.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-02-28 09:03:46.000000 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-02-28 09:03:46.000000 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 09:03:46.000000 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-28 09:03:46.000000 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-02-28 09:03:46.000000 osc_sdk_python-0.24.0/osc_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-28 09:03:46.849902 osc_sdk_python-0.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-02-28 09:03:28.000000 osc_sdk_python-0.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/call.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python/osc-api/
+-rw-r--r--   0 runner    (1001) docker     (122)   540333 2023-04-11 14:50:43.000000 osc_sdk_python-0.25.0/osc_sdk_python/osc-api/outscale.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8085 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/outscale_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/osc_sdk_python/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    24496 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/resources/gateway_errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/setup.py
```

### Comparing `osc_sdk_python-0.24.0/LICENSE` & `osc_sdk_python-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.24.0/PKG-INFO` & `osc_sdk_python-0.25.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: osc_sdk_python
-Version: 0.24.0
-Summary: Outscale Gateway python SDK
-Home-page: https://github.com/outscale/osc_sdk_python
-Author: Outscal SAS
-Author-email: opensource@outscale.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Project Graduated](https://docs.outscale.com/fr/userguide/_images/Project-Graduated-green.svg)](https://docs.outscale.com/en/userguide/Open-Source-Projects.html)
 
 # Outscale Python SDK
 
 This python SDK helps you to perform actions on [Outscale API](https://docs-beta.outscale.com/?python#3ds-outscale-api).
 
 You will need to have an Outscale account, please visit [Outscale website](https://outscale.com/).
@@ -33,15 +20,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.24.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.24.0/README.md` & `osc_sdk_python-0.25.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: osc_sdk_python
+Version: 0.25.0
+Summary: Outscale Gateway python SDK
+Home-page: https://github.com/outscale/osc_sdk_python
+Author: Outscal SAS
+Author-email: opensource@outscale.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Project Graduated](https://docs.outscale.com/fr/userguide/_images/Project-Graduated-green.svg)](https://docs.outscale.com/en/userguide/Open-Source-Projects.html)
 
 # Outscale Python SDK
 
 This python SDK helps you to perform actions on [Outscale API](https://docs-beta.outscale.com/?python#3ds-outscale-api).
 
 You will need to have an Outscale account, please visit [Outscale website](https://outscale.com/).
@@ -20,15 +33,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.24.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/__init__.py` & `osc_sdk_python-0.25.0/osc_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/authentication.py` & `osc_sdk_python-0.25.0/osc_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/call.py` & `osc_sdk_python-0.25.0/osc_sdk_python/call.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import json
 
 class Call(object):
     def __init__(self, logger=None, **kwargs):
         self.version = kwargs.pop('version', 'latest')
         self.host = kwargs.pop('host', None)
         self.ssl = kwargs.pop('_ssl', True)
-        self.user_agent = kwargs.pop("user_agent", DEFAULT_USER_AGENT)
+        self.user_agent = kwargs.pop('user_agent', DEFAULT_USER_AGENT)
+        self.max_retries = kwargs.pop('max_retries', 0)
         self.logger = logger
         self.update_credentials(access_key=kwargs.pop('access_key', None),
                                 secret_key=kwargs.pop('secret_key', None),
                                 region=kwargs.pop('region', None),
                                 profile=kwargs.pop('profile', None),
                                 email=kwargs.pop('email', None),
                                 password=kwargs.pop('password', None))
@@ -35,13 +36,13 @@
             credentials = Credentials(**self.credentials)
             host = (self.host if self.host
                     else 'api.{}.outscale.{}'.format(credentials.region, credentials.get_url_extension()))
             uri = '/api/{}/{}'.format(self.version, action)
             protocol = 'https' if self.ssl else 'http'
             endpoint = '{}://{}{}'.format(protocol, host, uri)
 
-            requester = Requester(Authentication(credentials, host, user_agent=self.user_agent), endpoint)
+            requester = Requester(Authentication(credentials, host, user_agent=self.user_agent), endpoint, self.max_retries)
             if self.logger != None:
                 self.logger.do_log("uri: " + uri + "\npayload:\n" + json.dumps(data, indent=2))
             return requester.send(uri, json.dumps(data))
         except Exception as err:
             raise err
```

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/credentials.py` & `osc_sdk_python-0.25.0/osc_sdk_python/credentials.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/osc-api/outscale.yaml` & `osc_sdk_python-0.25.0/osc_sdk_python/osc-api/outscale.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -39,46 +39,46 @@
       description: Information about the access key.
       properties:
         AccessKeyId:
           description: The ID of the access key.
           type: string
         CreationDate:
           description: The date and time (UTC) of creation of the access key.
-          format: datetime
+          format: date-time
           type: string
         ExpirationDate:
           description: The date (UTC) at which the access key expires.
-          format: datetime
+          format: date-time
           type: string
         LastModificationDate:
           description: The date and time (UTC) of the last modification of the access key.
-          format: datetime
+          format: date-time
           type: string
         State:
           description: The state of the access key (`ACTIVE` if the key is valid for API calls, or `INACTIVE` if not).
           type: string
       type: object
     AccessKeySecretKey:
       additionalProperties: false
       description: Information about the access key.
       properties:
         AccessKeyId:
           description: The ID of the access key.
           type: string
         CreationDate:
           description: The date and time (UTC) of creation of the access key.
-          format: datetime
+          format: date-time
           type: string
         ExpirationDate:
           description: The date and time (UTC) at which the access key expires.
-          format: datetime
+          format: date-time
           type: string
         LastModificationDate:
           description: The date and time (UTC) of the last modification of the access key.
-          format: datetime
+          format: date-time
           type: string
         SecretKey:
           description: The access key that enables you to send requests.
           type: string
         State:
           description: The state of the access key (`ACTIVE` if the key is valid for API calls, or `INACTIVE` if not).
           type: string
@@ -280,16 +280,16 @@
       additionalProperties: false
       description: Information about the created BSU volume.
       properties:
         DeleteOnVmDeletion:
           description: If true, the volume is deleted when terminating the VM. If false, the volume is not deleted when terminating the VM.
           type: boolean
         LinkDate:
-          description: The time and date of attachment of the volume to the VM.
-          format: date
+          description: The date and time of attachment of the volume to the VM, in ISO 8601 date-time format.
+          format: date-time
           type: string
         State:
           description: The state of the volume.
           type: string
         VolumeId:
           description: The ID of the volume.
           type: string
@@ -382,14 +382,38 @@
           description: The type of resource associated with the catalog entry.
           type: string
         UnitPrice:
           description: The unit price of the catalog entry, in the currency of the catalog of the Region where the API method was used.
           format: float
           type: number
       type: object
+    Catalogs:
+      additionalProperties: false
+      description: Information about the catalogs.
+      properties:
+        Entries:
+          description: One or more catalog entries.
+          items:
+            $ref: '#/components/schemas/CatalogEntry'
+          type: array
+        FromDate:
+          description: The beginning of the time period, in ISO 8601 date-time format.
+          format: date-time
+          type: string
+        State:
+          description: The state of the catalog (`CURRENT` \| `OBSOLETE`).
+          enum:
+          - CURRENT
+          - OBSOLETE
+          type: string
+        ToDate:
+          description: The end of the time period, in ISO 8601 date-time format.
+          format: date-time
+          type: string
+      type: object
     CheckAuthenticationRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Login:
@@ -440,16 +464,16 @@
         AccountId:
           description: The ID of your TINA account.
           type: string
         Category:
           description: The category of the resource (for example, `network`).
           type: string
         FromDate:
-          description: The beginning of the time period.
-          format: datetime
+          description: The beginning of the time period, in ISO 8601 date-time format.
+          format: date-time
           type: string
         Operation:
           description: The API call that triggered the resource consumption (for example, `RunInstances` or `CreateVolume`).
           type: string
         PayingAccountId:
           description: The ID of the TINA account which is billed for your consumption. It can be different from your account in the `AccountId` parameter.
           type: string
@@ -459,16 +483,16 @@
         SubregionName:
           description: The name of the Subregion.
           type: string
         Title:
           description: A description of the consumed resource.
           type: string
         ToDate:
-          description: The end of the time period.
-          format: datetime
+          description: The end of the time period, in ISO 8601 date-time format.
+          format: date-time
           type: string
         Type:
           description: The type of resource, depending on the API call.
           type: string
         Value:
           description: The consumed amount for the resource. The unit depends on the resource type. For more information, see the `Title` element.
           format: double
@@ -477,17 +501,20 @@
     CreateAccessKeyRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         ExpirationDate:
-          description: The date and time at which you want the access key to expire, in ISO 8601 format (for example, `2017-06-14` or `2017-06-14T00:00:00Z`). To remove an existing expiration date, use the method without specifying this parameter.
-          format: datetime
-          type: string
+          description: The date and time, or the date, at which you want the access key to expire, in ISO 8601 format (for example, `2020-06-14T00:00:00.000Z`, or `2020-06-14`). To remove an existing expiration date, use the method without specifying this parameter.
+          oneOf:
+          - format: date-time
+            type: string
+          - format: date
+            type: string
       type: object
     CreateAccessKeyResponse:
       additionalProperties: false
       properties:
         AccessKey:
           $ref: '#/components/schemas/AccessKeySecretKey'
         ResponseContext:
@@ -808,14 +835,19 @@
           description: 'A unique name for the new OMI.<br />
 
             Constraints: 3-128 alphanumeric characters, underscores (_), spaces ( ), parentheses (()), slashes (/), periods (.), or dashes (-).'
           type: string
         NoReboot:
           description: If false, the VM shuts down before creating the OMI and then reboots. If true, the VM does not.
           type: boolean
+        ProductCodes:
+          description: The product codes associated with the OMI.
+          items:
+            type: string
+          type: array
         RootDeviceName:
           description: 'The name of the root device. You must specify only one of the following parameters: `FileLocation`, `RootDeviceName`, `SourceImageId` or `VmId`.'
           type: string
         SourceImageId:
           description: 'The ID of the OMI you want to copy. You must specify only one of the following parameters: `FileLocation`, `RootDeviceName`, `SourceImageId` or `VmId`.'
           type: string
         SourceRegionName:
@@ -1490,14 +1522,123 @@
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
         VirtualGateway:
           $ref: '#/components/schemas/VirtualGateway'
       type: object
+    CreateVmGroupRequest:
+      additionalProperties: false
+      properties:
+        Description:
+          description: A description for the VM group.
+          type: string
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        PositioningStrategy:
+          default: no-strategy
+          description: The positioning strategy of VMs on hypervisors. By default, or if set to `no-strategy` our orchestrator determines the most adequate position for your VMs. If set to `attract`, your VMs are deployed on the same hypervisor, which improves network performance. If set to `repulse`, your VMs are deployed on a different hypervisor, which improves fault tolerance.
+          enum:
+          - attract
+          - no-strategy
+          - repulse
+          type: string
+        SecurityGroupIds:
+          description: One or more IDs of security groups for the VM group.
+          items:
+            type: string
+          type: array
+        SubnetId:
+          description: The ID of the Subnet in which you want to create the VM group.
+          type: string
+        Tags:
+          description: One or more tags to add to the VM group.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmCount:
+          description: The number of VMs deployed in the VM group.
+          type: integer
+        VmGroupName:
+          description: The name of the VM group.
+          type: string
+        VmTemplateId:
+          description: The ID of the VM template used to launch VMs in the VM group.
+          type: string
+      required:
+      - SecurityGroupIds
+      - SubnetId
+      - VmGroupName
+      - VmTemplateId
+      - VmCount
+      type: object
+    CreateVmGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmGroup:
+          $ref: '#/components/schemas/VmGroup'
+      type: object
+    CreateVmTemplateRequest:
+      additionalProperties: false
+      properties:
+        CpuCores:
+          description: The number of vCores to use for each VM.
+          type: integer
+        CpuGeneration:
+          description: The processor generation to use for each VM (for example, `v4`).
+          type: string
+        CpuPerformance:
+          default: high
+          description: 'The performance of the VMs (`medium` \| `high` \|  `highest`). '
+          enum:
+          - medium
+          - high
+          - highest
+          type: string
+        Description:
+          description: A description for the VM template.
+          type: string
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        ImageId:
+          description: The ID of the OMI to use for each VM. You can find a list of OMIs by calling the [ReadImages](#readimages) method.
+          type: string
+        KeypairName:
+          description: The name of the keypair to use for each VM.
+          type: string
+        Ram:
+          description: The amount of RAM to use for each VM.
+          type: integer
+        Tags:
+          description: One or more tags to add to the VM template.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmTemplateName:
+          description: The name of the VM template.
+          type: string
+      required:
+      - CpuCores
+      - CpuGeneration
+      - ImageId
+      - Ram
+      - VmTemplateName
+      type: object
+    CreateVmTemplateResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmTemplate:
+          $ref: '#/components/schemas/VmTemplate'
+      type: object
     CreateVmsRequest:
       additionalProperties: false
       properties:
         BlockDeviceMappings:
           description: One or more block device mappings.
           items:
             $ref: '#/components/schemas/BlockDeviceMappingVmCreation'
@@ -2319,14 +2460,50 @@
       type: object
     DeleteVirtualGatewayResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
       type: object
+    DeleteVmGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        VmGroupId:
+          description: The ID of the VM group you want to delete.
+          type: string
+      required:
+      - VmGroupId
+      type: object
+    DeleteVmGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
+    DeleteVmTemplateRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        VmTemplateId:
+          description: 'The ID of the VM template you want to delete. '
+          type: string
+      required:
+      - VmTemplateId
+      type: object
+    DeleteVmTemplateResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
     DeleteVmsRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         VmIds:
@@ -2664,21 +2841,27 @@
           type: array
         QueryCallNames:
           description: The names of the logged calls.
           items:
             type: string
           type: array
         QueryDateAfter:
-          description: The date after which you want to retrieve logged calls, in ISO 8601 format (for example, `2020-06-14`). By default, this date is set to 48 hours before the `QueryDateBefore` parameter value.
-          format: date
-          type: string
+          description: The date and time, or the date, after which you want to retrieve logged calls, in ISO 8601 format (for example, `2020-06-14T00:00:00.000Z` or `2020-06-14`). By default, this date is set to 48 hours before the `QueryDateBefore` parameter value.
+          oneOf:
+          - format: date-time
+            type: string
+          - format: date
+            type: string
         QueryDateBefore:
-          description: The date before which you want to retrieve logged calls, in ISO 8601 format (for example, `2020-06-30`). By default, this date is set to now, or 48 hours after the `QueryDateAfter` parameter value.
-          format: date
-          type: string
+          description: The date and time, or the date, before which you want to retrieve logged calls, in ISO 8601 format (for example, `2020-06-30T00:00:00.000Z` or `2020-06-14`). By default, this date is set to now, or 48 hours after the `QueryDateAfter` parameter value.
+          oneOf:
+          - format: date-time
+            type: string
+          - format: date
+            type: string
         QueryIpAddresses:
           description: The IPs used for the logged calls.
           items:
             type: string
           type: array
         QueryUserAgents:
           description: The user agents of the HTTP requests of the logged calls.
@@ -2712,14 +2895,30 @@
           type: array
         Descriptions:
           description: The descriptions of the CAs.
           items:
             type: string
           type: array
       type: object
+    FiltersCatalogs:
+      additionalProperties: false
+      description: One or more filters.
+      properties:
+        CurrentCatalogOnly:
+          description: By default or if set to true, only returns the current catalog. If false, returns the current catalog and past catalogs.
+          type: boolean
+        FromDate:
+          description: The beginning of the time period, in ISO 8601 date format (for example, `2020-06-14`). This date cannot be older than 3 years. You must specify the parameters `FromDate` and `ToDate` together.
+          format: date
+          type: string
+        ToDate:
+          description: The end of the time period, in ISO 8601 date format (for example, `2020-06-30`). You must specify the parameters `FromDate` and `ToDate` together.
+          format: date
+          type: string
+      type: object
     FiltersClientGateway:
       additionalProperties: false
       description: One or more filters.
       properties:
         BgpAsns:
           description: The Border Gateway Protocol (BGP) Autonomous System Numbers (ASNs) of the connections.
           items:
@@ -2954,15 +3153,15 @@
           items:
             type: string
           type: array
         PermissionsToLaunchGlobalPermission:
           description: If true, lists all public OMIs. If false, lists all private OMIs.
           type: boolean
         ProductCodes:
-          description: The product code associated with the OMI (`0001` Linux/Unix \| `0002` Windows \| `0004` Linux/Oracle \| `0005` Windows 10).
+          description: The product codes associated with the OMI.
           items:
             type: string
           type: array
         RootDeviceNames:
           description: The name of the root device. This value must be /dev/sda1.
           items:
             type: string
@@ -3733,14 +3932,18 @@
             type: string
           type: array
         Descriptions:
           description: The descriptions of the snapshots.
           items:
             type: string
           type: array
+        FromCreationDate:
+          description: The beginning of the time period, in ISO 8601 date-time format (for example, `2020-06-14T00:00:00.000Z`).
+          format: date-time
+          type: string
         PermissionsToCreateVolumeAccountIds:
           description: The account IDs of one or more users who have permissions to create volumes.
           items:
             type: string
           type: array
         PermissionsToCreateVolumeGlobalPermission:
           description: If true, lists all public volumes. If false, lists all private volumes.
@@ -3771,14 +3974,18 @@
             type: string
           type: array
         Tags:
           description: 'The key/value combination of the tags associated with the snapshots, in the following format: &quot;Filters&quot;:{&quot;Tags&quot;:[&quot;TAGKEY=TAGVALUE&quot;]}.'
           items:
             type: string
           type: array
+        ToCreationDate:
+          description: The end of the time period, in ISO 8601 date-time format (for example, `2020-06-30T00:00:00.000Z`).
+          format: date-time
+          type: string
         VolumeIds:
           description: The IDs of the volumes used to create the snapshots.
           items:
             type: string
           type: array
         VolumeSizes:
           description: The sizes of the volumes used to create the snapshots, in gibibytes (GiB).
@@ -3937,14 +4144,134 @@
           type: array
         VmIds:
           description: One or more IDs of VMs.
           items:
             type: string
           type: array
       type: object
+    FiltersVmGroup:
+      additionalProperties: false
+      description: One or more filters.
+      properties:
+        Descriptions:
+          description: The descriptions of the VM groups.
+          items:
+            type: string
+          type: array
+        SecurityGroupIds:
+          description: The IDs of the security groups.
+          items:
+            type: string
+          type: array
+        SubnetIds:
+          description: The IDs of the Subnets.
+          items:
+            type: string
+          type: array
+        TagKeys:
+          description: The keys of the tags associated with the VM groups.
+          items:
+            type: string
+          type: array
+        TagValues:
+          description: The values of the tags associated with the VM groups.
+          items:
+            type: string
+          type: array
+        Tags:
+          description: 'The key/value combination of the tags associated with the VMs, in the following format: &quot;Filters&quot;:{&quot;Tags&quot;:[&quot;TAGKEY=TAGVALUE&quot;]}.'
+          items:
+            type: string
+          type: array
+        VmCounts:
+          description: The number of VMs in the VM group.
+          items:
+            type: integer
+          type: array
+        VmGroupIds:
+          description: The IDs of the VM groups.
+          items:
+            type: string
+          type: array
+        VmGroupNames:
+          description: The names of the VM groups.
+          items:
+            type: string
+          type: array
+        VmTemplateIds:
+          description: The IDs of the VM templates.
+          items:
+            type: string
+          type: array
+      type: object
+    FiltersVmTemplate:
+      additionalProperties: false
+      description: One or more filters.
+      properties:
+        CpuCores:
+          description: The number of vCores.
+          items:
+            type: integer
+          type: array
+        CpuGenerations:
+          description: The processor generations (for example, `v4`).
+          items:
+            type: string
+          type: array
+        CpuPerformances:
+          description: The performances of the VMs.
+          items:
+            type: string
+          type: array
+        Descriptions:
+          description: The descriptions of the VM templates.
+          items:
+            type: string
+          type: array
+        ImageIds:
+          description: The IDs of the OMIs.
+          items:
+            type: string
+          type: array
+        KeypairNames:
+          description: The names of the keypairs.
+          items:
+            type: string
+          type: array
+        Rams:
+          description: The amount of RAM.
+          items:
+            type: integer
+          type: array
+        TagKeys:
+          description: The keys of the tags associated with the VM templates.
+          items:
+            type: string
+          type: array
+        TagValues:
+          description: The values of the tags associated with the VM templates.
+          items:
+            type: string
+          type: array
+        Tags:
+          description: 'The key/value combination of the tags associated with the VM templates, in the following format: "Filters":{"Tags":["TAGKEY=TAGVALUE"]}.'
+          items:
+            type: string
+          type: array
+        VmTemplateIds:
+          description: The IDs of the VM templates.
+          items:
+            type: string
+          type: array
+        VmTemplateNames:
+          description: The names of the VM templates.
+          items:
+            type: string
+          type: array
+      type: object
     FiltersVmType:
       additionalProperties: false
       description: One or more filters.
       properties:
         BsuOptimized:
           description: This parameter is not available. It is present in our API for the sake of historical compatibility with AWS.
           type: boolean
@@ -4018,31 +4345,31 @@
           type: array
       type: object
     FiltersVolume:
       additionalProperties: false
       description: One or more filters.
       properties:
         CreationDates:
-          description: The dates and times of creation of the volumes.
+          description: The dates and times of creation of the volumes, in ISO 8601 date-time format (for example, `2020-06-30T00:00:00.000Z`).
           items:
-            format: date
+            format: date-time
             type: string
           type: array
         LinkVolumeDeleteOnVmDeletion:
           description: Whether the volumes are deleted or not when terminating the VMs.
           type: boolean
         LinkVolumeDeviceNames:
           description: The VM device names.
           items:
             type: string
           type: array
         LinkVolumeLinkDates:
-          description: The dates and times of creation of the volumes.
+          description: The dates and times of creation of the volumes, in ISO 8601 date-time format (for example, `2020-06-30T00:00:00.000Z`).
           items:
-            format: date
+            format: date-time
             type: string
           type: array
         LinkVolumeLinkStates:
           description: The attachment states of the volumes (`attaching` \| `detaching` \| `attached` \| `detached`).
           items:
             type: string
           type: array
@@ -4251,16 +4578,16 @@
           type: string
         BlockDeviceMappings:
           description: One or more block device mappings.
           items:
             $ref: '#/components/schemas/BlockDeviceMappingImage'
           type: array
         CreationDate:
-          description: The date and time of creation of the OMI.
-          format: date
+          description: The date and time of creation of the OMI, in ISO 8601 date-time format.
+          format: date-time
           type: string
         Description:
           description: The description of the OMI.
           type: string
         FileLocation:
           description: The location of the bucket where the OMI files are stored.
           type: string
@@ -4272,15 +4599,15 @@
           type: string
         ImageType:
           description: The type of the OMI.
           type: string
         PermissionsToLaunch:
           $ref: '#/components/schemas/PermissionsOnResource'
         ProductCodes:
-          description: The product code associated with the OMI (`0001` Linux/Unix \| `0002` Windows \| `0004` Linux/Oracle \| `0005` Windows 10).
+          description: The product codes associated with the OMI.
           items:
             type: string
           type: array
         RootDeviceName:
           description: The name of the root device.
           type: string
         RootDeviceType:
@@ -4985,16 +5312,16 @@
         QueryApiVersion:
           description: The version of the API used by the logged call.
           type: string
         QueryCallName:
           description: The name of the logged call.
           type: string
         QueryDate:
-          description: The date of the logged call, in ISO 8601 format.
-          format: date
+          description: The date and time of the logged call, in ISO 8601 date-time format.
+          format: date-time
           type: string
         QueryHeaderRaw:
           description: The raw header of the HTTP request of the logged call.
           type: string
         QueryHeaderSize:
           description: The size of the raw header of the HTTP request of the logged call, in bytes.
           type: integer
@@ -5765,14 +6092,37 @@
       additionalProperties: false
       properties:
         Catalog:
           $ref: '#/components/schemas/Catalog'
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
       type: object
+    ReadCatalogsRequest:
+      additionalProperties: false
+      description: ReadCatalogsRequest
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Filters:
+          $ref: '#/components/schemas/FiltersCatalogs'
+          description: ReadCatalogsRequest_Filters
+      type: object
+    ReadCatalogsResponse:
+      additionalProperties: false
+      description: ReadCatalogsResponse
+      properties:
+        Catalogs:
+          description: Information about one or more catalogs.
+          items:
+            $ref: '#/components/schemas/Catalogs'
+          type: array
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
     ReadClientGatewaysRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Filters:
@@ -5816,25 +6166,31 @@
     ReadConsumptionAccountRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         FromDate:
-          description: The beginning of the time period, in ISO 8601 date-time format (for example, `2017-06-14` or `2017-06-14T00:00:00Z`).
-          format: datetime
-          type: string
+          description: The beginning of the time period, in ISO 8601 date format (for example, `2020-06-14`). The date-time format is also accepted, but only with a time set to midnight (for example, `2020-06-14T00:00:00.000Z`).
+          oneOf:
+          - format: date
+            type: string
+          - format: date-time
+            type: string
         Overall:
           default: false
           description: By default or if false, returns only the consumption of the specific account that sends this request. If true, returns either the overall consumption of your paying account and all linked accounts (if the account that sends this request is a paying account) or returns nothing (if the account that sends this request is a linked account).
           type: boolean
         ToDate:
-          description: The end of the time period, in ISO 8601 date-time format (for example, `2017-06-30` or `2017-06-30T00:00:00Z`).
-          format: datetime
-          type: string
+          description: The end of the time period, in ISO 8601 date format (for example, `2020-06-30`). The date-time format is also accepted, but only with a time set to midnight (for example, `2020-06-30T00:00:00.000Z`).
+          oneOf:
+          - format: date
+            type: string
+          - format: date-time
+            type: string
       required:
       - FromDate
       - ToDate
       type: object
     ReadConsumptionAccountResponse:
       additionalProperties: false
       properties:
@@ -6534,14 +6890,55 @@
           $ref: '#/components/schemas/ResponseContext'
         VirtualGateways:
           description: Information about one or more virtual gateways.
           items:
             $ref: '#/components/schemas/VirtualGateway'
           type: array
       type: object
+    ReadVmGroupsRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Filters:
+          $ref: '#/components/schemas/FiltersVmGroup'
+          description: ReadVmGroupsRequest_Filters
+      type: object
+    ReadVmGroupsResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmGroups:
+          description: Information about one or more VM groups.
+          items:
+            $ref: '#/components/schemas/VmGroup'
+          type: array
+      type: object
+    ReadVmTemplatesRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Filters:
+          $ref: '#/components/schemas/FiltersVmTemplate'
+      type: object
+    ReadVmTemplatesResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmTemplates:
+          description: Information about one or more VM templates.
+          items:
+            $ref: '#/components/schemas/VmTemplate'
+          type: array
+      type: object
     ReadVmTypesRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Filters:
@@ -6884,14 +7281,58 @@
           type: array
         Tags:
           description: One or more tags associated with the route table.
           items:
             $ref: '#/components/schemas/ResourceTag'
           type: array
       type: object
+    ScaleDownVmGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        VmGroupId:
+          description: The ID of the VM group you want to scale down.
+          type: string
+        VmSubtraction:
+          description: The number of VMs you want to delete from the VM group.
+          type: integer
+      required:
+      - VmGroupId
+      - VmSubtraction
+      type: object
+    ScaleDownVmGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
+    ScaleUpVmGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        VmAddition:
+          description: The number of VMs you want to add to the VM group.
+          type: integer
+        VmGroupId:
+          description: The ID of the VM group you want to scale up.
+          type: string
+      required:
+      - VmGroupId
+      - VmAddition
+      type: object
+    ScaleUpVmGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
     SecurityGroup:
       additionalProperties: false
       description: Information about the security group.
       properties:
         AccountId:
           description: The account ID of a user that has been granted permission.
           type: string
@@ -7044,15 +7485,15 @@
           description: The account alias of the owner of the snapshot.
           type: string
         AccountId:
           description: The account ID of the owner of the snapshot.
           type: string
         CreationDate:
           description: The date and time of creation of the snapshot.
-          format: datetime
+          format: date-time
           type: string
         Description:
           description: The description of the snapshot.
           type: string
         PermissionsToCreateVolume:
           $ref: '#/components/schemas/PermissionsOnResource'
         Progress:
@@ -7455,17 +7896,20 @@
         AccessKeyId:
           description: The ID of the access key.
           type: string
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         ExpirationDate:
-          description: The date and time at which you want the access key to expire, in ISO 8601 format (for example, `2017-06-14` or `2017-06-14T00:00:00Z`). If not specified, the access key is set to not expire.
-          format: datetime
-          type: string
+          description: The date and time, or the date, at which you want the access key to expire, in ISO 8601 format (for example, `2020-06-14T00:00:00.000Z` or `2020-06-14`). If not specified, the access key is set to not expire.
+          oneOf:
+          - format: date-time
+            type: string
+          - format: date
+            type: string
         State:
           description: The new state for the access key (`ACTIVE` \| `INACTIVE`). When set to `ACTIVE`, the access key is enabled and can be used to send requests. When set to `INACTIVE`, the access key is disabled.
           type: string
       required:
       - AccessKeyId
       - State
       type: object
@@ -7629,15 +8073,14 @@
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Mtu:
           description: The maximum transmission unit (MTU) of the DirectLink interface, in bytes (always `1500`).
           enum:
           - 1500
-          - 9000
           type: integer
       required:
       - DirectLinkInterfaceId
       - Mtu
       type: object
     UpdateDirectLinkInterfaceResponse:
       additionalProperties: false
@@ -7989,14 +8432,48 @@
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
         Subnet:
           $ref: '#/components/schemas/Subnet'
       type: object
+    UpdateVmGroupRequest:
+      additionalProperties: false
+      properties:
+        Description:
+          description: A new description for the VM group.
+          type: string
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Tags:
+          description: New tags for your VM group.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmGroupId:
+          description: The ID of the VM group you want to update.
+          type: string
+        VmGroupName:
+          description: A new name for your VM group.
+          type: string
+        VmTemplateId:
+          description: A new VM template ID for your VM group.
+          type: string
+      required:
+      - VmGroupId
+      type: object
+    UpdateVmGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmGroup:
+          $ref: '#/components/schemas/VmGroup'
+      type: object
     UpdateVmRequest:
       additionalProperties: false
       properties:
         BlockDeviceMappings:
           description: One or more block device mappings of the VM.
           items:
             $ref: '#/components/schemas/BlockDeviceMappingVmUpdate'
@@ -8052,14 +8529,45 @@
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
         Vm:
           $ref: '#/components/schemas/Vm'
       type: object
+    UpdateVmTemplateRequest:
+      additionalProperties: false
+      properties:
+        Description:
+          description: A new description for the VM template.
+          type: string
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Tags:
+          description: New tags for your VM template.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmTemplateId:
+          description: The ID of the VM template you want to update.
+          type: string
+        VmTemplateName:
+          description: A new name for your VM template.
+          type: string
+      required:
+      - VmTemplateId
+      type: object
+    UpdateVmTemplateResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        VmTemplate:
+          $ref: '#/components/schemas/VmTemplate'
+      type: object
     UpdateVolumeRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Iops:
@@ -8118,15 +8626,15 @@
       description: Information about the current state of a VPN tunnel.
       properties:
         AcceptedRouteCount:
           description: The number of routes accepted through BGP (Border Gateway Protocol) route exchanges.
           type: integer
         LastStateChangeDate:
           description: The date and time (UTC) of the latest state update.
-          format: datetime
+          format: date-time
           type: string
         OutsideIpAddress:
           description: The IP on the OUTSCALE side of the tunnel.
           type: string
         State:
           description: The state of the IPSEC tunnel (`UP` \| `DOWN`).
           type: string
@@ -8174,15 +8682,15 @@
           description: This parameter is not available. It is present in our API for the sake of historical compatibility with AWS.
           type: boolean
         ClientToken:
           description: The idempotency token provided when launching the VM.
           type: string
         CreationDate:
           description: The date and time of creation of the VM.
-          format: datetime
+          format: date-time
           type: string
         DeletionProtection:
           description: If true, you cannot delete the VM unless you change this parameter back to false.
           type: boolean
         Hypervisor:
           description: The hypervisor type of the VMs (`ovm` \| `xen`).
           type: string
@@ -8220,15 +8728,15 @@
         PrivateDnsName:
           description: The name of the private DNS.
           type: string
         PrivateIp:
           description: The primary private IP of the VM.
           type: string
         ProductCodes:
-          description: The product code associated with the OMI used to create the VM (`0001` Linux/Unix \| `0002` Windows \| `0004` Linux/Oracle \| `0005` Windows 10).
+          description: The product codes associated with the OMI used to create the VM.
           items:
             type: string
           type: array
         PublicDnsName:
           description: The name of the public DNS.
           type: string
         PublicIp:
@@ -8271,14 +8779,73 @@
         VmInitiatedShutdownBehavior:
           description: The VM behavior when you stop it. If set to `stop`, the VM stops. If set to `restart`, the VM stops then automatically restarts. If set to `terminate`, the VM stops and is deleted.
           type: string
         VmType:
           description: The type of VM. For more information, see [Instance Types](https://docs.outscale.com/en/userguide/Instance-Types.html).
           type: string
       type: object
+    VmGroup:
+      additionalProperties: false
+      description: Information about the VM group.
+      properties:
+        CreationDate:
+          description: The date and time of creation of the VM group.
+          format: date-time
+          type: string
+        Description:
+          description: The description of the VM group.
+          type: string
+        PositioningStrategy:
+          description: The positioning strategy of the VMs on hypervisors. By default, or if set to `no-strategy`, TINA determines the most adequate position for the VMs. If set to `attract`, the VMs are deployed on the same hypervisor, which improves network performance. If set to `repulse`, the VMs are deployed on a different hypervisor, which improves fault tolerance.
+          enum:
+          - attract
+          - no-strategy
+          - repulse
+          type: string
+        SecurityGroupIds:
+          description: One or more IDs of security groups for the VM group.
+          items:
+            type: string
+          type: array
+        State:
+          description: The state of the VM group (`pending` \| `available` \| `scaling up` \| `scaling down` \| `deleting` \| `deleted`).
+          enum:
+          - available
+          - deleted
+          - deleting
+          - pending
+          - scaling down
+          - scaling up
+          type: string
+        SubnetId:
+          description: The ID of the Subnet for the VM group.
+          type: string
+        Tags:
+          description: One or more tags associated with the VM group.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmCount:
+          description: The number of VMs in the VM group.
+          type: integer
+        VmGroupId:
+          description: The ID of the VM group.
+          type: string
+        VmGroupName:
+          description: The name of the VM group.
+          type: string
+        VmIds:
+          description: The IDs of the VMs in the VM group.
+          items:
+            type: string
+          type: array
+        VmTemplateId:
+          description: The ID of the VM template used by the VM group.
+          type: string
+      type: object
     VmState:
       additionalProperties: false
       description: Information about the state of the VM.
       properties:
         CurrentState:
           description: The current state of the VM (`InService` \| `OutOfService` \| `Unknown`).
           type: string
@@ -8304,14 +8871,66 @@
         VmId:
           description: The ID of the VM.
           type: string
         VmState:
           description: The state of the VM (`pending` \| `running` \| `stopping` \| `stopped` \| `shutting-down` \| `terminated` \| `quarantine`).
           type: string
       type: object
+    VmTemplate:
+      additionalProperties: false
+      description: Information about the VM template.
+      properties:
+        CpuCores:
+          description: The number of vCores.
+          type: integer
+        CpuGeneration:
+          description: The processor generation.
+          type: string
+        CpuPerformance:
+          description: The performance of the VMs.
+          enum:
+          - medium
+          - high
+          - highest
+          type: string
+        CreationDate:
+          description: The date and time of creation of the VM template.
+          format: date-time
+          type: string
+        Description:
+          description: The description of the VM template.
+          type: string
+        ImageId:
+          description: The ID of the OMI.
+          type: string
+        KeypairName:
+          description: The name of the keypair.
+          type: string
+        Ram:
+          description: The amount of RAM.
+          type: integer
+        Tags:
+          description: One or more tags associated with the VM template.
+          items:
+            $ref: '#/components/schemas/ResourceTag'
+          type: array
+        VmTemplateId:
+          description: The ID of the VM template.
+          type: string
+        VmTemplateName:
+          description: The name of the VM template.
+          type: string
+      required:
+      - CpuCores
+      - CpuGeneration
+      - ImageId
+      - Ram
+      - VmTemplateId
+      - VmTemplateName
+      type: object
     VmType:
       additionalProperties: false
       description: Information about the VM type.
       properties:
         BsuOptimized:
           description: This parameter is not available. It is present in our API for the sake of historical compatibility with AWS.
           type: boolean
@@ -8337,15 +8956,15 @@
       type: object
     Volume:
       additionalProperties: false
       description: Information about the volume.
       properties:
         CreationDate:
           description: The date and time of creation of the volume.
-          format: datetime
+          format: date-time
           type: string
         Iops:
           description: 'The number of I/O operations per second (IOPS):<br />
 
             - For `io1` volumes, the number of provisioned IOPS<br />
 
             - For `gp2` volumes, the baseline performance of the volume'
@@ -8533,15 +9152,15 @@
 
     An OpenAPI description of the OUTSCALE API is also available in this [GitHub repository](https://github.com/outscale/osc-api).'
   license:
     name: BSD 3 Clause
     url: https://opensource.org/licenses/BSD-3-Clause
   termsOfService: https://en.outscale.com/terms-of-service/
   title: 3DS OUTSCALE API
-  version: '1.25'
+  version: '1.26'
 openapi: 3.0.0
 paths:
   /AcceptNetPeering:
     description: 'Accepts a Net peering request.<br />
 
       To accept this request, you must be the owner of the peer Net. If you do not accept the request within 7 days, the state of the Net peering becomes `expired`.<br /><br />
 
@@ -9744,14 +10363,82 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/CreateVirtualGatewayResponse'
           description: The HTTP 200 response (OK).
       tags:
       - VirtualGateway
+  /CreateVmGroup:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Creates a group of virtual machines (VMs) containing the same characteristics as a specified VM template, and then launches them.<br />
+
+      You can create up to 100 VM groups in your account.'
+    post:
+      operationId: CreateVmGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/CreateVmGroupRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/CreateVmGroupResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
+  /CreateVmTemplate:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Creates a virtual machine (VM) template. You can then use the VM template to create VM groups.<br />
+
+      You can create up to 50 VM templates in your account.'
+    post:
+      operationId: CreateVmTemplate
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/CreateVmTemplateRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/CreateVmTemplateResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - VmTemplate
   /CreateVms:
     description: 'Creates virtual machines (VMs), and then launches them.<br />
 
       This action enables you to create a specified number of VMs using an OUTSCALE machine image (OMI) that you are allowed to use, and then to automatically launch them.<br />
 
       The VMs remain in the `pending` state until they are created and ready to be used. Once automatically launched, they are in the `running` state.<br />
 
@@ -10821,14 +11508,80 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/DeleteVirtualGatewayResponse'
           description: The HTTP 200 response (OK).
       tags:
       - VirtualGateway
+  /DeleteVmGroup:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Deletes a specified VM group.'
+    post:
+      operationId: DeleteVmGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/DeleteVmGroupRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/DeleteVmGroupResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
+  /DeleteVmTemplate:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Deletes a virtual machine (VM) template.<br />
+
+      You cannot delete a template currently used by a VM group.'
+    post:
+      operationId: DeleteVmTemplate
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/DeleteVmTemplateRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/DeleteVmTemplateResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - VmTemplate
   /DeleteVms:
     description: 'Terminates one or more virtual machines (VMs).<br />
 
       This operation is idempotent, that means that all calls succeed if you terminate a VM more than once.'
     post:
       operationId: DeleteVms
       requestBody:
@@ -11450,14 +12203,32 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ReadCatalogResponse'
           description: The HTTP 200 response (OK).
       tags:
       - Catalog
+  /ReadCatalogs:
+    description: Returns the price list of OUTSCALE products and services for the current Region within a specific time period.
+    post:
+      operationId: ReadCatalogs
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ReadCatalogsRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ReadCatalogsResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - Catalog
   /ReadClientGateways:
     description: 'Lists one or more of your client gateways.<br /><br />
 
 
       **[NOTE]**<br />
 
       If you exceed the number of identical requests allowed for a configured time period, the `RequestLimitExceeded` error message is returned.'
@@ -12572,14 +13343,78 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ReadVirtualGatewaysResponse'
           description: The HTTP 200 response (OK).
       tags:
       - VirtualGateway
+  /ReadVmGroups:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Lists one or more group of virtual machines (VMs).'
+    post:
+      operationId: ReadVmGroups
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ReadVmGroupsRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ReadVmGroupsResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
+  /ReadVmTemplates:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Lists one or more virtual machine (VM) templates.'
+    post:
+      operationId: ReadVmTemplates
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ReadVmTemplatesRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ReadVmTemplatesResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - VmTemplate
   /ReadVmTypes:
     description: 'Lists one or more predefined VM types.<br /><br />
 
 
       **[NOTE]**<br />
 
       If you exceed the number of identical requests allowed for a configured time period, the `RequestLimitExceeded` error message is returned.'
@@ -12896,14 +13731,100 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/ResetAccountPasswordResponse'
           description: The HTTP 200 response (OK).
       security: []
       tags:
       - Account
+  /ScaleDownVmGroup:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Deletes virtual machines (VMs) from a VM group.<br />
+
+      The oldest VMs are the first to be deleted.'
+    post:
+      operationId: ScaleDownVmGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ScaleDownVmGroupRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ScaleDownVmGroupResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
+  /ScaleUpVmGroup:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Creates additional virtual machines (VMs) in a VM group.<br />
+
+      The new VMs use the current version of the VM template.'
+    post:
+      operationId: ScaleUpVmGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ScaleUpVmGroupRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ScaleUpVmGroupResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
   /SendResetPasswordEmail:
     description: 'Sends an email to the email address provided for the account with a token to reset your password.<br />
 
       You need to provide this token when updating the account password using the ResetAccountPassword method.<br /><br />
 
       **[NOTE]**<br />
 
@@ -13842,14 +14763,78 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Vm
+  /UpdateVmGroup:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Modifies the specified attributes of a group of virtual machines (VMs).'
+    post:
+      operationId: UpdateVmGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/UpdateVmGroupRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/UpdateVmGroupResponse'
+          description: The HTTP 200 response (OK).
+        '400':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 400 response (Bad Request).
+        '401':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 401 response (Unauthorized).
+        '500':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
+          description: The HTTP 500 response (Internal Server Error).
+      tags:
+      - VmGroup
+  /UpdateVmTemplate:
+    description: '> [WARNING]<br />
+
+      > This feature is currently under development and may not function properly.<br />
+
+
+      Modifies the specified attributes of a template of virtual machines (VMs).'
+    post:
+      operationId: UpdateVmTemplate
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/UpdateVmTemplateRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/UpdateVmTemplateResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - VmTemplate
   /UpdateVolume:
     description: 'Modifies the specified attributes of a volume.<br />
 
       Cold volumes are volumes that are attached to stopped or stopping VMs, or that are detached. Hot volumes are volumes that are attached to running VMs.<br /><br />
 
 
       **[NOTE]**<br />
```

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/outscale_gateway.py` & `osc_sdk_python-0.25.0/osc_sdk_python/outscale_gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-import time
 import sys
+import threading
 from .call import Call
 import ruamel.yaml
 
 type_mapping = {'boolean': 'bool',
                 'string': 'str',
                 'integer': 'int',
                 'array': 'list'}
@@ -35,17 +35,17 @@
     pass
 
 class Logger:
     string = ""
     type = LOG_NONE
     what = LOG_ALL
     def config(self, type=None, what=None):
-        if type != None:
+        if type is not None:
             self.type=type
-        if what != None:
+        if what is not None:
             self.what=what
     def str(self):
         if self.type == LOG_MEMORY:
             return self.string
         return None
     def do_log(self, s):
         if self.type & LOG_MEMORY:
@@ -62,19 +62,17 @@
 
 class OutscaleGateway:
 
     def __init__(self, retry=True, **kwargs):
         self._load_gateway_structure()
         self._load_errors()
         self.log = Logger()
+        if retry:
+            kwargs['max_retries'] = 5
         self.call = Call(logger=self.log, **kwargs)
-        if retry is True:
-            self.retry = 5
-        else:
-            self.retry = 1
 
     def update_credentials(self, region=None, profile=None, access_key=None,
                            secret_key=None, email=None, password=None):
         """
         destroy and create a new credential map use for each call.
         so you can change your ak/sk, region without having to recreate the whole Gateway
         as the object is recreate, you can't expect to keep parameter from the old configuration
@@ -127,15 +125,15 @@
             if i_param != 'Filters' and \
                action_structure[i_param]['type'] is not None and \
                action_structure[i_param]['type'] != i_value.__class__.__name__:
                 raise ParameterHasWrongType('{} is <{}> instead of <{}>'.format(i_param, i_value.__class__.__name__,
                                                                                 action_structure[i_param]['type']))
 
     def _check_parameters_required(self, action_structure, input_structure):
-        action_mandatory_params = [param for param in action_structure if action_structure[param]['required'] == True]
+        action_mandatory_params = [param for param in action_structure if action_structure[param]['required']]
         difference = set(action_mandatory_params).difference(set(input_structure.keys()))
         if difference:
             raise ParameterIsRequired('Missing {}. Required parameters are {}'.format(', '.join(list(difference))
                                                                                 ,', '.join(action_mandatory_params)))
 
     def _check_parameters_valid(self, action_name, params):
         structure_parameters = self.gateway_structure[action_name].keys()
@@ -143,15 +141,15 @@
         different_parameters = list(input_parameters.difference(set(structure_parameters)))
         if different_parameters:
             raise ParameterNotValid("""{}. Available parameters are: {}.""".format(', '.join(different_parameters),
                                                                                    ', '.join(structure_parameters)))
 
     def _check(self, action_name, **params):
         if action_name not in self.gateway_structure:
-            raise ActionNotExists('Action {} does not exists'.format(self.action_name))
+            raise ActionNotExists('Action {} does not exists'.format(action_name))
         self._check_parameters_valid(action_name, params)
         self._check_parameters_required(self.gateway_structure[action_name], params)
         self._check_parameters_type(self.gateway_structure[action_name], params)
 
     @staticmethod
     def _remove_none_parameters(**params):
         """
@@ -159,23 +157,15 @@
         to perform CreateVolumes(Iops=None, Size=10)
         """
         return {key: value for key, value in params.items() if value is not None}
 
     def _action(self, **kwargs):
         kwargs = self._remove_none_parameters(**kwargs)
         self._check(self.action_name, **kwargs)
-        for _ in range(0, self.retry):
-            result = self.call.api(self.action_name, **kwargs)
-            if 'Errors' not in result:
-                break
-            time.sleep(1)
-        if 'Errors' in result:
-            for error in result['Errors']:
-                if int(error['Code']) in self.gateway_errors:
-                    error['Details'] = self.gateway_errors[int(error['Code'])]['Name']
+        result = self.call.api(self.action_name,**kwargs)
         self.action_name = None
         return result
 
     def __getattr__(self, attr):
         self.action_name = attr
         return self._action
```

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python/resources/gateway_errors.yaml` & `osc_sdk_python-0.25.0/osc_sdk_python/resources/gateway_errors.yaml`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.24.0/osc_sdk_python.egg-info/PKG-INFO` & `osc_sdk_python-0.25.0/osc_sdk_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-sdk-python
-Version: 0.24.0
+Version: 0.25.0
 Summary: Outscale Gateway python SDK
 Home-page: https://github.com/outscale/osc_sdk_python
 Author: Outscal SAS
 Author-email: opensource@outscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.24.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.24.0/setup.py` & `osc_sdk_python-0.25.0/setup.py`

 * *Files identical despite different names*

